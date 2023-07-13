# Comparing `tmp/fps_yjs-0.1.9.tar.gz` & `tmp/fps_yjs-0.2.0.tar.gz`

## Comparing `fps_yjs-0.1.9.tar` & `fps_yjs-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/py.typed
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/COPYING.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15108 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/fps_yjs/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/COPYING.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fps_yjs-0.2.0/PKG-INFO
```

### Comparing `fps_yjs-0.1.9/fps_yjs/main.py` & `fps_yjs-0.2.0/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.9/fps_yjs/routes.py` & `fps_yjs-0.2.0/fps_yjs/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,26 +144,28 @@
         self.contents = contents
         self.documents = {}  # a dictionary of room_name:document
         self.watchers = {}  # a dictionary of file_id:task
         self.savers = {}  # a dictionary of file_id:task
         self.cleaners = {}  # a dictionary of room:task
         self.last_modified = {}  # a dictionary of file_id:last_modification_date
         self.websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
+        self.websocket_server_task = asyncio.create_task(self.websocket_server.start())
         self.lock = asyncio.Lock()
 
     def stop(self):
         for watcher in self.watchers.values():
             watcher.cancel()
         for saver in self.savers.values():
             saver.cancel()
         for cleaner in self.cleaners.values():
             cleaner.cancel()
+        self.websocket_server.stop()
 
     async def serve(self, websocket: YpyWebsocket, permissions) -> None:
-        room = self.websocket_server.get_room(websocket.path)
+        room = await self.websocket_server.get_room(websocket.path)
         can_write = permissions is None or "write" in permissions.get("yjs", [])
         room.on_message = partial(self.filter_message, can_write)
         is_stored_document = websocket.path.count(":") >= 2
         if is_stored_document:
             assert room.ystore is not None
             file_format, file_type, file_id = websocket.path.split(":", 2)
             if room in self.cleaners:
@@ -205,14 +207,15 @@
                     )
                     # update the document when file changes
                     if file_id not in self.watchers:
                         self.watchers[file_id] = asyncio.create_task(
                             self.watch_file(file_format, file_id, document)
                         )
 
+        await self.websocket_server.started.wait()
         await self.websocket_server.serve(websocket)
 
         if is_stored_document and not room.clients:
             # no client in this room after we disconnect
             self.cleaners[room] = asyncio.create_task(self.maybe_clean_room(room, websocket.path))
 
     async def filter_message(self, can_write: bool, message: bytes) -> bool:
@@ -350,19 +353,21 @@
         room_name = self.websocket_server.get_room_name(room)
         self.websocket_server.delete_room(room=room)
         file_path = await self.get_file_path(file_id, document)
         logger.info(f"Closing collaboration room: {room_name} ({file_path})")
 
 
 class JupyterWebsocketServer(WebsocketServer):
-    def get_room(self, ws_path: str) -> YRoom:
+    async def get_room(self, ws_path: str) -> YRoom:
         if ws_path not in self.rooms:
             if ws_path.count(":") >= 2:
                 # it is a stored document (e.g. a notebook)
                 file_format, file_type, file_id = ws_path.split(":", 2)
                 updates_file_path = f".{file_type}:{file_id}.y"
                 ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
                 self.rooms[ws_path] = YRoom(ready=False, ystore=ystore)
             else:
                 # it is a transient document (e.g. awareness)
                 self.rooms[ws_path] = YRoom()
-        return self.rooms[ws_path]
+        room = self.rooms[ws_path]
+        await self.start_room(room)
+        return room
```

### Comparing `fps_yjs-0.1.9/.gitignore` & `fps_yjs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.9/COPYING.md` & `fps_yjs-0.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.9/pyproject.toml` & `fps_yjs-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "fps_yjs"
 description = "An FPS plugin for the Yjs API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
     "jupyter_ydoc >=1,<2",
-    "ypy-websocket >=0.8.2,<1",
+    "ypy-websocket >=0.12.1,<0.13.0",
     "y-py >=0.6.0,<0.7.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `fps_yjs-0.1.9/PKG-INFO` & `fps_yjs-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fps_yjs
-Version: 0.1.9
+Version: 0.2.0
 Summary: An FPS plugin for the Yjs API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
 Requires-Dist: jupyter-ydoc<2,>=1
 Requires-Dist: jupyverse-api<1,>=0.1.2
 Requires-Dist: y-py<0.7.0,>=0.6.0
-Requires-Dist: ypy-websocket<1,>=0.8.2
+Requires-Dist: ypy-websocket<0.13.0,>=0.12.1
 Description-Content-Type: text/markdown
 
 # fps-yjs
 
 An FPS plugin for the Yjs API.
```

