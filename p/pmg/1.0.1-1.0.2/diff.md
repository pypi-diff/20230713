# Comparing `tmp/pmg-1.0.1.tar.gz` & `tmp/pmg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmg-1.0.1.tar", last modified: Wed Jul 12 17:35:27 2023, max compression
+gzip compressed data, was "pmg-1.0.2.tar", last modified: Thu Jul 13 01:40:59 2023, max compression
```

## Comparing `pmg-1.0.1.tar` & `pmg-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.964714 pmg-1.0.1/
--rw-rw-r--   0 gm        (1000) gm        (1000)     1086 2022-07-25 11:43:49.000000 pmg-1.0.1/LICENSE
--rw-r--r--   0 gm        (1000) gm        (1000)     1235 2023-07-12 17:35:27.964714 pmg-1.0.1/PKG-INFO
--rw-rw-r--   0 gm        (1000) gm        (1000)      676 2022-07-25 16:00:44.000000 pmg-1.0.1/README.md
-drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.963714 pmg-1.0.1/pmg/
--rw-r--r--   0 gm        (1000) gm        (1000)    13150 2023-07-12 17:34:09.000000 pmg-1.0.1/pmg/__init__.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      693 2021-05-02 12:21:23.000000 pmg-1.0.1/pmg/base36.py
--rw-r--r--   0 gm        (1000) gm        (1000)     1525 2023-01-13 07:41:58.000000 pmg-1.0.1/pmg/db.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      362 2022-07-25 17:39:34.000000 pmg-1.0.1/pmg/latex.py
-drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.963714 pmg-1.0.1/pmg/sqlite/
--rw-r--r--   0 gm        (1000) gm        (1000)     1461 2023-01-13 07:41:58.000000 pmg-1.0.1/pmg/sqlite/__init__.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      422 2022-07-25 15:16:43.000000 pmg-1.0.1/pmg/sqlite/factories.py
--rw-r--r--   0 gm        (1000) gm        (1000)     3136 2023-01-13 07:41:58.000000 pmg-1.0.1/pmg/sqlite/queues.py
--rw-r--r--   0 gm        (1000) gm        (1000)     1752 2023-02-12 22:02:56.000000 pmg-1.0.1/pmg/system.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      635 2022-07-25 17:41:28.000000 pmg-1.0.1/pmg/temp.py
-drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.963714 pmg-1.0.1/pmg.egg-info/
--rw-rw-r--   0 gm        (1000) gm        (1000)     1235 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/PKG-INFO
--rw-rw-r--   0 gm        (1000) gm        (1000)      420 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/SOURCES.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)        1 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/dependency_links.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)       26 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/requires.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)        4 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/top_level.txt
--rw-r--r--   0 gm        (1000) gm        (1000)      745 2023-07-12 14:11:15.000000 pmg-1.0.1/pyproject.toml
--rw-r--r--   0 gm        (1000) gm        (1000)       38 2023-07-12 17:35:27.964714 pmg-1.0.1/setup.cfg
--rw-rw-r--   0 gm        (1000) gm        (1000)       38 2022-07-25 15:40:08.000000 pmg-1.0.1/setup.py
-drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.964714 pmg-1.0.1/tests/
--rw-rw-r--   0 gm        (1000) gm        (1000)      372 2022-07-25 17:27:37.000000 pmg-1.0.1/tests/test_base36.py
--rw-r--r--   0 gm        (1000) gm        (1000)     4604 2023-01-13 07:41:58.000000 pmg-1.0.1/tests/test_common.py
--rw-r--r--   0 gm        (1000) gm        (1000)     1683 2023-01-13 07:41:58.000000 pmg-1.0.1/tests/test_db.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      241 2022-07-25 17:56:49.000000 pmg-1.0.1/tests/test_latex.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      358 2022-07-25 17:58:50.000000 pmg-1.0.1/tests/test_temp.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-13 01:40:59.944789 pmg-1.0.2/
+-rw-rw-r--   0 gm        (1000) gm        (1000)     1086 2022-07-25 11:43:49.000000 pmg-1.0.2/LICENSE
+-rw-r--r--   0 gm        (1000) gm        (1000)     1235 2023-07-13 01:40:59.944789 pmg-1.0.2/PKG-INFO
+-rw-rw-r--   0 gm        (1000) gm        (1000)      676 2022-07-25 16:00:44.000000 pmg-1.0.2/README.md
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-13 01:40:59.943789 pmg-1.0.2/pmg/
+-rw-r--r--   0 gm        (1000) gm        (1000)    13148 2023-07-13 01:04:23.000000 pmg-1.0.2/pmg/__init__.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      693 2021-05-02 12:21:23.000000 pmg-1.0.2/pmg/base36.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     1525 2023-01-13 07:41:58.000000 pmg-1.0.2/pmg/db.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      362 2022-07-25 17:39:34.000000 pmg-1.0.2/pmg/latex.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-13 01:40:59.944789 pmg-1.0.2/pmg/sqlite/
+-rw-r--r--   0 gm        (1000) gm        (1000)     1461 2023-01-13 07:41:58.000000 pmg-1.0.2/pmg/sqlite/__init__.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      422 2022-07-25 15:16:43.000000 pmg-1.0.2/pmg/sqlite/factories.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     3136 2023-01-13 07:41:58.000000 pmg-1.0.2/pmg/sqlite/queues.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     1752 2023-02-12 22:02:56.000000 pmg-1.0.2/pmg/system.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      635 2022-07-25 17:41:28.000000 pmg-1.0.2/pmg/temp.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-13 01:40:59.944789 pmg-1.0.2/pmg.egg-info/
+-rw-rw-r--   0 gm        (1000) gm        (1000)     1235 2023-07-13 01:40:59.000000 pmg-1.0.2/pmg.egg-info/PKG-INFO
+-rw-rw-r--   0 gm        (1000) gm        (1000)      420 2023-07-13 01:40:59.000000 pmg-1.0.2/pmg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gm        (1000) gm        (1000)        1 2023-07-13 01:40:59.000000 pmg-1.0.2/pmg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gm        (1000) gm        (1000)       26 2023-07-13 01:40:59.000000 pmg-1.0.2/pmg.egg-info/requires.txt
+-rw-rw-r--   0 gm        (1000) gm        (1000)        4 2023-07-13 01:40:59.000000 pmg-1.0.2/pmg.egg-info/top_level.txt
+-rw-r--r--   0 gm        (1000) gm        (1000)      745 2023-07-13 01:05:10.000000 pmg-1.0.2/pyproject.toml
+-rw-r--r--   0 gm        (1000) gm        (1000)       38 2023-07-13 01:40:59.944789 pmg-1.0.2/setup.cfg
+-rw-rw-r--   0 gm        (1000) gm        (1000)       38 2022-07-25 15:40:08.000000 pmg-1.0.2/setup.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-13 01:40:59.944789 pmg-1.0.2/tests/
+-rw-rw-r--   0 gm        (1000) gm        (1000)      372 2022-07-25 17:27:37.000000 pmg-1.0.2/tests/test_base36.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     4604 2023-01-13 07:41:58.000000 pmg-1.0.2/tests/test_common.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     1683 2023-01-13 07:41:58.000000 pmg-1.0.2/tests/test_db.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      241 2022-07-25 17:56:49.000000 pmg-1.0.2/tests/test_latex.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      358 2022-07-25 17:58:50.000000 pmg-1.0.2/tests/test_temp.py
```

### Comparing `pmg-1.0.1/LICENSE` & `pmg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/PKG-INFO` & `pmg-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmg
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolbox full of handy little helper functions and utilities.
 Author-email: Preston Meyer Group <dev@pmgroup.ch>
 License: MIT
 Keywords: tools,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pmg-1.0.1/README.md` & `pmg-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg/__init__.py` & `pmg-1.0.2/pmg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     return '\n'.join(traceback.format_exception(*sys.exc_info()))
 
 
 # CSV Helpers
 def csv_to_namedtuples(path, **kwargs):
     Record = None
     if 'delimiter' not in kwargs:
