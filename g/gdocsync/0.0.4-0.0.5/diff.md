# Comparing `tmp/gdocsync-0.0.4.tar.gz` & `tmp/gdocsync-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdocsync-0.0.4.tar", last modified: Thu Jul 13 03:15:53 2023, max compression
+gzip compressed data, was "gdocsync-0.0.5.tar", last modified: Thu Jul 13 04:20:40 2023, max compression
```

## Comparing `gdocsync-0.0.4.tar` & `gdocsync-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.132387 gdocsync-0.0.4/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.4/LICENSE
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 03:15:53.132456 gdocsync-0.0.4/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.4/README.rst
--rw-r--r--   0 peterdemin   (503) staff       (20)    21045 2023-07-10 04:49:41.000000 gdocsync-0.0.4/pyproject.toml
--rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-07-13 03:15:53.132707 gdocsync-0.0.4/setup.cfg
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.129832 gdocsync-0.0.4/src/
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.131513 gdocsync-0.0.4/src/gdocsync/
--rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.4/src/gdocsync/__init__.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      333 2023-07-13 02:07:34.000000 gdocsync-0.0.4/src/gdocsync/cli.py
--rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.4/src/gdocsync/constants.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 02:41:29.000000 gdocsync-0.0.4/src/gdocsync/docs_importer.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     3124 2023-07-13 02:23:07.000000 gdocsync-0.0.4/src/gdocsync/google_drive_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      348 2023-07-13 03:10:28.000000 gdocsync-0.0.4/src/gdocsync/html_cleaner.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1366 2023-07-13 02:31:07.000000 gdocsync-0.0.4/src/gdocsync/johnny_decimal.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      760 2023-07-13 02:09:05.000000 gdocsync-0.0.4/src/gdocsync/pandoc_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.4/src/gdocsync/regexes.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.4/src/gdocsync/shelve_cache.py
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 03:15:53.132287 gdocsync-0.0.4/src/gdocsync.egg-info/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/SOURCES.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/dependency_links.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/entry_points.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/requires.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-13 03:15:53.000000 gdocsync-0.0.4/src/gdocsync.egg-info/top_level.txt
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.773572 gdocsync-0.0.5/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.5/LICENSE
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:20:40.773643 gdocsync-0.0.5/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.5/README.rst
+-rw-r--r--   0 peterdemin   (503) staff       (20)    21043 2023-07-13 03:49:48.000000 gdocsync-0.0.5/pyproject.toml
+-rw-r--r--   0 peterdemin   (503) staff       (20)      757 2023-07-13 04:20:40.773913 gdocsync-0.0.5/setup.cfg
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.769523 gdocsync-0.0.5/src/
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.772563 gdocsync-0.0.5/src/gdocsync/
+-rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.5/src/gdocsync/__init__.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      333 2023-07-13 02:07:34.000000 gdocsync-0.0.5/src/gdocsync/cli.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.5/src/gdocsync/constants.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3262 2023-07-13 02:41:29.000000 gdocsync-0.0.5/src/gdocsync/docs_importer.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     3124 2023-07-13 02:23:07.000000 gdocsync-0.0.5/src/gdocsync/google_drive_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1055 2023-07-13 04:17:52.000000 gdocsync-0.0.5/src/gdocsync/html_cleaner.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1366 2023-07-13 02:31:07.000000 gdocsync-0.0.5/src/gdocsync/johnny_decimal.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      760 2023-07-13 02:09:05.000000 gdocsync-0.0.5/src/gdocsync/pandoc_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.5/src/gdocsync/regexes.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.5/src/gdocsync/shelve_cache.py
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-13 04:20:40.773462 gdocsync-0.0.5/src/gdocsync.egg-info/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      541 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/SOURCES.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/dependency_links.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/entry_points.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       78 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/requires.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-13 04:20:40.000000 gdocsync-0.0.5/src/gdocsync.egg-info/top_level.txt
```

### Comparing `gdocsync-0.0.4/LICENSE` & `gdocsync-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/PKG-INFO` & `gdocsync-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.4/README.rst` & `gdocsync-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/pyproject.toml` & `gdocsync-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -542,9 +542,7 @@
 
 # Tells whether we should check for unused import in __init__ files.
 # init-import =
 
 # List of qualified module names which can have objects that can redefine
 # builtins.
 redefining-builtins-modules = ["six.moves", "past.builtins", "future.builtins", "builtins", "io"]
-
-
```

### Comparing `gdocsync-0.0.4/setup.cfg` & `gdocsync-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdocsync
-version = 0.0.4
+version = 0.0.5
 author = Peter Demin
 author_email = peterdemin@gmail.com
 description = 
 long_description = file:README.rst
 url = https://github.com/peterdemin/gdocsync
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `gdocsync-0.0.4/src/gdocsync/docs_importer.py` & `gdocsync-0.0.5/src/gdocsync/docs_importer.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/src/gdocsync/google_drive_client.py` & `gdocsync-0.0.5/src/gdocsync/google_drive_client.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/src/gdocsync/johnny_decimal.py` & `gdocsync-0.0.5/src/gdocsync/johnny_decimal.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/src/gdocsync/pandoc_client.py` & `gdocsync-0.0.5/src/gdocsync/pandoc_client.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/src/gdocsync/shelve_cache.py` & `gdocsync-0.0.5/src/gdocsync/shelve_cache.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.4/src/gdocsync.egg-info/PKG-INFO` & `gdocsync-0.0.5/src/gdocsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.4/src/gdocsync.egg-info/SOURCES.txt` & `gdocsync-0.0.5/src/gdocsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

