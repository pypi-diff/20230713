# Comparing `tmp/cjio-0.8.1.tar.gz` & `tmp/cjio-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjio-0.8.1.tar", last modified: Mon Feb  6 17:51:14 2023, max compression
+gzip compressed data, was "cjio-0.8.2.tar", last modified: Thu Jul 13 13:27:04 2023, max compression
```

## Comparing `cjio-0.8.1.tar` & `cjio-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:51:14.181148 cjio-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-06 17:51:03.000000 cjio-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-02-06 17:51:14.181148 cjio-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-02-06 17:51:03.000000 cjio-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:51:14.181148 cjio-0.8.1/cjio/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97811 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/cityjson.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28516 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/cjio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24498 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7744 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/geom_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    27524 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5701 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-02-06 17:51:03.000000 cjio-0.8.1/cjio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:51:14.181148 cjio-0.8.1/cjio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-02-06 17:51:14.000000 cjio-0.8.1/cjio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-06 17:51:14.000000 cjio-0.8.1/cjio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 17:51:14.000000 cjio-0.8.1/cjio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-06 17:51:14.000000 cjio-0.8.1/cjio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-06 17:51:14.000000 cjio-0.8.1/cjio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-06 17:51:14.000000 cjio-0.8.1/cjio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-06 17:51:14.181148 cjio-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-02-06 17:51:03.000000 cjio-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:27:04.365967 cjio-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-13 13:26:49.000000 cjio-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-13 13:27:04.365967 cjio-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-13 13:26:49.000000 cjio-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:27:04.361967 cjio-0.8.2/cjio/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97811 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/cityjson.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28518 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/cjio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24498 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7744 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/geom_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27524 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5701 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 13:26:49.000000 cjio-0.8.2/cjio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:27:04.365967 cjio-0.8.2/cjio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-13 13:27:04.000000 cjio-0.8.2/cjio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 13:27:04.000000 cjio-0.8.2/cjio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:27:04.000000 cjio-0.8.2/cjio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 13:27:04.000000 cjio-0.8.2/cjio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 13:27:04.000000 cjio-0.8.2/cjio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 13:27:04.000000 cjio-0.8.2/cjio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 13:27:04.365967 cjio-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 13:26:49.000000 cjio-0.8.2/setup.py
```

### Comparing `cjio-0.8.1/LICENSE` & `cjio-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/PKG-INFO` & `cjio-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjio
-Version: 0.8.1
+Version: 0.8.2
 Summary: CLI to process and manipulate CityJSON files
 Home-page: https://github.com/cityjson/cjio
 Author: Hugo Ledoux, Balázs Dukai
 Author-email: h.ledoux@tudelft.nl, balazs.dukai@3dgi.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cjio-0.8.1/README.rst` & `cjio-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/cityjson.py` & `cjio-0.8.2/cjio/cityjson.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/cjio.py` & `cjio-0.8.2/cjio/cjio.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,18 +95,18 @@
 
 
 @cli.command('info')
 @click.option('--long', is_flag=True, help='More gory details about the file.')
 def info_cmd(long):
     """Output information about the dataset."""
     def processor(cm):
-        print_cmd_status('Information ⬇️')
+        print_cmd_status('=== Information ===')
         s = linesep.join(cm.get_info(long=long))
         print_cmd_info(s)
-        print_cmd_status('Information ⬆️')
+        print_cmd_status('=== Information ===')
         return cm
     return processor
 
 
 @cli.command('export')
 @click.argument('format',
               type=click.Choice(['obj', 'jsonl', 'stl', 'glb', 'b3dm']),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cjio-0.8.1/cjio/convert.py` & `cjio-0.8.2/cjio/convert.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/errors.py` & `cjio-0.8.2/cjio/errors.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/geom_help.py` & `cjio-0.8.2/cjio/geom_help.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/metadata.py` & `cjio-0.8.2/cjio/metadata.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/models.py` & `cjio-0.8.2/cjio/models.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/subset.py` & `cjio-0.8.2/cjio/subset.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio/utils.py` & `cjio-0.8.2/cjio/utils.py`

 * *Files identical despite different names*

### Comparing `cjio-0.8.1/cjio.egg-info/PKG-INFO` & `cjio-0.8.2/cjio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjio
-Version: 0.8.1
+Version: 0.8.2
 Summary: CLI to process and manipulate CityJSON files
 Home-page: https://github.com/cityjson/cjio
 Author: Hugo Ledoux, Balázs Dukai
 Author-email: h.ledoux@tudelft.nl, balazs.dukai@3dgi.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cjio-0.8.1/setup.cfg` & `cjio-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.1
+current_version = 0.8.2
 commit = True
 tag = True
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
```

### Comparing `cjio-0.8.1/setup.py` & `cjio-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 CURRENT_DIR = Path(__file__).parent
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cjio',
-    version='0.8.1',
+    version='0.8.2',
     description='CLI to process and manipulate CityJSON files',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://github.com/cityjson/cjio',
     author='Hugo Ledoux, Balázs Dukai',
     author_email='h.ledoux@tudelft.nl, balazs.dukai@3dgi.nl',
     python_requires='>=3.6',
```

