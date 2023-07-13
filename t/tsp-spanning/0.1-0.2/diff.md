# Comparing `tmp/tsp_spanning-0.1.tar.gz` & `tmp/tsp_spanning-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelhouse/tsp_spanning-0.1.tar", last modified: Wed Nov  6 15:42:40 2019, max compression
+gzip compressed data, was "tsp_spanning-0.2.tar", last modified: Wed Jul 12 21:26:17 2023, max compression
```

## Comparing `tsp_spanning-0.1.tar` & `tsp_spanning-0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-11-06 15:42:40.000000 tsp_spanning-0.1/
--rw-r--r--   0 vsts      (1001) docker     (117)      874 2019-11-06 15:37:07.000000 tsp_spanning-0.1/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning/
--rw-r--r--   0 vsts      (1001) docker     (117)     1402 2019-11-06 15:37:07.000000 tsp_spanning-0.1/tsp_spanning/tsp_wrap.pyx
--rw-r--r--   0 vsts      (1001) docker     (117)   332466 2019-11-06 15:37:07.000000 tsp_spanning-0.1/tsp_spanning/tsp_wrap.cpp
--rw-r--r--   0 vsts      (1001) docker     (117)     5012 2019-11-06 15:37:07.000000 tsp_spanning-0.1/tsp_spanning/tsp_cpp.cpp
--rw-r--r--   0 vsts      (1001) docker     (117)     1854 2019-11-06 15:37:07.000000 tsp_spanning-0.1/tsp_spanning/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (117)     1682 2019-11-06 15:37:07.000000 tsp_spanning-0.1/setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)       85 2019-11-06 15:37:07.000000 tsp_spanning-0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (117)     1826 2019-11-06 15:42:40.000000 tsp_spanning-0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)       38 2019-11-06 15:42:40.000000 tsp_spanning-0.1/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (117)     1826 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)       13 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (117)       13 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      312 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-11-06 15:42:40.000000 tsp_spanning-0.1/tsp_spanning.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:26:17.378145 tsp_spanning-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 21:26:06.000000 tsp_spanning-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:26:06.000000 tsp_spanning-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 21:26:17.378145 tsp_spanning-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 21:26:06.000000 tsp_spanning-0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 21:26:06.000000 tsp_spanning-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:26:17.378145 tsp_spanning-0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-07-12 21:26:06.000000 tsp_spanning-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:26:17.378145 tsp_spanning-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-12 21:26:06.000000 tsp_spanning-0.2/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:26:17.378145 tsp_spanning-0.2/tsp_spanning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-12 21:26:06.000000 tsp_spanning-0.2/tsp_spanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-12 21:26:06.000000 tsp_spanning-0.2/tsp_spanning/tsp_cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 21:26:06.000000 tsp_spanning-0.2/tsp_spanning/tsp_cpp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 21:26:06.000000 tsp_spanning-0.2/tsp_spanning/tsp_wrap.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:26:17.378145 tsp_spanning-0.2/tsp_spanning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 21:26:17.000000 tsp_spanning-0.2/tsp_spanning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 21:26:17.000000 tsp_spanning-0.2/tsp_spanning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:26:17.000000 tsp_spanning-0.2/tsp_spanning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 21:26:17.000000 tsp_spanning-0.2/tsp_spanning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 21:26:17.000000 tsp_spanning-0.2/tsp_spanning.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tsp_spanning-0.1/README.rst` & `tsp_spanning-0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
   :target: https://tsp-spanning.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 
 .. image:: https://dev.azure.com/bokota/tsp%20spanning/_apis/build/status/Czaki.tsp_spanning?branchName=master
   :target: https://dev.azure.com/bokota/tsp%20spanning/_build/latest?definitionId=1&branchName=master
   :alt: Build Status  
 
-.. image:: https://badge.fury.io/py/tsp_spanning.svg
-  :target: https://badge.fury.io/py/tsp_spanning
+.. image:: https://badge.fury.io/py/tsp-spanning.svg
+  :target: https://badge.fury.io/py/tsp-spanning
   :alt: PyPI version
 
 tsp_spanning is package which implements Traveling
 Salesman Problem with spanning tree heuristic.
 
 For performance reason algorithm is inplemented in C
 
 instalation
 -----------
 
 .. code:: bash 
    
-   pip install tsp_spanning
+   pip install tsp-spanning
 
 
 @copyright
 Code created by Grzegorz Bokota, Iwona Kotlarska, Jakub Bartmiński
