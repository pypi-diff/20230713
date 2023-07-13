# Comparing `tmp/propel_client-0.0.1.tar.gz` & `tmp/propel_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propel_client-0.0.1.tar", max compression
+gzip compressed data, was "propel_client-0.0.2.tar", max compression
```

## Comparing `propel_client-0.0.1.tar` & `propel_client-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11339 2023-07-12 10:36:09.705023 propel_client-0.0.1/LICENSE
--rw-r--r--   0        0        0      601 2023-07-12 10:36:09.705023 propel_client-0.0.1/README.md
--rw-r--r--   0        0        0      808 2023-07-12 10:36:09.705023 propel_client-0.0.1/propel_client/__init__.py
--rw-r--r--   0        0        0    13936 2023-07-12 10:36:09.705023 propel_client-0.0.1/propel_client/cli.py
--rw-r--r--   0        0        0     1443 2023-07-12 10:36:09.705023 propel_client-0.0.1/propel_client/constants.py
--rw-r--r--   0        0        0     1890 2023-07-12 10:36:09.705023 propel_client-0.0.1/propel_client/cred_storage.py
--rw-r--r--   0        0        0    13267 2023-07-12 10:36:09.705023 propel_client-0.0.1/propel_client/propel.py
--rw-r--r--   0        0        0      724 2023-07-12 10:36:09.705023 propel_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 propel_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-13 11:44:37.904710 propel_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0      601 2023-07-13 11:44:37.904710 propel_client-0.0.2/README.md
+-rw-r--r--   0        0        0      808 2023-07-13 11:44:37.904710 propel_client-0.0.2/propel_client/__init__.py
+-rw-r--r--   0        0        0    18071 2023-07-13 11:44:37.904710 propel_client-0.0.2/propel_client/cli.py
+-rw-r--r--   0        0        0     1443 2023-07-13 11:44:37.904710 propel_client-0.0.2/propel_client/constants.py
+-rw-r--r--   0        0        0     1890 2023-07-13 11:44:37.904710 propel_client-0.0.2/propel_client/cred_storage.py
+-rw-r--r--   0        0        0    13267 2023-07-13 11:44:37.904710 propel_client-0.0.2/propel_client/propel.py
+-rw-r--r--   0        0        0      724 2023-07-13 11:44:37.904710 propel_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 propel_client-0.0.2/PKG-INFO
```

### Comparing `propel_client-0.0.1/LICENSE` & `propel_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propel_client-0.0.1/README.md` & `propel_client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `propel_client-0.0.1/propel_client/__init__.py` & `propel_client-0.0.2/propel_client/__init__.py`

 * *Files identical despite different names*

### Comparing `propel_client-0.0.1/propel_client/constants.py` & `propel_client-0.0.2/propel_client/constants.py`

 * *Files identical despite different names*

### Comparing `propel_client-0.0.1/propel_client/cred_storage.py` & `propel_client-0.0.2/propel_client/cred_storage.py`

 * *Files identical despite different names*

### Comparing `propel_client-0.0.1/propel_client/propel.py` & `propel_client-0.0.2/propel_client/propel.py`

 * *Files identical despite different names*

### Comparing `propel_client-0.0.1/pyproject.toml` & `propel_client-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "propel-client"
-version = "v0.0.1"
+version = "v0.0.2"
 description = "Propel service client"
 authors = ["Yuri Turchenkov <yuri.turchenkov@valory.xyz>"]
 readme = "README.md"
 packages = [{ include = "propel_client" }]
 
 
 [tool.poetry.dependencies]
```

### Comparing `propel_client-0.0.1/PKG-INFO` & `propel_client-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propel-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Propel service client
 Author: Yuri Turchenkov
 Author-email: yuri.turchenkov@valory.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

