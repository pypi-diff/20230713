# Comparing `tmp/BlaApi-1.7.tar.gz` & `tmp/BlaApi-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.7.tar", last modified: Mon Jul 10 13:04:20 2023, max compression
+gzip compressed data, was "BlaApi-1.8.tar", last modified: Thu Jul 13 20:05:24 2023, max compression
```

## Comparing `BlaApi-1.7.tar` & `BlaApi-1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-10 13:04:20.627675 BlaApi-1.7/
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-10 13:04:20.619675 BlaApi-1.7/BlaApi/
--rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.7/BlaApi/__init__.py
--rw-r--r--   0 muddi     (1000) muddi     (1001)     8185 2023-07-10 13:03:41.000000 BlaApi-1.7/BlaApi/client.py
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-10 13:04:20.624675 BlaApi-1.7/BlaApi.egg-info/
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/SOURCES.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/dependency_links.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)       31 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/requires.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/top_level.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.7/LICENSE
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-10 13:04:20.626675 BlaApi-1.7/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.7/README.md
--rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-07-10 13:04:20.627675 BlaApi-1.7/setup.cfg
--rw-r--r--   0 muddi     (1000) muddi     (1001)     3594 2023-07-10 12:46:26.000000 BlaApi-1.7/setup.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-13 20:05:24.508015 BlaApi-1.8/
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-13 20:05:24.497015 BlaApi-1.8/BlaApi/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.8/BlaApi/__init__.py
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     8231 2023-07-13 20:04:42.000000 BlaApi-1.8/BlaApi/client.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-13 20:05:24.505015 BlaApi-1.8/BlaApi.egg-info/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/SOURCES.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/dependency_links.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       33 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/requires.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/top_level.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.8/LICENSE
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-13 20:05:24.506015 BlaApi-1.8/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.8/README.md
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-07-13 20:05:24.508015 BlaApi-1.8/setup.cfg
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     3596 2023-07-13 20:05:13.000000 BlaApi-1.8/setup.py
```

### Comparing `BlaApi-1.7/BlaApi/client.py` & `BlaApi-1.8/BlaApi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import json
 import httpx
 from fake_useragent import UserAgent as ua
-from html2text import html2text as h2t
+# from html2text import html2text as h2t
+from markdownify import markdownify
 import re
 
 class Client:
     client = httpx.Client(verify=False) # instanciate 
     #! BLA credentials must be passed in as string
     def __init__(self, username: str, password: str):
         # Random UserAgent
@@ -111,15 +112,15 @@
             # error handling
             if json.loads(response.content).get('success') == False:
                 raise ValueError(json.loads(response.content).get('error'))
             
             # Retrieve diary data from JSON response
             data = json.loads(response.content)['data']
             # parse diary details by converting to markdown
-            data['details'] = h2t(data.get('details'))
+            data['details'] = markdownify(data.get('details'))
             
             output.append(data)
 
         return output
     
     def search_by_student(self, passthru=None, student_id=None):
```

### Comparing `BlaApi-1.7/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.8/BlaApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.7
+Version: 1.8
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.7/LICENSE` & `BlaApi-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.7/PKG-INFO` & `BlaApi-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.7
+Version: 1.8
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.7/README.md` & `BlaApi-1.8/README.md`

 * *Files identical despite different names*

### Comparing `BlaApi-1.7/setup.py` & `BlaApi-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.7'
+VERSION = '1.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-     'httpx', 'fake_useragent','html2text'
+     'httpx', 'fake_useragent','markdownify'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

