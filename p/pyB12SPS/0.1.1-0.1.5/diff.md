# Comparing `tmp/pyB12SPS-0.1.1.tar.gz` & `tmp/pyB12SPS-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyB12SPS-0.1.1.tar", last modified: Tue Jun 13 16:08:54 2023, max compression
+gzip compressed data, was "pyB12SPS-0.1.5.tar", last modified: Thu Jul 13 09:44:03 2023, max compression
```

## Comparing `pyB12SPS-0.1.1.tar` & `pyB12SPS-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:54.019988 pyB12SPS-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-13 16:08:54.019988 pyB12SPS-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:54.015988 pyB12SPS-0.1.1/pyB12SPS/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/pyB12SPS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/pyB12SPS/pyB12SPS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/pyB12SPS/pyB12SPSGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/pyB12SPS/pyB12SPSGUI.ui
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/pyB12SPS/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:54.019988 pyB12SPS-0.1.1/pyB12SPS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-13 16:08:54.000000 pyB12SPS-0.1.1/pyB12SPS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 16:08:54.000000 pyB12SPS-0.1.1/pyB12SPS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:08:54.000000 pyB12SPS-0.1.1/pyB12SPS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 16:08:54.000000 pyB12SPS-0.1.1/pyB12SPS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 16:08:54.000000 pyB12SPS-0.1.1/pyB12SPS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 16:08:54.000000 pyB12SPS-0.1.1/pyB12SPS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:08:54.019988 pyB12SPS-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-13 16:08:38.000000 pyB12SPS-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:44:03.561858 pyB12SPS-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 09:44:03.557858 pyB12SPS-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:44:03.557858 pyB12SPS-0.1.5/pyB12SPS/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/pyB12SPS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/pyB12SPS/pyB12SPS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/pyB12SPS/pyB12SPSGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/pyB12SPS/pyB12SPSGUI.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:44:03.557858 pyB12SPS-0.1.5/pyB12SPS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 09:44:03.000000 pyB12SPS-0.1.5/pyB12SPS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 09:44:03.000000 pyB12SPS-0.1.5/pyB12SPS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:44:03.000000 pyB12SPS-0.1.5/pyB12SPS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 09:44:03.000000 pyB12SPS-0.1.5/pyB12SPS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 09:44:03.000000 pyB12SPS-0.1.5/pyB12SPS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 09:44:03.000000 pyB12SPS-0.1.5/pyB12SPS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:44:03.561858 pyB12SPS-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-13 09:43:53.000000 pyB12SPS-0.1.5/setup.py
```

### Comparing `pyB12SPS-0.1.1/LICENSE.txt` & `pyB12SPS-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyB12SPS-0.1.1/PKG-INFO` & `pyB12SPS-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyB12SPS
-Version: 0.1.1
+Version: 0.1.5
 Summary: A Python Package for Interfacing with the Bridge12 Shim Power Supply
 Home-page: http://www.bridge12.com/
 Author: Bridge12 Technologies, Inc
 Author-email: yhuang@bridge12.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyB12SPS-0.1.1/pyB12SPS/pyB12SPS.py` & `pyB12SPS-0.1.5/pyB12SPS/pyB12SPS.py`

 * *Files identical despite different names*

### Comparing `pyB12SPS-0.1.1/pyB12SPS/pyB12SPSGUI.py` & `pyB12SPS-0.1.5/pyB12SPS/pyB12SPSGUI.py`

 * *Files identical despite different names*

### Comparing `pyB12SPS-0.1.1/pyB12SPS/pyB12SPSGUI.ui` & `pyB12SPS-0.1.5/pyB12SPS/pyB12SPSGUI.ui`

 * *Files identical despite different names*

### Comparing `pyB12SPS-0.1.1/pyB12SPS.egg-info/PKG-INFO` & `pyB12SPS-0.1.5/pyB12SPS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyB12SPS
-Version: 0.1.1
+Version: 0.1.5
 Summary: A Python Package for Interfacing with the Bridge12 Shim Power Supply
 Home-page: http://www.bridge12.com/
 Author: Bridge12 Technologies, Inc
 Author-email: yhuang@bridge12.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyB12SPS-0.1.1/setup.py` & `pyB12SPS-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup
 
 with open('README.md','r') as f:
     long_description = f.read()
 
 setup(
     name='pyB12SPS',
-    version= "0.1.1",
+    version= "0.1.5",
     author='Bridge12 Technologies, Inc',
     author_email='yhuang@bridge12.com',
     description='A Python Package for Interfacing with the Bridge12 Shim Power Supply',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='http://www.bridge12.com/',
     project_urls={
```

