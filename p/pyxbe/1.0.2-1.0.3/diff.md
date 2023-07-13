# Comparing `tmp/pyxbe-1.0.2.tar.gz` & `tmp/pyxbe-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxbe-1.0.2.tar", last modified: Fri Jul  7 08:05:34 2023, max compression
+gzip compressed data, was "pyxbe-1.0.3.tar", last modified: Thu Jul 13 20:52:54 2023, max compression
```

## Comparing `pyxbe-1.0.2.tar` & `pyxbe-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 08:04:24.000000 pyxbe-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 08:04:24.000000 pyxbe-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 08:05:34.868189 pyxbe-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-07 08:04:24.000000 pyxbe-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 08:04:24.000000 pyxbe-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/pyxbe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 08:05:34.000000 pyxbe-1.0.2/pyxbe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-07 08:05:34.868189 pyxbe-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 08:04:24.000000 pyxbe-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:24.000000 pyxbe-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 08:04:24.000000 pyxbe-1.0.2/tests/test_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:34.868189 pyxbe-1.0.2/xbe/
--rw-r--r--   0 runner    (1001) docker     (123)    50913 2023-07-07 08:04:24.000000 pyxbe-1.0.2/xbe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-07 08:04:24.000000 pyxbe-1.0.2/xbe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:24.000000 pyxbe-1.0.2/xbe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:52:54.319328 pyxbe-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-13 20:52:13.000000 pyxbe-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 20:52:13.000000 pyxbe-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-13 20:52:54.319328 pyxbe-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 20:52:13.000000 pyxbe-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 20:52:13.000000 pyxbe-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:52:54.319328 pyxbe-1.0.3/pyxbe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-13 20:52:53.000000 pyxbe-1.0.3/pyxbe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 20:52:54.000000 pyxbe-1.0.3/pyxbe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:52:53.000000 pyxbe-1.0.3/pyxbe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 20:52:53.000000 pyxbe-1.0.3/pyxbe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 20:52:53.000000 pyxbe-1.0.3/pyxbe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 20:52:54.319328 pyxbe-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 20:52:13.000000 pyxbe-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:52:54.319328 pyxbe-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 20:52:13.000000 pyxbe-1.0.3/tests/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:52:54.319328 pyxbe-1.0.3/xbe/
+-rw-r--r--   0 runner    (1001) docker     (123)    50913 2023-07-13 20:52:13.000000 pyxbe-1.0.3/xbe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-13 20:52:13.000000 pyxbe-1.0.3/xbe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:52:13.000000 pyxbe-1.0.3/xbe/py.typed
```

### Comparing `pyxbe-1.0.2/LICENSE.txt` & `pyxbe-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxbe-1.0.2/PKG-INFO` & `pyxbe-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxbe
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to work with XBE files
 Home-page: https://github.com/mborgerson/pyxbe
 Author: Matt Borgerson
 Author-email: contact@mborgerson.com
 License: MIT
 Description: pyxbe
         =====
```

### Comparing `pyxbe-1.0.2/pyxbe.egg-info/PKG-INFO` & `pyxbe-1.0.3/pyxbe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxbe
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to work with XBE files
 Home-page: https://github.com/mborgerson/pyxbe
 Author: Matt Borgerson
 Author-email: contact@mborgerson.com
 License: MIT
 Description: pyxbe
         =====
```

### Comparing `pyxbe-1.0.2/setup.cfg` & `pyxbe-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license_file = LICENSE.txt
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find:
+packages = xbe
 python_requires = >=3.8
 include_package_data = True
 
 [options.extras_require]
 docs = 
 	furo
 	ipython
```

### Comparing `pyxbe-1.0.2/xbe/__init__.py` & `pyxbe-1.0.3/xbe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 )
 
 if TYPE_CHECKING:
     RGBA = Tuple[float, float, float, float]
 
 log = logging.getLogger(__name__)
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 
 class XbeKernelImage:
     """
     xboxkrnl.exe model
     """
```

### Comparing `pyxbe-1.0.2/xbe/__main__.py` & `pyxbe-1.0.3/xbe/__main__.py`

 * *Files identical despite different names*

