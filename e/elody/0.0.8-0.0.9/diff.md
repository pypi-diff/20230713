# Comparing `tmp/elody-0.0.8.tar.gz` & `tmp/elody-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elody-0.0.8.tar", last modified: Wed Jul 12 10:12:47 2023, max compression
+gzip compressed data, was "elody-0.0.9.tar", last modified: Wed Jul 12 10:58:58 2023, max compression
```

## Comparing `elody-0.0.8.tar` & `elody-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:12:47.640883 elody-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 10:12:37.000000 elody-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:12:47.640883 elody-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 10:12:37.000000 elody-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 10:12:37.000000 elody-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:12:47.640883 elody-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:12:47.636883 elody-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:12:47.640883 elody-0.0.8/src/elody/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 10:12:37.000000 elody-0.0.8/src/elody/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 10:12:37.000000 elody-0.0.8/src/elody/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 10:12:37.000000 elody-0.0.8/src/elody/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-12 10:12:37.000000 elody-0.0.8/src/elody/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 10:12:37.000000 elody-0.0.8/src/elody/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:12:47.640883 elody-0.0.8/src/elody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:12:47.000000 elody-0.0.8/src/elody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 10:12:47.000000 elody-0.0.8/src/elody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:12:47.000000 elody-0.0.8/src/elody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 10:12:47.000000 elody-0.0.8/src/elody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:12:47.000000 elody-0.0.8/src/elody.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.971030 elody-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 10:58:44.000000 elody-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:58:58.971030 elody-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 10:58:44.000000 elody-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 10:58:44.000000 elody-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:58:58.971030 elody-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.967030 elody-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.971030 elody-0.0.9/src/elody/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 10:58:44.000000 elody-0.0.9/src/elody/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:58:58.971030 elody-0.0.9/src/elody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:58:58.000000 elody-0.0.9/src/elody.egg-info/top_level.txt
```

### Comparing `elody-0.0.8/LICENSE` & `elody-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elody-0.0.8/PKG-INFO` & `elody-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.8
+Version: 0.0.9
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `elody-0.0.8/README.md` & `elody-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `elody-0.0.8/pyproject.toml` & `elody-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elody"
-version = "0.0.8"
+version = "0.0.9"
 description = "elody SDK for Python"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
```

### Comparing `elody-0.0.8/src/elody/client.py` & `elody-0.0.9/src/elody/client.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.8/src/elody/loader.py` & `elody-0.0.9/src/elody/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 from importlib import import_module
 from inuits_policy_based_auth.exceptions import (
     PolicyFactoryException,
 )
 
 
-def load_apps(flask_app):
-    apps = util.read_json_as_dict(os.getenv("APPS_MANIFEST"))
+def load_apps(flask_app, logger):
+    apps = util.read_json_as_dict(os.getenv("APPS_MANIFEST"), logger)
     for app in apps:
         for resource in apps[app].get("resources", []):
             api_bp = import_module(f"apps.{app}.resources.{resource}").api_bp
             flask_app.register_blueprint(api_bp)
 
 
 def load_policies(policy_factory, logger):
-    apps = util.read_json_as_dict(os.getenv("APPS_MANIFEST"))
+    apps = util.read_json_as_dict(os.getenv("APPS_MANIFEST"), logger)
     for app in apps:
         try:
             auth_type = "authentication"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
                 policy = __instantiate_authentication_policy(
                     policy_module_name, policy, logger
@@ -34,16 +34,16 @@
             policy_factory.set_fallback_key_for_policy_mapping(f"apps.{app}")
         except Exception as error:
             raise PolicyFactoryException(
                 f"Policy factory was not configured correctly: {str(error)}"
             ).with_traceback(error.__traceback__)
 
 
-def load_queues():
-    apps = util.read_json_as_dict(os.getenv("APPS_MANIFEST"))
+def load_queues(logger):
+    apps = util.read_json_as_dict(os.getenv("APPS_MANIFEST"), logger)
     for app in apps:
         try:
             import_module(f"apps.{app}.resources.queues")
         except ModuleNotFoundError:
             pass
```

### Comparing `elody-0.0.8/src/elody/util.py` & `elody-0.0.9/src/elody/util.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.8/src/elody.egg-info/PKG-INFO` & `elody-0.0.9/src/elody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.8
+Version: 0.0.9
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

