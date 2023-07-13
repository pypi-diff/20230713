# Comparing `tmp/testit-adapter-nose-2.2.0.tar.gz` & `tmp/testit-adapter-nose-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-nose-2.2.0.tar", last modified: Tue Jul  4 08:50:14 2023, max compression
+gzip compressed data, was "testit-adapter-nose-2.2.1.tar", last modified: Thu Jul 13 08:39:44 2023, max compression
```

## Comparing `testit-adapter-nose-2.2.0.tar` & `testit-adapter-nose-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.120272 testit-adapter-nose-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.120272 testit-adapter-nose-2.2.0/src/testit_adapter_nose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:44.615941 testit-adapter-nose-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-13 08:39:44.615941 testit-adapter-nose-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-13 08:39:27.000000 testit-adapter-nose-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:39:44.615941 testit-adapter-nose-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-13 08:39:27.000000 testit-adapter-nose-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:44.611941 testit-adapter-nose-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:44.615941 testit-adapter-nose-2.2.1/src/testit_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:27.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-13 08:39:27.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-13 08:39:27.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-13 08:39:27.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:44.615941 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-13 08:39:44.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-13 08:39:44.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:39:44.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 08:39:44.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 08:39:44.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 08:39:44.000000 testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/top_level.txt
```

### Comparing `testit-adapter-nose-2.2.0/PKG-INFO` & `testit-adapter-nose-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.2.0
+Version: 2.2.1
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-nose-2.2.0/README.md` & `testit-adapter-nose-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.2.0/setup.py` & `testit-adapter-nose-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testit-adapter-nose',
-    version='2.2.0',
+    version='2.2.1',
     description='Nose adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,14 +16,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testit-python-commons==2.2.0'],
+    install_requires=['attrs', 'nose2', 'testit-python-commons==2.2.1'],
     entry_points={
             'nose.plugins.0.10': [
                 'testit_adapter_nose = testit_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testit-adapter-nose-2.2.0/src/testit_adapter_nose/listener.py` & `testit-adapter-nose-2.2.1/src/testit_adapter_nose/listener.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.2.0/src/testit_adapter_nose/plugin.py` & `testit-adapter-nose-2.2.1/src/testit_adapter_nose/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.2.0/src/testit_adapter_nose/utils.py` & `testit-adapter-nose-2.2.1/src/testit_adapter_nose/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/PKG-INFO` & `testit-adapter-nose-2.2.1/src/testit_adapter_nose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.2.0
+Version: 2.2.1
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

