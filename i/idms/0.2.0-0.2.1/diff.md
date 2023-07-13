# Comparing `tmp/idms-0.2.0.tar.gz` & `tmp/idms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idms-0.2.0.tar", last modified: Thu Jul  6 21:58:20 2023, max compression
+gzip compressed data, was "idms-0.2.1.tar", last modified: Thu Jul 13 09:31:42 2023, max compression
```

## Comparing `idms-0.2.0.tar` & `idms-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-06 21:58:09.000000 idms-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 21:58:09.000000 idms-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 21:58:20.329176 idms-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 21:58:09.000000 idms-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.325176 idms-0.2.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 21:58:09.000000 idms-0.2.0/data/data_file
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 21:58:09.000000 idms-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 21:58:20.329176 idms-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-06 21:58:09.000000 idms-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.325176 idms-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.325176 idms-0.2.0/src/idms/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/src/idms/api/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/api/contentserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/src/idms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/src/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 21:58:09.000000 idms-0.2.0/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 21:58:09.000000 idms-0.2.0/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 21:58:09.000000 idms-0.2.0/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-13 09:31:31.000000 idms-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 09:31:31.000000 idms-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 09:31:42.876928 idms-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-13 09:31:31.000000 idms-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 09:31:31.000000 idms-0.2.1/data/data_file
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 09:31:31.000000 idms-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 09:31:42.880928 idms-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 09:31:31.000000 idms-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/idms/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/idms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/api/contentserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/idms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 09:31:31.000000 idms-0.2.1/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 09:31:31.000000 idms-0.2.1/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 09:31:31.000000 idms-0.2.1/src/sample/simple.py
```

### Comparing `idms-0.2.0/LICENSE.txt` & `idms-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idms-0.2.0/PKG-INFO` & `idms-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/Provincie-Zuid-Holland/idms
 Author: Daniel Overdevest
 Author-email: d.overdevest@pzh.nl
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
 Keywords: idms,contentserver,restapi,searchapi
```

### Comparing `idms-0.2.0/README.md` & `idms-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `idms-0.2.0/setup.py` & `idms-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="idms",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.0",  # Required
+    version="0.2.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Python class to talk to idms REST and Search API, better known as iDMS.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `idms-0.2.0/src/idms/api/contentserver.py` & `idms-0.2.1/src/idms/api/contentserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,24 @@
 
 def dotfield(input_dict: dict, input_key: str, notFound=None) -> str:
     """
     Magic function to get nested properties from dictionary writen as level1.level2.level3.
 
     Example:
     dotfield({"a": {"b": {"c": "def"}}}, "a.b.c") -> "def"
+
+    TODO: Add support for list (error: AttributeError: 'list' object has no attribute 'get')
     """
-    return reduce(
-        lambda d, k: d.get(k) if d else notFound, input_key.split("."), input_dict
-    )
+    try:
+        return reduce(
+            lambda d, k: d.get(k) if d else notFound, input_key.split("."), input_dict
+        )
+    except Exception as err:
+        logging.debug(f"Dotfield error: {err}\n{input_key}")
+        return ""
 
 
 class crawler:
     def __init__(
         self,
         baseUrl: str,
         username: str = None,
```

### Comparing `idms-0.2.0/src/idms/functions.py` & `idms-0.2.1/src/idms/functions.py`

 * *Files identical despite different names*

### Comparing `idms-0.2.0/src/idms.egg-info/PKG-INFO` & `idms-0.2.1/src/idms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/Provincie-Zuid-Holland/idms
 Author: Daniel Overdevest
 Author-email: d.overdevest@pzh.nl
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
 Keywords: idms,contentserver,restapi,searchapi
```

