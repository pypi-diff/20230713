# Comparing `tmp/galvoplotter-0.1.0.tar.gz` & `tmp/galvoplotter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galvoplotter-0.1.0.tar", last modified: Thu Jul  6 09:13:27 2023, max compression
+gzip compressed data, was "galvoplotter-0.1.1.tar", last modified: Thu Jul 13 08:05:56 2023, max compression
```

## Comparing `galvoplotter-0.1.0.tar` & `galvoplotter-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 09:13:27.394621 galvoplotter-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-06-28 05:27:33.000000 galvoplotter-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    11309 2023-07-06 09:13:27.395620 galvoplotter-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10481 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 09:13:27.376619 galvoplotter-0.1.0/examples/
--rw-rw-rw-   0        0        0        0 2023-06-28 03:52:49.000000 galvoplotter-0.1.0/examples/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/examples/gpio_detect.py
--rw-rw-rw-   0        0        0     1655 2023-07-06 08:28:29.000000 galvoplotter-0.1.0/examples/joystick.py
--rw-rw-rw-   0        0        0     1764 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/examples/light_circle_abort.py
--rw-rw-rw-   0        0        0      368 2023-07-06 08:28:29.000000 galvoplotter-0.1.0/examples/light_simple_cross.py
--rw-rw-rw-   0        0        0      321 2023-07-06 08:28:29.000000 galvoplotter-0.1.0/examples/mark_square.py
--rw-rw-rw-   0        0        0      403 2023-07-06 08:28:29.000000 galvoplotter-0.1.0/examples/position_sync_grid.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:13:27.382620 galvoplotter-0.1.0/galvo/
--rw-rw-rw-   0        0        0      596 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/galvo/__init__.py
--rw-rw-rw-   0        0        0     5054 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/galvo/consts.py
--rw-rw-rw-   0        0        0    48705 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/galvo/controller.py
--rw-rw-rw-   0        0        0     3633 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/galvo/mock_connection.py
--rw-rw-rw-   0        0        0    10924 2023-06-28 01:39:37.000000 galvoplotter-0.1.0/galvo/usb_connection.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:13:27.393620 galvoplotter-0.1.0/galvoplotter.egg-info/
--rw-rw-rw-   0        0        0    11309 2023-07-06 09:13:27.000000 galvoplotter-0.1.0/galvoplotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-07-06 09:13:27.000000 galvoplotter-0.1.0/galvoplotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 09:13:27.000000 galvoplotter-0.1.0/galvoplotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 09:13:27.000000 galvoplotter-0.1.0/galvoplotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-06 09:13:27.000000 galvoplotter-0.1.0/galvoplotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 09:13:27.000000 galvoplotter-0.1.0/galvoplotter.egg-info/zip-safe
--rw-rw-rw-   0        0        0      962 2023-07-06 09:13:27.396621 galvoplotter-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       91 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:13:27.385620 galvoplotter-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2023-07-06 08:28:29.000000 galvoplotter-0.1.0/test/__init__.py
--rw-rw-rw-   0        0        0     5523 2023-07-06 09:12:43.000000 galvoplotter-0.1.0/test/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.409263 galvoplotter-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-28 05:27:33.000000 galvoplotter-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    11320 2023-07-13 08:05:56.410263 galvoplotter-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10492 2023-07-13 08:04:21.000000 galvoplotter-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.381261 galvoplotter-0.1.1/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-28 03:52:49.000000 galvoplotter-0.1.1/examples/__init__.py
+-rw-rw-rw-   0        0        0     1186 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/examples/gpio_detect.py
+-rw-rw-rw-   0        0        0     1655 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/joystick.py
+-rw-rw-rw-   0        0        0     1764 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/examples/light_circle_abort.py
+-rw-rw-rw-   0        0        0      368 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/light_simple_cross.py
+-rw-rw-rw-   0        0        0      321 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/mark_square.py
+-rw-rw-rw-   0        0        0      403 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/examples/position_sync_grid.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.390262 galvoplotter-0.1.1/galvo/
+-rw-rw-rw-   0        0        0      596 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/galvo/__init__.py
+-rw-rw-rw-   0        0        0     5054 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/galvo/consts.py
+-rw-rw-rw-   0        0        0    49487 2023-07-13 08:00:47.000000 galvoplotter-0.1.1/galvo/controller.py
+-rw-rw-rw-   0        0        0     3633 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/galvo/mock_connection.py
+-rw-rw-rw-   0        0        0    10924 2023-06-28 01:39:37.000000 galvoplotter-0.1.1/galvo/usb_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.408263 galvoplotter-0.1.1/galvoplotter.egg-info/
+-rw-rw-rw-   0        0        0    11320 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-13 08:05:56.000000 galvoplotter-0.1.1/galvoplotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 09:13:27.000000 galvoplotter-0.1.1/galvoplotter.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      962 2023-07-13 08:05:56.411263 galvoplotter-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       91 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:05:56.394262 galvoplotter-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2023-07-06 08:28:29.000000 galvoplotter-0.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0     5523 2023-07-06 09:12:43.000000 galvoplotter-0.1.1/test/test_api.py
```

### Comparing `galvoplotter-0.1.0/LICENSE` & `galvoplotter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/PKG-INFO` & `galvoplotter-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galvoplotter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Galvo Plotter
 Home-page: https://github.com/meerk40t/galvoplotter
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
 Keywords: ezcad2,galvo,laser
 Classifier: Development Status :: 4 - Beta
