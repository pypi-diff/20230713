# Comparing `tmp/kk-plugins-0.1.230628.tar.gz` & `tmp/kk-plugins-0.1.230713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-plugins-0.1.230628.tar", last modified: Wed Jun 28 02:01:16 2023, max compression
+gzip compressed data, was "kk-plugins-0.1.230713.tar", last modified: Thu Jul 13 15:06:13 2023, max compression
```

## Comparing `kk-plugins-0.1.230628.tar` & `kk-plugins-0.1.230713.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 02:01:16.161346 kk-plugins-0.1.230628/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-28 02:01:16.161346 kk-plugins-0.1.230628/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 02:01:06.000000 kk-plugins-0.1.230628/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 02:01:16.161346 kk-plugins-0.1.230628/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-28 02:01:06.000000 kk-plugins-0.1.230628/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 02:01:16.157346 kk-plugins-0.1.230628/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 02:01:16.161346 kk-plugins-0.1.230628/src/kk_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-28 02:01:06.000000 kk-plugins-0.1.230628/src/kk_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-28 02:01:06.000000 kk-plugins-0.1.230628/src/kk_plugins/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-28 02:01:06.000000 kk-plugins-0.1.230628/src/kk_plugins/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 02:01:16.161346 kk-plugins-0.1.230628/src/kk_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-28 02:01:16.000000 kk-plugins-0.1.230628/src/kk_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-28 02:01:16.000000 kk-plugins-0.1.230628/src/kk_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 02:01:16.000000 kk-plugins-0.1.230628/src/kk_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-28 02:01:16.000000 kk-plugins-0.1.230628/src/kk_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 02:01:16.000000 kk-plugins-0.1.230628/src/kk_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:06:13.182284 kk-plugins-0.1.230713/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-13 15:06:13.182284 kk-plugins-0.1.230713/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 15:06:03.000000 kk-plugins-0.1.230713/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:06:13.182284 kk-plugins-0.1.230713/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-13 15:06:03.000000 kk-plugins-0.1.230713/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:06:13.182284 kk-plugins-0.1.230713/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:06:13.182284 kk-plugins-0.1.230713/src/kk_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 15:06:03.000000 kk-plugins-0.1.230713/src/kk_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-13 15:06:03.000000 kk-plugins-0.1.230713/src/kk_plugins/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-13 15:06:03.000000 kk-plugins-0.1.230713/src/kk_plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:06:13.182284 kk-plugins-0.1.230713/src/kk_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-13 15:06:13.000000 kk-plugins-0.1.230713/src/kk_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-13 15:06:13.000000 kk-plugins-0.1.230713/src/kk_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:06:13.000000 kk-plugins-0.1.230713/src/kk_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 15:06:13.000000 kk-plugins-0.1.230713/src/kk_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 15:06:13.000000 kk-plugins-0.1.230713/src/kk_plugins.egg-info/top_level.txt
```

### Comparing `kk-plugins-0.1.230628/PKG-INFO` & `kk-plugins-0.1.230713/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.1.230628
+Version: 0.1.230713
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kk-plugins-0.1.230628/setup.py` & `kk-plugins-0.1.230713/setup.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.230628/src/kk_plugins/project.py` & `kk-plugins-0.1.230713/src/kk_plugins/project.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.230628/src/kk_plugins.egg-info/PKG-INFO` & `kk-plugins-0.1.230713/src/kk_plugins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.1.230628
+Version: 0.1.230713
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

