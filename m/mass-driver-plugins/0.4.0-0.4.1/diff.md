# Comparing `tmp/mass_driver_plugins-0.4.0.tar.gz` & `tmp/mass_driver_plugins-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_driver_plugins-0.4.0.tar", max compression
+gzip compressed data, was "mass_driver_plugins-0.4.1.tar", max compression
```

## Comparing `mass_driver_plugins-0.4.0.tar` & `mass_driver_plugins-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2520 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/README.md
--rw-r--r--   0        0        0     2612 2023-07-05 00:44:09.249599 mass_driver_plugins-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/src/mass_driver_plugins/__init__.py
--rw-r--r--   0        0        0      756 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/src/mass_driver_plugins/cli.py
--rw-r--r--   0        0        0     2845 2023-07-05 00:40:22.790344 mass_driver_plugins-0.4.0/src/mass_driver_plugins/jsonpatch.py
--rw-r--r--   0        0        0     2354 2023-07-05 00:40:30.318451 mass_driver_plugins-0.4.0/src/mass_driver_plugins/poetry.py
--rw-r--r--   0        0        0       26 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.0/src/mass_driver_plugins/py.typed
--rw-r--r--   0        0        0     8578 2023-07-05 00:40:35.454524 mass_driver_plugins-0.4.0/src/mass_driver_plugins/surgical.py
--rw-r--r--   0        0        0      886 2023-07-05 00:40:39.494582 mass_driver_plugins-0.4.0/src/mass_driver_plugins/template.py
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 mass_driver_plugins-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2520 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.1/README.md
+-rw-r--r--   0        0        0     2612 2023-07-13 20:48:39.583675 mass_driver_plugins-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.1/src/mass_driver_plugins/__init__.py
+-rw-r--r--   0        0        0      756 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.1/src/mass_driver_plugins/cli.py
+-rw-r--r--   0        0        0     2845 2023-07-05 00:40:22.790344 mass_driver_plugins-0.4.1/src/mass_driver_plugins/jsonpatch.py
+-rw-r--r--   0        0        0     2354 2023-07-05 00:40:30.318451 mass_driver_plugins-0.4.1/src/mass_driver_plugins/poetry.py
+-rw-r--r--   0        0        0       26 2023-01-17 14:11:51.400445 mass_driver_plugins-0.4.1/src/mass_driver_plugins/py.typed
+-rw-r--r--   0        0        0     8578 2023-07-05 00:40:35.454524 mass_driver_plugins-0.4.1/src/mass_driver_plugins/surgical.py
+-rw-r--r--   0        0        0      886 2023-07-05 00:40:39.494582 mass_driver_plugins-0.4.1/src/mass_driver_plugins/template.py
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 mass_driver_plugins-0.4.1/PKG-INFO
```

### Comparing `mass_driver_plugins-0.4.0/README.md` & `mass_driver_plugins-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.4.0/pyproject.toml` & `mass_driver_plugins-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "mass_driver_plugins"
-version = "0.4.0"
+version = "0.4.1"
 description = "Experimental plugin ecosystem for Mass Driver"
 authors = ["Jb Doyon <jb@jiby.tech>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 mass-driver-plugins = "mass_driver_plugins.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 # The project that these plugins extend
-mass-driver = "^0.15"
+mass-driver = "^0.16"
 # Poetry driver
 poetry-core = "*"
 # Json path resolving within
 jsonpointer = "*"
 # And json patching itself via pointers
 jsonpatch = "*"
 # Templates
```

### Comparing `mass_driver_plugins-0.4.0/src/mass_driver_plugins/cli.py` & `mass_driver_plugins-0.4.1/src/mass_driver_plugins/cli.py`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.4.0/src/mass_driver_plugins/jsonpatch.py` & `mass_driver_plugins-0.4.1/src/mass_driver_plugins/jsonpatch.py`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.4.0/src/mass_driver_plugins/poetry.py` & `mass_driver_plugins-0.4.1/src/mass_driver_plugins/poetry.py`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.4.0/src/mass_driver_plugins/surgical.py` & `mass_driver_plugins-0.4.1/src/mass_driver_plugins/surgical.py`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.4.0/src/mass_driver_plugins/template.py` & `mass_driver_plugins-0.4.1/src/mass_driver_plugins/template.py`

 * *Files identical despite different names*

### Comparing `mass_driver_plugins-0.4.0/PKG-INFO` & `mass_driver_plugins-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mass-driver-plugins
-Version: 0.4.0
+Version: 0.4.1
 Summary: Experimental plugin ecosystem for Mass Driver
 Author: Jb Doyon
 Author-email: jb@jiby.tech
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonpatch
 Requires-Dist: jsonpointer
-Requires-Dist: mass-driver (>=0.15,<0.16)
+Requires-Dist: mass-driver (>=0.16,<0.17)
 Requires-Dist: poetry-core
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: tree-sitter
 Requires-Dist: tree-sitter-languages
 Description-Content-Type: text/markdown
 
 # Mass Driver Plugins
```