@@ -173,9 +173,9 @@
 
 # Examples
 See https://github.com/meerk40t/galvoplotter/tree/main/examples for example scripts.
 
 # Thanks
 * Bryce Schroeder - Did the initial work for reverse engineering the format for the laser.
   * See: https://gitlab.com/bryce15/balor for his project.
-* inpain / tiger12506 - Did considerable with galvo lasers to faciliate the reverse engineering.
+* inpain / tiger12506 - Did considerable debugging with galvo lasers to facilitate the reverse engineering.
 * Sandor Konya - Introductions, advice and support
```

### Comparing `galvoplotter-0.1.0/README.md` & `galvoplotter-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -150,9 +150,9 @@
 
 # Examples
 See https://github.com/meerk40t/galvoplotter/tree/main/examples for example scripts.
 
 # Thanks
 * Bryce Schroeder - Did the initial work for reverse engineering the format for the laser.
   * See: https://gitlab.com/bryce15/balor for his project.
-* inpain / tiger12506 - Did considerable with galvo lasers to faciliate the reverse engineering.
+* inpain / tiger12506 - Did considerable debugging with galvo lasers to facilitate the reverse engineering.
 * Sandor Konya - Introductions, advice and support
```

### Comparing `galvoplotter-0.1.0/examples/gpio_detect.py` & `galvoplotter-0.1.1/examples/gpio_detect.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/examples/joystick.py` & `galvoplotter-0.1.1/examples/joystick.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/examples/light_circle_abort.py` & `galvoplotter-0.1.1/examples/light_circle_abort.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/galvo/__init__.py` & `galvoplotter-0.1.1/galvo/__init__.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/galvo/consts.py` & `galvoplotter-0.1.1/galvo/consts.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/galvo/controller.py` & `galvoplotter-0.1.1/galvo/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 Galvo Controller
 
 The balor controller takes low level lmc galvo commands and converts them into lists and shorts commands to send
-to the hardware controller.
+to the hardware controller as both spooled and realtime commands.
 """
 
 import struct
 import threading
 import time
 from contextlib import contextmanager
 from copy import copy
 
 from .consts import *
 from .mock_connection import MockConnection
 from .usb_connection import USBConnection
 
 BUSY = 0x04
 READY = 0x20
+AXIS = 0x40
 
 nop = [0x02, 0x80, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
 empty = bytearray(nop * 0x100)
 
 
 class GalvoController:
     """
     Galvo controller is tasked with sending queued data to the controller board and ensuring that the connection to the
     controller board is established to perform these actions.
 
     This should serve as a next generation command sequencer written from scratch for galvo lasers. The goal is to
     provide all the given commands in a coherent queue structure which provides correct sequences between list and
