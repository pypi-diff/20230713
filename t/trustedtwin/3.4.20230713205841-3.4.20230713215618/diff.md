# Comparing `tmp/trustedtwin-3.4.20230713205841.tar.gz` & `tmp/trustedtwin-3.4.20230713215618.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustedtwin-3.4.20230713205841.tar", last modified: Thu Jul 13 20:58:58 2023, max compression
+gzip compressed data, was "trustedtwin-3.4.20230713215618.tar", last modified: Thu Jul 13 21:56:36 2023, max compression
```

## Comparing `trustedtwin-3.4.20230713205841.tar` & `trustedtwin-3.4.20230713215618.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/LICENSE
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:58:58.699361 trustedtwin-3.4.20230713205841/trustedtwin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api.py
--rw-r--r--   0 root         (0) root         (0)   105509 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api_async.py
--rw-r--r--   0 root         (0) root         (0)   126439 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api_async.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api_base.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:56:36.358293 trustedtwin-3.4.20230713215618/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-13 21:56:36.358293 trustedtwin-3.4.20230713215618/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-13 21:56:36.359293 trustedtwin-3.4.20230713215618/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:56:36.357293 trustedtwin-3.4.20230713215618/trustedtwin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/trustedtwin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/trustedtwin/tt_api.py
+-rw-r--r--   0 root         (0) root         (0)   105509 2023-07-13 21:56:35.000000 trustedtwin-3.4.20230713215618/trustedtwin/tt_api.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/trustedtwin/tt_api_async.py
+-rw-r--r--   0 root         (0) root         (0)   126439 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin/tt_api_async.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-13 21:56:15.000000 trustedtwin-3.4.20230713215618/trustedtwin/tt_api_base.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-07-13 21:56:35.000000 trustedtwin-3.4.20230713215618/trustedtwin/tt_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:56:36.358293 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 21:56:36.000000 trustedtwin-3.4.20230713215618/trustedtwin.egg-info/top_level.txt
```

### Comparing `trustedtwin-3.4.20230713205841/LICENSE` & `trustedtwin-3.4.20230713215618/LICENSE`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/PKG-INFO` & `trustedtwin-3.4.20230713215618/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 3.4.20230713205841
+Version: 3.4.20230713215618
 Summary: Trusted Twin Python client
 Home-page: https://gitlab.com/trustedtwin/trustedtwin-python
 Author: TrustedTwin
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
```

### Comparing `trustedtwin-3.4.20230713205841/README.md` & `trustedtwin-3.4.20230713215618/README.md`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/setup.py` & `trustedtwin-3.4.20230713215618/setup.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin/tt_api.py` & `trustedtwin-3.4.20230713215618/trustedtwin/tt_api.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin/tt_api.pyi` & `trustedtwin-3.4.20230713215618/trustedtwin/tt_api.pyi`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin/tt_api_async.py` & `trustedtwin-3.4.20230713215618/trustedtwin/tt_api_async.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin/tt_api_async.pyi` & `trustedtwin-3.4.20230713215618/trustedtwin/tt_api_async.pyi`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin/tt_api_base.py` & `trustedtwin-3.4.20230713215618/trustedtwin/tt_api_base.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin/tt_endpoints.py` & `trustedtwin-3.4.20230713215618/trustedtwin/tt_endpoints.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-3.4.20230713205841/trustedtwin.egg-info/PKG-INFO` & `trustedtwin-3.4.20230713215618/trustedtwin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 3.4.20230713205841
+Version: 3.4.20230713215618
 Summary: Trusted Twin Python client
 Home-page: https://gitlab.com/trustedtwin/trustedtwin-python
 Author: TrustedTwin
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
```