-        kwargs.update({'delimiter': DEFAULT_FIELD_DELIMITER})
+        kwargs.update({'delimiter': DEFAULT_CSV_DELIMITER})
     with open(path, 'rt') as f:
         reader = csv.reader(f, **kwargs)
         for i, r in enumerate(reader):
             if i == 0:
                 Record = collections.namedtuple('Record', r)
                 continue
             yield Record(*r)
```

### Comparing `pmg-1.0.1/pmg/base36.py` & `pmg-1.0.2/pmg/base36.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg/db.py` & `pmg-1.0.2/pmg/db.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg/sqlite/__init__.py` & `pmg-1.0.2/pmg/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg/sqlite/queues.py` & `pmg-1.0.2/pmg/sqlite/queues.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg/system.py` & `pmg-1.0.2/pmg/system.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg/temp.py` & `pmg-1.0.2/pmg/temp.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/pmg.egg-info/PKG-INFO` & `pmg-1.0.2/pmg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmg
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolbox full of handy little helper functions and utilities.
 Author-email: Preston Meyer Group <dev@pmgroup.ch>
 License: MIT
 Keywords: tools,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pmg-1.0.1/pyproject.toml` & `pmg-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmg"
-version = "1.0.1"
+version = "1.0.2"
 description = "A toolbox full of handy little helper functions and utilities."
 readme = "README.md"
 authors = [{ name = "Preston Meyer Group", email = "dev@pmgroup.ch" }]
 license = { text = "MIT" }
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
```

### Comparing `pmg-1.0.1/tests/test_common.py` & `pmg-1.0.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.1/tests/test_db.py` & `pmg-1.0.2/tests/test_db.py`

 * *Files identical despite different names*

