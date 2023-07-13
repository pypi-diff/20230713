# Comparing `tmp/ossit-0.2.1.tar.gz` & `tmp/ossit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossit-0.2.1.tar", last modified: Wed Jul 12 23:00:50 2023, max compression
+gzip compressed data, was "ossit-0.2.2.tar", last modified: Thu Jul 13 16:16:32 2023, max compression
```

## Comparing `ossit-0.2.1.tar` & `ossit-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 23:00:36.000000 ossit-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 23:00:50.520480 ossit-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-12 23:00:36.000000 ossit-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/ossit/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/ossit/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_resources/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_resources/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/ossit_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/ossit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 23:00:36.000000 ossit-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 23:00:50.520480 ossit-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:00:36.000000 ossit-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:16:32.686318 ossit-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 16:16:19.000000 ossit-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-13 16:16:32.686318 ossit-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-13 16:16:19.000000 ossit-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:16:32.686318 ossit-0.2.2/ossit/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:16:32.686318 ossit-0.2.2/ossit/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/api_resources/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/api_resources/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/ossit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-13 16:16:19.000000 ossit-0.2.2/ossit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:16:32.686318 ossit-0.2.2/ossit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-13 16:16:32.000000 ossit-0.2.2/ossit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 16:16:32.000000 ossit-0.2.2/ossit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:16:32.000000 ossit-0.2.2/ossit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 16:16:32.000000 ossit-0.2.2/ossit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 16:16:19.000000 ossit-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 16:16:32.686318 ossit-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:16:19.000000 ossit-0.2.2/setup.py
```

### Comparing `ossit-0.2.1/LICENSE.txt` & `ossit-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ossit-0.2.1/PKG-INFO` & `ossit-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Package to connect to ossit API
 Author: Wesley Howery
 Author-email: wesleyh@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ossit-0.2.1/README.md` & `ossit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ossit-0.2.1/ossit/api_requestor.py` & `ossit-0.2.2/ossit/api_requestor.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.1/ossit/api_resources/domain.py` & `ossit-0.2.2/ossit/api_resources/domain.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.1/ossit/api_resources/statistic.py` & `ossit-0.2.2/ossit/api_resources/statistic.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.1/ossit/config.py` & `ossit-0.2.2/ossit/config.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.1/ossit/utils.py` & `ossit-0.2.2/ossit/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from typing import Callable
 from concurrent.futures import ThreadPoolExecutor
 
 
-def send_non_blocking_request(ossit_request: Callable[..., any], **callable_kwargs) -> None:
+class OssitRequest:
+    def __init__(self, ossit_api_requestor: Callable[..., any], **kwargs):
+        self.ossit_api_requestor = ossit_api_requestor
+        self.kwargs = kwargs
 
-    def make_request(ossit_request: Callable[..., any], **callable_kwargs) -> None:
-        ossit_request(**callable_kwargs)
+    def __call__(self, *args, **kwargs):
+        self.ossit_api_requestor(**self.kwargs)
+
+
+def send_threaded_requests(*ossit_requests: OssitRequest) -> None:
 
     # Create an executor and start the request in a new thread
-    executor = ThreadPoolExecutor(max_workers=1)
-    executor.submit(make_request, ossit_request, **callable_kwargs)
+    executor = ThreadPoolExecutor(max_workers=5)
+    for ossit_request in ossit_requests:
+        executor.submit(ossit_request)
+
     # Shutdown the executor. This doesn't block the running request
     executor.shutdown(wait=False)
```

### Comparing `ossit-0.2.1/ossit.egg-info/PKG-INFO` & `ossit-0.2.2/ossit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Package to connect to ossit API
 Author: Wesley Howery
 Author-email: wesleyh@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ossit-0.2.1/setup.cfg` & `ossit-0.2.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ossit
-version = 0.2.1
+version = 0.2.2
 author = Wesley Howery
 author_email = wesleyh@stratusadv.com
 description = Python Package to connect to ossit API
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

