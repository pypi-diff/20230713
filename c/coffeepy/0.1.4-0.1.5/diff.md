# Comparing `tmp/coffeepy-0.1.4.tar.gz` & `tmp/coffeepy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.4.tar", last modified: Thu Jul 13 13:13:40 2023, max compression
+gzip compressed data, was "coffeepy-0.1.5.tar", last modified: Thu Jul 13 13:37:38 2023, max compression
```

## Comparing `coffeepy-0.1.4.tar` & `coffeepy-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.315354 coffeepy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 13:13:25.000000 coffeepy-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-13 13:13:40.315354 coffeepy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 13:13:25.000000 coffeepy-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 13:13:25.000000 coffeepy-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:13:40.315354 coffeepy-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.311353 coffeepy-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.311353 coffeepy-0.1.4/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 13:13:25.000000 coffeepy-0.1.4/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-13 13:13:25.000000 coffeepy-0.1.4/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.315354 coffeepy-0.1.4/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 13:37:24.000000 coffeepy-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 13:37:38.894291 coffeepy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 13:37:24.000000 coffeepy-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 13:37:24.000000 coffeepy-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:37:38.894291 coffeepy-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 13:37:24.000000 coffeepy-0.1.5/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 13:37:24.000000 coffeepy-0.1.5/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/top_level.txt
```

### Comparing `coffeepy-0.1.4/LICENSE` & `coffeepy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.4/PKG-INFO` & `coffeepy-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,23 +31,24 @@
 Simply run the program from command line
 ```sh
 coffeepy
 ```
 
 By default the program runs indefinitely. Press `Ctrl-C` to quit
 
-Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
+Optional: You can set the time in minutes with `-t` or `--time` flag. For example, to run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 You can also disable animation with `-a` or `--no-animation` flag.
 ```sh
 coffeepy -a
 ```
+You can view the full parameter list with `-h` or `--help`.
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
```

### Comparing `coffeepy-0.1.4/README.md` & `coffeepy-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 Simply run the program from command line
 ```sh
 coffeepy
 ```
 
 By default the program runs indefinitely. Press `Ctrl-C` to quit
 
-Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
+Optional: You can set the time in minutes with `-t` or `--time` flag. For example, to run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 You can also disable animation with `-a` or `--no-animation` flag.
 ```sh
 coffeepy -a
 ```
+You can view the full parameter list with `-h` or `--help`.
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
```

### Comparing `coffeepy-0.1.4/pyproject.toml` & `coffeepy-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `coffeepy-0.1.4/src/coffeepy/coffeepy.py` & `coffeepy-0.1.5/src/coffeepy/coffeepy.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from importlib.metadata import version
 
 import ctypes
 import sys
 import subprocess
 import time
 import argparse
-
+import os
 
 animation = [
     "  ☕️   ",
     " ☁️☕️   ",
     "  ☕️   ",
     "  ☕️☁️  ",
     " ☁️☕️   ",
@@ -34,17 +34,19 @@
     try:
         subprocess.check_output(['which', 'caffeinate'])
         return True
     except subprocess.CalledProcessError:
         return False
 
 def check_windows_terminal():
-    is_windows_terminal = sys.platform == "win32" and os.environ.get("WT_SESSION")
-    if is_windows_terminal is not None:
-        return True
+    if 'win32' in sys.platform:
+        if os.environ.get("WT_SESSION") is not None:
+            return True
+        else:
+            return False
     else:
         return False
 
 def run(runtime=None, no_animation=False):
     parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
                                                  'You can set the time with -t flag\n'
                                                  'Made by kuvaus',
@@ -94,15 +96,15 @@
     print('Press Ctrl-C to quit')
     
     try:
         start_time = time.time()
         while time.time() - start_time < duration or duration == float('inf'):
             if not args.no_animation:
                 if 'win32' in sys.platform:
-                    if check_windows_terminal:
+                    if check_windows_terminal() == True:
                         display_animation()
                     else:
                         display_animation(ascii_animation)
                 else:
                     display_animation()
 
     except KeyboardInterrupt:
```

### Comparing `coffeepy-0.1.4/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.5/src/coffeepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,23 +31,24 @@
 Simply run the program from command line
 ```sh
 coffeepy
 ```
 
 By default the program runs indefinitely. Press `Ctrl-C` to quit
 
-Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
+Optional: You can set the time in minutes with `-t` or `--time` flag. For example, to run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 You can also disable animation with `-a` or `--no-animation` flag.
 ```sh
 coffeepy -a
 ```
+You can view the full parameter list with `-h` or `--help`.
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
```

