# Comparing `tmp/coffeepy-0.1.1.tar.gz` & `tmp/coffeepy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.1.tar", last modified: Wed Jul 12 17:21:58 2023, max compression
+gzip compressed data, was "coffeepy-0.1.2.tar", last modified: Thu Jul 13 05:43:18 2023, max compression
```

## Comparing `coffeepy-0.1.1.tar` & `coffeepy-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 17:21:44.000000 coffeepy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-12 17:21:58.306758 coffeepy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-12 17:21:44.000000 coffeepy-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 17:21:44.000000 coffeepy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:21:58.306758 coffeepy-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 17:21:44.000000 coffeepy-0.1.1/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-12 17:21:44.000000 coffeepy-0.1.1/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.949919 coffeepy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 05:43:07.000000 coffeepy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-13 05:43:18.949919 coffeepy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-13 05:43:07.000000 coffeepy-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 05:43:07.000000 coffeepy-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:43:18.949919 coffeepy-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.945919 coffeepy-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.949919 coffeepy-0.1.2/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 05:43:07.000000 coffeepy-0.1.2/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-13 05:43:07.000000 coffeepy-0.1.2/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:43:18.949919 coffeepy-0.1.2/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 05:43:18.000000 coffeepy-0.1.2/src/coffeepy.egg-info/top_level.txt
```

### Comparing `coffeepy-0.1.1/LICENSE` & `coffeepy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.1/PKG-INFO` & `coffeepy-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Coffeepy prevents the system from sleeping
-Author-email: kuvaus <kuvaus@users.noreply.github.com>
+Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/coffeepy.svg?style=flat)](https://pypi.python.org/pypi/coffeepy/) [![PyPI Version](https://img.shields.io/pypi/v/coffeepy.svg)](https://pypi.python.org/pypi/coffeepy)
 # Coffeepy
 
 Coffeepy ☕️ is a small program that prevents the system from sleeping.
 Works on MacOS, Windows and Linux.
 
-<img alt="coffeepy" src="https://github.com/kuvaus/coffeepy/assets/22169537/d2954958-4c92-4791-92b9-36e46f448abc.gif" width="600" />
+<img alt="coffeepy" src="https://github-production-user-asset-6210df.s3.amazonaws.com/22169537/253075028-9eaccaca-a567-4bd8-86c1-63d4870664ad.gif" width="600" />
 
 ## Installation
 
 ```sh
 pip install -U coffeepy
 ```
 
@@ -44,15 +45,16 @@
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
 
 coffeepy.run()
+
+# you can also specify the time in minutes
+coffeepy.run(60)
 ```
 
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
-
-
```

### Comparing `coffeepy-0.1.1/pyproject.toml` & `coffeepy-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
-  { name="kuvaus", email="kuvaus@users.noreply.github.com" },
+  { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `coffeepy-0.1.1/src/coffeepy/coffeepy.py` & `coffeepy-0.1.2/src/coffeepy/coffeepy.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,28 +28,35 @@
     try:
         subprocess.check_output(['which', 'caffeinate'])
         return True
     except subprocess.CalledProcessError:
         return False
 
 
-def run():
+def run(time=None):
     parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
                                                  'You can set the time with -t flag\n'
                                                  'Made by kuvaus',
                                                  formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-t', '--time', type=int, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
     args = parser.parse_args()
 
     if args.time == 0:
         duration = float('inf')  # Set duration to infinity
     else:
         duration = args.time * 60  # Convert minutes to seconds
-        
+    
+    #if time is provided as run argument, it will overwrite args
+    #this is only relevant when coffeepy is run as a python module
+    if time is None:
+        duration = duration
+    else:
+        duration = time *60
+
     proc = None
 
     if 'darwin' in sys.platform:
         print('Running \'coffeepy\' on MacOS to prevent the system from sleeping')
         proc = subprocess.Popen(['caffeinate', '-dims'])
 
     elif 'linux' in sys.platform:
```

### Comparing `coffeepy-0.1.1/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.2/src/coffeepy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Coffeepy prevents the system from sleeping
-Author-email: kuvaus <kuvaus@users.noreply.github.com>
+Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/coffeepy.svg?style=flat)](https://pypi.python.org/pypi/coffeepy/) [![PyPI Version](https://img.shields.io/pypi/v/coffeepy.svg)](https://pypi.python.org/pypi/coffeepy)
 # Coffeepy
 
 Coffeepy ☕️ is a small program that prevents the system from sleeping.
 Works on MacOS, Windows and Linux.
 
-<img alt="coffeepy" src="https://github.com/kuvaus/coffeepy/assets/22169537/d2954958-4c92-4791-92b9-36e46f448abc.gif" width="600" />
+<img alt="coffeepy" src="https://github-production-user-asset-6210df.s3.amazonaws.com/22169537/253075028-9eaccaca-a567-4bd8-86c1-63d4870664ad.gif" width="600" />
 
 ## Installation
 
 ```sh
 pip install -U coffeepy
 ```
 
@@ -44,15 +45,16 @@
 
 You can also import coffeepy as a python module
 
 ```python
 import coffeepy
 
 coffeepy.run()
+
+# you can also specify the time in minutes
+coffeepy.run(60)
 ```
 
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
-
-
```

