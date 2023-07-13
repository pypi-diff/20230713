# Comparing `tmp/msgram-parser-1.0.0.tar.gz` & `tmp/msgram-parser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-1.0.0.tar", last modified: Mon Jul 10 04:35:15 2023, max compression
+gzip compressed data, was "msgram-parser-1.1.0.tar", last modified: Thu Jul 13 03:01:48 2023, max compression
```

## Comparing `msgram-parser-1.0.0.tar` & `msgram-parser-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/genericparser/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/accept_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/genericparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/genericparser/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/genericparser/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/plugins/dinamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/plugins/dinamic/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/genericparser/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/genericparser/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/genericparser/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/genericparser/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-10 04:35:15.000000 msgram-parser-1.0.0/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-10 04:35:15.000000 msgram-parser-1.0.0/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:35:15.000000 msgram-parser-1.0.0/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 04:35:15.000000 msgram-parser-1.0.0/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 04:35:15.000000 msgram-parser-1.0.0/msgram_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:15.436027 msgram-parser-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-10 04:34:58.000000 msgram-parser-1.0.0/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/plugins/dinamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/plugins/dinamic/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-13 03:01:48.000000 msgram-parser-1.1.0/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-13 03:01:48.000000 msgram-parser-1.1.0/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:01:48.000000 msgram-parser-1.1.0/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 03:01:48.000000 msgram-parser-1.1.0/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 03:01:48.000000 msgram-parser-1.1.0/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:01:48.352814 msgram-parser-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 03:01:31.000000 msgram-parser-1.1.0/tests/tests_main_file.py
```

### Comparing `msgram-parser-1.0.0/LICENSE` & `msgram-parser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-1.0.0/PKG-INFO` & `msgram-parser-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 1.0.0
+Version: 1.1.0
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-1.0.0/README.md` & `msgram-parser-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-1.0.0/genericparser/genericparser.py` & `msgram-parser-1.1.0/genericparser/genericparser.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-1.0.0/genericparser/plugins/domain/generic_class.py` & `msgram-parser-1.1.0/genericparser/plugins/domain/generic_class.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-1.0.0/genericparser/plugins/statics/sonarqube.py` & `msgram-parser-1.1.0/genericparser/plugins/statics/sonarqube.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-1.0.0/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-1.1.0/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 1.0.0
+Version: 1.1.0
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-1.0.0/msgram_parser.egg-info/SOURCES.txt` & `msgram-parser-1.1.0/msgram_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-parser-1.0.0/pyproject.toml` & `msgram-parser-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "1.0.0"
+version = "1.1.0"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

