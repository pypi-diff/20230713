# Comparing `tmp/dcg_service-0.0.4.tar.gz` & `tmp/dcg_service-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcg_service-0.0.4.tar", last modified: Thu Jul 13 06:40:33 2023, max compression
+gzip compressed data, was "dcg_service-0.0.5.tar", last modified: Thu Jul 13 10:26:37 2023, max compression
```

## Comparing `dcg_service-0.0.4.tar` & `dcg_service-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 06:40:33.945000 dcg_service-0.0.4/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-0.0.4/LICENCE
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-13 06:40:33.945000 dcg_service-0.0.4/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-0.0.4/README.md
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      532 2023-07-13 06:40:20.000000 dcg_service-0.0.4/pyproject.toml
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-13 06:40:33.945000 dcg_service-0.0.4/setup.cfg
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 06:40:33.932999 dcg_service-0.0.4/src/
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 06:40:33.936999 dcg_service-0.0.4/src/dcg_service/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-0.0.4/src/dcg_service/__init__.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 06:40:33.945000 dcg_service-0.0.4/src/dcg_service/core/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-0.0.4/src/dcg_service/core/__init__.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2497 2023-07-10 10:44:32.000000 dcg_service-0.0.4/src/dcg_service/core/authentication.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      829 2023-07-10 07:54:07.000000 dcg_service-0.0.4/src/dcg_service/core/encryption.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7591 2023-07-12 05:42:02.000000 dcg_service-0.0.4/src/dcg_service/core/events.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2889 2023-07-13 06:38:05.000000 dcg_service-0.0.4/src/dcg_service/core/exceptions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-0.0.4/src/dcg_service/core/filters.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-0.0.4/src/dcg_service/core/logger.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1800 2023-07-10 09:41:05.000000 dcg_service-0.0.4/src/dcg_service/core/permissions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-0.0.4/src/dcg_service/core/response.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16189 2023-07-12 05:41:48.000000 dcg_service-0.0.4/src/dcg_service/core/services.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1080 2023-07-10 10:33:28.000000 dcg_service-0.0.4/src/dcg_service/core/utils.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 06:40:33.936999 dcg_service-0.0.4/src/dcg_service.egg-info/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-13 06:40:33.000000 dcg_service-0.0.4/src/dcg_service.egg-info/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      584 2023-07-13 06:40:33.000000 dcg_service-0.0.4/src/dcg_service.egg-info/SOURCES.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-13 06:40:33.000000 dcg_service-0.0.4/src/dcg_service.egg-info/dependency_links.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-13 06:40:33.000000 dcg_service-0.0.4/src/dcg_service.egg-info/top_level.txt
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 10:26:37.943920 dcg_service-0.0.5/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-0.0.5/LICENCE
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-13 10:26:37.939920 dcg_service-0.0.5/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-0.0.5/README.md
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      629 2023-07-13 10:26:21.000000 dcg_service-0.0.5/pyproject.toml
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      174 2023-07-11 12:09:47.000000 dcg_service-0.0.5/requirement.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-13 10:26:37.943920 dcg_service-0.0.5/setup.cfg
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 10:26:37.931920 dcg_service-0.0.5/src/
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 10:26:37.935920 dcg_service-0.0.5/src/dcg_service/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-0.0.5/src/dcg_service/__init__.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 10:26:37.939920 dcg_service-0.0.5/src/dcg_service/core/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-0.0.5/src/dcg_service/core/__init__.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2497 2023-07-10 10:44:32.000000 dcg_service-0.0.5/src/dcg_service/core/authentication.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      829 2023-07-10 07:54:07.000000 dcg_service-0.0.5/src/dcg_service/core/encryption.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7591 2023-07-12 05:42:02.000000 dcg_service-0.0.5/src/dcg_service/core/events.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2889 2023-07-13 06:38:05.000000 dcg_service-0.0.5/src/dcg_service/core/exceptions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-0.0.5/src/dcg_service/core/filters.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-0.0.5/src/dcg_service/core/logger.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1800 2023-07-10 09:41:05.000000 dcg_service-0.0.5/src/dcg_service/core/permissions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-0.0.5/src/dcg_service/core/response.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16189 2023-07-12 05:41:48.000000 dcg_service-0.0.5/src/dcg_service/core/services.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1080 2023-07-10 10:33:28.000000 dcg_service-0.0.5/src/dcg_service/core/utils.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-13 10:26:37.935920 dcg_service-0.0.5/src/dcg_service.egg-info/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6923 2023-07-13 10:26:37.000000 dcg_service-0.0.5/src/dcg_service.egg-info/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      638 2023-07-13 10:26:37.000000 dcg_service-0.0.5/src/dcg_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-13 10:26:37.000000 dcg_service-0.0.5/src/dcg_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      175 2023-07-13 10:26:37.000000 dcg_service-0.0.5/src/dcg_service.egg-info/requires.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-13 10:26:37.000000 dcg_service-0.0.5/src/dcg_service.egg-info/top_level.txt
```

### Comparing `dcg_service-0.0.4/LICENCE` & `dcg_service-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/PKG-INFO` & `dcg_service-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcg_service
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for DCG DOT Compliance Group, used for flask based projects.
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcg_service-0.0.4/README.md` & `dcg_service-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/pyproject.toml` & `dcg_service-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [project]
 name = "dcg_service"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Aman Kumar", email="amankumar@zapbuild.com" },
 ]
 description = "Package for DCG DOT Compliance Group, used for flask based projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dynamic = ["dependencies"]
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirement.txt"]}
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `dcg_service-0.0.4/src/dcg_service/core/authentication.py` & `dcg_service-0.0.5/src/dcg_service/core/authentication.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/encryption.py` & `dcg_service-0.0.5/src/dcg_service/core/encryption.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/events.py` & `dcg_service-0.0.5/src/dcg_service/core/events.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/exceptions.py` & `dcg_service-0.0.5/src/dcg_service/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/filters.py` & `dcg_service-0.0.5/src/dcg_service/core/filters.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/logger.py` & `dcg_service-0.0.5/src/dcg_service/core/logger.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/permissions.py` & `dcg_service-0.0.5/src/dcg_service/core/permissions.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/response.py` & `dcg_service-0.0.5/src/dcg_service/core/response.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/services.py` & `dcg_service-0.0.5/src/dcg_service/core/services.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service/core/utils.py` & `dcg_service-0.0.5/src/dcg_service/core/utils.py`

 * *Files identical despite different names*

### Comparing `dcg_service-0.0.4/src/dcg_service.egg-info/PKG-INFO` & `dcg_service-0.0.5/src/dcg_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcg-service
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for DCG DOT Compliance Group, used for flask based projects.
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcg_service-0.0.4/src/dcg_service.egg-info/SOURCES.txt` & `dcg_service-0.0.5/src/dcg_service.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENCE
 README.md
 pyproject.toml
+requirement.txt
 src/dcg_service/__init__.py
 src/dcg_service.egg-info/PKG-INFO
 src/dcg_service.egg-info/SOURCES.txt
 src/dcg_service.egg-info/dependency_links.txt
+src/dcg_service.egg-info/requires.txt
 src/dcg_service.egg-info/top_level.txt
 src/dcg_service/core/__init__.py
 src/dcg_service/core/authentication.py
 src/dcg_service/core/encryption.py
 src/dcg_service/core/events.py
 src/dcg_service/core/exceptions.py
 src/dcg_service/core/filters.py
```

