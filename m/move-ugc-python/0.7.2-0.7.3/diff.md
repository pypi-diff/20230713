# Comparing `tmp/move_ugc_python-0.7.2.tar.gz` & `tmp/move_ugc_python-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "move_ugc_python-0.7.2.tar", max compression
+gzip compressed data, was "move_ugc_python-0.7.3.tar", max compression
```

## Comparing `move_ugc_python-0.7.2.tar` & `move_ugc_python-0.7.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1324 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/README.md
--rw-r--r--   0        0        0       90 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/__init__.py
--rw-r--r--   0        0        0       56 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/gql_requests/__init__.py
--rw-r--r--   0        0        0      306 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/gql_requests/additional_file.py
--rw-r--r--   0        0        0      116 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/gql_requests/client.py
--rw-r--r--   0        0        0     1067 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/gql_requests/file.py
--rw-r--r--   0        0        0     1102 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/gql_requests/job.py
--rw-r--r--   0        0        0     1334 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/gql_requests/take.py
--rw-r--r--   0        0        0        0 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/py.typed
--rw-r--r--   0        0        0       36 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/__init__.py
--rw-r--r--   0        0        0     2165 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/additional_file.py
--rw-r--r--   0        0        0      709 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/client.py
--rw-r--r--   0        0        0      250 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/constants.py
--rw-r--r--   0        0        0     1489 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/file.py
--rw-r--r--   0        0        0      866 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/gql.py
--rw-r--r--   0        0        0     1937 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/job.py
--rw-r--r--   0        0        0     1198 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/metaclient.py
--rw-r--r--   0        0        0     1827 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/take.py
--rw-r--r--   0        0        0      998 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/schemas/transport.py
--rw-r--r--   0        0        0       54 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/services/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/services/base.py
--rw-r--r--   0        0        0     2296 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/services/file.py
--rw-r--r--   0        0        0     2432 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/services/job.py
--rw-r--r--   0        0        0     3239 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/services/take.py
--rw-r--r--   0        0        0      639 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/settings.py
--rw-r--r--   0        0        0      886 2023-07-13 13:19:05.073724 move_ugc_python-0.7.2/move_ugc/ugc_client.py
--rw-r--r--   0        0        0     1279 2023-07-13 13:19:05.077724 move_ugc_python-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 move_ugc_python-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-07-13 13:32:35.763951 move_ugc_python-0.7.3/README.md
+-rw-r--r--   0        0        0       90 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/gql_requests/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/gql_requests/additional_file.py
+-rw-r--r--   0        0        0      116 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/gql_requests/client.py
+-rw-r--r--   0        0        0     1067 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/gql_requests/file.py
+-rw-r--r--   0        0        0     1102 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/gql_requests/job.py
+-rw-r--r--   0        0        0     1334 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/gql_requests/take.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/py.typed
+-rw-r--r--   0        0        0       36 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/__init__.py
+-rw-r--r--   0        0        0     2165 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/additional_file.py
+-rw-r--r--   0        0        0      709 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/client.py
+-rw-r--r--   0        0        0      250 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/constants.py
+-rw-r--r--   0        0        0     1489 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/file.py
+-rw-r--r--   0        0        0      866 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/gql.py
+-rw-r--r--   0        0        0     1937 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/job.py
+-rw-r--r--   0        0        0     1198 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/metaclient.py
+-rw-r--r--   0        0        0     1827 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/take.py
+-rw-r--r--   0        0        0      998 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/schemas/transport.py
+-rw-r--r--   0        0        0       54 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/services/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/services/base.py
+-rw-r--r--   0        0        0     2296 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/services/file.py
+-rw-r--r--   0        0        0     2432 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/services/job.py
+-rw-r--r--   0        0        0     3239 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/services/take.py
+-rw-r--r--   0        0        0      639 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/settings.py
+-rw-r--r--   0        0        0      886 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/move_ugc/ugc_client.py
+-rw-r--r--   0        0        0     1279 2023-07-13 13:32:35.767951 move_ugc_python-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 move_ugc_python-0.7.3/PKG-INFO
```

### Comparing `move_ugc_python-0.7.2/README.md` & `move_ugc_python-0.7.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Move UGC Python SDK
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-7F00FF.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 ![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
 ![Tests](./badges/tests.svg)
 ![Coverage](./badges/coverage.svg)
-[![CI](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml/badge.svg?branch=main&event=workflow_run)](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml)
+[![CI](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml/badge.svg)](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml)
 ![Documentation Style](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)
 
 ## Full documentation
 
 The full documentation is available at https://move-ai.github.io/move-ugc-python/
 
 ## Installation
 
 ### With pip:
 
 ```bash
-pip install move-ugc
+pip install move-ugc-python
 ```
 ### With poetry:
 
 ```bash
-poetry add move-ugc
+poetry add move-ugc-python
 ```
 
 
 ## Initialize with your API key
 
 ```python
 from move_ugc import MoveUgc
```

### Comparing `move_ugc_python-0.7.2/move_ugc/gql_requests/file.py` & `move_ugc_python-0.7.3/move_ugc/gql_requests/file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/gql_requests/job.py` & `move_ugc_python-0.7.3/move_ugc/gql_requests/job.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/gql_requests/take.py` & `move_ugc_python-0.7.3/move_ugc/gql_requests/take.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/additional_file.py` & `move_ugc_python-0.7.3/move_ugc/schemas/additional_file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/client.py` & `move_ugc_python-0.7.3/move_ugc/schemas/client.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/file.py` & `move_ugc_python-0.7.3/move_ugc/schemas/file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/gql.py` & `move_ugc_python-0.7.3/move_ugc/schemas/gql.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/job.py` & `move_ugc_python-0.7.3/move_ugc/schemas/job.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/metaclient.py` & `move_ugc_python-0.7.3/move_ugc/schemas/metaclient.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/take.py` & `move_ugc_python-0.7.3/move_ugc/schemas/take.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/schemas/transport.py` & `move_ugc_python-0.7.3/move_ugc/schemas/transport.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/services/base.py` & `move_ugc_python-0.7.3/move_ugc/services/base.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/services/file.py` & `move_ugc_python-0.7.3/move_ugc/services/file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/services/job.py` & `move_ugc_python-0.7.3/move_ugc/services/job.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/services/take.py` & `move_ugc_python-0.7.3/move_ugc/services/take.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/settings.py` & `move_ugc_python-0.7.3/move_ugc/settings.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/move_ugc/ugc_client.py` & `move_ugc_python-0.7.3/move_ugc/ugc_client.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.2/pyproject.toml` & `move_ugc_python-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "move-ugc-python"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["Move.ai"]
 readme = "README.md"
 packages = [{include = "move_ugc"}, {include = "move_ugc/py.typed"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `move_ugc_python-0.7.2/PKG-INFO` & `move_ugc_python-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: move-ugc-python
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 Author: Move.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,32 +15,32 @@
 
 # Move UGC Python SDK
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-7F00FF.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 ![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
 ![Tests](./badges/tests.svg)
 ![Coverage](./badges/coverage.svg)
-[![CI](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml/badge.svg?branch=main&event=workflow_run)](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml)
+[![CI](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml/badge.svg)](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml)
 ![Documentation Style](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)
 
 ## Full documentation
 
 The full documentation is available at https://move-ai.github.io/move-ugc-python/
 
 ## Installation
 
 ### With pip:
 
 ```bash
-pip install move-ugc
+pip install move-ugc-python
 ```
 ### With poetry:
 
 ```bash
-poetry add move-ugc
+poetry add move-ugc-python
 ```
 
 
 ## Initialize with your API key
 
 ```python
 from move_ugc import MoveUgc
```

