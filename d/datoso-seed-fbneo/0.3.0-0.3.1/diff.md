# Comparing `tmp/datoso_seed_fbneo-0.3.0.tar.gz` & `tmp/datoso_seed_fbneo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_fbneo-0.3.0.tar", last modified: Sat Jun 10 20:43:03 2023, max compression
+gzip compressed data, was "datoso_seed_fbneo-0.3.1.tar", last modified: Thu Jul 13 14:08:28 2023, max compression
```

## Comparing `datoso_seed_fbneo-0.3.0.tar` & `datoso_seed_fbneo-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:28.540078 datoso_seed_fbneo-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-13 14:08:28.540078 datoso_seed_fbneo-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 14:08:28.540078 datoso_seed_fbneo-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:28.536078 datoso_seed_fbneo-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:28.536078 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-13 14:08:15.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:28.536078 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-13 14:08:28.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-13 14:08:28.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:08:28.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 14:08:28.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 14:08:28.000000 datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/top_level.txt
```

### Comparing `datoso_seed_fbneo-0.3.0/LICENSE` & `datoso_seed_fbneo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.3.0/PKG-INFO` & `datoso_seed_fbneo-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso_seed_fbneo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_fbneo
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso_seed_fbneo-0.3.0/README.md` & `datoso_seed_fbneo-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.3.0/pyproject.toml` & `datoso_seed_fbneo-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.3.1",
+    "datoso>=0.3.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_fbneo"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/actions.py` & `datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/actions.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/dats.py` & `datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/fetch.py` & `datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from datetime import datetime
 from pathlib import Path
 import urllib.request
 import zipfile
 from datoso_seed_fbneo import __preffix__
 
 from datoso.configuration import config, logger
+from datoso.helpers import show_progress
 from datoso.configuration.folder_helper import Folders
 
 url = 'https://github.com/libretro/FBNeo/archive/refs/heads/master.zip'
 
 def download(folders):
     logger.info(f'Downloading {url} to {folders.download}\n')
-    urllib.request.urlretrieve(url, os.path.join(folders.download, 'fbneo.zip'))
+    urllib.request.urlretrieve(url, os.path.join(folders.download, 'fbneo.zip'), reporthook=show_progress)
     logger.info(f'Extracting dats from {folders.download}\n')
 
 def extract_dats(folders, full=False, light=False):
     with zipfile.ZipFile(os.path.join(folders.download, 'fbneo.zip'), 'r') as zip_ref:
         filelist = [f for f in zip_ref.filelist if f.filename.startswith('FBNeo-master/dats/') and f.filename.endswith('.dat')]
         filelist_full = [f for f in filelist if '/light/' not in f.filename]
         filelist_light = [f for f in filelist if '/light/' in f.filename]
```

### Comparing `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/rules.py` & `datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/PKG-INFO` & `datoso_seed_fbneo-0.3.1/src/datoso_seed_fbneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso-seed-fbneo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_fbneo
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

