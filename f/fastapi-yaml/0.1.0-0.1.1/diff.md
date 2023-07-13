# Comparing `tmp/fastapi_yaml-0.1.0.tar.gz` & `tmp/fastapi_yaml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_yaml-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_yaml-0.1.1.tar", max compression
```

## Comparing `fastapi_yaml-0.1.0.tar` & `fastapi_yaml-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1008 2023-07-13 15:24:33.747218 fastapi_yaml-0.1.0/README.md
--rw-r--r--   0        0        0       41 2023-07-13 14:55:47.229802 fastapi_yaml-0.1.0/fastapi_yaml/__init__.py
--rw-r--r--   0        0        0      950 2023-07-13 15:01:10.251015 fastapi_yaml-0.1.0/fastapi_yaml/main.py
--rw-r--r--   0        0        0      533 2023-07-13 15:18:57.632047 fastapi_yaml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 fastapi_yaml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-13 15:43:10.046115 fastapi_yaml-0.1.1/README.md
+-rw-r--r--   0        0        0       49 2023-07-13 15:42:07.820796 fastapi_yaml-0.1.1/fastapi_yaml/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-13 15:41:58.989542 fastapi_yaml-0.1.1/fastapi_yaml/main.py
+-rw-r--r--   0        0        0      470 2023-07-13 15:44:26.950939 fastapi_yaml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 fastapi_yaml-0.1.1/PKG-INFO
```

### Comparing `fastapi_yaml-0.1.0/README.md` & `fastapi_yaml-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -34,18 +34,24 @@
 ```bash
 curl --request POST \
   --url http://localhost:8000/person \
   --header "content-type: application/x-yaml" \
   --data "name: John Doe\nage: 42"
 ```
 
-# Coverage
+# Tests
+
+```bash
+poetry run pytest --cov fastapi_yaml tests/
+```
+
+## Coverage
 
 ```text
 ---------- coverage: platform darwin, python 3.11.2-final-0 ----------
 Name                       Stmts   Miss  Cover
 ----------------------------------------------
 fastapi_yaml/__init__.py       1      0   100%
 fastapi_yaml/main.py          20      0   100%
 ----------------------------------------------
 TOTAL                         21      0   100%
-```
+```
```

### Comparing `fastapi_yaml-0.1.0/fastapi_yaml/main.py` & `fastapi_yaml-0.1.1/fastapi_yaml/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Callable
 
 import yaml
-from fastapi import Body, FastAPI, Request, Response
+from fastapi import Request, Response
 from fastapi.routing import APIRoute
-from pydantic import BaseModel, Extra
 
 
 class YamlRequest(Request):
     async def body(self) -> bytes:
         if not hasattr(self, "_body"):
             body = await super().body()
             if self.headers.get("content-type") in [
```

### Comparing `fastapi_yaml-0.1.0/PKG-INFO` & `fastapi_yaml-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-yaml
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Mohamed Cherkaoui
 Author-email: chermed@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
@@ -47,18 +47,25 @@
 ```bash
 curl --request POST \
   --url http://localhost:8000/person \
   --header "content-type: application/x-yaml" \
   --data "name: John Doe\nage: 42"
 ```
 
-# Coverage
+# Tests
+
+```bash
+poetry run pytest --cov fastapi_yaml tests/
+```
+
+## Coverage
 
 ```text
 ---------- coverage: platform darwin, python 3.11.2-final-0 ----------
 Name                       Stmts   Miss  Cover
 ----------------------------------------------
 fastapi_yaml/__init__.py       1      0   100%
 fastapi_yaml/main.py          20      0   100%
 ----------------------------------------------
 TOTAL                         21      0   100%
 ```
+
```

