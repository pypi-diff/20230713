# Comparing `tmp/pwed-cdk-0.0.67.tar.gz` & `tmp/pwed-cdk-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwed-cdk-0.0.67.tar", last modified: Thu Jul 13 05:40:31 2023, max compression
+gzip compressed data, was "pwed-cdk-0.0.68.tar", last modified: Thu Jul 13 06:31:38 2023, max compression
```

## Comparing `pwed-cdk-0.0.67.tar` & `pwed-cdk-0.0.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.637454 pwed-cdk-0.0.67/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-13 05:40:31.637454 pwed-cdk-0.0.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:40:31.637454 pwed-cdk-0.0.67/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.629454 pwed-cdk-0.0.67/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.629454 pwed-cdk-0.0.67/src/pwed_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.633454 pwed-cdk-0.0.67/src/pwed_cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  3954542 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/_jsii/pwed-cdk@0.0.67.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.637454 pwed-cdk-0.0.67/src/pwed_cdk/bastion/
--rw-r--r--   0 runner    (1001) docker     (123)    91868 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/bastion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.637454 pwed-cdk-0.0.67/src/pwed_cdk/static_site/
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/static_site/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.637454 pwed-cdk-0.0.67/src/pwed_cdk/ttl/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-13 05:40:18.000000 pwed-cdk-0.0.67/src/pwed_cdk/ttl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:40:31.633454 pwed-cdk-0.0.67/src/pwed_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-13 05:40:31.000000 pwed-cdk-0.0.67/src/pwed_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-13 05:40:31.000000 pwed-cdk-0.0.67/src/pwed_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:40:31.000000 pwed-cdk-0.0.67/src/pwed_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 05:40:31.000000 pwed-cdk-0.0.67/src/pwed_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 05:40:31.000000 pwed-cdk-0.0.67/src/pwed_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.472788 pwed-cdk-0.0.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-13 06:31:38.472788 pwed-cdk-0.0.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:31:38.472788 pwed-cdk-0.0.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.464788 pwed-cdk-0.0.68/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.464788 pwed-cdk-0.0.68/src/pwed_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.464788 pwed-cdk-0.0.68/src/pwed_cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  5494583 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/_jsii/pwed-cdk@0.0.68.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.472788 pwed-cdk-0.0.68/src/pwed_cdk/bastion/
+-rw-r--r--   0 runner    (1001) docker     (123)    91868 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/bastion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.472788 pwed-cdk-0.0.68/src/pwed_cdk/static_site/
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/static_site/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.472788 pwed-cdk-0.0.68/src/pwed_cdk/ttl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-13 06:31:25.000000 pwed-cdk-0.0.68/src/pwed_cdk/ttl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:31:38.464788 pwed-cdk-0.0.68/src/pwed_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-13 06:31:38.000000 pwed-cdk-0.0.68/src/pwed_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-13 06:31:38.000000 pwed-cdk-0.0.68/src/pwed_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:31:38.000000 pwed-cdk-0.0.68/src/pwed_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 06:31:38.000000 pwed-cdk-0.0.68/src/pwed_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 06:31:38.000000 pwed-cdk-0.0.68/src/pwed_cdk.egg-info/top_level.txt
```

### Comparing `pwed-cdk-0.0.67/LICENSE` & `pwed-cdk-0.0.68/LICENSE`

 * *Files identical despite different names*

### Comparing `pwed-cdk-0.0.67/PKG-INFO` & `pwed-cdk-0.0.68/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwed-cdk
-Version: 0.0.67
+Version: 0.0.68
 Summary: A library of AWS CDK constructs that I have created
 Home-page: https://github.com/pwed/pwed-cdk.git
 Author: Fred Stoddart<pwed@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/pwed/pwed-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pwed-cdk-0.0.67/README.md` & `pwed-cdk-0.0.68/README.md`

 * *Files identical despite different names*

### Comparing `pwed-cdk-0.0.67/setup.py` & `pwed-cdk-0.0.68/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pwed-cdk",
-    "version": "0.0.67",
+    "version": "0.0.68",
     "description": "A library of AWS CDK constructs that I have created",
     "license": "MIT",
     "url": "https://github.com/pwed/pwed-cdk.git",
     "long_description_content_type": "text/markdown",
     "author": "Fred Stoddart<pwed@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -25,15 +25,15 @@
         "pwed_cdk._jsii",
         "pwed_cdk.bastion",
         "pwed_cdk.static_site",
         "pwed_cdk.ttl"
     ],
     "package_data": {
         "pwed_cdk._jsii": [
-            "pwed-cdk@0.0.67.jsii.tgz"
+            "pwed-cdk@0.0.68.jsii.tgz"
         ],
         "pwed_cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pwed-cdk-0.0.67/src/pwed_cdk/__init__.py` & `pwed-cdk-0.0.68/src/pwed_cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pwed-cdk-0.0.67/src/pwed_cdk/bastion/__init__.py` & `pwed-cdk-0.0.68/src/pwed_cdk/bastion/__init__.py`

 * *Files identical despite different names*

### Comparing `pwed-cdk-0.0.67/src/pwed_cdk/static_site/__init__.py` & `pwed-cdk-0.0.68/src/pwed_cdk/static_site/__init__.py`

 * *Files identical despite different names*

### Comparing `pwed-cdk-0.0.67/src/pwed_cdk/ttl/__init__.py` & `pwed-cdk-0.0.68/src/pwed_cdk/ttl/__init__.py`

 * *Files identical despite different names*

### Comparing `pwed-cdk-0.0.67/src/pwed_cdk.egg-info/PKG-INFO` & `pwed-cdk-0.0.68/src/pwed_cdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwed-cdk
-Version: 0.0.67
+Version: 0.0.68
 Summary: A library of AWS CDK constructs that I have created
 Home-page: https://github.com/pwed/pwed-cdk.git
 Author: Fred Stoddart<pwed@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/pwed/pwed-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

