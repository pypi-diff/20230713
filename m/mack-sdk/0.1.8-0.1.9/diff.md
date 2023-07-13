# Comparing `tmp/mack_sdk-0.1.8.tar.gz` & `tmp/mack_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mack_sdk-0.1.8.tar", max compression
+gzip compressed data, was "mack_sdk-0.1.9.tar", max compression
```

## Comparing `mack_sdk-0.1.8.tar` & `mack_sdk-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      702 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/__init__.py
--rw-r--r--   0        0        0     3081 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/client.py
--rw-r--r--   0        0        0        0 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/resources/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/resources/models.py
--rw-r--r--   0        0        0     2619 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/resources/movie.py
--rw-r--r--   0        0        0     1745 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/resources/quote.py
--rw-r--r--   0        0        0        0 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/tools/__init__.py
--rw-r--r--   0        0        0      906 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/tools/raise_for_status.py
--rw-r--r--   0        0        0      941 2023-06-03 19:20:11.447102 mack_sdk-0.1.8/mack_SDK/tools/settings.py
--rw-r--r--   0        0        0     2330 2023-06-03 19:20:28.531087 mack_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 mack_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      702 2023-07-13 13:36:20.222842 mack_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/client.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/resources/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/resources/models.py
+-rw-r--r--   0        0        0     2619 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/resources/movie.py
+-rw-r--r--   0        0        0     1745 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/resources/quote.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/tools/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/tools/raise_for_status.py
+-rw-r--r--   0        0        0      941 2023-07-13 13:36:20.226842 mack_sdk-0.1.9/mack_SDK/tools/settings.py
+-rw-r--r--   0        0        0     2330 2023-07-13 13:36:37.850619 mack_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 mack_sdk-0.1.9/PKG-INFO
```

### Comparing `mack_sdk-0.1.8/README.md` & `mack_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/mack_SDK/client.py` & `mack_sdk-0.1.9/mack_SDK/client.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/mack_SDK/resources/models.py` & `mack_sdk-0.1.9/mack_SDK/resources/models.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/mack_SDK/resources/movie.py` & `mack_sdk-0.1.9/mack_SDK/resources/movie.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/mack_SDK/resources/quote.py` & `mack_sdk-0.1.9/mack_SDK/resources/quote.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/mack_SDK/tools/raise_for_status.py` & `mack_sdk-0.1.9/mack_SDK/tools/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/mack_SDK/tools/settings.py` & `mack_sdk-0.1.9/mack_SDK/tools/settings.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.8/pyproject.toml` & `mack_sdk-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mack-SDK"
 version = "0.1.0"
 description = "LOTR SDK"
 requires-python = ">=3.11"
 
 [tool.poetry]
 name = "mack-SDK"
-version = "0.1.8"
+version = "0.1.9"
 description = "LOTR SDK"
 authors = ["Maksym Iv <maxim.ivaschenko@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "mack_SDK" }]
 
 [tool.poetry.dependencies]
 python = "~3.11"
```

### Comparing `mack_sdk-0.1.8/PKG-INFO` & `mack_sdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mack-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: LOTR SDK
 Author: Maksym Iv
 Author-email: maxim.ivaschenko@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
```

