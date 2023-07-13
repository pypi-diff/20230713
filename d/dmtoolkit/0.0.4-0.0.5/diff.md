# Comparing `tmp/dmtoolkit-0.0.4.tar.gz` & `tmp/dmtoolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtoolkit-0.0.4.tar", last modified: Thu Jul 13 17:55:20 2023, max compression
+gzip compressed data, was "dmtoolkit-0.0.5.tar", last modified: Thu Jul 13 18:28:11 2023, max compression
```

## Comparing `dmtoolkit-0.0.4.tar` & `dmtoolkit-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 17:55:20.900513 dmtoolkit-0.0.4/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.4/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 17:55:20.899513 dmtoolkit-0.0.4/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.4/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.4/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.4/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-13 17:55:20.900513 dmtoolkit-0.0.4/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.4/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 17:55:20.894513 dmtoolkit-0.0.4/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 17:55:20.897513 dmtoolkit-0.0.4/src/dmtoolkit/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-13 17:54:41.000000 dmtoolkit-0.0.4/src/dmtoolkit/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 17:55:20.898513 dmtoolkit-0.0.4/src/dmtoolkit/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      101 2023-07-05 17:45:33.000000 dmtoolkit-0.0.4/src/dmtoolkit/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.4/src/dmtoolkit/apis/dndbeyondapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.4/src/dmtoolkit/apis/foundryapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5957 2023-07-11 18:36:58.000000 dmtoolkit-0.0.4/src/dmtoolkit/apis/open5eapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.4/src/dmtoolkit/apis/wikijsapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.4/src/dmtoolkit/dmtools.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 17:55:20.899513 dmtoolkit-0.0.4/src/dmtoolkit/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1958 2023-07-13 16:05:59.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/dndcharacter.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      951 2023-07-13 17:54:09.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/dnditem.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1824 2023-07-11 18:24:05.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/dndmonster.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1521 2023-07-13 17:47:51.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/dndobject.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/dndshop.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1053 2023-07-11 18:24:41.000000 dmtoolkit-0.0.4/src/dmtoolkit/models/dndspell.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 17:55:20.898513 dmtoolkit-0.0.4/src/dmtoolkit.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 17:55:20.000000 dmtoolkit-0.0.4/src/dmtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)      692 2023-07-13 17:55:20.000000 dmtoolkit-0.0.4/src/dmtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-13 17:55:20.000000 dmtoolkit-0.0.4/src/dmtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-13 17:55:20.000000 dmtoolkit-0.0.4/src/dmtoolkit.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-13 17:55:20.000000 dmtoolkit-0.0.4/src/dmtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 18:28:11.698290 dmtoolkit-0.0.5/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.5/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 18:28:11.698290 dmtoolkit-0.0.5/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.5/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.5/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.5/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-13 18:28:11.698290 dmtoolkit-0.0.5/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.5/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 18:28:11.693290 dmtoolkit-0.0.5/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 18:28:11.694290 dmtoolkit-0.0.5/src/dmtoolkit/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-13 18:27:59.000000 dmtoolkit-0.0.5/src/dmtoolkit/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 18:28:11.695290 dmtoolkit-0.0.5/src/dmtoolkit/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      101 2023-07-05 17:45:33.000000 dmtoolkit-0.0.5/src/dmtoolkit/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.5/src/dmtoolkit/apis/dndbeyondapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.5/src/dmtoolkit/apis/foundryapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     5957 2023-07-11 18:36:58.000000 dmtoolkit-0.0.5/src/dmtoolkit/apis/open5eapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.5/src/dmtoolkit/apis/wikijsapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.5/src/dmtoolkit/dmtools.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 18:28:11.697290 dmtoolkit-0.0.5/src/dmtoolkit/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1958 2023-07-13 16:05:59.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/dndcharacter.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      951 2023-07-13 17:54:09.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/dnditem.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1824 2023-07-11 18:24:05.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/dndmonster.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1482 2023-07-13 18:27:44.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/dndobject.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/dndshop.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1053 2023-07-11 18:24:41.000000 dmtoolkit-0.0.5/src/dmtoolkit/models/dndspell.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 18:28:11.695290 dmtoolkit-0.0.5/src/dmtoolkit.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 18:28:11.000000 dmtoolkit-0.0.5/src/dmtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      692 2023-07-13 18:28:11.000000 dmtoolkit-0.0.5/src/dmtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-13 18:28:11.000000 dmtoolkit-0.0.5/src/dmtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-13 18:28:11.000000 dmtoolkit-0.0.5/src/dmtoolkit.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-13 18:28:11.000000 dmtoolkit-0.0.5/src/dmtoolkit.egg-info/top_level.txt
```

### Comparing `dmtoolkit-0.0.4/LICENSE` & `dmtoolkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/PKG-INFO` & `dmtoolkit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.4/README.md` & `dmtoolkit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/pyproject.toml` & `dmtoolkit-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/setup.py` & `dmtoolkit-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/apis/dndbeyondapi.py` & `dmtoolkit-0.0.5/src/dmtoolkit/apis/dndbeyondapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/apis/open5eapi.py` & `dmtoolkit-0.0.5/src/dmtoolkit/apis/open5eapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/apis/wikijsapi.py` & `dmtoolkit-0.0.5/src/dmtoolkit/apis/wikijsapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/dmtools.py` & `dmtoolkit-0.0.5/src/dmtoolkit/dmtools.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/models/dndcharacter.py` & `dmtoolkit-0.0.5/src/dmtoolkit/models/dndcharacter.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/models/dnditem.py` & `dmtoolkit-0.0.5/src/dmtoolkit/models/dnditem.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/models/dndmonster.py` & `dmtoolkit-0.0.5/src/dmtoolkit/models/dndmonster.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/models/dndobject.py` & `dmtoolkit-0.0.5/src/dmtoolkit/models/dndobject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dmtoolkit.db.dndorm import DnDORM
 from dmtoolkit.apis import open5eapi
 
 from autonomous.apis import OpenAI
 from autonomous.storage.cloudinarystorage import CloudinaryStorage
 from autonomous.model.automodel import AutoModel
 from autonomous import log
```

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/models/dndshop.py` & `dmtoolkit-0.0.5/src/dmtoolkit/models/dndshop.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit/models/dndspell.py` & `dmtoolkit-0.0.5/src/dmtoolkit/models/dndspell.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit.egg-info/PKG-INFO` & `dmtoolkit-0.0.5/src/dmtoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.4/src/dmtoolkit.egg-info/SOURCES.txt` & `dmtoolkit-0.0.5/src/dmtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

