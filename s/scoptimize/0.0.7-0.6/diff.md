# Comparing `tmp/scoptimize-0.0.7.tar.gz` & `tmp/scoptimize-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoptimize-0.0.7.tar", last modified: Thu Jul 13 13:16:58 2023, max compression
+gzip compressed data, was "scoptimize-0.6.tar", last modified: Wed Jan 18 14:19:05 2023, max compression
```

## Comparing `scoptimize-0.0.7.tar` & `scoptimize-0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 13:16:58.227121 scoptimize-0.0.7/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-02-13 16:33:50.000000 scoptimize-0.0.7/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4514 2023-07-13 13:16:58.227121 scoptimize-0.0.7/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     3898 2023-07-13 13:13:22.000000 scoptimize-0.0.7/README.md
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      100 2023-02-13 16:33:50.000000 scoptimize-0.0.7/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 13:16:58.227121 scoptimize-0.0.7/scoptimize/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      153 2023-02-13 16:33:50.000000 scoptimize-0.0.7/scoptimize/__init__.py
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)    13900 2023-07-13 13:15:13.000000 scoptimize-0.0.7/scoptimize/network.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1316 2023-02-13 16:33:50.000000 scoptimize-0.0.7/scoptimize/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 13:16:58.227121 scoptimize-0.0.7/scoptimize.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4514 2023-07-13 13:16:58.000000 scoptimize-0.0.7/scoptimize.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      345 2023-07-13 13:16:58.000000 scoptimize-0.0.7/scoptimize.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-13 13:16:58.000000 scoptimize-0.0.7/scoptimize.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2023-07-13 13:16:58.000000 scoptimize-0.0.7/scoptimize.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-07-13 13:16:58.000000 scoptimize-0.0.7/scoptimize.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-13 13:16:58.227121 scoptimize-0.0.7/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      934 2023-07-13 13:16:35.000000 scoptimize-0.0.7/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 13:16:58.227121 scoptimize-0.0.7/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      478 2023-02-13 16:33:50.000000 scoptimize-0.0.7/test/test_0.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1312 2023-02-13 16:33:50.000000 scoptimize-0.0.7/test/test_1.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      853 2023-02-13 16:33:50.000000 scoptimize-0.0.7/test/test_2.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      486 2023-02-13 16:33:50.000000 scoptimize-0.0.7/test/test_3.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-01-18 14:19:05.455439 scoptimize-0.6/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2022-08-29 14:53:58.000000 scoptimize-0.6/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4326 2023-01-18 14:19:05.455439 scoptimize-0.6/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     3712 2022-08-30 13:58:56.000000 scoptimize-0.6/README.md
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      100 2022-08-29 14:53:58.000000 scoptimize-0.6/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-01-18 14:19:05.455439 scoptimize-0.6/scoptimize/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      153 2022-08-29 15:23:07.000000 scoptimize-0.6/scoptimize/__init__.py
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)    13608 2022-08-30 13:57:39.000000 scoptimize-0.6/scoptimize/network.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1316 2022-08-29 14:53:58.000000 scoptimize-0.6/scoptimize/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-01-18 14:19:05.455439 scoptimize-0.6/scoptimize.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4326 2023-01-18 14:19:05.000000 scoptimize-0.6/scoptimize.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      345 2023-01-18 14:19:05.000000 scoptimize-0.6/scoptimize.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-01-18 14:19:05.000000 scoptimize-0.6/scoptimize.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2023-01-18 14:19:05.000000 scoptimize-0.6/scoptimize.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-01-18 14:19:05.000000 scoptimize-0.6/scoptimize.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-01-18 14:19:05.455439 scoptimize-0.6/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      933 2023-01-18 14:17:01.000000 scoptimize-0.6/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-01-18 14:19:05.455439 scoptimize-0.6/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      478 2022-08-29 15:26:21.000000 scoptimize-0.6/test/test_0.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1312 2022-08-29 15:27:25.000000 scoptimize-0.6/test/test_1.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      853 2022-08-29 15:28:07.000000 scoptimize-0.6/test/test_2.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      486 2022-08-29 15:29:44.000000 scoptimize-0.6/test/test_3.py
```

### Comparing `scoptimize-0.0.7/LICENSE` & `scoptimize-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scoptimize-0.0.7/PKG-INFO` & `scoptimize-0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: scoptimize
-Version: 0.0.7
+Version: 0.6
 Summary: Supply Chain Optimization Package
 Home-page: https://github.com/connor-makowski/scoptimize
