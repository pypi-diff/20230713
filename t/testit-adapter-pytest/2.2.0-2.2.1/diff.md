# Comparing `tmp/testit-adapter-pytest-2.2.0.tar.gz` & `tmp/testit-adapter-pytest-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-pytest-2.2.0.tar", last modified: Tue Jul  4 08:50:12 2023, max compression
+gzip compressed data, was "testit-adapter-pytest-2.2.1.tar", last modified: Thu Jul 13 08:39:29 2023, max compression
```

## Comparing `testit-adapter-pytest-2.2.0.tar` & `testit-adapter-pytest-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.158275 testit-adapter-pytest-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:29.393837 testit-adapter-pytest-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-13 08:39:29.393837 testit-adapter-pytest-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-13 08:39:19.000000 testit-adapter-pytest-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:39:29.393837 testit-adapter-pytest-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-13 08:39:19.000000 testit-adapter-pytest-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:29.389837 testit-adapter-pytest-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:29.393837 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:19.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-13 08:39:19.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-13 08:39:19.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-13 08:39:19.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:39:29.393837 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-13 08:39:29.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 08:39:29.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:39:29.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 08:39:29.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 08:39:29.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 08:39:29.000000 testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit-adapter-pytest-2.2.0/PKG-INFO` & `testit-adapter-pytest-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.2.0
+Version: 2.2.1
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-pytest-2.2.0/README.md` & `testit-adapter-pytest-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.2.0/setup.py` & `testit-adapter-pytest-2.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='2.2.0',
+    version='2.2.1',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,10 +16,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.2.0'],
+    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.2.1'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/listener.py` & `testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/listener.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/plugin.py` & `testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/utils.py` & `testit-adapter-pytest-2.2.1/src/testit_adapter_pytest/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit-adapter-pytest-2.2.1/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.2.0
+Version: 2.2.1
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

