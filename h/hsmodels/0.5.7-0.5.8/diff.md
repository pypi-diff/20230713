# Comparing `tmp/hsmodels-0.5.7.tar.gz` & `tmp/hsmodels-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmodels-0.5.7.tar", last modified: Thu Jul 13 14:23:28 2023, max compression
+gzip compressed data, was "hsmodels-0.5.8.tar", last modified: Thu Jul 13 16:01:18 2023, max compression
```

## Comparing `hsmodels-0.5.7.tar` & `hsmodels-0.5.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:28.677176 hsmodels-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-13 14:23:15.000000 hsmodels-0.5.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 14:23:28.677176 hsmodels-0.5.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:28.669176 hsmodels-0.5.7/hsmodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:28.673176 hsmodels-0.5.7/hsmodels/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19940 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    35730 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/fields.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14232 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/languages_iso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:28.673176 hsmodels-0.5.7/hsmodels/schemas/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/rdf/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/rdf/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/rdf/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/rdf/root_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/rdf/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/root_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/schemas/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 14:23:15.000000 hsmodels-0.5.7/hsmodels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:23:28.669176 hsmodels-0.5.7/hsmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 14:23:28.000000 hsmodels-0.5.7/hsmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 14:23:28.000000 hsmodels-0.5.7/hsmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:23:28.000000 hsmodels-0.5.7/hsmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 14:23:28.000000 hsmodels-0.5.7/hsmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 14:23:28.000000 hsmodels-0.5.7/hsmodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 14:23:28.677176 hsmodels-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 14:23:15.000000 hsmodels-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:18.096802 hsmodels-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-13 16:01:05.000000 hsmodels-0.5.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 16:01:18.096802 hsmodels-0.5.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:18.092802 hsmodels-0.5.8/hsmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:18.096802 hsmodels-0.5.8/hsmodels/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19940 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35730 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/fields.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14232 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/languages_iso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:18.096802 hsmodels-0.5.8/hsmodels/schemas/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/rdf/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/rdf/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/rdf/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/rdf/root_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/rdf/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/root_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/schemas/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 16:01:05.000000 hsmodels-0.5.8/hsmodels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:18.092802 hsmodels-0.5.8/hsmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 16:01:18.000000 hsmodels-0.5.8/hsmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 16:01:18.000000 hsmodels-0.5.8/hsmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:01:18.000000 hsmodels-0.5.8/hsmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-13 16:01:18.000000 hsmodels-0.5.8/hsmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 16:01:18.000000 hsmodels-0.5.8/hsmodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 16:01:18.096802 hsmodels-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-13 16:01:05.000000 hsmodels-0.5.8/setup.py
```

### Comparing `hsmodels-0.5.7/LICENSE.txt` & `hsmodels-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/PKG-INFO` & `hsmodels-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmodels
-Version: 0.5.7
+Version: 0.5.8
 Summary: Pydantic models for HydroShare metadata
 Home-page: https://github.com/hydroshare/hsmodels
 Author: Scott Black
 Author-email: sblack@cuahsi.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hsmodels-0.5.7/hsmodels/namespaces.py` & `hsmodels-0.5.8/hsmodels/namespaces.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/__init__.py` & `hsmodels-0.5.8/hsmodels/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/aggregations.py` & `hsmodels-0.5.8/hsmodels/schemas/aggregations.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/base_models.py` & `hsmodels-0.5.8/hsmodels/schemas/base_models.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/enums.py` & `hsmodels-0.5.8/hsmodels/schemas/enums.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/fields.py` & `hsmodels-0.5.8/hsmodels/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/languages_iso.py` & `hsmodels-0.5.8/hsmodels/schemas/languages_iso.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/rdf/aggregations.py` & `hsmodels-0.5.8/hsmodels/schemas/rdf/aggregations.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/rdf/fields.py` & `hsmodels-0.5.8/hsmodels/schemas/rdf/fields.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/rdf/resource.py` & `hsmodels-0.5.8/hsmodels/schemas/rdf/resource.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/rdf/root_validators.py` & `hsmodels-0.5.8/hsmodels/schemas/rdf/root_validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/rdf/validators.py` & `hsmodels-0.5.8/hsmodels/schemas/rdf/validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/resource.py` & `hsmodels-0.5.8/hsmodels/schemas/resource.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/root_validators.py` & `hsmodels-0.5.8/hsmodels/schemas/root_validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels/schemas/validators.py` & `hsmodels-0.5.8/hsmodels/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/hsmodels.egg-info/PKG-INFO` & `hsmodels-0.5.8/hsmodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmodels
-Version: 0.5.7
+Version: 0.5.8
 Summary: Pydantic models for HydroShare metadata
 Home-page: https://github.com/hydroshare/hsmodels
 Author: Scott Black
 Author-email: sblack@cuahsi.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hsmodels-0.5.7/hsmodels.egg-info/SOURCES.txt` & `hsmodels-0.5.8/hsmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsmodels-0.5.7/setup.py` & `hsmodels-0.5.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 README = 'Refer to the models section of https://hydroshare.github.io/hsclient/'# (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='hsmodels',
-    version='0.5.7',
+    version='0.5.8',
     packages=find_packages(include=['hsmodels', 'hsmodels.*', 'hsmodels.schemas.*', 'hsmodels.schemas.rdf.*'],
                            exclude=("tests",)),
     install_requires=[
         'rdflib<6.0.0',
-        'pydantic~=1.8.1',
+        'pydantic>=1.8.1,<2.0',
         'email-validator'
     ],
     url='https://github.com/hydroshare/hsmodels',
     license='MIT',
     author='Scott Black',
     author_email='sblack@cuahsi.org',
     description='Pydantic models for HydroShare metadata',
```

