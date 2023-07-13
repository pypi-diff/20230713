# Comparing `tmp/specklia-1.2.8.tar.gz` & `tmp/specklia-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.2.8.tar", last modified: Fri Jul  7 18:58:19 2023, max compression
+gzip compressed data, was "specklia-1.2.9.tar", last modified: Mon Jul 10 09:56:54 2023, max compression
```

## Comparing `specklia-1.2.8.tar` & `specklia-1.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:58:19.880058 specklia-1.2.8/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-07 18:58:12.000000 specklia-1.2.8/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2712 2023-07-07 18:58:19.880058 specklia-1.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-07 18:58:12.000000 specklia-1.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-07 18:58:19.880058 specklia-1.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2365 2023-07-07 18:58:12.000000 specklia-1.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:58:19.880058 specklia-1.2.8/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-07 18:58:12.000000 specklia-1.2.8/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-07-07 18:58:12.000000 specklia-1.2.8/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    35318 2023-07-07 18:58:12.000000 specklia-1.2.8/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:58:19.880058 specklia-1.2.8/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2712 2023-07-07 18:58:19.000000 specklia-1.2.8/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-07 18:58:19.000000 specklia-1.2.8/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 18:58:19.000000 specklia-1.2.8/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-07 18:58:19.000000 specklia-1.2.8/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-07 18:58:19.000000 specklia-1.2.8/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:58:19.880058 specklia-1.2.8/tests/
--rw-r--r--   0 root         (0) root         (0)    10232 2023-07-07 18:58:12.000000 specklia-1.2.8/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-07-07 18:58:12.000000 specklia-1.2.8/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:56:54.815211 specklia-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-10 09:38:23.000000 specklia-1.2.9/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-10 09:56:54.815211 specklia-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-10 09:38:23.000000 specklia-1.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-10 09:56:54.815211 specklia-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-10 09:38:23.000000 specklia-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:56:54.815211 specklia-1.2.9/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-10 09:38:23.000000 specklia-1.2.9/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-07-10 09:38:23.000000 specklia-1.2.9/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35318 2023-07-10 09:38:23.000000 specklia-1.2.9/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:56:54.815211 specklia-1.2.9/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-10 09:56:54.000000 specklia-1.2.9/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-10 09:56:54.000000 specklia-1.2.9/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:56:54.000000 specklia-1.2.9/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-10 09:56:54.000000 specklia-1.2.9/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-10 09:56:54.000000 specklia-1.2.9/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:56:54.815211 specklia-1.2.9/tests/
+-rw-r--r--   0 root         (0) root         (0)    10232 2023-07-10 09:38:23.000000 specklia-1.2.9/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-07-10 09:38:23.000000 specklia-1.2.9/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.2.8/LICENCE` & `specklia-1.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.2.8/PKG-INFO` & `specklia-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/change_log.html
```

### Comparing `specklia-1.2.8/README.md` & `specklia-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.2.8/setup.py` & `specklia-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.8/specklia/_websocket_helpers.py` & `specklia-1.2.9/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.8/specklia/client.py` & `specklia-1.2.9/specklia/client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.8/specklia.egg-info/PKG-INFO` & `specklia-1.2.9/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/change_log.html
```

### Comparing `specklia-1.2.8/tests/test_client.py` & `specklia-1.2.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.8/tests/test_websocket_helpers.py` & `specklia-1.2.9/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

