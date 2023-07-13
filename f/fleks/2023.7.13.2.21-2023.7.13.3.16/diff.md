# Comparing `tmp/fleks-2023.7.13.2.21.tar.gz` & `tmp/fleks-2023.7.13.3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleks-2023.7.13.2.21.tar", last modified: Thu Jul 13 02:21:26 2023, max compression
+gzip compressed data, was "fleks-2023.7.13.3.16.tar", last modified: Thu Jul 13 03:16:49 2023, max compression
```

## Comparing `fleks-2023.7.13.2.21.tar` & `fleks-2023.7.13.3.16.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.877799 fleks-2023.7.13.2.21/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 02:21:26.877799 fleks-2023.7.13.2.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-13 02:21:26.877799 fleks-2023.7.13.2.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.869799 fleks-2023.7.13.2.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.873798 fleks-2023.7.13.2.21/src/fleks/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 02:21:21.000000 fleks-2023.7.13.2.21/src/fleks/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.873798 fleks-2023.7.13.2.21/src/fleks/app/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.877799 fleks-2023.7.13.2.21/src/fleks/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-13 02:20:24.000000 fleks-2023.7.13.2.21/src/fleks/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/cli/root_group.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.877799 fleks-2023.7.13.2.21/src/fleks/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/meta/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-13 02:20:24.000000 fleks-2023.7.13.2.21/src/fleks/meta/oop.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.877799 fleks-2023.7.13.2.21/src/fleks/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-13 02:19:30.000000 fleks-2023.7.13.2.21/src/fleks/util/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-13 02:20:24.000000 fleks-2023.7.13.2.21/src/fleks/util/lme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-13 02:20:24.000000 fleks-2023.7.13.2.21/src/fleks/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:21:26.873798 fleks-2023.7.13.2.21/src/fleks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 02:21:26.000000 fleks-2023.7.13.2.21/src/fleks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-13 02:21:26.000000 fleks-2023.7.13.2.21/src/fleks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:21:26.000000 fleks-2023.7.13.2.21/src/fleks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:21:26.000000 fleks-2023.7.13.2.21/src/fleks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 02:21:26.000000 fleks-2023.7.13.2.21/src/fleks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 02:21:26.000000 fleks-2023.7.13.2.21/src/fleks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.309157 fleks-2023.7.13.3.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 03:16:49.309157 fleks-2023.7.13.3.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-13 03:16:49.309157 fleks-2023.7.13.3.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.301157 fleks-2023.7.13.3.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.305157 fleks-2023.7.13.3.16/src/fleks/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 03:16:45.000000 fleks-2023.7.13.3.16/src/fleks/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.305157 fleks-2023.7.13.3.16/src/fleks/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.309157 fleks-2023.7.13.3.16/src/fleks/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-13 03:16:05.000000 fleks-2023.7.13.3.16/src/fleks/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/cli/root_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.309157 fleks-2023.7.13.3.16/src/fleks/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/meta/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-13 03:16:05.000000 fleks-2023.7.13.3.16/src/fleks/meta/oop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.309157 fleks-2023.7.13.3.16/src/fleks/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-13 03:15:27.000000 fleks-2023.7.13.3.16/src/fleks/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-13 03:16:05.000000 fleks-2023.7.13.3.16/src/fleks/util/lme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-13 03:16:05.000000 fleks-2023.7.13.3.16/src/fleks/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:16:49.305157 fleks-2023.7.13.3.16/src/fleks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 03:16:49.000000 fleks-2023.7.13.3.16/src/fleks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-13 03:16:49.000000 fleks-2023.7.13.3.16/src/fleks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:16:49.000000 fleks-2023.7.13.3.16/src/fleks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:16:49.000000 fleks-2023.7.13.3.16/src/fleks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 03:16:49.000000 fleks-2023.7.13.3.16/src/fleks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 03:16:49.000000 fleks-2023.7.13.3.16/src/fleks.egg-info/top_level.txt
```

### Comparing `fleks-2023.7.13.2.21/PKG-INFO` & `fleks-2023.7.13.3.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2023.7.13.2.21
+Version: 2023.7.13.3.16
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
```

### Comparing `fleks-2023.7.13.2.21/README.md` & `fleks-2023.7.13.3.16/README.md`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/setup.cfg` & `fleks-2023.7.13.3.16/setup.cfg`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/setup.py` & `fleks-2023.7.13.3.16/setup.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/cli/click.py` & `fleks-2023.7.13.3.16/src/fleks/cli/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/cli/options.py` & `fleks-2023.7.13.3.16/src/fleks/cli/options.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/cli/root_group.py` & `fleks-2023.7.13.3.16/src/fleks/cli/root_group.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/meta/namespace.py` & `fleks-2023.7.13.3.16/src/fleks/meta/namespace.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/meta/oop.py` & `fleks-2023.7.13.3.16/src/fleks/meta/oop.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/plugin.py` & `fleks-2023.7.13.3.16/src/fleks/plugin.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/util/__init__.py` & `fleks-2023.7.13.3.16/src/fleks/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/util/click.py` & `fleks-2023.7.13.3.16/src/fleks/util/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/util/lme.py` & `fleks-2023.7.13.3.16/src/fleks/util/lme.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks/util/typing.py` & `fleks-2023.7.13.3.16/src/fleks/util/typing.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.13.2.21/src/fleks.egg-info/PKG-INFO` & `fleks-2023.7.13.3.16/src/fleks.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2023.7.13.2.21
+Version: 2023.7.13.3.16
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
```

### Comparing `fleks-2023.7.13.2.21/src/fleks.egg-info/SOURCES.txt` & `fleks-2023.7.13.3.16/src/fleks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

