# Comparing `tmp/proteusPy-0.74.tar.gz` & `tmp/proteusPy-0.74b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteusPy-0.74.tar", last modified: Wed Jul 12 22:41:40 2023, max compression
+gzip compressed data, was "proteusPy-0.74b0.tar", last modified: Wed Jul 12 22:56:22 2023, max compression
```

## Comparing `proteusPy-0.74.tar` & `proteusPy-0.74b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:41:40.507990 proteusPy-0.74/
--rw-r--r--   0 egs        (505) staff       (20)       65 2023-07-09 01:16:52.000000 proteusPy-0.74/MANIFEST.in
--rw-r--r--   0 egs        (505) staff       (20)     5279 2023-07-12 22:41:40.508065 proteusPy-0.74/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)     4141 2023-07-05 01:07:02.000000 proteusPy-0.74/README.md
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:41:40.504658 proteusPy-0.74/proteusPy/
--rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.74/proteusPy/Disulfide.py
--rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.74/proteusPy/DisulfideClass_Constructor.py
--rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.74/proteusPy/DisulfideClasses.py
--rw-r--r--   0 egs        (505) staff       (20)     1027 2023-07-11 00:53:43.000000 proteusPy-0.74/proteusPy/DisulfideExceptions.py
--rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.74/proteusPy/DisulfideList.py
--rw-r--r--   0 egs        (505) staff       (20)    23705 2023-07-06 15:13:40.000000 proteusPy-0.74/proteusPy/DisulfideLoader.py
--rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.74/proteusPy/ProteusGlobals.py
--rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.74/proteusPy/ProteusPyWarning.py
--rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.74/proteusPy/Residue.py
--rw-r--r--   0 egs        (505) staff       (20)     1641 2023-07-12 21:25:45.000000 proteusPy-0.74/proteusPy/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.74/proteusPy/angle_annotation.py
--rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.74/proteusPy/atoms.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:41:40.507630 proteusPy-0.74/proteusPy/data/
--rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-04 13:46:04.000000 proteusPy-0.74/proteusPy/data/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.74/proteusPy/data/ss_completed.txt
--rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.74/proteusPy/data/ss_ids.txt
--rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.74/proteusPy/data/ss_query.json
--rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.74/proteusPy/turtle3D.py
--rw-r--r--   0 egs        (505) staff       (20)    12468 2023-07-11 00:53:43.000000 proteusPy-0.74/proteusPy/utility.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:41:40.505840 proteusPy-0.74/proteusPy.egg-info/
--rw-r--r--   0 egs        (505) staff       (20)     5279 2023-07-12 22:41:40.000000 proteusPy-0.74/proteusPy.egg-info/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)      776 2023-07-12 22:41:40.000000 proteusPy-0.74/proteusPy.egg-info/SOURCES.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-12 22:41:40.000000 proteusPy-0.74/proteusPy.egg-info/dependency_links.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.74/proteusPy.egg-info/not-zip-safe
--rw-r--r--   0 egs        (505) staff       (20)       57 2023-07-12 22:41:40.000000 proteusPy-0.74/proteusPy.egg-info/requires.txt
--rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-12 22:41:40.000000 proteusPy-0.74/proteusPy.egg-info/top_level.txt
--rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-12 22:41:40.508283 proteusPy-0.74/setup.cfg
--rw-r--r--   0 egs        (505) staff       (20)     3706 2023-07-12 21:27:03.000000 proteusPy-0.74/setup.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.034607 proteusPy-0.74b0/
+-rw-r--r--   0 egs        (505) staff       (20)       65 2023-07-09 01:16:52.000000 proteusPy-0.74b0/MANIFEST.in
+-rw-r--r--   0 egs        (505) staff       (20)     5281 2023-07-12 22:56:22.034685 proteusPy-0.74b0/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)     4141 2023-07-05 01:07:02.000000 proteusPy-0.74b0/README.md
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.030958 proteusPy-0.74b0/proteusPy/
+-rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.74b0/proteusPy/Disulfide.py
+-rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.74b0/proteusPy/DisulfideClass_Constructor.py
+-rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.74b0/proteusPy/DisulfideClasses.py
+-rw-r--r--   0 egs        (505) staff       (20)     1027 2023-07-11 00:53:43.000000 proteusPy-0.74b0/proteusPy/DisulfideExceptions.py
+-rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.74b0/proteusPy/DisulfideList.py
+-rw-r--r--   0 egs        (505) staff       (20)    23705 2023-07-06 15:13:40.000000 proteusPy-0.74b0/proteusPy/DisulfideLoader.py
+-rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.74b0/proteusPy/ProteusGlobals.py
+-rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.74b0/proteusPy/ProteusPyWarning.py
+-rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.74b0/proteusPy/Residue.py
+-rw-r--r--   0 egs        (505) staff       (20)     1642 2023-07-12 22:55:58.000000 proteusPy-0.74b0/proteusPy/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.74b0/proteusPy/angle_annotation.py
+-rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.74b0/proteusPy/atoms.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.034251 proteusPy-0.74b0/proteusPy/data/
+-rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-04 13:46:04.000000 proteusPy-0.74b0/proteusPy/data/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.74b0/proteusPy/data/ss_completed.txt
+-rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.74b0/proteusPy/data/ss_ids.txt
+-rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.74b0/proteusPy/data/ss_query.json
+-rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.74b0/proteusPy/turtle3D.py
+-rw-r--r--   0 egs        (505) staff       (20)    12468 2023-07-11 00:53:43.000000 proteusPy-0.74b0/proteusPy/utility.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.032138 proteusPy-0.74b0/proteusPy.egg-info/
+-rw-r--r--   0 egs        (505) staff       (20)     5281 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)      776 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/SOURCES.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/dependency_links.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.74b0/proteusPy.egg-info/not-zip-safe
+-rw-r--r--   0 egs        (505) staff       (20)       47 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/requires.txt
+-rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/top_level.txt
+-rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-12 22:56:22.034908 proteusPy-0.74b0/setup.cfg
+-rw-r--r--   0 egs        (505) staff       (20)     3693 2023-07-12 22:55:43.000000 proteusPy-0.74b0/setup.py
```

### Comparing `proteusPy-0.74/PKG-INFO` & `proteusPy-0.74b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.74
+Version: 0.74b0
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
```

### Comparing `proteusPy-0.74/README.md` & `proteusPy-0.74b0/README.md`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/Disulfide.py` & `proteusPy-0.74b0/proteusPy/Disulfide.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/DisulfideClass_Constructor.py` & `proteusPy-0.74b0/proteusPy/DisulfideClass_Constructor.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/DisulfideClasses.py` & `proteusPy-0.74b0/proteusPy/DisulfideClasses.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/DisulfideExceptions.py` & `proteusPy-0.74b0/proteusPy/DisulfideExceptions.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/DisulfideList.py` & `proteusPy-0.74b0/proteusPy/DisulfideList.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/DisulfideLoader.py` & `proteusPy-0.74b0/proteusPy/DisulfideLoader.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/ProteusGlobals.py` & `proteusPy-0.74b0/proteusPy/ProteusGlobals.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/Residue.py` & `proteusPy-0.74b0/proteusPy/Residue.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/__init__.py` & `proteusPy-0.74b0/proteusPy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Eric G. Suchanek, PhD., all rights reserved
 # Subject to the MIT public license.
 
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.74"
+__version__ = "0.74b"
 
 import sys
 import os
 import glob
 import warnings
 import copy
```

