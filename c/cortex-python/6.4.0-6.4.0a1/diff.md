# Comparing `tmp/cortex-python-6.4.0.tar.gz` & `tmp/cortex-python-6.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex-python-6.4.0.tar", last modified: Thu Jul 13 17:40:31 2023, max compression
+gzip compressed data, was "cortex-python-6.4.0a1.tar", last modified: Thu Jul 13 20:00:48 2023, max compression
```

## Comparing `cortex-python-6.4.0.tar` & `cortex-python-6.4.0a1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.683555 cortex-python-6.4.0/
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-13 17:37:47.000000 cortex-python-6.4.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11368 2023-07-13 17:37:47.000000 cortex-python-6.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-13 17:37:47.000000 cortex-python-6.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4621 2023-07-13 17:40:31.683555 cortex-python-6.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3938 2023-07-13 17:37:47.000000 cortex-python-6.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/cortex/
--rw-r--r--   0 root         (0) root         (0)      667 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/auth.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/camel.py
--rw-r--r--   0 root         (0) root         (0)    27238 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/client.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/connection.py
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/constant.py
--rw-r--r--   0 root         (0) root         (0)     9669 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/content.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/env.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/cortex/experiment/
--rw-r--r--   0 root         (0) root         (0)      675 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7794 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/local.py
--rw-r--r--   0 root         (0) root         (0)    10770 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/model.py
--rw-r--r--   0 root         (0) root         (0)    37474 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/experiment/remote.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/message.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/model.py
--rw-r--r--   0 root         (0) root         (0)    10071 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/properties.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/secrets.py
--rw-r--r--   0 root         (0) root         (0)    11705 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/serviceconnector.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/session.py
--rw-r--r--   0 root         (0) root         (0)     8521 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/skill.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/timer.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/types.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/utils.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-07-13 17:37:47.000000 cortex-python-6.4.0/cortex/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/cortex_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4621 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 17:40:31.000000 cortex-python-6.4.0/cortex_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 17:40:31.683555 cortex-python-6.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2178 2023-07-13 17:37:47.000000 cortex-python-6.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.679555 cortex-python-6.4.0/test/
--rw-r--r--   0 root         (0) root         (0)      590 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:40:31.683555 cortex-python-6.4.0/test/unit/
--rw-r--r--   0 root         (0) root         (0)      590 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/authenticationclient_test.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/connectionclient_test.py
--rw-r--r--   0 root         (0) root         (0)     9029 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/cortex_test.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/environment_config_test.py
--rw-r--r--   0 root         (0) root         (0)     6424 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/experiment_test.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     8439 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/run_test.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/serviceconnector_test.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-07-13 17:37:47.000000 cortex-python-6.4.0/test/unit/sessionclient_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:00:48.402646 cortex-python-6.4.0a1/
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11368 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-07-13 20:00:48.402646 cortex-python-6.4.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:00:48.398646 cortex-python-6.4.0a1/cortex/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/camel.py
+-rw-r--r--   0 root         (0) root         (0)    27238 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/client.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/connection.py
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/constant.py
+-rw-r--r--   0 root         (0) root         (0)     9669 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/content.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/env.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:00:48.398646 cortex-python-6.4.0a1/cortex/experiment/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7794 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/experiment/local.py
+-rw-r--r--   0 root         (0) root         (0)    10770 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/experiment/model.py
+-rw-r--r--   0 root         (0) root         (0)    37474 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/experiment/remote.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/message.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/model.py
+-rw-r--r--   0 root         (0) root         (0)    10071 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/properties.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/secrets.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/serviceconnector.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/session.py
+-rw-r--r--   0 root         (0) root         (0)     8521 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/skill.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/timer.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/types.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/cortex/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:00:48.398646 cortex-python-6.4.0a1/cortex_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-07-13 20:00:48.000000 cortex-python-6.4.0a1/cortex_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-13 20:00:48.000000 cortex-python-6.4.0a1/cortex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 20:00:48.000000 cortex-python-6.4.0a1/cortex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-13 20:00:48.000000 cortex-python-6.4.0a1/cortex_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 20:00:48.000000 cortex-python-6.4.0a1/cortex_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-13 20:00:48.402646 cortex-python-6.4.0a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:00:48.398646 cortex-python-6.4.0a1/test/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:00:48.398646 cortex-python-6.4.0a1/test/unit/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/authenticationclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/connectionclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     9029 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/cortex_test.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/environment_config_test.py
+-rw-r--r--   0 root         (0) root         (0)     6424 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/experiment_test.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     8439 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/run_test.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/serviceconnector_test.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-13 19:58:29.000000 cortex-python-6.4.0a1/test/unit/sessionclient_test.py
```

### Comparing `cortex-python-6.4.0/CHANGELOG.md` & `cortex-python-6.4.0a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/LICENSE` & `cortex-python-6.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/PKG-INFO` & `cortex-python-6.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.4.0
+Version: 6.4.0a1
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.4.0/README.md` & `cortex-python-6.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/__init__.py` & `cortex-python-6.4.0a1/cortex/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/auth.py` & `cortex-python-6.4.0a1/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/camel.py` & `cortex-python-6.4.0a1/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/client.py` & `cortex-python-6.4.0a1/cortex/client.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/connection.py` & `cortex-python-6.4.0a1/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/constant.py` & `cortex-python-6.4.0a1/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/content.py` & `cortex-python-6.4.0a1/cortex/content.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/env.py` & `cortex-python-6.4.0a1/cortex/env.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/exceptions.py` & `cortex-python-6.4.0a1/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/experiment/__init__.py` & `cortex-python-6.4.0a1/cortex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/experiment/local.py` & `cortex-python-6.4.0a1/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/experiment/model.py` & `cortex-python-6.4.0a1/cortex/experiment/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/experiment/remote.py` & `cortex-python-6.4.0a1/cortex/experiment/remote.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/message.py` & `cortex-python-6.4.0a1/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/model.py` & `cortex-python-6.4.0a1/cortex/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/properties.py` & `cortex-python-6.4.0a1/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/secrets.py` & `cortex-python-6.4.0a1/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/serviceconnector.py` & `cortex-python-6.4.0a1/cortex/serviceconnector.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/session.py` & `cortex-python-6.4.0a1/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/skill.py` & `cortex-python-6.4.0a1/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/timer.py` & `cortex-python-6.4.0a1/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/types.py` & `cortex-python-6.4.0a1/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/utils.py` & `cortex-python-6.4.0a1/cortex/utils.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex/viz.py` & `cortex-python-6.4.0a1/cortex/viz.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/cortex_python.egg-info/PKG-INFO` & `cortex-python-6.4.0a1/cortex_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.4.0
+Version: 6.4.0a1
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.4.0/cortex_python.egg-info/SOURCES.txt` & `cortex-python-6.4.0a1/cortex_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/setup.py` & `cortex-python-6.4.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/__init__.py` & `cortex-python-6.4.0a1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/__init__.py` & `cortex-python-6.4.0a1/test/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/authenticationclient_test.py` & `cortex-python-6.4.0a1/test/unit/authenticationclient_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/connectionclient_test.py` & `cortex-python-6.4.0a1/test/unit/connectionclient_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/cortex_test.py` & `cortex-python-6.4.0a1/test/unit/cortex_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/environment_config_test.py` & `cortex-python-6.4.0a1/test/unit/environment_config_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/experiment_test.py` & `cortex-python-6.4.0a1/test/unit/experiment_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/fixtures.py` & `cortex-python-6.4.0a1/test/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/run_test.py` & `cortex-python-6.4.0a1/test/unit/run_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/serviceconnector_test.py` & `cortex-python-6.4.0a1/test/unit/serviceconnector_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0/test/unit/sessionclient_test.py` & `cortex-python-6.4.0a1/test/unit/sessionclient_test.py`

 * *Files identical despite different names*

