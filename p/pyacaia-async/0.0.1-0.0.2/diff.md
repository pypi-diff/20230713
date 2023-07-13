# Comparing `tmp/pyacaia_async-0.0.1.tar.gz` & `tmp/pyacaia_async-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacaia_async-0.0.1.tar", last modified: Thu Jul 13 06:44:30 2023, max compression
+gzip compressed data, was "pyacaia_async-0.0.2.tar", last modified: Thu Jul 13 09:54:33 2023, max compression
```

## Comparing `pyacaia_async-0.0.1.tar` & `pyacaia_async-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:30.133456 pyacaia_async-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-13 06:44:30.133456 pyacaia_async-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:30.133456 pyacaia_async-0.0.1/pyacaia_async/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/pyacaia_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/pyacaia_async/acaiascale.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/pyacaia_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/pyacaia_async/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/pyacaia_async/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/pyacaia_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:30.133456 pyacaia_async-0.0.1/pyacaia_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-13 06:44:30.000000 pyacaia_async-0.0.1/pyacaia_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 06:44:30.000000 pyacaia_async-0.0.1/pyacaia_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:44:30.000000 pyacaia_async-0.0.1/pyacaia_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 06:44:30.000000 pyacaia_async-0.0.1/pyacaia_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 06:44:30.000000 pyacaia_async-0.0.1/pyacaia_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:44:30.133456 pyacaia_async-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-13 06:44:13.000000 pyacaia_async-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/pyacaia_async/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/acaiascale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/pyacaia_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/pyacaia_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 09:54:33.000000 pyacaia_async-0.0.2/pyacaia_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:54:33.320812 pyacaia_async-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-13 09:54:16.000000 pyacaia_async-0.0.2/setup.py
```

### Comparing `pyacaia_async-0.0.1/LICENSE` & `pyacaia_async-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.1/pyacaia_async/acaiascale.py` & `pyacaia_async-0.0.2/pyacaia_async/acaiascale.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,48 +13,50 @@
 from .helpers import encode, encodeId
 from .exceptions import AcaiaDeviceNotFound, AcaiaError
 
 _LOGGER = logging.getLogger(__name__)
 
 class AcaiaScale():
 
-    def __init__(self, mac: str = None, bleDevice: BLEDevice = None, isPyxisStyle: bool=False):
+    def __init__(self, mac: str = None, isPyxisStyle: bool=False):
         """Initialize the scale."""
     
         self._isPyxisStyle = isPyxisStyle
 
         self._client = None
         self._connected = False
         self._disconnecting = False
         self._timestamp_last_command = None
         self._timer_running = False
         self._timer_start = None
         self._timer_stop = None
+        self._mac = mac
 
         self._queue = asyncio.Queue()
 
         self._msg_types = {
             "tare": encode(4, [0]),
             "startTimer": encode(13, [0,0]),
             "stopTimer": encode(13, [0,2]),
             "resetTimer": encode(13, [0,1]),
             "heartbeat": encode(0, [2,0])
         }
 
+    @classmethod
+    async def create(cls, mac: str = None, bleDevice: BLEDevice = None, isPyxisStyle: bool=False, callback = None) -> AcaiaScale:
+        """Create a new scale."""
+
         if bleDevice:
             self._client = BleakClient(bleDevice)
         elif mac:
             self._client = BleakClient(mac)
         else:
             raise ValueError("Either mac or bleDevice must be specified")
-
-    @classmethod
-    async def create(cls, mac: str = None, bleDevice: BLEDevice = None, isPyxisStyle: bool=False, callback = None) -> AcaiaScale:
-        """Create a new scale."""
-        self = cls(mac, bleDevice, isPyxisStyle)
+        
+        self = cls(mac, isPyxisStyle)
         await self.connect(callback)
         asyncio.create_task(self._send_heartbeats())
         asyncio.create_task(self._process_queue())
         return self
 
     @property
     def msg_types(self) -> dict:
```

### Comparing `pyacaia_async-0.0.1/pyacaia_async/decode.py` & `pyacaia_async-0.0.2/pyacaia_async/decode.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.1/pyacaia_async/helpers.py` & `pyacaia_async-0.0.2/pyacaia_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.1/setup.py` & `pyacaia_async-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="pyacaia_async",
-    version="0.0.1",
+    version="0.0.2",
     description="An async implementation of PyAcaia",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pyacaia_async",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
@@ -19,12 +19,12 @@
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=setuptools.find_packages(),
-    install_requires=["aiohttp>=3.8.4", "bleak>=0.20.2"],
+    install_requires=["bleak>=0.20.2", "asyncio>=3.4.3"],
     package_data={
         "license": ["LICENSE"],
     },
 )
```

