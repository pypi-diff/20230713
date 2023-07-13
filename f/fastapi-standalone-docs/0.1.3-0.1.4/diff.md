# Comparing `tmp/fastapi_standalone_docs-0.1.3.tar.gz` & `tmp/fastapi_standalone_docs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_standalone_docs-0.1.3.tar", max compression
+gzip compressed data, was "fastapi_standalone_docs-0.1.4.tar", max compression
```

## Comparing `fastapi_standalone_docs-0.1.3.tar` & `fastapi_standalone_docs-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/LICENSE
--rw-r--r--   0        0        0     4609 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/README.md
--rw-r--r--   0        0        0       82 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/__init__.py
--rw-r--r--   0        0        0     1828 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/scripts.py
--rw-r--r--   0        0        0     2759 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/standalone_docs.py
--rw-r--r--   0        0        0     1086 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/fastapi/LICENSE
--rw-r--r--   0        0        0      412 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/fastapi/favicon.png
--rw-r--r--   0        0        0     1174 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/logo-mini.svg
--rw-r--r--   0        0        0  1042510 2023-06-30 12:21:39.148592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js
--rw-r--r--   0        0        0     2628 2023-06-30 12:21:39.148592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0        0        0    11358 2023-06-30 12:21:39.148592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/LICENSE
--rw-r--r--   0        0        0  1048219 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
--rw-r--r--   0        0        0   145206 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui.css
--rw-r--r--   0        0        0        0 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/conftests.py
--rw-r--r--   0        0        0     6131 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/test_standalone_docs.py
--rw-r--r--   0        0        0      852 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4609 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/README.md
+-rw-r--r--   0        0        0       82 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/__init__.py
+-rw-r--r--   0        0        0     1828 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/scripts.py
+-rw-r--r--   0        0        0     2759 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/standalone_docs.py
+-rw-r--r--   0        0        0     1086 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/fastapi/LICENSE
+-rw-r--r--   0        0        0      412 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/fastapi/favicon.png
+-rw-r--r--   0        0        0     1174 2023-07-13 12:50:50.934921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/redoc/logo-mini.svg
+-rw-r--r--   0        0        0  1042510 2023-07-13 12:50:50.942921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/redoc/redoc.standalone.js
+-rw-r--r--   0        0        0     2628 2023-07-13 12:50:50.942921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0    11358 2023-07-13 12:50:50.942921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/swagger/LICENSE
+-rw-r--r--   0        0        0  1048219 2023-07-13 12:50:50.950921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   145206 2023-07-13 12:50:50.950921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/swagger/swagger-ui.css
+-rw-r--r--   0        0        0        0 2023-07-13 12:50:50.950921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 12:50:50.950921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/tests/conftests.py
+-rw-r--r--   0        0        0     6131 2023-07-13 12:50:50.950921 fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/tests/test_standalone_docs.py
+-rw-r--r--   0        0        0      847 2023-07-13 12:50:50.950921 fastapi_standalone_docs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5299 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.4/PKG-INFO
```

### Comparing `fastapi_standalone_docs-0.1.3/LICENSE` & `fastapi_standalone_docs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/README.md` & `fastapi_standalone_docs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/scripts.py` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/scripts.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/standalone_docs.py` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/standalone_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/fastapi/LICENSE` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/fastapi/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/logo-mini.svg` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/redoc/logo-mini.svg`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/redoc/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/LICENSE` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/swagger/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui.css` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/static/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/test_standalone_docs.py` & `fastapi_standalone_docs-0.1.4/fastapi_standalone_docs/tests/test_standalone_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.3/pyproject.toml` & `fastapi_standalone_docs-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fastapi-standalone-docs"
-version = "0.1.3"
+version = "0.1.4"
 description = "Host FastAPI Swagger UI and ReDoc without third party CDNs"
 authors = ["IOXIO Ltd"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/fastapi-standalone-docs"
 packages = [{include = "fastapi_standalone_docs"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-fastapi = ">=0.95.2,<0.99.0"
+fastapi = ">=0.95.2,<1"
 
 [tool.poetry.scripts]
 update-fastapi-standalone-docs = { callable = "fastapi_standalone_docs.scripts:update_docs", extras = ["scripts"] }
 
 [tool.poetry.extras]
 scripts = []
```

### Comparing `fastapi_standalone_docs-0.1.3/PKG-INFO` & `fastapi_standalone_docs-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fastapi-standalone-docs
-Version: 0.1.3
+Version: 0.1.4
 Summary: Host FastAPI Swagger UI and ReDoc without third party CDNs
 Home-page: https://github.com/ioxiocom/fastapi-standalone-docs
 License: MIT
 Author: IOXIO Ltd
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: scripts
-Requires-Dist: fastapi (>=0.95.2,<0.99.0)
+Requires-Dist: fastapi (>=0.95.2,<1)
 Project-URL: Repository, https://github.com/ioxiocom/fastapi-standalone-docs
 Description-Content-Type: text/markdown
 
 # FastAPI Standalone Docs
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ioxiocom/fastapi-standalone-docs/publish.yaml)](https://github.com/ioxiocom/fastapi-standalone-docs/actions/workflows/publish.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