-Download-URL: https://github.com/connor-makowski/scoptimize/dist/scoptimize-0.0.7.tar.gz
+Download-URL: https://github.com/connor-makowski/scoptimize/dist/scoptimize-0.0.3.tar.gz
 Author: Connor Makowski
 Author-email: conmak@mit.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SC Optimize
-[![PyPI version](https://badge.fury.io/py/scoptimize.svg)](https://badge.fury.io/py/scoptimize)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
+SC Optimize
+==========
 Supply Chain Optimization package in python using PuLP.
 
-# Setup
+Setup
+----------
 
 Make sure you have Python 3.6.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
 
-## Installation
+### Installation
 
 ```
 pip install scoptimize
 ```
 
 # Getting Started
```

### Comparing `scoptimize-0.0.7/README.md` & `scoptimize-0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# SC Optimize
-[![PyPI version](https://badge.fury.io/py/scoptimize.svg)](https://badge.fury.io/py/scoptimize)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
+SC Optimize
+==========
 Supply Chain Optimization package in python using PuLP.
 
-# Setup
+Setup
+----------
 
 Make sure you have Python 3.6.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
 
-## Installation
+### Installation
 
 ```
 pip install scoptimize
 ```
 
 # Getting Started
```

### Comparing `scoptimize-0.0.7/scoptimize/network.py` & `scoptimize-0.6/scoptimize/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,22 +154,18 @@
 
         - `objects`:
             - Type: dict
             - What: An object dictionary (key=Object.name, Value=Object) for all nodes in the current model
         """
         start_entity = objects.get(self.start)
         if start_entity == None:
-            self.exception(
-                f"`start` entity ({self.start}) not found in current objects list. Did you forget to add it to your nodes? This should be done prior to adding flows. See the `add_nodes` method."
-            )
+            self.exception(f"`start` entity not found in current objects list: `{start}`")
         end_entity = objects.get(self.end)
         if end_entity == None:
-            self.exception(
-                f"`end` entity ({self.end}) not found in current objects list. Did you forget to add it to your nodes? This should be done prior to adding flows. See the `add_nodes` method."
-            )
+            self.exception(f"`end` entity not found in current objects list: `{end}`")
         start_entity.add_outflow(self)
         end_entity.add_inflow(self)
 
     def get_stats(self):
         """
         Get the stats relevant to this flow object
         """
```

### Comparing `scoptimize-0.0.7/scoptimize/utils.py` & `scoptimize-0.6/scoptimize/utils.py`

 * *Files identical despite different names*

### Comparing `scoptimize-0.0.7/scoptimize.egg-info/PKG-INFO` & `scoptimize-0.6/scoptimize.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: scoptimize
-Version: 0.0.7
+Version: 0.6
 Summary: Supply Chain Optimization Package
 Home-page: https://github.com/connor-makowski/scoptimize
-Download-URL: https://github.com/connor-makowski/scoptimize/dist/scoptimize-0.0.7.tar.gz
+Download-URL: https://github.com/connor-makowski/scoptimize/dist/scoptimize-0.0.3.tar.gz
 Author: Connor Makowski
 Author-email: conmak@mit.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SC Optimize
-[![PyPI version](https://badge.fury.io/py/scoptimize.svg)](https://badge.fury.io/py/scoptimize)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
+SC Optimize
+==========
 Supply Chain Optimization package in python using PuLP.
 
-# Setup
+Setup
+----------
 
 Make sure you have Python 3.6.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
 
-## Installation
+### Installation
 
 ```
 pip install scoptimize
 ```
 
 # Getting Started
```

### Comparing `scoptimize-0.0.7/setup.py` & `scoptimize-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scoptimize',
   packages = ['scoptimize'],
-  version = '0.0.7',
+  version = '0.06',
   license='MIT',
   description = 'Supply Chain Optimization Package',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'conmak@mit.edu',
   url = 'https://github.com/connor-makowski/scoptimize',
-  download_url = 'https://github.com/connor-makowski/scoptimize/dist/scoptimize-0.0.7.tar.gz',
+  download_url = 'https://github.com/connor-makowski/scoptimize/dist/scoptimize-0.0.3.tar.gz',
   keywords = [],
   install_requires=["PuLP>=2.7.0", "type_enforced>=0.0.14"],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

### Comparing `scoptimize-0.0.7/test/test_1.py` & `scoptimize-0.6/test/test_1.py`

 * *Files identical despite different names*

### Comparing `scoptimize-0.0.7/test/test_2.py` & `scoptimize-0.6/test/test_2.py`

 * *Files identical despite different names*

