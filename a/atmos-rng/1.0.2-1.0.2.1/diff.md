# Comparing `tmp/atmos-rng-1.0.2.tar.gz` & `tmp/atmos-rng-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmos-rng-1.0.2.tar", last modified: Wed Jul 12 18:22:48 2023, max compression
+gzip compressed data, was "atmos-rng-1.0.2.1.tar", last modified: Thu Jul 13 15:44:49 2023, max compression
```

## Comparing `atmos-rng-1.0.2.tar` & `atmos-rng-1.0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/atmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/atmos_rng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:44:49.467782 atmos-rng-1.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 15:44:37.000000 atmos-rng-1.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 15:44:49.467782 atmos-rng-1.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 15:44:37.000000 atmos-rng-1.0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-13 15:44:37.000000 atmos-rng-1.0.2.1/atmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:44:49.467782 atmos-rng-1.0.2.1/atmos_rng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 15:44:49.000000 atmos-rng-1.0.2.1/atmos_rng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 15:44:49.000000 atmos-rng-1.0.2.1/atmos_rng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:44:49.000000 atmos-rng-1.0.2.1/atmos_rng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 15:44:49.000000 atmos-rng-1.0.2.1/atmos_rng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 15:44:49.000000 atmos-rng-1.0.2.1/atmos_rng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:44:49.467782 atmos-rng-1.0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-13 15:44:37.000000 atmos-rng-1.0.2.1/setup.py
```

### Comparing `atmos-rng-1.0.2/LICENSE` & `atmos-rng-1.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atmos-rng-1.0.2/PKG-INFO` & `atmos-rng-1.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmos-rng
-Version: 1.0.2
+Version: 1.0.2.1
 Summary: A simple random generator based off of atmospheric noise instead of math.
 Home-page: https://github.com/therealOri/atmos-rng
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `atmos-rng-1.0.2/README.md` & `atmos-rng-1.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `atmos-rng-1.0.2/atmos.py` & `atmos-rng-1.0.2.1/atmos.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,21 +119,21 @@
 
 
 
 def gen_bits(length):
     if not isinstance(length, int):
         raise ValueError(f'\n\nInvalid type, "gen_bits()" takes type "int", value given is "{type(length)}".')
     else:
-        if k == 1:
+        if length == 1:
             bit = randint(0, 1, 1)
             result = 0
             result = (result << 1) | int(bit)
             return result
 
-        elif k > 1:
+        elif length > 1:
             bits = randint(0, 1, length)
             result = 0
             for bit in bits:
                 result = (result << 1) | int(bit)
             return result
 
         else:
```

### Comparing `atmos-rng-1.0.2/atmos_rng.egg-info/PKG-INFO` & `atmos-rng-1.0.2.1/atmos_rng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmos-rng
-Version: 1.0.2
+Version: 1.0.2.1
 Summary: A simple random generator based off of atmospheric noise instead of math.
 Home-page: https://github.com/therealOri/atmos-rng
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `atmos-rng-1.0.2/setup.py` & `atmos-rng-1.0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="atmos-rng",
-    version="1.0.2",
+    version="1.0.2.1",
     author="therealOri",
     license="GPL-3.0",
     install_requires=[
         "requests",
     ],
     author_email="therealOri@duck.com",
     description="A simple random generator based off of atmospheric noise instead of math.",
```

