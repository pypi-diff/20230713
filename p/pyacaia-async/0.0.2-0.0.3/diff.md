# Comparing `tmp/pyacaia_async-0.0.2.tar.gz` & `tmp/pyacaia_async-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacaia_async-0.0.2.tar", last modified: Thu Jul 13 09:54:33 2023, max compression
+gzip compressed data, was "pyacaia_async-0.0.3.tar", last modified: Thu Jul 13 11:04:30 2023, max compression
```

## Comparing `pyacaia_async-0.0.2.tar` & `pyacaia_async-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/pyacaia_async/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/acaiascale.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/pyacaia_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/pyacaia_async/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/acaiascale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/pyacaia_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/setup.py
```

### Comparing `pyacaia_async-0.0.2/LICENSE` & `pyacaia_async-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.2/PKG-INFO` & `pyacaia_async-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia_async
-Version: 0.0.2
+Version: 0.0.3
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyacaia_async-0.0.2/README.md` & `pyacaia_async-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.2/pyacaia_async/acaiascale.py` & `pyacaia_async-0.0.3/pyacaia_async/acaiascale.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,47 +16,47 @@
 _LOGGER = logging.getLogger(__name__)
 
 class AcaiaScale():
 
     def __init__(self, mac: str = None, isPyxisStyle: bool=False):
         """Initialize the scale."""
     
+        self._mac = mac
         self._isPyxisStyle = isPyxisStyle
 
         self._client = None
         self._connected = False
         self._disconnecting = False
         self._timestamp_last_command = None
         self._timer_running = False
         self._timer_start = None
         self._timer_stop = None
-        self._mac = mac
 
         self._queue = asyncio.Queue()
 
         self._msg_types = {
             "tare": encode(4, [0]),
             "startTimer": encode(13, [0,0]),
             "stopTimer": encode(13, [0,2]),
             "resetTimer": encode(13, [0,1]),
             "heartbeat": encode(0, [2,0])
         }
 
     @classmethod
     async def create(cls, mac: str = None, bleDevice: BLEDevice = None, isPyxisStyle: bool=False, callback = None) -> AcaiaScale:
-        """Create a new scale."""
+        """Create a new scale."""  
+        self = cls(mac, isPyxisStyle)
 
         if bleDevice:
             self._client = BleakClient(bleDevice)
         elif mac:
             self._client = BleakClient(mac)
         else:
             raise ValueError("Either mac or bleDevice must be specified")
         
-        self = cls(mac, isPyxisStyle)
         await self.connect(callback)
         asyncio.create_task(self._send_heartbeats())
         asyncio.create_task(self._process_queue())
         return self
 
     @property
     def msg_types(self) -> dict:
@@ -64,14 +64,18 @@
     
     @property
     def timer(self) -> int:
         if self._timer_running:
             return int(time.time() - self._timer_start)
         else:
             return int(self._timer_stop - self._timer_start)
+        
+
+    def new_client_from_ble_device(self, BLED: BLEDevice) -> None:
+        self._client = BleakClient(BLED)
 
 
     async def _write_msg(self, char_id: str, payload: bytearray) -> None:
         try:
             if not self._connected:
                 return
```

### Comparing `pyacaia_async-0.0.2/pyacaia_async/decode.py` & `pyacaia_async-0.0.3/pyacaia_async/decode.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.2/pyacaia_async/helpers.py` & `pyacaia_async-0.0.3/pyacaia_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.2/pyacaia_async.egg-info/PKG-INFO` & `pyacaia_async-0.0.3/pyacaia_async.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia-async
-Version: 0.0.2
+Version: 0.0.3
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyacaia_async-0.0.2/setup.py` & `pyacaia_async-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="pyacaia_async",
-    version="0.0.2",
+    version="0.0.3",
     description="An async implementation of PyAcaia",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pyacaia_async",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

