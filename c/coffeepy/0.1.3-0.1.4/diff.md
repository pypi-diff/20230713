# Comparing `tmp/coffeepy-0.1.3.tar.gz` & `tmp/coffeepy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.3.tar", last modified: Thu Jul 13 06:18:13 2023, max compression
+gzip compressed data, was "coffeepy-0.1.4.tar", last modified: Thu Jul 13 13:13:40 2023, max compression
```

## Comparing `coffeepy-0.1.3.tar` & `coffeepy-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 06:18:01.000000 coffeepy-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 06:18:13.123894 coffeepy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 06:18:01.000000 coffeepy-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 06:18:01.000000 coffeepy-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:18:13.123894 coffeepy-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 06:18:01.000000 coffeepy-0.1.3/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-13 06:18:01.000000 coffeepy-0.1.3/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:18:13.123894 coffeepy-0.1.3/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 06:18:13.000000 coffeepy-0.1.3/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.315354 coffeepy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 13:13:25.000000 coffeepy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-13 13:13:40.315354 coffeepy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 13:13:25.000000 coffeepy-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 13:13:25.000000 coffeepy-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:13:40.315354 coffeepy-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.311353 coffeepy-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.311353 coffeepy-0.1.4/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 13:13:25.000000 coffeepy-0.1.4/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-13 13:13:25.000000 coffeepy-0.1.4/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:13:40.315354 coffeepy-0.1.4/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 13:13:40.000000 coffeepy-0.1.4/src/coffeepy.egg-info/top_level.txt
```

### Comparing `coffeepy-0.1.3/LICENSE` & `coffeepy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.3/PKG-INFO` & `coffeepy-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,25 +37,38 @@
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 You can also disable animation with `-a` or `--no-animation` flag.
+```sh
+coffeepy -a
+```
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
 
 coffeepy.run()
+```
+
+Optional settings when run as a python module:
+
+```python
+import coffeepy
 
 # you can also specify the time in minutes
+# if no time is provided or time = 0, the program will run indefinitely
 coffeepy.run(60)
+
+# to disable animation when run as a module, you can set the second argument to True
+coffeepy.run(0, True)
 ```
 
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
```

### Comparing `coffeepy-0.1.3/README.md` & `coffeepy-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -23,25 +23,38 @@
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 You can also disable animation with `-a` or `--no-animation` flag.
+```sh
+coffeepy -a
+```
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
 
 coffeepy.run()
+```
+
+Optional settings when run as a python module:
+
+```python
+import coffeepy
 
 # you can also specify the time in minutes
+# if no time is provided or time = 0, the program will run indefinitely
 coffeepy.run(60)
+
+# to disable animation when run as a module, you can set the second argument to True
+coffeepy.run(0, True)
 ```
 
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
```

### Comparing `coffeepy-0.1.3/pyproject.toml` & `coffeepy-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `coffeepy-0.1.3/src/coffeepy/coffeepy.py` & `coffeepy-0.1.4/src/coffeepy/coffeepy.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         return True
     except subprocess.CalledProcessError:
         return False
 
 def check_windows_terminal():
     is_windows_terminal = sys.platform == "win32" and os.environ.get("WT_SESSION")
     if is_windows_terminal is not None:
-        return true
+        return True
     else:
-        return false
+        return False
 
-def run(runtime=None):
+def run(runtime=None, no_animation=False):
     parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
                                                  'You can set the time with -t flag\n'
                                                  'Made by kuvaus',
                                                  formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-t', '--time', type=int, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
     parser.add_argument('-a', '--no-animation', action='store_true', help='Optional: Disable animation')
@@ -60,17 +60,23 @@
     else:
         duration = args.time * 60  # Convert minutes to seconds
     
     #if time is provided as run argument, it will overwrite args
     #this is only relevant when coffeepy is run as a python module
     if runtime is None:
         duration = duration
+    elif runtime == 0:
+        duration = float('inf')
     else:
         duration = runtime * 60
 
+    #this disables animation when used as a module
+    if no_animation == True:
+        args.no_animation = True
+
     proc = None
 
     if 'darwin' in sys.platform:
         print('Running \'coffeepy\' on MacOS to prevent the system from sleeping')
         proc = subprocess.Popen(['caffeinate', '-dims'])
 
     elif 'linux' in sys.platform:
```

### Comparing `coffeepy-0.1.3/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.4/src/coffeepy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,25 +37,38 @@
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 You can also disable animation with `-a` or `--no-animation` flag.
+```sh
+coffeepy -a
+```
 
 ## Python module
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
 
 coffeepy.run()
+```
+
+Optional settings when run as a python module:
+
+```python
+import coffeepy
 
 # you can also specify the time in minutes
+# if no time is provided or time = 0, the program will run indefinitely
 coffeepy.run(60)
+
+# to disable animation when run as a module, you can set the second argument to True
+coffeepy.run(0, True)
 ```
 
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
```