```

### Comparing `tsp_spanning-0.1/tsp_spanning/tsp_wrap.pyx` & `tsp_spanning-0.2/tsp_spanning/tsp_wrap.pyx`

 * *Files identical despite different names*

### Comparing `tsp_spanning-0.1/tsp_spanning/tsp_cpp.cpp` & `tsp_spanning-0.2/tsp_spanning/tsp_cpp.cpp`

 * *Files identical despite different names*

### Comparing `tsp_spanning-0.1/tsp_spanning/__init__.py` & `tsp_spanning-0.2/tsp_spanning/__init__.py`

 * *Files identical despite different names*

### Comparing `tsp_spanning-0.1/setup.py` & `tsp_spanning-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def readme():
     this_directory = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(this_directory, 'README.rst')) as f:
         return f.read()
 
 
 setuptools.setup(
-  version="0.1",
+  version="0.2",
   name = 'tsp_spanning',
   author="Grzegorz Bokota",
   author_email="g.bokota@cent.uw.edu.pl",
   packages=setuptools.find_packages(),
   install_requires=['numpy', 'cython'],
   ext_modules = extensions,
   long_description=readme(),
```

### Comparing `tsp_spanning-0.1/PKG-INFO` & `tsp_spanning-0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: tsp_spanning
-Version: 0.1
-Summary: UNKNOWN
+Version: 0.2
 Home-page: https://github.com/Czaki/tsp_spanning
 Author: Grzegorz Bokota
 Author-email: g.bokota@cent.uw.edu.pl
-License: UNKNOWN
-Description: tsp_spanning
-        ============
-        .. image:: https://readthedocs.org/projects/tsp-spanning/badge/?version=latest
-          :target: https://tsp-spanning.readthedocs.io/en/latest/?badge=latest
-          :alt: Documentation Status
-        
-        .. image:: https://dev.azure.com/bokota/tsp%20spanning/_apis/build/status/Czaki.tsp_spanning?branchName=master
-          :target: https://dev.azure.com/bokota/tsp%20spanning/_build/latest?definitionId=1&branchName=master
-          :alt: Build Status  
-        
-        .. image:: https://badge.fury.io/py/tsp_spanning.svg
-          :target: https://badge.fury.io/py/tsp_spanning
-          :alt: PyPI version
-        
-        tsp_spanning is package which implements Traveling
-        Salesman Problem with spanning tree heuristic.
-        
-        For performance reason algorithm is inplemented in C
-        
-        instalation
-        -----------
-        
-        .. code:: bash 
-           
-           pip install tsp_spanning
-        
-        
-        @copyright
-        Code created by Grzegorz Bokota, Iwona Kotlarska, Jakub Bartmiński
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+tsp_spanning
+============
+.. image:: https://readthedocs.org/projects/tsp-spanning/badge/?version=latest
+  :target: https://tsp-spanning.readthedocs.io/en/latest/?badge=latest
+  :alt: Documentation Status
+
+.. image:: https://dev.azure.com/bokota/tsp%20spanning/_apis/build/status/Czaki.tsp_spanning?branchName=master
+  :target: https://dev.azure.com/bokota/tsp%20spanning/_build/latest?definitionId=1&branchName=master
+  :alt: Build Status  
+
+.. image:: https://badge.fury.io/py/tsp-spanning.svg
+  :target: https://badge.fury.io/py/tsp-spanning
+  :alt: PyPI version
+
+tsp_spanning is package which implements Traveling
+Salesman Problem with spanning tree heuristic.
+
+For performance reason algorithm is inplemented in C
+
+instalation
+-----------
+
+.. code:: bash 
+   
+   pip install tsp-spanning
+
+
+@copyright
+Code created by Grzegorz Bokota, Iwona Kotlarska, Jakub Bartmiński
```

### Comparing `tsp_spanning-0.1/tsp_spanning.egg-info/PKG-INFO` & `tsp_spanning-0.2/tsp_spanning.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: tsp-spanning
-Version: 0.1
-Summary: UNKNOWN
+Version: 0.2
 Home-page: https://github.com/Czaki/tsp_spanning
 Author: Grzegorz Bokota
 Author-email: g.bokota@cent.uw.edu.pl
-License: UNKNOWN
-Description: tsp_spanning
-        ============
-        .. image:: https://readthedocs.org/projects/tsp-spanning/badge/?version=latest
-          :target: https://tsp-spanning.readthedocs.io/en/latest/?badge=latest
-          :alt: Documentation Status
-        
-        .. image:: https://dev.azure.com/bokota/tsp%20spanning/_apis/build/status/Czaki.tsp_spanning?branchName=master
-          :target: https://dev.azure.com/bokota/tsp%20spanning/_build/latest?definitionId=1&branchName=master
-          :alt: Build Status  
-        
-        .. image:: https://badge.fury.io/py/tsp_spanning.svg
-          :target: https://badge.fury.io/py/tsp_spanning
-          :alt: PyPI version
-        
-        tsp_spanning is package which implements Traveling
-        Salesman Problem with spanning tree heuristic.
-        
-        For performance reason algorithm is inplemented in C
-        
-        instalation
-        -----------
-        
-        .. code:: bash 
-           
-           pip install tsp_spanning
-        
-        
-        @copyright
-        Code created by Grzegorz Bokota, Iwona Kotlarska, Jakub Bartmiński
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+tsp_spanning
+============
+.. image:: https://readthedocs.org/projects/tsp-spanning/badge/?version=latest
+  :target: https://tsp-spanning.readthedocs.io/en/latest/?badge=latest
+  :alt: Documentation Status
+
+.. image:: https://dev.azure.com/bokota/tsp%20spanning/_apis/build/status/Czaki.tsp_spanning?branchName=master
+  :target: https://dev.azure.com/bokota/tsp%20spanning/_build/latest?definitionId=1&branchName=master
+  :alt: Build Status  
+
+.. image:: https://badge.fury.io/py/tsp-spanning.svg
+  :target: https://badge.fury.io/py/tsp-spanning
+  :alt: PyPI version
+
+tsp_spanning is package which implements Traveling
+Salesman Problem with spanning tree heuristic.
+
+For performance reason algorithm is inplemented in C
+
+instalation
+-----------
+
+.. code:: bash 
+   
+   pip install tsp-spanning
+
+
+@copyright
+Code created by Grzegorz Bokota, Iwona Kotlarska, Jakub Bartmiński
```

