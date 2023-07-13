# Comparing `tmp/reliableGPT-0.2.986.tar.gz` & `tmp/reliableGPT-0.2.987.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.986.tar", last modified: Thu Jul 13 15:30:15 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.987.tar", last modified: Thu Jul 13 15:31:34 2023, max compression
```

## Comparing `reliableGPT-0.2.986.tar` & `reliableGPT-0.2.987.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:30:15.378785 reliableGPT-0.2.986/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.986/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 15:30:15.378674 reliableGPT-0.2.986/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.986/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.986/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:30:15.377318 reliableGPT-0.2.986/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 15:30:15.000000 reliableGPT-0.2.986/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 15:30:15.000000 reliableGPT-0.2.986/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 15:30:15.000000 reliableGPT-0.2.986/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 15:30:15.000000 reliableGPT-0.2.986/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 15:30:15.000000 reliableGPT-0.2.986/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:30:15.378366 reliableGPT-0.2.986/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.986/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    21936 2023-07-13 15:26:49.000000 reliableGPT-0.2.986/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.986/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.986/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5288 2023-07-13 15:12:21.000000 reliableGPT-0.2.986/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 15:30:15.378830 reliableGPT-0.2.986/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 15:29:35.000000 reliableGPT-0.2.986/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:31:34.617816 reliableGPT-0.2.987/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.987/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 15:31:34.617629 reliableGPT-0.2.987/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.987/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.987/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:31:34.616514 reliableGPT-0.2.987/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:31:34.617436 reliableGPT-0.2.987/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.987/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    21936 2023-07-13 15:26:49.000000 reliableGPT-0.2.987/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.987/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.987/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5288 2023-07-13 15:30:45.000000 reliableGPT-0.2.987/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 15:31:34.617864 reliableGPT-0.2.987/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 15:31:31.000000 reliableGPT-0.2.987/setup.py
```

### Comparing `reliableGPT-0.2.986/LICENSE` & `reliableGPT-0.2.987/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.986/README.md` & `reliableGPT-0.2.987/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.986/reliablegpt/Alerting.py` & `reliableGPT-0.2.987/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.986/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.987/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.986/reliablegpt/Model.py` & `reliableGPT-0.2.987/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.986/reliablegpt/main.py` & `reliableGPT-0.2.987/reliablegpt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # # Prod Imports
-# from reliablegpt.IndividualRequest import IndividualRequest
-# from reliablegpt.Model import Model
-# from reliablegpt.Alerting import Alerting
+from reliablegpt.IndividualRequest import IndividualRequest
+from reliablegpt.Model import Model
+from reliablegpt.Alerting import Alerting
 import requests
 import asyncio 
 
 # # Dev Imports
-from IndividualRequest import IndividualRequest
-from Model import Model
-from Alerting import Alerting
+# from IndividualRequest import IndividualRequest
+# from Model import Model
+# from Alerting import Alerting
 
 from posthog import Posthog
 from flask import Flask, request
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
```

