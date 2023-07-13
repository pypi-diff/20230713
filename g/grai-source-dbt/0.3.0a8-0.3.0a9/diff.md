# Comparing `tmp/grai_source_dbt-0.3.0a8.tar.gz` & `tmp/grai_source_dbt-0.3.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.3.0a8.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.3.0a9.tar", max compression
```

## Comparing `grai_source_dbt-0.3.0a8.tar` & `grai_source_dbt-0.3.0a9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      124 2023-05-02 08:01:59.695588 grai_source_dbt-0.3.0a8/README.md
--rw-r--r--   0        0        0     1078 2023-07-05 08:38:29.904069 grai_source_dbt-0.3.0a8/pyproject.toml
--rw-r--r--   0        0        0      217 2023-07-05 08:38:33.696703 grai_source_dbt-0.3.0a8/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-22 09:54:48.652302 grai_source_dbt-0.3.0a8/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     8357 2023-07-05 08:36:46.112652 grai_source_dbt-0.3.0a8/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      695 2023-06-06 17:35:16.802940 grai_source_dbt-0.3.0a8/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      929 2023-06-30 17:13:40.673550 grai_source_dbt-0.3.0a8/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-02-14 12:06:39.089774 grai_source_dbt-0.3.0a8/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-02-14 12:06:39.090263 grai_source_dbt-0.3.0a8/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      995 2023-06-06 17:35:16.803842 grai_source_dbt-0.3.0a8/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     2043 2023-06-06 17:35:16.804153 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      985 2023-06-06 17:35:16.804291 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      288 2023-06-06 17:35:16.804400 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     6197 2023-06-16 16:15:18.431432 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-22 09:54:48.653526 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-22 09:54:48.653655 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-22 09:54:48.653765 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653884 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653991 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2423 2023-06-06 17:35:16.804770 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-24 17:33:29.685755 grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-22 09:54:48.654363 grai_source_dbt-0.3.0a8/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2501 2023-06-16 16:15:18.431554 grai_source_dbt-0.3.0a8/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2584 2023-06-06 17:35:16.805007 grai_source_dbt-0.3.0a8/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      189 2023-06-06 17:35:16.805133 grai_source_dbt-0.3.0a8/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     2631 2023-06-29 13:30:53.867579 grai_source_dbt-0.3.0a8/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.090850 grai_source_dbt-0.3.0a8/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0     1243 2023-06-06 17:35:16.805384 grai_source_dbt-0.3.0a8/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.0a8/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-05-02 08:01:59.695588 grai_source_dbt-0.3.0a9/README.md
+-rw-r--r--   0        0        0     1078 2023-07-12 11:23:17.119508 grai_source_dbt-0.3.0a9/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-07-12 10:52:48.694390 grai_source_dbt-0.3.0a9/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-22 09:54:48.652302 grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     8357 2023-07-12 10:52:48.699928 grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      695 2023-06-06 17:35:16.802940 grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0     1085 2023-07-12 11:10:18.665361 grai_source_dbt-0.3.0a9/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-02-14 12:06:39.089774 grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-02-14 12:06:39.090263 grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      995 2023-06-06 17:35:16.803842 grai_source_dbt-0.3.0a9/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     2043 2023-06-06 17:35:16.804153 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-06 17:35:16.804291 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      288 2023-06-06 17:35:16.804400 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     6197 2023-06-16 16:15:18.431432 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-22 09:54:48.653526 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-22 09:54:48.653655 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-22 09:54:48.653765 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653884 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653991 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2423 2023-06-06 17:35:16.804770 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-24 17:33:29.685755 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-22 09:54:48.654363 grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2501 2023-06-16 16:15:18.431554 grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2584 2023-06-06 17:35:16.805007 grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      189 2023-06-06 17:35:16.805133 grai_source_dbt-0.3.0a9/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     2631 2023-07-12 10:52:48.701382 grai_source_dbt-0.3.0a9/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.090850 grai_source_dbt-0.3.0a9/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0     1243 2023-06-06 17:35:16.805384 grai_source_dbt-0.3.0a9/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.0a9/PKG-INFO
```

### Comparing `grai_source_dbt-0.3.0a8/pyproject.toml` & `grai_source_dbt-0.3.0a9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt"
-version = "0.3.0-alpha8"
+version = "0.3.0-alpha9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt", from = "src" },
 ]
 readme = "README.md"
@@ -12,15 +12,15 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a11", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 dbt-artifacts-parser = "^0.2.4"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.991"
```

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v1.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/processor.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/processor.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.3.0a9/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a8/PKG-INFO` & `grai_source_dbt-0.3.0a9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.3.0a8
+Version: 0.3.0a9
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbt-artifacts-parser (>=0.2.4,<0.3.0)
-Requires-Dist: grai-client (>=0.3.0a11,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt
 Description-Content-Type: text/markdown
 
 # Grai dbt Integration
```

