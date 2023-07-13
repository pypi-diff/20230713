# Comparing `tmp/fps_contents-0.1.9.tar.gz` & `tmp/fps_contents-0.2.0.tar.gz`

## Comparing `fps_contents-0.1.9.tar` & `fps_contents-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.9/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/__init__.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/py.typed
--rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.9/COPYING.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.9/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.2.0/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 fps_contents-0.2.0/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.2.0/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.2.0/fps_contents/py.typed
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 fps_contents-0.2.0/fps_contents/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.2.0/COPYING.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.2.0/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.2.0/PKG-INFO
```

### Comparing `fps_contents-0.1.9/fps_contents/fileid.py` & `fps_contents-0.2.0/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.9/fps_contents/routes.py` & `fps_contents-0.2.0/fps_contents/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     ) -> Content:
         if isinstance(path, str):
             path = Path(path)
         content: Optional[Union[str, Dict, List[Dict]]] = None
         if get_content:
             if path.is_dir():
                 content = [
-                    (await self.read_content(subpath, get_content=False)).dict()
+                    (await self.read_content(subpath, get_content=False)).model_dump()
                     for subpath in path.iterdir()
                     if not subpath.name.startswith(".")
                 ]
             elif path.is_file() or path.is_symlink():
                 try:
                     async with await open_file(path, mode="rb") as f:
                         content_bytes = await f.read()
```

### Comparing `fps_contents-0.1.9/.gitignore` & `fps_contents-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.9/COPYING.md` & `fps_contents-0.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.9/pyproject.toml` & `fps_contents-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.9/PKG-INFO` & `fps_contents-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_contents
-Version: 0.1.9
+Version: 0.2.0
 Summary: An FPS plugin for the contents API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

