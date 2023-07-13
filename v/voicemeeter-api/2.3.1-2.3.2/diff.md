# Comparing `tmp/voicemeeter_api-2.3.1.tar.gz` & `tmp/voicemeeter_api-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.3.1.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.3.2.tar", max compression
```

## Comparing `voicemeeter_api-2.3.1.tar` & `voicemeeter_api-2.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.1/LICENSE
--rw-r--r--   0        0        0     1102 2023-07-12 03:48:54.989633 voicemeeter_api-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    18156 2023-07-11 18:43:59.775001 voicemeeter_api-2.3.1/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.1/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.3.1/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.1/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.1/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.1/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.1/voicemeeterlib/device.py
--rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.1/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.1/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.1/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.1/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.1/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.3.1/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.3.1/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.1/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.1/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.1/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12243 2023-07-12 03:43:21.313261 voicemeeter_api-2.3.1/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.3.1/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.1/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-07-10 02:00:50.034407 voicemeeter_api-2.3.1/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     2449 2023-07-12 01:53:12.508493 voicemeeter_api-2.3.1/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.3.1/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17969 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.2/LICENSE
+-rw-r--r--   0        0        0     1102 2023-07-12 08:41:43.355965 voicemeeter_api-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0    18156 2023-07-11 18:43:59.775001 voicemeeter_api-2.3.2/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.2/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.3.2/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.2/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.2/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.2/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.2/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.2/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.2/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.2/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.2/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.2/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2370 2023-07-12 04:22:12.387405 voicemeeter_api-2.3.2/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.3.2/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.2/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.2/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.2/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12243 2023-07-12 03:43:21.313261 voicemeeter_api-2.3.2/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-07-12 07:44:11.180313 voicemeeter_api-2.3.2/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.2/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2978 2023-07-10 02:00:50.034407 voicemeeter_api-2.3.2/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2449 2023-07-12 01:53:12.508493 voicemeeter_api-2.3.2/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     6316 2023-07-12 07:56:56.692493 voicemeeter_api-2.3.2/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17969 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.2/PKG-INFO
```

### Comparing `voicemeeter_api-2.3.1/LICENSE` & `voicemeeter_api-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/pyproject.toml` & `voicemeeter_api-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.3.1"
+version = "2.3.2"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.3.1/README.md` & `voicemeeter_api-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/bus.py` & `voicemeeter_api-2.3.2/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.3.2/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/command.py` & `voicemeeter_api-2.3.2/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/config.py` & `voicemeeter_api-2.3.2/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/device.py` & `voicemeeter_api-2.3.2/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/error.py` & `voicemeeter_api-2.3.2/voicemeeterlib/error.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/event.py` & `voicemeeter_api-2.3.2/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/factory.py` & `voicemeeter_api-2.3.2/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/inst.py` & `voicemeeter_api-2.3.2/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/iremote.py` & `voicemeeter_api-2.3.2/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/kinds.py` & `voicemeeter_api-2.3.2/voicemeeterlib/kinds.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,35 +60,35 @@
 
 
 @dataclass
 class BasicMap(KindMapClass):
     name: str
     ins: tuple = (2, 1)
     outs: tuple = (1, 1)
-    vban: tuple = (4, 4)
+    vban: tuple = (4, 4, 1, 1)
     asio: tuple = (0, 0)
     insert: int = 0
 
 
 @dataclass
 class BananaMap(KindMapClass):
     name: str
     ins: tuple = (3, 2)
     outs: tuple = (3, 2)
-    vban: tuple = (8, 8)
+    vban: tuple = (8, 8, 1, 1)
     asio: tuple = (6, 8)
     insert: int = 22
 
 
 @dataclass
 class PotatoMap(KindMapClass):
     name: str
     ins: tuple = (5, 3)
     outs: tuple = (5, 3)
-    vban: tuple = (8, 8)
+    vban: tuple = (8, 8, 1, 1)
     asio: tuple = (10, 8)
     insert: int = 34
 
 
 def kind_factory(kind_id):
     match kind_id:
         case "basic":
```

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.3.2/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/meta.py` & `voicemeeter_api-2.3.2/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/misc.py` & `voicemeeter_api-2.3.2/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/recorder.py` & `voicemeeter_api-2.3.2/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/remote.py` & `voicemeeter_api-2.3.2/voicemeeterlib/remote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/strip.py` & `voicemeeter_api-2.3.2/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/subject.py` & `voicemeeter_api-2.3.2/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/updater.py` & `voicemeeter_api-2.3.2/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/util.py` & `voicemeeter_api-2.3.2/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.1/voicemeeterlib/vban.py` & `voicemeeter_api-2.3.2/voicemeeterlib/vban.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import abstractmethod
 
 from .iremote import IRemote
+from .kinds import kinds_all
 
 
 class VbanStream(IRemote):
     """
     Implements the common interface
 
     Defines concrete implementation for vban stream
@@ -129,14 +130,29 @@
         return super(VbanInstream, self).channel
 
     @property
     def bit(self) -> int:
         return super(VbanInstream, self).bit
 
 
+class VbanAudioInstream(VbanInstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+class VbanMidiInstream(VbanInstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+class VbanTextInstream(VbanInstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
 class VbanOutstream(VbanStream):
     """
     class representing a vban outstream
 
     Subclasses VbanStream
     """
 
@@ -144,26 +160,70 @@
         return f"{type(self).__name__}{self._remote.kind}{self.index}"
 
     @property
     def direction(self) -> str:
         return "out"
 
 
+class VbanAudioOutstream(VbanOutstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+class VbanMidiOutstream(VbanOutstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+def _make_stream_pair(remote, kind):
+    num_instream, num_outstream, num_midi, num_text = kind.vban
+
+    def _generate_streams(i, dir):
+        """generator function for instream/outstream types"""
+        if dir == "in":
+            if i < num_instream:
+                yield VbanAudioInstream
+            elif i < num_instream + num_midi:
+                yield VbanMidiInstream
+            else:
+                yield VbanTextInstream
+        else:
+            if i < num_outstream:
+                yield VbanAudioOutstream
+            else:
+                yield VbanMidiOutstream
+
+    return (
+        tuple(
+            cls(remote, i)
+            for i in range(num_instream + num_midi + num_text)
+            for cls in _generate_streams(i, "in")
+        ),
+        tuple(
+            cls(remote, i)
+            for i in range(num_outstream + num_midi)
+            for cls in _generate_streams(i, "out")
+        ),
+    )
+
+
+def _make_stream_pairs(remote):
+    return {kind.name: _make_stream_pair(remote, kind) for kind in kinds_all}
+
+
 class Vban:
     """
     class representing the vban module
 
     Contains two tuples, one for each stream type
     """
 
     def __init__(self, remote):
         self.remote = remote
-        num_instream, num_outstream = remote.kind.vban
-        self.instream = tuple(VbanInstream(remote, i) for i in range(num_instream))
-        self.outstream = tuple(VbanOutstream(remote, i) for i in range(num_outstream))
+        self.instream, self.outstream = _make_stream_pairs(remote)[remote.kind.name]
 
     def enable(self):
         self.remote.set("vban.Enable", 1)
 
     def disable(self):
         self.remote.set("vban.Enable", 0)
```

### Comparing `voicemeeter_api-2.3.1/PKG-INFO` & `voicemeeter_api-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.3.1
+Version: 2.3.2
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