### Comparing `proteusPy-0.74/proteusPy/angle_annotation.py` & `proteusPy-0.74b0/proteusPy/angle_annotation.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/atoms.py` & `proteusPy-0.74b0/proteusPy/atoms.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/data/__init__.py` & `proteusPy-0.74b0/proteusPy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/data/ss_completed.txt` & `proteusPy-0.74b0/proteusPy/data/ss_completed.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/data/ss_ids.txt` & `proteusPy-0.74b0/proteusPy/data/ss_ids.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/data/ss_query.json` & `proteusPy-0.74b0/proteusPy/data/ss_query.json`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/turtle3D.py` & `proteusPy-0.74b0/proteusPy/turtle3D.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy/utility.py` & `proteusPy-0.74b0/proteusPy/utility.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/proteusPy.egg-info/PKG-INFO` & `proteusPy-0.74b0/proteusPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.74
+Version: 0.74b0
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
```

### Comparing `proteusPy-0.74/proteusPy.egg-info/SOURCES.txt` & `proteusPy-0.74b0/proteusPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74/setup.py` & `proteusPy-0.74b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
       long_description_content_type='text/markdown',
       url='https://github.com/suchanek/proteusPy/',
       author='Eric G. Suchanek, PhD',
       author_email='suchanek@mac.com',
       license='MIT',
       packages=['proteusPy'],
       keywords='proteus suchanek disulfide',
-      install_requires=['pandas', 'numpy', 'matplotlib', 'pyvista', 'pip', 'tqdm', 'gdown', 'ipyvtlink'],
+      install_requires=['pandas', 'numpy', 'matplotlib', 'pyvista', 'pip', 'tqdm', 'gdown'],
       source='https://github.com/suchanek/proteusPy/',
       project_urls={
         "Documentation": "https://suchanek.github.io/proteusPy/",
         "Source": "https://github.com/suchanek/proteusPy/",
         "Tracker": "https://github.com/suchanek/proteusPy/issues",
       },
       classifiers=[
```

