# Comparing `tmp/pyOpenHaptics-0.0.3.tar.gz` & `tmp/pyOpenHaptics-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyOpenHaptics-0.0.3.tar", last modified: Thu Jul 13 08:25:43 2023, max compression
+gzip compressed data, was "pyOpenHaptics-1.0.0.tar", last modified: Thu Jul 13 16:10:38 2023, max compression
```

## Comparing `pyOpenHaptics-0.0.3.tar` & `pyOpenHaptics-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/PKG-INFO
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      128 2023-07-12 15:54:52.000000 pyOpenHaptics-0.0.3/README.md
-drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/PKG-INFO
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      245 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/SOURCES.txt
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        1 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/dependency_links.txt
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        4 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/top_level.txt
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       38 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/setup.cfg
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      730 2023-07-13 08:25:36.000000 pyOpenHaptics-0.0.3/setup.py
-drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/src/
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       18 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/__init__.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      623 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/exceptions.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     3658 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/hd.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     5292 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/hd_define.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       82 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/hdu_matrix.py
+drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 16:10:38.305517 pyOpenHaptics-1.0.0/
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-13 16:10:38.305517 pyOpenHaptics-1.0.0/PKG-INFO
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     1241 2023-07-13 09:56:59.000000 pyOpenHaptics-1.0.0/README.md
+drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 16:10:38.305517 pyOpenHaptics-1.0.0/pyOpenHaptics/
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       18 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/__init__.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      623 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/exceptions.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     3666 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/hd.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      785 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/hd_callback.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     5292 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/hd_define.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      981 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/hd_device.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       82 2023-07-13 16:07:01.000000 pyOpenHaptics-1.0.0/pyOpenHaptics/hdu_matrix.py
+drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 16:10:38.305517 pyOpenHaptics-1.0.0/pyOpenHaptics.egg-info/
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-13 16:10:38.000000 pyOpenHaptics-1.0.0/pyOpenHaptics.egg-info/PKG-INFO
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      351 2023-07-13 16:10:38.000000 pyOpenHaptics-1.0.0/pyOpenHaptics.egg-info/SOURCES.txt
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        1 2023-07-13 16:10:38.000000 pyOpenHaptics-1.0.0/pyOpenHaptics.egg-info/dependency_links.txt
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       14 2023-07-13 16:10:38.000000 pyOpenHaptics-1.0.0/pyOpenHaptics.egg-info/top_level.txt
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       38 2023-07-13 16:10:38.305517 pyOpenHaptics-1.0.0/setup.cfg
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      730 2023-07-13 16:07:54.000000 pyOpenHaptics-1.0.0/setup.py
```

### Comparing `pyOpenHaptics-0.0.3/setup.py` & `pyOpenHaptics-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION="0.0.3"
+VERSION="1.0.0"
 DESCRIPTION="Python binding for OpenHaptics"
 LONG_DESCRIPTION="Basic functions to mimic the OpenHaptics library on C++. Written into a more Python friendly language"
 
 setup(
     name="pyOpenHaptics",
     version=VERSION,
     author="Mikel De Iturrate Reyzabal",
```

### Comparing `pyOpenHaptics-0.0.3/src/exceptions.py` & `pyOpenHaptics-1.0.0/pyOpenHaptics/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyOpenHaptics-0.0.3/src/hd.py` & `pyOpenHaptics-1.0.0/pyOpenHaptics/hd.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,19 @@
     _lib_hd.hdSetDoublev(code, data)
 
 def _get_error() -> HDErrorInfo:
     _lib_hd.hdGetError.restype = HDErrorInfo
     return _lib_hd.hdGetError()
 
 
-def init_device(name: str = None) -> int:
+def init_device(name: str = "Default Device") -> int:
     _lib_hd.hdInitDevice.argtypes = [c_char_p]
     _lib_hd.hdInitDevice.restype = HHD
     try:
-        id = _lib_hd.hdInitDevice(HD_DEFAULT_DEVICE)
+        id = _lib_hd.hdInitDevice(name.encode())
         if id == HD_BAD_HANDLE:
             raise DeviceInitException
         else:
             return id
     except DeviceInitException:
         print("Unable to initialize the device. Check the connection!")
```

### Comparing `pyOpenHaptics-0.0.3/src/hd_define.py` & `pyOpenHaptics-1.0.0/pyOpenHaptics/hd_define.py`

 * *Files identical despite different names*

