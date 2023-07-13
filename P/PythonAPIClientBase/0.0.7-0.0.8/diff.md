# Comparing `tmp/PythonAPIClientBase-0.0.7.tar.gz` & `tmp/PythonAPIClientBase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonAPIClientBase-0.0.7.tar", last modified: Sat Jul 30 20:28:34 2022, max compression
+gzip compressed data, was "PythonAPIClientBase-0.0.8.tar", last modified: Thu Jul 13 12:31:05 2023, max compression
```

## Comparing `PythonAPIClientBase-0.0.7.tar` & `PythonAPIClientBase-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-30 20:28:34.736160 PythonAPIClientBase-0.0.7/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       62 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)      343 2022-07-30 20:28:34.736160 PythonAPIClientBase-0.0.7/PKG-INFO
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-30 20:28:34.736160 PythonAPIClientBase-0.0.7/PythonAPIClientBase/
--rw-rw-r--   0 robert    (1000) robert    (1000)     4567 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase/APIClientBase.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      503 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase/LoginSession.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5911 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase/Mock.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      271 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      497 2022-07-30 20:28:34.736160 PythonAPIClientBase-0.0.7/PythonAPIClientBase/_version.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-30 20:28:34.736160 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)      343 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      483 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)       53 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       20 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.7/PythonAPIClientBase.egg-info/top_level.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       25 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      313 2022-07-30 20:28:34.736160 PythonAPIClientBase-0.0.7/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)      987 2022-07-30 20:26:56.000000 PythonAPIClientBase-0.0.7/setup.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.7/versioneer.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       62 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)      343 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PKG-INFO
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PythonAPIClientBase/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4567 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/APIClientBase.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      503 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/LoginSession.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5911 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/Mock.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      271 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      497 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PythonAPIClientBase/_version.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      343 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      483 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)       53 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       20 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/top_level.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       25 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      313 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)      987 2023-07-13 12:30:44.000000 PythonAPIClientBase-0.0.8/setup.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/versioneer.py
```

### Comparing `PythonAPIClientBase-0.0.7/LICENSE` & `PythonAPIClientBase-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonAPIClientBase-0.0.7/PythonAPIClientBase/APIClientBase.py` & `PythonAPIClientBase-0.0.8/PythonAPIClientBase/APIClientBase.py`

 * *Files identical despite different names*

### Comparing `PythonAPIClientBase-0.0.7/PythonAPIClientBase/Mock.py` & `PythonAPIClientBase-0.0.8/PythonAPIClientBase/Mock.py`

 * *Files identical despite different names*

### Comparing `PythonAPIClientBase-0.0.7/setup.py` & `PythonAPIClientBase-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import versioneer
 
 #Dependancy lists maintained here and in tox.ini
 sp_install_requires = [
-  'requests==2.28.1',
+  'requests==2.31.0',
   'pytz==2019.3',
   'python-dateutil==2.8.1'
 ]
 sp_tests_require = [
   'nose==1.3.7',
   'python_Testing_Utilities==0.1.9'
 ]
```

### Comparing `PythonAPIClientBase-0.0.7/versioneer.py` & `PythonAPIClientBase-0.0.8/versioneer.py`

 * *Files identical despite different names*

