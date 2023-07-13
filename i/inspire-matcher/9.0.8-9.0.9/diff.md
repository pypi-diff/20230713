# Comparing `tmp/inspire-matcher-9.0.8.tar.gz` & `tmp/inspire-matcher-9.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspire-matcher-9.0.8.tar", last modified: Fri Nov 20 16:59:42 2020, max compression
+gzip compressed data, was "dist/inspire-matcher-9.0.9.tar", last modified: Fri Nov 27 11:48:44 2020, max compression
```

## Comparing `inspire-matcher-9.0.8.tar` & `inspire-matcher-9.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2741 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3857 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/validators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7272 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1999 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3763 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1065 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/inspire_matcher/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2741 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      482 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2020-11-20 16:59:42.000000 inspire-matcher-9.0.8/inspire_matcher.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2020-11-20 16:59:00.000000 inspire-matcher-9.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1373 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      780 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      482 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-27 11:48:41.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3573 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 11:48:44.000000 inspire-matcher-9.0.9/inspire_matcher/
+-rw-r--r--   0 runner    (1001) docker     (116)     1999 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3857 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/validators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1065 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7272 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2809 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3763 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1407 2020-11-27 11:48:11.000000 inspire-matcher-9.0.9/inspire_matcher/ext.py
```

### Comparing `inspire-matcher-9.0.8/PKG-INFO` & `inspire-matcher-9.0.9/inspire_matcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspire-matcher
-Version: 9.0.8
+Version: 9.0.9
 Summary: Find the records in INSPIRE most similar to a given record or reference.
 Home-page: https://github.com/inspirehep/inspire-matcher
 Author: CERN
 Author-email: admin@inspirehep.net
 License: GPLv3
 Description: ..
             This file is part of INSPIRE.
```

### Comparing `inspire-matcher-9.0.8/README.rst` & `inspire-matcher-9.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/validators.py` & `inspire-matcher-9.0.9/inspire_matcher/validators.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/core.py` & `inspire-matcher-9.0.9/inspire_matcher/core.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/ext.py` & `inspire-matcher-9.0.9/inspire_matcher/ext.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/utils.py` & `inspire-matcher-9.0.9/inspire_matcher/utils.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/config.py` & `inspire-matcher-9.0.9/inspire_matcher/config.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/api.py` & `inspire-matcher-9.0.9/inspire_matcher/api.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher/__init__.py` & `inspire-matcher-9.0.9/inspire_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/inspire_matcher.egg-info/PKG-INFO` & `inspire-matcher-9.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspire-matcher
-Version: 9.0.8
+Version: 9.0.9
 Summary: Find the records in INSPIRE most similar to a given record or reference.
 Home-page: https://github.com/inspirehep/inspire-matcher
 Author: CERN
 Author-email: admin@inspirehep.net
 License: GPLv3
 Description: ..
             This file is part of INSPIRE.
```

### Comparing `inspire-matcher-9.0.8/inspire_matcher.egg-info/requires.txt` & `inspire-matcher-9.0.9/inspire_matcher.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inspire-matcher-9.0.8/setup.py` & `inspire-matcher-9.0.9/setup.py`

 * *Files identical despite different names*

