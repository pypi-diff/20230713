# Comparing `tmp/ossit-0.2.0.tar.gz` & `tmp/ossit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossit-0.2.0.tar", last modified: Thu May 18 17:24:19 2023, max compression
+gzip compressed data, was "ossit-0.2.1.tar", last modified: Wed Jul 12 23:00:50 2023, max compression
```

## Comparing `ossit-0.2.0.tar` & `ossit-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 17:24:08.000000 ossit-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-18 17:24:19.032308 ossit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-18 17:24:08.000000 ossit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/ossit/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/ossit/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_resources/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_resources/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/ossit_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/ossit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-18 17:24:18.000000 ossit-0.2.0/ossit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-18 17:24:19.000000 ossit-0.2.0/ossit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:24:18.000000 ossit-0.2.0/ossit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 17:24:18.000000 ossit-0.2.0/ossit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 17:24:08.000000 ossit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 17:24:19.032308 ossit-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:24:08.000000 ossit-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 23:00:36.000000 ossit-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 23:00:50.520480 ossit-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-12 23:00:36.000000 ossit-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/ossit/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/ossit/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_resources/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/api_resources/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/ossit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 23:00:36.000000 ossit-0.2.1/ossit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:00:50.520480 ossit-0.2.1/ossit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 23:00:50.000000 ossit-0.2.1/ossit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 23:00:36.000000 ossit-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 23:00:50.520480 ossit-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:00:36.000000 ossit-0.2.1/setup.py
```

### Comparing `ossit-0.2.0/LICENSE.txt` & `ossit-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ossit-0.2.0/PKG-INFO` & `ossit-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Package to connect to ossit API
 Author: Wesley Howery
 Author-email: wesleyh@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ossit-0.2.0/README.md` & `ossit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ossit-0.2.0/ossit/api_requestor.py` & `ossit-0.2.1/ossit/api_requestor.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.0/ossit/api_resources/domain.py` & `ossit-0.2.1/ossit/api_resources/domain.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.0/ossit/api_resources/statistic.py` & `ossit-0.2.1/ossit/api_resources/statistic.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.0/ossit/config.py` & `ossit-0.2.1/ossit/config.py`

 * *Files identical despite different names*

### Comparing `ossit-0.2.0/ossit.egg-info/PKG-INFO` & `ossit-0.2.1/ossit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Package to connect to ossit API
 Author: Wesley Howery
 Author-email: wesleyh@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ossit-0.2.0/setup.cfg` & `ossit-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ossit
-version = 0.2.0
+version = 0.2.1
 author = Wesley Howery
 author_email = wesleyh@stratusadv.com
 description = Python Package to connect to ossit API
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

