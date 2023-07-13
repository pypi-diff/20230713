# Comparing `tmp/coffeepy-0.1.2.tar.gz` & `tmp/coffeepy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.2.tar", last modified: Thu Jul 13 05:43:18 2023, max compression
+gzip compressed data, was "coffeepy-0.1.3.tar", last modified: Thu Jul 13 06:18:13 2023, max compression
```

## Comparing `coffeepy-0.1.2.tar` & `coffeepy-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.949919 coffeepy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 05:43:07.000000 coffeepy-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-13 05:43:18.949919 coffeepy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-13 05:43:07.000000 coffeepy-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 05:43:07.000000 coffeepy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:43:18.949919 coffeepy-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.945919 coffeepy-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.949919 coffeepy-0.1.2/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 05:43:07.000000 coffeepy-0.1.2/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-13 05:43:07.000000 coffeepy-0.1.2/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.949919 coffeepy-0.1.2/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 06:18:01.000000 coffeepy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 06:18:13.123894 coffeepy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 06:18:01.000000 coffeepy-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 06:18:01.000000 coffeepy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:18:13.123894 coffeepy-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 06:18:01.000000 coffeepy-0.1.3/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-13 06:18:01.000000 coffeepy-0.1.3/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/top_level.txt
```

### Comparing `coffeepy-0.1.2/LICENSE` & `coffeepy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.2/PKG-INFO` & `coffeepy-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,15 @@
 By default the program runs indefinitely. Press `Ctrl-C` to quit
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
+You can also disable animation with `-a` or `--no-animation` flag.
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
```

### Comparing `coffeepy-0.1.2/README.md` & `coffeepy-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 By default the program runs indefinitely. Press `Ctrl-C` to quit
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
+You can also disable animation with `-a` or `--no-animation` flag.
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
```

### Comparing `coffeepy-0.1.2/pyproject.toml` & `coffeepy-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `coffeepy-0.1.2/src/coffeepy/coffeepy.py` & `coffeepy-0.1.3/src/coffeepy/coffeepy.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,49 +13,63 @@
     " ☁️☕️   ",
     "  ☕️   ",
     "  ☕️☁️  ",
     " ☁️☕️   ",
     "  ☕️   ",
 ]
 
+ascii_animation = [
+    "  |   ",
+    "  /   ",
+    "  -   ",
+    "  \\   ",
+]
 
 def display_animation(animation=animation):
     for frame in animation:
         print('\r' + frame, end='')
         time.sleep(0.5)  # Adjust the delay time as desired
 
 
 def check_caffeinate():
     try:
         subprocess.check_output(['which', 'caffeinate'])
         return True
     except subprocess.CalledProcessError:
         return False
 
+def check_windows_terminal():
+    is_windows_terminal = sys.platform == "win32" and os.environ.get("WT_SESSION")
+    if is_windows_terminal is not None:
+        return true
+    else:
+        return false
 
-def run(time=None):
+def run(runtime=None):
     parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
                                                  'You can set the time with -t flag\n'
                                                  'Made by kuvaus',
                                                  formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-t', '--time', type=int, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
+    parser.add_argument('-a', '--no-animation', action='store_true', help='Optional: Disable animation')
+
     args = parser.parse_args()
 
     if args.time == 0:
         duration = float('inf')  # Set duration to infinity
     else:
         duration = args.time * 60  # Convert minutes to seconds
     
     #if time is provided as run argument, it will overwrite args
     #this is only relevant when coffeepy is run as a python module
-    if time is None:
+    if runtime is None:
         duration = duration
     else:
-        duration = time *60
+        duration = runtime * 60
 
     proc = None
 
     if 'darwin' in sys.platform:
         print('Running \'coffeepy\' on MacOS to prevent the system from sleeping')
         proc = subprocess.Popen(['caffeinate', '-dims'])
 
@@ -72,15 +86,23 @@
         ctypes.windll.kernel32.SetThreadExecutionState(0x80000002)
 
     print('Press Ctrl-C to quit')
     
     try:
         start_time = time.time()
         while time.time() - start_time < duration or duration == float('inf'):
-            display_animation()
+            if not args.no_animation:
+                if 'win32' in sys.platform:
+                    if check_windows_terminal:
+                        display_animation()
+                    else:
+                        display_animation(ascii_animation)
+                else:
+                    display_animation()
+
     except KeyboardInterrupt:
         print('\nExiting')
 
     finally:
         if proc:
             proc.terminate()
         if 'linux' in sys.platform and not check_caffeinate():
```

### Comparing `coffeepy-0.1.2/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.3/src/coffeepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,15 @@
 By default the program runs indefinitely. Press `Ctrl-C` to quit
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
+You can also disable animation with `-a` or `--no-animation` flag.
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
```

