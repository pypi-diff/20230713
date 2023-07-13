# Comparing `tmp/vmc_reporter-1.99.100.tar.gz` & `tmp/vmc_reporter-1.99.101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmc_reporter-1.99.100.tar", last modified: Thu Jul 13 13:25:49 2023, max compression
+gzip compressed data, was "vmc_reporter-1.99.101.tar", last modified: Thu Jul 13 13:40:28 2023, max compression
```

## Comparing `vmc_reporter-1.99.100.tar` & `vmc_reporter-1.99.101.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oli       (1000) oli       (1000)        0 2023-07-13 13:25:49.213021 vmc_reporter-1.99.100/
--rw-r--r--   0 oli       (1000) oli       (1000)      532 2023-07-13 13:25:49.213021 vmc_reporter-1.99.100/PKG-INFO
--rw-r--r--   0 oli       (1000) oli       (1000)       38 2023-07-13 13:25:49.213021 vmc_reporter-1.99.100/setup.cfg
--rw-r--r--   0 oli       (1000) oli       (1000)      854 2023-07-13 13:25:42.000000 vmc_reporter-1.99.100/setup.py
-drwxr-xr-x   0 oli       (1000) oli       (1000)        0 2023-07-13 13:25:49.213021 vmc_reporter-1.99.100/vmc_reporter/
--rw-r--r--   0 oli       (1000) oli       (1000)       45 2023-07-13 13:24:11.000000 vmc_reporter-1.99.100/vmc_reporter/__init__.py
-drwxr-xr-x   0 oli       (1000) oli       (1000)        0 2023-07-13 13:25:49.213021 vmc_reporter-1.99.100/vmc_reporter.egg-info/
--rw-r--r--   0 oli       (1000) oli       (1000)      532 2023-07-13 13:25:49.000000 vmc_reporter-1.99.100/vmc_reporter.egg-info/PKG-INFO
--rw-r--r--   0 oli       (1000) oli       (1000)      247 2023-07-13 13:25:49.000000 vmc_reporter-1.99.100/vmc_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 oli       (1000) oli       (1000)        1 2023-07-13 13:25:49.000000 vmc_reporter-1.99.100/vmc_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 oli       (1000) oli       (1000)        1 2023-07-13 13:13:16.000000 vmc_reporter-1.99.100/vmc_reporter.egg-info/not-zip-safe
--rw-r--r--   0 oli       (1000) oli       (1000)       10 2023-07-13 13:25:49.000000 vmc_reporter-1.99.100/vmc_reporter.egg-info/requires.txt
--rw-r--r--   0 oli       (1000) oli       (1000)       13 2023-07-13 13:25:49.000000 vmc_reporter-1.99.100/vmc_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 oli       (1000) oli       (1000)        0 2023-07-13 13:40:27.993021 vmc_reporter-1.99.101/
+-rw-r--r--   0 oli       (1000) oli       (1000)      532 2023-07-13 13:40:27.993021 vmc_reporter-1.99.101/PKG-INFO
+-rw-r--r--   0 oli       (1000) oli       (1000)       38 2023-07-13 13:40:27.993021 vmc_reporter-1.99.101/setup.cfg
+-rw-r--r--   0 oli       (1000) oli       (1000)      875 2023-07-13 13:40:19.000000 vmc_reporter-1.99.101/setup.py
+drwxr-xr-x   0 oli       (1000) oli       (1000)        0 2023-07-13 13:40:27.993021 vmc_reporter-1.99.101/vmc_reporter/
+-rw-r--r--   0 oli       (1000) oli       (1000)       45 2023-07-13 13:24:11.000000 vmc_reporter-1.99.101/vmc_reporter/__init__.py
+drwxr-xr-x   0 oli       (1000) oli       (1000)        0 2023-07-13 13:40:27.993021 vmc_reporter-1.99.101/vmc_reporter.egg-info/
+-rw-r--r--   0 oli       (1000) oli       (1000)      532 2023-07-13 13:40:27.000000 vmc_reporter-1.99.101/vmc_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 oli       (1000) oli       (1000)      247 2023-07-13 13:40:27.000000 vmc_reporter-1.99.101/vmc_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 oli       (1000) oli       (1000)        1 2023-07-13 13:40:27.000000 vmc_reporter-1.99.101/vmc_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 oli       (1000) oli       (1000)        1 2023-07-13 13:13:16.000000 vmc_reporter-1.99.101/vmc_reporter.egg-info/not-zip-safe
+-rw-r--r--   0 oli       (1000) oli       (1000)       10 2023-07-13 13:40:27.000000 vmc_reporter-1.99.101/vmc_reporter.egg-info/requires.txt
+-rw-r--r--   0 oli       (1000) oli       (1000)       13 2023-07-13 13:40:27.000000 vmc_reporter-1.99.101/vmc_reporter.egg-info/top_level.txt
```

### Comparing `vmc_reporter-1.99.100/PKG-INFO` & `vmc_reporter-1.99.101/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmc_reporter
-Version: 1.99.100
+Version: 1.99.101
 Summary: This package is supposed to prove a Dependency Confusion Attack
 Home-page: https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610
 Author: Appsec@SBB
 Author-email: application-security@sbb.ch
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vmc_reporter-1.99.100/setup.py` & `vmc_reporter-1.99.101/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 
+import vmc_reporter
+
 from setuptools import setup
 
 # package configuration - for reference see:
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#id9
 setup(
     name="vmc_reporter",
     description="This package is supposed to prove a Dependency Confusion Attack",
     long_description="This package is supposed to prove a Dependency Confusion Attack",
-    version="1.99.100",
+    version="1.99.101",
     author="Appsec@SBB",
     author_email="application-security@sbb.ch",
     url="https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610",
     packages=["vmc_reporter"],
     python_requires=">=3.10",
     install_requires=["packaging"],
     license="",
```

### Comparing `vmc_reporter-1.99.100/vmc_reporter.egg-info/PKG-INFO` & `vmc_reporter-1.99.101/vmc_reporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmc-reporter
-Version: 1.99.100
+Version: 1.99.101
 Summary: This package is supposed to prove a Dependency Confusion Attack
 Home-page: https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610
 Author: Appsec@SBB
 Author-email: application-security@sbb.ch
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

