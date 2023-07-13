# Comparing `tmp/remarshal-0.9.1.tar.gz` & `tmp/remarshal-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/remarshal-0.9.1.tar", last modified: Thu Apr  4 19:18:37 2019, max compression
+gzip compressed data, was "dist/remarshal-0.9.2.tar", last modified: Thu Apr  4 20:27:49 2019, max compression
```

## Comparing `remarshal-0.9.1.tar` & `remarshal-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 19:18:37.000000 remarshal-0.9.1/
-drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 19:18:37.000000 remarshal-0.9.1/remarshal.egg-info/
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      236 2019-04-04 19:18:36.000000 remarshal-0.9.1/remarshal.egg-info/PKG-INFO
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      608 2019-04-04 19:18:36.000000 remarshal-0.9.1/remarshal.egg-info/SOURCES.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)        1 2019-04-04 19:18:36.000000 remarshal-0.9.1/remarshal.egg-info/dependency_links.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      289 2019-04-04 19:18:36.000000 remarshal-0.9.1/remarshal.egg-info/entry_points.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       51 2019-04-04 19:18:36.000000 remarshal-0.9.1/remarshal.egg-info/requires.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       10 2019-04-04 19:18:36.000000 remarshal-0.9.1/remarshal.egg-info/top_level.txt
-drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 19:18:37.000000 remarshal-0.9.1/tests/
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)        0 2016-09-02 12:13:21.000000 remarshal-0.9.1/tests/__init__.py
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       26 2016-09-02 12:13:21.000000 remarshal-0.9.1/tests/array.json
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       41 2017-07-07 16:52:23.000000 remarshal-0.9.1/tests/array.toml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       81 2016-09-02 12:13:21.000000 remarshal-0.9.1/tests/context.py
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       34 2016-09-03 12:23:17.000000 remarshal-0.9.1/tests/garbage
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      157 2016-09-02 18:25:18.000000 remarshal-0.9.1/tests/long-line-default.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      170 2016-09-02 18:35:31.000000 remarshal-0.9.1/tests/long-line-double-quote.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      177 2016-09-02 18:36:30.000000 remarshal-0.9.1/tests/long-line-gt.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      173 2016-09-02 18:36:37.000000 remarshal-0.9.1/tests/long-line-pipe.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      167 2016-09-02 18:35:22.000000 remarshal-0.9.1/tests/long-line-single-quote.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      180 2016-09-02 18:23:56.000000 remarshal-0.9.1/tests/long-line.json
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       39 2018-11-02 13:38:02.000000 remarshal-0.9.1/tests/order.json
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       24 2018-11-02 13:38:02.000000 remarshal-0.9.1/tests/order.toml
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       21 2018-11-02 13:38:02.000000 remarshal-0.9.1/tests/order.yaml
--rwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)     9602 2019-04-04 19:17:25.000000 remarshal-0.9.1/tests/test_remarshal.py
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       76 2019-04-04 19:09:17.000000 remarshal-0.9.1/MANIFEST.in
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)     5247 2018-11-02 13:38:02.000000 remarshal-0.9.1/README.md
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      889 2016-09-02 12:13:21.000000 remarshal-0.9.1/example.json
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      875 2018-08-04 15:49:38.000000 remarshal-0.9.1/example.toml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      563 2016-09-02 12:13:21.000000 remarshal-0.9.1/example.yaml
--rwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)     9751 2019-04-04 19:17:25.000000 remarshal-0.9.1/remarshal.py
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)     1263 2019-04-04 19:08:44.000000 remarshal-0.9.1/setup.py
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)      236 2019-04-04 19:18:37.000000 remarshal-0.9.1/PKG-INFO
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       38 2019-04-04 19:18:37.000000 remarshal-0.9.1/setup.cfg
+drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 20:27:49.000000 remarshal-0.9.2/
+drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      236 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/PKG-INFO
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      608 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/SOURCES.txt
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)        1 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/dependency_links.txt
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      289 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/entry_points.txt
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       50 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/requires.txt
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       10 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/top_level.txt
+drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 20:27:49.000000 remarshal-0.9.2/tests/
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)        0 2016-09-02 12:13:21.000000 remarshal-0.9.2/tests/__init__.py
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       26 2016-09-02 12:13:21.000000 remarshal-0.9.2/tests/array.json
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       41 2019-04-04 20:12:19.000000 remarshal-0.9.2/tests/array.toml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       81 2016-09-02 12:13:21.000000 remarshal-0.9.2/tests/context.py
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       34 2016-09-03 12:23:17.000000 remarshal-0.9.2/tests/garbage
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      157 2016-09-02 18:25:18.000000 remarshal-0.9.2/tests/long-line-default.yaml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      170 2016-09-02 18:35:31.000000 remarshal-0.9.2/tests/long-line-double-quote.yaml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      177 2016-09-02 18:36:30.000000 remarshal-0.9.2/tests/long-line-gt.yaml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      173 2016-09-02 18:36:37.000000 remarshal-0.9.2/tests/long-line-pipe.yaml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      167 2016-09-02 18:35:22.000000 remarshal-0.9.2/tests/long-line-single-quote.yaml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      180 2016-09-02 18:23:56.000000 remarshal-0.9.2/tests/long-line.json
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       39 2018-11-02 13:38:02.000000 remarshal-0.9.2/tests/order.json
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       24 2018-11-02 13:38:02.000000 remarshal-0.9.2/tests/order.toml
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       21 2018-11-02 13:38:02.000000 remarshal-0.9.2/tests/order.yaml
+-rwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)     9602 2019-04-04 20:21:38.000000 remarshal-0.9.2/tests/test_remarshal.py
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       76 2019-04-04 20:21:38.000000 remarshal-0.9.2/MANIFEST.in
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)     5308 2019-04-04 20:21:38.000000 remarshal-0.9.2/README.md
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      889 2016-09-02 12:13:21.000000 remarshal-0.9.2/example.json
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)      875 2019-04-04 20:12:19.000000 remarshal-0.9.2/example.toml
+-rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      563 2016-09-02 12:13:21.000000 remarshal-0.9.2/example.yaml
+-rwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)     9751 2019-04-04 20:21:38.000000 remarshal-0.9.2/remarshal.py
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)     1262 2019-04-04 20:21:38.000000 remarshal-0.9.2/setup.py
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)      236 2019-04-04 20:27:49.000000 remarshal-0.9.2/PKG-INFO
+-rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       38 2019-04-04 20:27:49.000000 remarshal-0.9.2/setup.cfg
```

### Comparing `remarshal-0.9.1/remarshal.egg-info/SOURCES.txt` & `remarshal-0.9.2/remarshal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.1/tests/test_remarshal.py` & `remarshal-0.9.2/tests/test_remarshal.py`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.1/README.md` & `remarshal-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 Convert between TOML, YAML and JSON. When installed provides the command line
 commands `toml2yaml`, `toml2json`, `yaml2toml`, `yaml2json`. `json2toml` and
 `json2yaml` for format conversion as well as `toml2toml`, `yaml2yaml` and
 `json2json` for reformatting and error detection.
 
 # Installation
 
-You will need Python 2.7 or Python 3.3 or later.
+You will need Python 2.7 or Python 3.5 or later. Earlier versions of Python 3
+may work but are not supported.
 
 You can install the latest release from PyPI using pip.
 
 ```sh
 python3 -m pip install remarshal --user
 ```
```

### Comparing `remarshal-0.9.1/example.json` & `remarshal-0.9.2/example.json`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.1/example.toml` & `remarshal-0.9.2/example.toml`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.1/example.yaml` & `remarshal-0.9.2/example.yaml`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.1/remarshal.py` & `remarshal-0.9.2/remarshal.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import sys
 import pytoml
 import yaml
 
 from collections import OrderedDict
 
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 FORMATS = ['json', 'toml', 'yaml']
 if hasattr(json, 'JSONDecodeError'):
     JSONDecodeError = json.JSONDecodeError
 else:
     JSONDecodeError = ValueError
```

### Comparing `remarshal-0.9.1/setup.py` & `remarshal-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url='https://github.com/dbohdan/remarshal',
     license='MIT',
     py_modules=['remarshal'],
     test_suite='tests',
     install_requires=[
         'python-dateutil >= 2.5.0',
         'pytoml >= 0.1.11',
-        'PyYAML >= 3.12',
+        'PyYAML >= 5.1',
     ],
     entry_points={
         'console_scripts': [
             'remarshal = remarshal:main',
             'json2json = remarshal:main',
             'json2toml = remarshal:main',
             'json2yaml = remarshal:main',
```