-    single commands.
+    single commands. As well as some higher level helper commands tasked with simplifying scripts and workflows.
     """
 
     def __init__(
         self,
         settings_file=None,
         x=0x8000,
         y=0x8000,
@@ -636,14 +637,20 @@
         if override_list is not None:
             use_list = override_list
         if use_list:
             self.list_write_port()
         else:
             self.write_port()
 
+    def rotary(self, position, min_speed=100, max_speed=5000, origin_param=100, **kwgs):
+        self.set_axis_motion_param(min_speed & 0xFFFF, max_speed & 0xFFFF)
+        self.set_axis_origin_param(origin_param)
+        self.move_axis_to(position & 0xFFFF)
+        self.wait_axis()
+
     def get_last_xy(self):
         return self._last_x, self._last_y
 
     #######################
     # WAIT STATE COMMANDS
     #######################
 
@@ -651,24 +658,34 @@
         status = self.status()
         return bool(status & BUSY)
 
     def is_ready(self):
         status = self.status()
         return bool(status & READY)
 
+    def is_axis(self):
+        status = self.status()
+        return bool(status & AXIS)
+
     def is_ready_and_not_busy(self):
         status = self.status()
         return bool(status & READY) and not bool(status & BUSY)
 
     def wait_finished(self):
         while not self.is_ready_and_not_busy():
             time.sleep(0.01)
             if not self._sending:
                 return
 
+    def wait_axis(self):
+        while self.is_axis():
+            time.sleep(0.01)
+            if not self._sending:
+                return
+
     def wait_ready(self):
         while not self.is_ready():
             time.sleep(0.01)
             if not self._sending:
                 return
 
     def wait_idle(self):
@@ -1436,25 +1453,25 @@
 
     def write_analog_port_x(self, port):
         return self._command(WriteAnalogPortX, port)
 
     def read_port(self):
         return self._command(ReadPort)
 
-    def set_axis_motion_param(self, param):
-        return self._command(SetAxisMotionParam, param)
+    def set_axis_motion_param(self, p0=0, p1=0, p2=0, p3=0):
+        return self._command(SetAxisMotionParam, p0, p1, p2, p3)
 
-    def set_axis_origin_param(self, param):
-        return self._command(SetAxisOriginParam, param)
+    def set_axis_origin_param(self, p0=0, p1=0, p2=0, p3=0):
+        return self._command(SetAxisOriginParam, p0, p1, p2, p3)
 
-    def axis_go_origin(self):
-        return self._command(AxisGoOrigin)
+    def axis_go_origin(self, p0=0, p1=0):
+        return self._command(AxisGoOrigin, p0, p1)
 
-    def move_axis_to(self, a):
-        return self._command(MoveAxisTo)
+    def move_axis_to(self, p0, p1=0, p2=0, p3=0):
+        return self._command(MoveAxisTo, p0, p1, p2, p3)
 
     def get_axis_pos(self):
         return self._command(GetAxisPos)
 
     def get_fly_wait_count(self):
         return self._command(GetFlyWaitCount)
```

### Comparing `galvoplotter-0.1.0/galvo/mock_connection.py` & `galvoplotter-0.1.1/galvo/mock_connection.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/galvo/usb_connection.py` & `galvoplotter-0.1.1/galvo/usb_connection.py`

 * *Files identical despite different names*

### Comparing `galvoplotter-0.1.0/galvoplotter.egg-info/PKG-INFO` & `galvoplotter-0.1.1/galvoplotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galvoplotter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Galvo Plotter
 Home-page: https://github.com/meerk40t/galvoplotter
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
 Keywords: ezcad2,galvo,laser
 Classifier: Development Status :: 4 - Beta
@@ -173,9 +173,9 @@
 
 # Examples
 See https://github.com/meerk40t/galvoplotter/tree/main/examples for example scripts.
 
 # Thanks
 * Bryce Schroeder - Did the initial work for reverse engineering the format for the laser.
   * See: https://gitlab.com/bryce15/balor for his project.
-* inpain / tiger12506 - Did considerable with galvo lasers to faciliate the reverse engineering.
+* inpain / tiger12506 - Did considerable debugging with galvo lasers to facilitate the reverse engineering.
 * Sandor Konya - Introductions, advice and support
```

### Comparing `galvoplotter-0.1.0/galvoplotter.egg-info/SOURCES.txt` & `galvoplotter-0.1.1/galvoplotter.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,27 @@
 ./galvo/__init__.py
 ./galvo/consts.py
 ./galvo/controller.py
 ./galvo/mock_connection.py
 ./galvo/usb_connection.py
 ./test/__init__.py
 ./test/test_api.py
+examples/__init__.py
+examples/gpio_detect.py
+examples/joystick.py
+examples/light_circle_abort.py
+examples/light_simple_cross.py
+examples/mark_square.py
+examples/position_sync_grid.py
+galvo/__init__.py
+galvo/consts.py
+galvo/controller.py
+galvo/mock_connection.py
+galvo/usb_connection.py
 galvoplotter.egg-info/PKG-INFO
 galvoplotter.egg-info/SOURCES.txt
 galvoplotter.egg-info/dependency_links.txt
 galvoplotter.egg-info/requires.txt
 galvoplotter.egg-info/top_level.txt
 galvoplotter.egg-info/zip-safe
+test/__init__.py
 test/test_api.py
```

### Comparing `galvoplotter-0.1.0/setup.cfg` & `galvoplotter-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 616c 766f 706c 6f74 7465 720d   = galvoplotter.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e31  .version = 0.1.1
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 4761 6c76 6f20 506c 6f74 7465 720d 0a6c  Galvo Plotter..l
 00000050: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 00000060: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 00000070: 6578 742f 6d61 726b 646f 776e 0d0a 6c6f  ext/markdown..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
 00000090: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
```

### Comparing `galvoplotter-0.1.0/test/test_api.py` & `galvoplotter-0.1.1/test/test_api.py`

 * *Files identical despite different names*

