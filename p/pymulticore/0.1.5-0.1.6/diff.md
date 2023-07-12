# Comparing `tmp/pymulticore-0.1.5.tar.gz` & `tmp/pymulticore-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymulticore-0.1.5.tar", last modified: Wed Jul 12 19:19:58 2023, max compression
+gzip compressed data, was "pymulticore-0.1.6.tar", last modified: Wed Jul 12 22:53:49 2023, max compression
```

## Comparing `pymulticore-0.1.5.tar` & `pymulticore-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:19:58.505000 pymulticore-0.1.5/
--rw-rw-rw-   0        0        0     2697 2023-07-12 19:19:58.498000 pymulticore-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2452 2023-07-12 19:17:08.000000 pymulticore-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 19:19:58.434000 pymulticore-0.1.5/pymulticore/
--rw-rw-rw-   0        0        0       26 2023-07-09 15:44:29.000000 pymulticore-0.1.5/pymulticore/__init__.py
--rw-rw-rw-   0        0        0      138 2023-07-12 17:56:50.000000 pymulticore-0.1.5/pymulticore/devicestatus.py
--rw-rw-rw-   0        0        0    14675 2023-07-12 19:08:15.000000 pymulticore-0.1.5/pymulticore/pymulticore.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:19:58.488000 pymulticore-0.1.5/pymulticore.egg-info/
--rw-rw-rw-   0        0        0     2697 2023-07-12 19:19:58.000000 pymulticore-0.1.5/pymulticore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-12 19:19:58.000000 pymulticore-0.1.5/pymulticore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:19:58.000000 pymulticore-0.1.5/pymulticore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 19:19:58.000000 pymulticore-0.1.5/pymulticore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 19:19:58.000000 pymulticore-0.1.5/pymulticore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 19:19:58.504000 pymulticore-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-07-12 19:19:51.000000 pymulticore-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:53:49.496000 pymulticore-0.1.6/
+-rw-rw-rw-   0        0        0       79 2023-07-12 22:50:31.000000 pymulticore-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2697 2023-07-12 22:53:49.487000 pymulticore-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2452 2023-07-12 19:17:08.000000 pymulticore-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 22:53:49.226000 pymulticore-0.1.6/pymulticore/
+-rw-rw-rw-   0        0        0       26 2023-07-12 19:24:01.000000 pymulticore-0.1.6/pymulticore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:53:49.312000 pymulticore-0.1.6/pymulticore/c-libraries/
+-rw-rw-rw-   0        0        0    51683 2023-07-12 19:07:18.000000 pymulticore-0.1.6/pymulticore/c-libraries/clib.dll
+drwxrwxrwx   0        0        0        0 2023-07-12 22:53:49.477000 pymulticore-0.1.6/pymulticore/cuda-libraries/
+-rw-rw-rw-   0        0        0   308224 2023-07-12 03:04:43.000000 pymulticore-0.1.6/pymulticore/cuda-libraries/cudalib.dll
+-rw-rw-rw-   0        0        0      138 2023-07-12 17:56:50.000000 pymulticore-0.1.6/pymulticore/devicestatus.py
+-rw-rw-rw-   0        0        0    14675 2023-07-12 19:08:15.000000 pymulticore-0.1.6/pymulticore/pymulticore.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:53:49.295000 pymulticore-0.1.6/pymulticore.egg-info/
+-rw-rw-rw-   0        0        0     2697 2023-07-12 22:53:48.000000 pymulticore-0.1.6/pymulticore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-12 22:53:49.000000 pymulticore-0.1.6/pymulticore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:53:48.000000 pymulticore-0.1.6/pymulticore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 22:53:48.000000 pymulticore-0.1.6/pymulticore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 22:53:49.000000 pymulticore-0.1.6/pymulticore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 22:53:49.494000 pymulticore-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-07-12 22:51:51.000000 pymulticore-0.1.6/setup.py
```

### Comparing `pymulticore-0.1.5/PKG-INFO` & `pymulticore-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymulticore
-Version: 0.1.5
+Version: 0.1.6
 Summary: A secure python library for parallelizing tasks across several CPU cores
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # Warning, Not ready for use!!
```

### Comparing `pymulticore-0.1.5/README.md` & `pymulticore-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pymulticore-0.1.5/pymulticore/pymulticore.py` & `pymulticore-0.1.6/pymulticore/pymulticore.py`

 * *Files identical despite different names*

### Comparing `pymulticore-0.1.5/pymulticore.egg-info/PKG-INFO` & `pymulticore-0.1.6/pymulticore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymulticore
-Version: 0.1.5
+Version: 0.1.6
 Summary: A secure python library for parallelizing tasks across several CPU cores
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # Warning, Not ready for use!!
```

### Comparing `pymulticore-0.1.5/setup.py` & `pymulticore-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pymulticore',
-    version='0.1.5',
+    version='0.1.6',
     description='A secure python library for parallelizing tasks across several CPU cores',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='Anish Kanthamneni',
     packages=find_packages(),
     package_data={
         '': ['*.dll'],
```

