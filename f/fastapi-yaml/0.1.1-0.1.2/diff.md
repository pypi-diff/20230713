# Comparing `tmp/fastapi_yaml-0.1.1.tar.gz` & `tmp/fastapi_yaml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_yaml-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_yaml-0.1.2.tar", max compression
```

## Comparing `fastapi_yaml-0.1.1.tar` & `fastapi_yaml-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-13 15:43:10.046115 fastapi_yaml-0.1.1/README.md
--rw-r--r--   0        0        0       49 2023-07-13 15:42:07.820796 fastapi_yaml-0.1.1/fastapi_yaml/__init__.py
--rw-r--r--   0        0        0      897 2023-07-13 15:41:58.989542 fastapi_yaml-0.1.1/fastapi_yaml/main.py
--rw-r--r--   0        0        0      470 2023-07-13 15:44:26.950939 fastapi_yaml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 fastapi_yaml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-13 15:43:10.046115 fastapi_yaml-0.1.2/README.md
+-rw-r--r--   0        0        0       49 2023-07-13 15:42:07.820796 fastapi_yaml-0.1.2/fastapi_yaml/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-13 15:41:58.989542 fastapi_yaml-0.1.2/fastapi_yaml/main.py
+-rw-r--r--   0        0        0      566 2023-07-13 15:47:43.839802 fastapi_yaml-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 fastapi_yaml-0.1.2/PKG-INFO
```

### Comparing `fastapi_yaml-0.1.1/README.md` & `fastapi_yaml-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_yaml-0.1.1/fastapi_yaml/main.py` & `fastapi_yaml-0.1.2/fastapi_yaml/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_yaml-0.1.1/PKG-INFO` & `fastapi_yaml-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: fastapi-yaml
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Handle YAML data in FastAPI
+Home-page: https://github.com/chermed/fastapi-yaml
+License: MIT
 Author: Mohamed Cherkaoui
 Author-email: chermed@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 # Overview
```

