# Comparing `tmp/arcaflow_lib_kubernetes-0.1.1.tar.gz` & `tmp/arcaflow_lib_kubernetes-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcaflow_lib_kubernetes-0.1.1.tar", max compression
+gzip compressed data, was "arcaflow_lib_kubernetes-0.1.2.tar", max compression
```

## Comparing `arcaflow_lib_kubernetes-0.1.1.tar` & `arcaflow_lib_kubernetes-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10174 2023-04-06 12:05:31.443204 arcaflow_lib_kubernetes-0.1.1/LICENSE
--rw-r--r--   0        0        0       45 2023-04-06 12:05:31.443204 arcaflow_lib_kubernetes-0.1.1/README.md
--rw-r--r--   0        0        0      516 2023-04-06 12:05:31.511204 arcaflow_lib_kubernetes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       60 2023-04-06 12:05:31.447203 arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/__init__.py
--rw-r--r--   0        0        0    23378 2023-04-06 12:05:45.147333 arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/convert.py
--rw-r--r--   0        0        0     9612 2023-04-06 12:05:45.243334 arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/model.py
--rw-r--r--   0        0        0     6964 2023-04-06 12:05:45.887340 arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/test_convert.py
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 arcaflow_lib_kubernetes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-07-13 13:52:06.688152 arcaflow_lib_kubernetes-0.1.2/LICENSE
+-rw-r--r--   0        0        0       45 2023-07-13 13:52:06.688152 arcaflow_lib_kubernetes-0.1.2/README.md
+-rw-r--r--   0        0        0      516 2023-07-13 13:52:06.760152 arcaflow_lib_kubernetes-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-07-13 13:52:06.688152 arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/__init__.py
+-rw-r--r--   0        0        0    23416 2023-07-13 13:52:29.460781 arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/convert.py
+-rw-r--r--   0        0        0     9612 2023-07-13 13:52:29.540783 arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/model.py
+-rw-r--r--   0        0        0     6964 2023-07-13 13:52:30.252800 arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/test_convert.py
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 arcaflow_lib_kubernetes-0.1.2/PKG-INFO
```

### Comparing `arcaflow_lib_kubernetes-0.1.1/LICENSE` & `arcaflow_lib_kubernetes-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcaflow_lib_kubernetes-0.1.1/pyproject.toml` & `arcaflow_lib_kubernetes-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcaflow-lib-kubernetes"
-version = "v0.1.1"
+version = "v0.1.2"
 description = "Kubernetes connection handling library for Arcaflow"
 authors = ["Arcalot Contributors"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/convert.py` & `arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,18 +365,18 @@
     if connection.key is not None:
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             temp_file.write(bytes(connection.key, "ascii"))
             config.key_file = temp_file.name
 
     config.username = connection.username
     config.password = connection.password
-    config.api_key_prefix = "Bearer"
+    config.api_key_prefix = {"authorization": "Bearer"}
 
     if connection.bearer_token is not None:
-        config.api_key = connection.bearer_token
+        config.api_key = {"authorization": connection.bearer_token}
 
     if connection.bearer_token_file is not None:
         try:
             with open(connection.bearer_token_file) as f:
                 config.api_key = f.read()
         except Exception as e:
             raise InvalidKubeConfigException(
```

### Comparing `arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/model.py` & `arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/model.py`

 * *Files identical despite different names*

### Comparing `arcaflow_lib_kubernetes-0.1.1/src/arcaflow_lib_kubernetes/test_convert.py` & `arcaflow_lib_kubernetes-0.1.2/src/arcaflow_lib_kubernetes/test_convert.py`

 * *Files identical despite different names*

### Comparing `arcaflow_lib_kubernetes-0.1.1/PKG-INFO` & `arcaflow_lib_kubernetes-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcaflow-lib-kubernetes
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kubernetes connection handling library for Arcaflow
 License: Apache-2.0
 Author: Arcalot Contributors
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

