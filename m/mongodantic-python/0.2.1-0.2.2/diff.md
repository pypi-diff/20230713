# Comparing `tmp/mongodantic_python-0.2.1.tar.gz` & `tmp/mongodantic_python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodantic_python-0.2.1.tar", max compression
+gzip compressed data, was "mongodantic_python-0.2.2.tar", max compression
```

## Comparing `mongodantic_python-0.2.1.tar` & `mongodantic_python-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1506 2023-03-07 17:42:59.650982 mongodantic_python-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     5869 2023-03-07 17:42:59.654982 mongodantic_python-0.2.1/README.md
--rw-r--r--   0        0        0      260 2023-03-07 17:42:59.654982 mongodantic_python-0.2.1/mongodantic/__init__.py
--rw-r--r--   0        0        0      315 2023-03-07 17:42:59.654982 mongodantic_python-0.2.1/mongodantic/conftest.py
--rw-r--r--   0        0        0     4618 2023-03-07 17:42:59.654982 mongodantic_python-0.2.1/mongodantic/model.py
--rw-r--r--   0        0        0     2301 2023-03-07 17:42:59.654982 mongodantic_python-0.2.1/mongodantic/test_mongodantic.py
--rw-r--r--   0        0        0      843 2023-03-07 17:42:59.654982 mongodantic_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6836 1970-01-01 00:00:00.000000 mongodantic_python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     5869 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/README.md
+-rw-r--r--   0        0        0      260 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/mongodantic/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/mongodantic/conftest.py
+-rw-r--r--   0        0        0     4618 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/mongodantic/model.py
+-rw-r--r--   0        0        0     2301 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/mongodantic/test_mongodantic.py
+-rw-r--r--   0        0        0      848 2023-07-13 14:37:06.245993 mongodantic_python-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6827 1970-01-01 00:00:00.000000 mongodantic_python-0.2.2/PKG-INFO
```

### Comparing `mongodantic_python-0.2.1/LICENSE.md` & `mongodantic_python-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mongodantic_python-0.2.1/README.md` & `mongodantic_python-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mongodantic_python-0.2.1/mongodantic/model.py` & `mongodantic_python-0.2.2/mongodantic/model.py`

 * *Files identical despite different names*

### Comparing `mongodantic_python-0.2.1/mongodantic/test_mongodantic.py` & `mongodantic_python-0.2.2/mongodantic/test_mongodantic.py`

 * *Files identical despite different names*

### Comparing `mongodantic_python-0.2.1/pyproject.toml` & `mongodantic_python-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "mongodantic-python"
-version = "0.2.1"
+version = "0.2.2"
 description = "Pydantic models for MongoDB"
 authors = ["Janne Enberg <janne.enberg@lietu.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/cocreators-ee/mongodantic/"
 repository = "https://github.com/cocreators-ee/mongodantic/"
 documentation = "https://github.com/cocreators-ee/mongodantic/"
 keywords = ["database", "mongodb", "pymongo", "odm", "async"]
 packages = [
     { include = "mongodantic" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pydantic = "^1.10.4"
+python = ">=3.7,<4"
+pydantic = ">=1.10.4"
 motor = "^3.1.1"
 pymongo = "^4.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-watch = "^4.2.0"
```

### Comparing `mongodantic_python-0.2.1/PKG-INFO` & `mongodantic_python-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mongodantic-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pydantic models for MongoDB
 Home-page: https://github.com/cocreators-ee/mongodantic/
 License: BSD-3-Clause
 Keywords: database,mongodb,pymongo,odm,async
 Author: Janne Enberg
 Author-email: janne.enberg@lietu.net
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: motor (>=3.1.1,<4.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=1.10.4)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Project-URL: Documentation, https://github.com/cocreators-ee/mongodantic/
 Project-URL: Repository, https://github.com/cocreators-ee/mongodantic/
 Description-Content-Type: text/markdown
 
 # Mongodantic
```

