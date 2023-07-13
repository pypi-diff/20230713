# Comparing `tmp/upstox-2.0.2.tar.gz` & `tmp/upstox-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/upstox-2.0.2.tar", last modified: Thu Jul 13 18:18:25 2023, max compression
+gzip compressed data, was "dist/upstox-2.0.3.tar", last modified: Thu Jul 13 18:21:32 2023, max compression
```

## Comparing `upstox-2.0.2.tar` & `upstox-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/
--rw-r--r--   0 foolish-works   (502) staff       (20)     1063 2023-07-13 18:03:38.000000 upstox-2.0.2/LICENSE
--rw-r--r--   0 foolish-works   (502) staff       (20)       68 2023-07-13 18:03:38.000000 upstox-2.0.2/MANIFEST.in
--rw-r--r--   0 foolish-works   (502) staff       (20)     1134 2023-07-13 18:18:25.000000 upstox-2.0.2/PKG-INFO
--rw-r--r--   0 foolish-works   (502) staff       (20)    21317 2023-07-13 18:03:38.000000 upstox-2.0.2/README.md
--rw-r--r--   0 foolish-works   (502) staff       (20)      108 2023-07-13 18:18:25.000000 upstox-2.0.2/setup.cfg
--rw-r--r--   0 foolish-works   (502) staff       (20)     1272 2023-07-13 18:18:12.000000 upstox-2.0.2/setup.py
-drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/
--rw-r--r--   0 foolish-works   (502) staff       (20)     1134 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/PKG-INFO
--rw-r--r--   0 foolish-works   (502) staff       (20)      385 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/SOURCES.txt
--rw-r--r--   0 foolish-works   (502) staff       (20)        1 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/dependency_links.txt
--rw-r--r--   0 foolish-works   (502) staff       (20)       33 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/requires.txt
--rw-r--r--   0 foolish-works   (502) staff       (20)       11 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox.egg-info/top_level.txt
-drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox_api/
--rw-r--r--   0 foolish-works   (502) staff       (20)      391 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/__init__.py
--rw-r--r--   0 foolish-works   (502) staff       (20)    37605 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/api.py
-drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:18:25.000000 upstox-2.0.2/upstox_api/constants/
--rw-r--r--   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/constants/__init__.py
--rw-r--r--   0 foolish-works   (502) staff       (20)      365 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/constants/exchanges.py
--rw-r--r--   0 foolish-works   (502) staff       (20)      188 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/constants/misc.py
--rw-r--r--   0 foolish-works   (502) staff       (20)     1281 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/service_config.json
--rw-r--r--   0 foolish-works   (502) staff       (20)     6489 2023-07-13 18:03:38.000000 upstox-2.0.2/upstox_api/utils.py
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:21:32.000000 upstox-2.0.3/
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1063 2023-07-13 18:03:38.000000 upstox-2.0.3/LICENSE
+-rw-r--r--   0 foolish-works   (502) staff       (20)       68 2023-07-13 18:03:38.000000 upstox-2.0.3/MANIFEST.in
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1179 2023-07-13 18:21:32.000000 upstox-2.0.3/PKG-INFO
+-rw-r--r--   0 foolish-works   (502) staff       (20)    21317 2023-07-13 18:03:38.000000 upstox-2.0.3/README.md
+-rw-r--r--   0 foolish-works   (502) staff       (20)      108 2023-07-13 18:21:32.000000 upstox-2.0.3/setup.cfg
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1349 2023-07-13 18:21:22.000000 upstox-2.0.3/setup.py
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox.egg-info/
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1179 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox.egg-info/PKG-INFO
+-rw-r--r--   0 foolish-works   (502) staff       (20)      385 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox.egg-info/SOURCES.txt
+-rw-r--r--   0 foolish-works   (502) staff       (20)        1 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox.egg-info/dependency_links.txt
+-rw-r--r--   0 foolish-works   (502) staff       (20)       33 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox.egg-info/requires.txt
+-rw-r--r--   0 foolish-works   (502) staff       (20)       11 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox.egg-info/top_level.txt
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox_api/
+-rw-r--r--   0 foolish-works   (502) staff       (20)      391 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/__init__.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)    37605 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/api.py
+drwxr-xr-x   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:21:32.000000 upstox-2.0.3/upstox_api/constants/
+-rw-r--r--   0 foolish-works   (502) staff       (20)        0 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/constants/__init__.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)      365 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/constants/exchanges.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)      188 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/constants/misc.py
+-rw-r--r--   0 foolish-works   (502) staff       (20)     1281 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/service_config.json
+-rw-r--r--   0 foolish-works   (502) staff       (20)     6489 2023-07-13 18:03:38.000000 upstox-2.0.3/upstox_api/utils.py
```

### Comparing `upstox-2.0.2/LICENSE` & `upstox-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `upstox-2.0.2/PKG-INFO` & `upstox-2.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: upstox
-Version: 2.0.2
-Summary: DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.
+Version: 2.0.3
+Summary: DEPRECATED - Official Python library for Upstox APIs
 Home-page: https://github.com/upstox/upstox-python
 Author: Upstox Development Team
 Author-email: support@upstox.com
 License: UNKNOWN
-Description: UNKNOWN
+Description: DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.
 Keywords: upstox,python,sdk,trading,stock markets
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `upstox-2.0.2/README.md` & `upstox-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `upstox-2.0.2/setup.py` & `upstox-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 setup(
   name = 'upstox',
   packages = ['upstox_api', 'upstox_api.constants'],
-  version = '2.0.2',
+  version = '2.0.3',
   include_package_data=True,
-  description = 'DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.',
+  description = 'DEPRECATED - Official Python library for Upstox APIs',
+  long_description = 'DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.',
   author = 'Upstox Development Team',
   author_email = 'support@upstox.com',
   url = 'https://github.com/upstox/upstox-python',
   install_requires=['future', 'requests', 'websocket_client'],
   keywords = ['upstox', 'python', 'sdk', 'trading', 'stock markets'],
   classifiers=[
     'Intended Audience :: Developers',
```

### Comparing `upstox-2.0.2/upstox.egg-info/PKG-INFO` & `upstox-2.0.3/upstox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: upstox
-Version: 2.0.2
-Summary: DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.
+Version: 2.0.3
+Summary: DEPRECATED - Official Python library for Upstox APIs
 Home-page: https://github.com/upstox/upstox-python
 Author: Upstox Development Team
 Author-email: support@upstox.com
 License: UNKNOWN
-Description: UNKNOWN
+Description: DEPRECATED - The Upstox Python SDK is in its end-of-life stage and has been deprecated. We strongly encourage you to transition to the updated package, upstox-python-sdk. This can be installed via pip install upstox-python-sdk (find further details at https://pypi.org/project/upstox-python-sdk/). The new package ensures full compatibility with Upstox API v2.0, as well as subsequent versions, and will receive ongoing updates and support.
 Keywords: upstox,python,sdk,trading,stock markets
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `upstox-2.0.2/upstox_api/api.py` & `upstox-2.0.3/upstox_api/api.py`

 * *Files identical despite different names*

### Comparing `upstox-2.0.2/upstox_api/service_config.json` & `upstox-2.0.3/upstox_api/service_config.json`

 * *Files identical despite different names*

### Comparing `upstox-2.0.2/upstox_api/utils.py` & `upstox-2.0.3/upstox_api/utils.py`

 * *Files identical despite different names*

