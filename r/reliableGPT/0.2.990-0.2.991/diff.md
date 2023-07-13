# Comparing `tmp/reliableGPT-0.2.990.tar.gz` & `tmp/reliableGPT-0.2.991.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.990.tar", last modified: Thu Jul 13 20:07:04 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.991.tar", last modified: Thu Jul 13 20:10:28 2023, max compression
```

## Comparing `reliableGPT-0.2.990.tar` & `reliableGPT-0.2.991.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 20:07:04.582752 reliableGPT-0.2.990/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.990/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 20:07:04.582622 reliableGPT-0.2.990/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8826 2023-07-13 16:51:59.000000 reliableGPT-0.2.990/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.990/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 20:07:04.581308 reliableGPT-0.2.990/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 20:07:04.000000 reliableGPT-0.2.990/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 20:07:04.000000 reliableGPT-0.2.990/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 20:07:04.000000 reliableGPT-0.2.990/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 20:07:04.000000 reliableGPT-0.2.990/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 20:07:04.000000 reliableGPT-0.2.990/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 20:07:04.582400 reliableGPT-0.2.990/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3148 2023-07-13 16:49:27.000000 reliableGPT-0.2.990/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    22051 2023-07-13 20:04:41.000000 reliableGPT-0.2.990/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.990/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.990/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5370 2023-07-13 20:01:09.000000 reliableGPT-0.2.990/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 20:07:04.582805 reliableGPT-0.2.990/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 20:06:00.000000 reliableGPT-0.2.990/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 20:10:28.848659 reliableGPT-0.2.991/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.991/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 20:10:28.848527 reliableGPT-0.2.991/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8826 2023-07-13 16:51:59.000000 reliableGPT-0.2.991/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.991/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 20:10:28.847056 reliableGPT-0.2.991/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 20:10:28.000000 reliableGPT-0.2.991/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 20:10:28.000000 reliableGPT-0.2.991/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 20:10:28.000000 reliableGPT-0.2.991/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 20:10:28.000000 reliableGPT-0.2.991/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 20:10:28.000000 reliableGPT-0.2.991/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 20:10:28.848188 reliableGPT-0.2.991/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3148 2023-07-13 16:49:27.000000 reliableGPT-0.2.991/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    22051 2023-07-13 20:04:41.000000 reliableGPT-0.2.991/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.991/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.991/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5368 2023-07-13 20:09:28.000000 reliableGPT-0.2.991/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 20:10:28.848708 reliableGPT-0.2.991/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 20:09:33.000000 reliableGPT-0.2.991/setup.py
```

### Comparing `reliableGPT-0.2.990/LICENSE` & `reliableGPT-0.2.991/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.990/README.md` & `reliableGPT-0.2.991/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.990/reliablegpt/Alerting.py` & `reliableGPT-0.2.991/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.990/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.991/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.990/reliablegpt/Model.py` & `reliableGPT-0.2.991/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.990/reliablegpt/main.py` & `reliableGPT-0.2.991/reliablegpt/main.py`

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
 
-# # Dev Imports
-from IndividualRequest import IndividualRequest
-from Model import Model
-from Alerting import Alerting
+# Dev Imports
+# from IndividualRequest import IndividualRequest
+# from Model import Model
+# from Alerting import Alerting
 
 from posthog import Posthog
 from flask import Flask, request
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
```

