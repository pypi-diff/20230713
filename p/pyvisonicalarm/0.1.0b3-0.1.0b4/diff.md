# Comparing `tmp/pyvisonicalarm-0.1.0b3.tar.gz` & `tmp/pyvisonicalarm-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisonicalarm-0.1.0b3.tar", last modified: Sat May  6 12:27:22 2023, max compression
+gzip compressed data, was "pyvisonicalarm-0.1.0b4.tar", last modified: Thu Jul 13 18:57:06 2023, max compression
```

## Comparing `pyvisonicalarm-0.1.0b3.tar` & `pyvisonicalarm-0.1.0b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/pyvisonicalarm/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/device_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/pyvisonicalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/device_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/setup.py
```

### Comparing `pyvisonicalarm-0.1.0b3/LICENSE` & `pyvisonicalarm-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/PKG-INFO` & `pyvisonicalarm-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b3/README.md` & `pyvisonicalarm-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/alarm.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/alarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,20 @@
     def disable_siren(self, mode="all"):
         """Disable the siren (mute the alarm)."""
         return self.__api.disable_siren(mode=mode)["process_token"]
 
     def disarm(self, partition=-1):
         """Send Disarm command to the alarm system."""
         return self.__api.disarm(partition)["process_token"]
+    
+    def get_alarms(self):
+        return self.__api.get_alarms()
+    
+    def get_alerts(self):
+        return self.__api.get_alerts()
 
     def get_cameras(self):
         """Fetch all the devices that are available."""
         cameras = self.__api.get_cameras()
         return [Camera(camera) for camera in cameras]
 
     def get_devices(self):
```

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/classes.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/classes.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/const.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/const.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/core.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class API(object):
     """Class used for communication with the Visonic API"""
 
     # Client configuration
     __app_type = "com.visonic.powermaxapp"
     __user_agent = "Dart/2.10 (dart:io)"
-    __rest_version = "9.0"
+    __rest_version = "10.0"
 
     # API tokens
     __user_token = None
     __session_token = None
 
     # Use a session to reuse one TCP connection instead of creating a new
     # connection for every call to the API
```

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/device_definitions.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/device_definitions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/devices.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/devices.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm/exceptions.py` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/PKG-INFO` & `pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b3/setup.py` & `pyvisonicalarm-0.1.0b4/setup.py`

 * *Files identical despite different names*

