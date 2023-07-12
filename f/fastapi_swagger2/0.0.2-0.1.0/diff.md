# Comparing `tmp/fastapi_swagger2-0.0.2.tar.gz` & `tmp/fastapi_swagger2-0.1.0.tar.gz`

## Comparing `fastapi_swagger2-0.0.2.tar` & `fastapi_swagger2-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/requirements.txt
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/scripts/build.sh
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/scripts/clean.sh
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/scripts/format.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/scripts/lint.sh
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/scripts/publish.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/scripts/test.sh
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/src/fastapi_swagger2/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/src/fastapi_swagger2/constants.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/src/fastapi_swagger2/models.py
--rw-r--r--   0        0        0    18893 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/src/fastapi_swagger2/utils.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/README.md
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/requirements.txt
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/scripts/build.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/scripts/clean.sh
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/scripts/format.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/scripts/test.sh
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/src/fastapi_swagger2/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/src/fastapi_swagger2/constants.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/src/fastapi_swagger2/models.py
+-rw-r--r--   0        0        0    18673 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/src/fastapi_swagger2/utils.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/README.md
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 fastapi_swagger2-0.1.0/PKG-INFO
```

### Comparing `fastapi_swagger2-0.0.2/src/fastapi_swagger2/__init__.py` & `fastapi_swagger2-0.1.0/src/fastapi_swagger2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 from typing import Any, Dict, List, Optional, TypeVar
 
 from fastapi import FastAPI
 from fastapi.openapi.docs import (
     get_redoc_html,
     get_swagger_ui_html,
```

### Comparing `fastapi_swagger2-0.0.2/src/fastapi_swagger2/models.py` & `fastapi_swagger2-0.1.0/src/fastapi_swagger2/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.2/src/fastapi_swagger2/utils.py` & `fastapi_swagger2-0.1.0/src/fastapi_swagger2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,17 +169,15 @@
         )[0]
         if field_info.in_.value == "body":
             parameter["schema"] = schema
         else:
             parameter.update({k: v for (k, v) in schema.items() if k != "title"})
         if field_info.description:
             parameter["description"] = field_info.description
-        if field_info.examples:
-            parameter["examples"] = jsonable_encoder(field_info.examples)
-        elif field_info.example != Undefined:
+        if field_info.example != Undefined:
             parameter["example"] = jsonable_encoder(field_info.example)
         if field_info.deprecated:
             parameter["deprecated"] = field_info.deprecated
         parameters.append(parameter)
     return parameters
 
 
@@ -200,17 +198,15 @@
     request_body_oai: Dict[str, Any] = {}
     request_body_oai["name"] = body_field.alias
     request_body_oai["in"] = "body"
     if required:
         request_body_oai["required"] = required
 
     request_media_content: Dict[str, Any] = {"schema": body_schema}
-    if field_info.examples:
-        request_media_content["examples"] = jsonable_encoder(field_info.examples)
-    elif field_info.example != Undefined:
+    if field_info.example != Undefined:
         request_media_content["example"] = jsonable_encoder(field_info.example)
     # request_body_oai["content"] = {request_media_type: request_media_content}
     request_body_oai.update(request_media_content)
     return request_body_oai
 
 
 def get_swagger2_path(
```

### Comparing `fastapi_swagger2-0.0.2/.gitignore` & `fastapi_swagger2-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.2/LICENSE` & `fastapi_swagger2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.2/README.md` & `fastapi_swagger2-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ---
 
 ## Requirements
 
 Python 3.8+
 
 0.0.2 - FastAPI >= 0.79.0, <= 0.98.0
+0.1.0 - FastAPI >= 0.99.0, <= 0.99.1
 
 ## Installation
 
 <div class="termy">
 
 ```console
 $ pip install fastapi_swagger2
```

### Comparing `fastapi_swagger2-0.0.2/pyproject.toml` & `fastapi_swagger2-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
-    "fastapi >=0.79.0,<=0.98.0",
+    "fastapi >=0.99.0,<=0.99.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/virajkanwade/fastapi_swagger2"
 Documentation = "https://github.com/virajkanwade/fastapi_swagger2"
```

### Comparing `fastapi_swagger2-0.0.2/PKG-INFO` & `fastapi_swagger2-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_swagger2
-Version: 0.0.2
+Version: 0.1.0
 Summary: Swagger2 support for FastAPI framework
 Project-URL: Homepage, https://github.com/virajkanwade/fastapi_swagger2
 Project-URL: Documentation, https://github.com/virajkanwade/fastapi_swagger2
 Author-email: Viraj Kanwade <virajk.oib@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Viraj Kanwade
@@ -48,15 +48,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: fastapi<=0.98.0,>=0.79.0
+Requires-Dist: fastapi<=0.99.1,>=0.99.0
 Provides-Extra: all
 Requires-Dist: httpx>=0.23.0; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: ruff==0.0.272; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: coverage[toml]<8.0,>=6.5.0; extra == 'test'
@@ -89,14 +89,15 @@
 ---
 
 ## Requirements
 
 Python 3.8+
 
 0.0.2 - FastAPI >= 0.79.0, <= 0.98.0
+0.1.0 - FastAPI >= 0.99.0, <= 0.99.1
 
 ## Installation
 
 <div class="termy">
 
 ```console
 $ pip install fastapi_swagger2
```

