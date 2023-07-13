# Comparing `tmp/upstox-2.0.1.tar.gz` & `tmp/upstox-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/upstox-2.0.1.tar", last modified: Sat Mar 21 11:45:40 2020, max compression
+gzip compressed data, was "dist/upstox-2.0.2.tar", last modified: Thu Jul 13 18:18:25 2023, max compression
```

## Comparing `upstox-2.0.1.tar` & `upstox-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 rishabhjain   (501) wheel        (0)        0 2020-03-21 11:45:40.000000 upstox-2.0.1/
--rw-r--r--   0 rishabhjain   (501) wheel        (0)     1063 2020-03-21 11:43:51.000000 upstox-2.0.1/LICENSE
--rw-r--r--   0 rishabhjain   (501) wheel        (0)       68 2020-03-21 11:43:51.000000 upstox-2.0.1/MANIFEST.in
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      733 2020-03-21 11:45:40.000000 upstox-2.0.1/PKG-INFO
--rw-r--r--   0 rishabhjain   (501) wheel        (0)    21317 2020-03-21 11:44:10.000000 upstox-2.0.1/README.md
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      108 2020-03-21 11:45:40.000000 upstox-2.0.1/setup.cfg
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      871 2020-03-21 11:44:10.000000 upstox-2.0.1/setup.py
-drwxr-xr-x   0 rishabhjain   (501) wheel        (0)        0 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox.egg-info/
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      733 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox.egg-info/PKG-INFO
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      385 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhjain   (501) wheel        (0)        1 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhjain   (501) wheel        (0)       33 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox.egg-info/requires.txt
--rw-r--r--   0 rishabhjain   (501) wheel        (0)       11 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox.egg-info/top_level.txt
-drwxr-xr-x   0 rishabhjain   (501) wheel        (0)        0 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox_api/
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      391 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/__init__.py
--rw-r--r--   0 rishabhjain   (501) wheel        (0)    37605 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/api.py
-drwxr-xr-x   0 rishabhjain   (501) wheel        (0)        0 2020-03-21 11:45:40.000000 upstox-2.0.1/upstox_api/constants/
--rw-r--r--   0 rishabhjain   (501) wheel        (0)        0 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/constants/__init__.py
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      365 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/constants/exchanges.py
--rw-r--r--   0 rishabhjain   (501) wheel        (0)      188 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/constants/misc.py
--rw-r--r--   0 rishabhjain   (501) wheel        (0)     1281 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/service_config.json
--rw-r--r--   0 rishabhjain   (501) wheel        (0)     6489 2020-03-21 11:44:10.000000 upstox-2.0.1/upstox_api/utils.py
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1063 2023-07-13 18:03:38.000000 upstox-2.0.2/LICENSE
+-rw-r--r--   0 foolish-works   (502) staff       (20)       68 2023-07-13 18:03:38.000000 upstox-2.0.2/MANIFEST.in
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1134 2023-07-13 18:18:25.000000 upstox-2.0.2/PKG-INFO
+-rw-r--r--   0 foolish-works   (502) staff       (20)    21317 2023-07-13 18:03:38.000000 upstox-2.0.2/README.md
+-rw-r--r--   0 foolish-works   (502) staff       (20)      108 2023-07-13 18:18:25.000000 upstox-2.0.2/setup.cfg
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1272 2023-07-13 18:18:12.000000 upstox-2.0.2/setup.py
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1134 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/PKG-INFO
+-rw-r--r--   0 foolish-works   (502) staff       (20)      385 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/SOURCES.txt
+-rw-r--r--   0 foolish-works   (502) staff       (20)        1 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/dependency_links.txt
+-rw-r--r--   0 foolish-works   (502) staff       (20)       33 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/requires.txt
+-rw-r--r--   0 foolish-works   (502) staff       (20)       11 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/top_level.txt
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox_api/
+-rw-r--r--   0 foolish-works   (502) staff       (20)      391 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/__init__.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)    37605 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/api.py
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox_api/constants/
+-rw-r--r--   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/constants/__init__.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)      365 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/constants/exchanges.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)      188 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/constants/misc.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1281 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/service_config.json
+-rw-r--r--   0 foolish-works   (502) staff       (20)     6489 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/utils.py
```

### Comparing `upstox-2.0.1/LICENSE` & `upstox-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upstox-2.0.1/PKG-INFO` & `upstox-2.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: upstox
-Version: 2.0.1
-Summary: Official Python library for Upstox APIs
+Version: 2.0.2
+Summary: DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.
 Home-page: https://github.com/upstox/upstox-python
 Author: Upstox Development Team
 Author-email: support@upstox.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: upstox,python,sdk,trading,stock markets
 Platform: UNKNOWN
```

### Comparing `upstox-2.0.1/README.md` & `upstox-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `upstox-2.0.1/upstox.egg-info/PKG-INFO` & `upstox-2.0.2/upstox.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: upstox
-Version: 2.0.1
-Summary: Official Python library for Upstox APIs
+Version: 2.0.2
+Summary: DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.
 Home-page: https://github.com/upstox/upstox-python
 Author: Upstox Development Team
 Author-email: support@upstox.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: upstox,python,sdk,trading,stock markets
 Platform: UNKNOWN
```

### Comparing `upstox-2.0.1/upstox_api/api.py` & `upstox-2.0.2/upstox_api/api.py`

 * *Files identical despite different names*

### Comparing `upstox-2.0.1/upstox_api/service_config.json` & `upstox-2.0.2/upstox_api/service_config.json`

 * *Files identical despite different names*

### Comparing `upstox-2.0.1/upstox_api/utils.py` & `upstox-2.0.2/upstox_api/utils.py`

 * *Files identical despite different names*

