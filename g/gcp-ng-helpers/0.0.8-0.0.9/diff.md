# Comparing `tmp/gcp_ng_helpers-0.0.8.tar.gz` & `tmp/gcp_ng_helpers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_ng_helpers-0.0.8.tar", last modified: Tue Jul  4 14:58:33 2023, max compression
+gzip compressed data, was "gcp_ng_helpers-0.0.9.tar", last modified: Wed Jul  5 09:02:48 2023, max compression
```

## Comparing `gcp_ng_helpers-0.0.8.tar` & `gcp_ng_helpers-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-04 14:58:33.593765 gcp_ng_helpers-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/firestore/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/firestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/firestore/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/functions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/functions/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 14:58:33.593765 gcp_ng_helpers-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:48.473689 gcp_ng_helpers-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-05 09:02:48.473689 gcp_ng_helpers-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:48.469689 gcp_ng_helpers-0.0.9/gcp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:48.469689 gcp_ng_helpers-0.0.9/gcp_helpers/cloud_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/cloud_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/cloud_tasks/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:48.469689 gcp_ng_helpers-0.0.9/gcp_helpers/firestore/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/firestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/firestore/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:48.469689 gcp_ng_helpers-0.0.9/gcp_helpers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/functions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/gcp_helpers/functions/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:02:48.473689 gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-05 09:02:48.000000 gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 09:02:48.000000 gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:02:48.000000 gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 09:02:48.000000 gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 09:02:48.000000 gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-05 09:02:24.000000 gcp_ng_helpers-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-05 09:02:48.473689 gcp_ng_helpers-0.0.9/setup.cfg
```

### Comparing `gcp_ng_helpers-0.0.8/LICENSE` & `gcp_ng_helpers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.8/PKG-INFO` & `gcp_ng_helpers-0.0.9/gcp_ng_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gcp_ng_helpers
-Version: 0.0.8
+Name: gcp-ng-helpers
+Version: 0.0.9
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `gcp_ng_helpers-0.0.8/README.md` & `gcp_ng_helpers-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/manager.py` & `gcp_ng_helpers-0.0.9/gcp_helpers/cloud_tasks/manager.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.8/gcp_helpers/firestore/collections.py` & `gcp_ng_helpers-0.0.9/gcp_helpers/firestore/collections.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from dataclasses import field, dataclass
 from typing import Generator, Any
 
 from google.cloud import firestore
 from google.oauth2 import service_account
 
 
 def get_firestore_client(project) -> firestore.Client:
@@ -65,14 +66,26 @@
             }
             if append_id:
                 item[doc.id]["docId"] = doc.id
             res.update(item)
         return res
 
 
+@dataclass
+class FirestoreOrderBy:
+    field_path: str
+    direction: str = field(default=firestore.Query.ASCENDING)
+
+    def ASC(self):
+        self.direction = firestore.Query.ASCENDING
+
+    def DESC(self):
+        self.direction = firestore.Query.DESCENDING
+
+
 class FirestoreFilter(list):
     ALLOWED_OP = [
         "<",
         "<=",
         "==",
         ">",
         ">=",
@@ -95,21 +108,27 @@
         self._col_ref = self._cli.collection(collection_name)
 
     def get_all(self):
         stream = self._col_ref.stream()
 
         return FirestoreMultiResult(stream)
 
-    def search(self, filter_query: FirestoreFilter | list[FirestoreFilter]):
+    def search(self, filter_query: FirestoreFilter | list[FirestoreFilter],
+               order_by: FirestoreOrderBy | None = None, limit: int | None = None):
         query = self._col_ref
         if isinstance(filter_query, list):
             for f in filter_query:
                 query = query.where(*f)
         else:
             query = self._col_ref.where(*filter_query)
+        if order_by:
+            query = query.order_by(order_by.field_path, direction=order_by.direction)
+        if limit:
+            query = query.limit(limit)
+
         stream = query.stream()
         return FirestoreMultiResult(stream)
 
     def get_one(self, docId):
         doc_ref = self._col_ref.document(docId)
         doc = doc_ref.get()
         if doc and doc.exists:
@@ -151,13 +170,13 @@
         document = doc_ref.get()
         if document and document.exists:
             return FirestoreResult(document)
         else:
             return None
 
     def get_first_from_stream(self, docId):
-        query = self._col_ref.stream()
+        query = self._col_ref.limit(1).stream()
         document = next((doc for doc in query if doc.id == docId), None)
         if document and document.exists:
             return FirestoreResult(document)
         else:
             return None
```

### Comparing `gcp_ng_helpers-0.0.8/gcp_helpers/functions/decorators.py` & `gcp_ng_helpers-0.0.9/gcp_helpers/functions/decorators.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.8/gcp_helpers/functions/routers.py` & `gcp_ng_helpers-0.0.9/gcp_helpers/functions/routers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 import json
+import traceback
 from collections import defaultdict
+from functools import wraps
 from typing import Callable
 
 from flask import Request, make_response, Response
 
 
 class HttpRouter:
     def __init__(self, prefix=''):
         self.__route_prefix = self._strip_path(prefix)
         self._routes = defaultdict(dict)
 
-    def route(self, path: str, method: str = 'GET') -> Callable:
+    @staticmethod
+    def _error_handling_decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except Exception as e:
+                print(traceback.format_exc())
+                # Handle the error and return an appropriate response
+                error_message = f"An error occurred: {str(e)}"
+                return make_response(error_message, 500)
+
+        return wrapper
+
+    def route(self, path: str, method: str = 'GET', error_handling: bool = True) -> Callable:
         def decorator(func: Callable) -> Callable:
             formatted_path = self._format_path(path)
+            if error_handling:
+                func = self._error_handling_decorator(func)
             self.register(func, formatted_path, method)
             return func
 
         return decorator
 
     @staticmethod
     def _strip_path(path: str):
```

### Comparing `gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/PKG-INFO` & `gcp_ng_helpers-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gcp-ng-helpers
-Version: 0.0.8
+Name: gcp_ng_helpers
+Version: 0.0.9
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `gcp_ng_helpers-0.0.8/setup.cfg` & `gcp_ng_helpers-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_file = LICENSE
 name = gcp_ng_helpers
-version = 0.0.8
+version = 0.0.9
 author = Dmitriy Tischenko aka NGhost
 author_email = nghostik@gmail.com
 description = Various helper functions for Google Cloud services
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/NGhostClub/gcp-helpers
 project_urls =
```

