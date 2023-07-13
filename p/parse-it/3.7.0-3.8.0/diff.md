# Comparing `tmp/parse_it-3.7.0.tar.gz` & `tmp/parse_it-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parse_it-3.7.0.tar", last modified: Mon May  3 12:08:39 2021, max compression
+gzip compressed data, was "dist/parse_it-3.8.0.tar", last modified: Tue Jun  1 13:28:51 2021, max compression
```

## Comparing `parse_it-3.7.0.tar` & `parse_it-3.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.796697 parse_it-3.7.0/
--rw-r--r--   0 root         (0) root         (0)    17806 2021-05-03 12:08:39.796697 parse_it-3.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14005 2021-05-03 12:08:19.000000 parse_it-3.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.792696 parse_it-3.7.0/parse_it/
--rw-r--r--   0 root         (0) root         (0)       22 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.792696 parse_it-3.7.0/parse_it/command_line_args/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/command_line_args/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1480 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/command_line_args/command_line_args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.792696 parse_it-3.7.0/parse_it/envvars/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/envvars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4547 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/envvars/envvars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.796697 parse_it-3.7.0/parse_it/file/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)      379 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/env.py
--rw-r--r--   0 root         (0) root         (0)     3951 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/file_reader.py
--rw-r--r--   0 root         (0) root         (0)      391 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/hcl.py
--rw-r--r--   0 root         (0) root         (0)      387 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/ini.py
--rw-r--r--   0 root         (0) root         (0)      399 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/json.py
--rw-r--r--   0 root         (0) root         (0)      399 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/toml.py
--rw-r--r--   0 root         (0) root         (0)      525 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/xml.py
--rw-r--r--   0 root         (0) root         (0)      422 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/file/yaml.py
--rw-r--r--   0 root         (0) root         (0)    21448 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.796697 parse_it-3.7.0/parse_it/type_estimate/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/type_estimate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1280 2021-05-03 12:08:19.000000 parse_it-3.7.0/parse_it/type_estimate/type_estimate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.792696 parse_it-3.7.0/parse_it.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17806 2021-05-03 12:08:39.000000 parse_it-3.7.0/parse_it.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      680 2021-05-03 12:08:39.000000 parse_it-3.7.0/parse_it.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-03 12:08:39.000000 parse_it-3.7.0/parse_it.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2021-05-03 12:08:39.000000 parse_it-3.7.0/parse_it.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-05-03 12:08:39.000000 parse_it-3.7.0/parse_it.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-03 12:08:39.796697 parse_it-3.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2141 2021-05-03 12:08:19.000000 parse_it-3.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-03 12:08:39.796697 parse_it-3.7.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-03 12:08:19.000000 parse_it-3.7.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64071 2021-05-03 12:08:19.000000 parse_it-3.7.0/test/test_prase_it.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.055864 parse_it-3.8.0/
+-rw-r--r--   0 root         (0) root         (0)    17806 2021-06-01 13:28:51.055864 parse_it-3.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14005 2021-06-01 13:28:39.000000 parse_it-3.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.051864 parse_it-3.8.0/parse_it/
+-rw-r--r--   0 root         (0) root         (0)       22 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.051864 parse_it-3.8.0/parse_it/command_line_args/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/command_line_args/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1480 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/command_line_args/command_line_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.051864 parse_it-3.8.0/parse_it/envvars/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/envvars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/envvars/envvars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.055864 parse_it-3.8.0/parse_it/file/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      379 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/env.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/file_reader.py
+-rw-r--r--   0 root         (0) root         (0)      391 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/hcl.py
+-rw-r--r--   0 root         (0) root         (0)      387 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/ini.py
+-rw-r--r--   0 root         (0) root         (0)      399 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/json.py
+-rw-r--r--   0 root         (0) root         (0)      399 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/toml.py
+-rw-r--r--   0 root         (0) root         (0)      525 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/xml.py
+-rw-r--r--   0 root         (0) root         (0)      422 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/file/yaml.py
+-rw-r--r--   0 root         (0) root         (0)    21448 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.055864 parse_it-3.8.0/parse_it/type_estimate/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/type_estimate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2021-06-01 13:28:39.000000 parse_it-3.8.0/parse_it/type_estimate/type_estimate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.051864 parse_it-3.8.0/parse_it.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17806 2021-06-01 13:28:50.000000 parse_it-3.8.0/parse_it.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      680 2021-06-01 13:28:50.000000 parse_it-3.8.0/parse_it.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-06-01 13:28:50.000000 parse_it-3.8.0/parse_it.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2021-06-01 13:28:50.000000 parse_it-3.8.0/parse_it.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-06-01 13:28:50.000000 parse_it-3.8.0/parse_it.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-01 13:28:51.055864 parse_it-3.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2141 2021-06-01 13:28:39.000000 parse_it-3.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 13:28:51.055864 parse_it-3.8.0/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-01 13:28:39.000000 parse_it-3.8.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64071 2021-06-01 13:28:39.000000 parse_it-3.8.0/test/test_prase_it.py
```

### Comparing `parse_it-3.7.0/PKG-INFO` & `parse_it-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_it
-Version: 3.7.0
+Version: 3.8.0
 Summary: A python library for parsing multiple types of config files, envvars and command line arguments which takes the headache out of setting app configurations.
 Home-page: https://github.com/naorlivne/parse_it
 Author: Naor Livne
 Author-email: naorlivne@gmail.com
 License: LGPLv3
 Description: # parse_it
```

### Comparing `parse_it-3.7.0/README.md` & `parse_it-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it/command_line_args/command_line_args.py` & `parse_it-3.8.0/parse_it/command_line_args/command_line_args.py`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it/envvars/envvars.py` & `parse_it-3.8.0/parse_it/envvars/envvars.py`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it/file/file_reader.py` & `parse_it-3.8.0/parse_it/file/file_reader.py`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it/file/xml.py` & `parse_it-3.8.0/parse_it/file/xml.py`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it/parser.py` & `parse_it-3.8.0/parse_it/parser.py`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it/type_estimate/type_estimate.py` & `parse_it-3.8.0/parse_it/type_estimate/type_estimate.py`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/parse_it.egg-info/PKG-INFO` & `parse_it-3.8.0/parse_it.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-it
-Version: 3.7.0
+Version: 3.8.0
 Summary: A python library for parsing multiple types of config files, envvars and command line arguments which takes the headache out of setting app configurations.
 Home-page: https://github.com/naorlivne/parse_it
 Author: Naor Livne
 Author-email: naorlivne@gmail.com
 License: LGPLv3
 Description: # parse_it
```

### Comparing `parse_it-3.7.0/parse_it.egg-info/SOURCES.txt` & `parse_it-3.8.0/parse_it.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parse_it-3.7.0/setup.py` & `parse_it-3.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 __author__ = 'Naor Livne'
 __author_email__ = 'naorlivne@gmail.com'
-__version__ = "3.7.0"
+__version__ = "3.8.0"
 
 # read the README.md file for the long description of the package
 with open('README.md') as f:
     long_description = f.read()
 
 # minimum requirement list
 requirements = [
```

### Comparing `parse_it-3.7.0/test/test_prase_it.py` & `parse_it-3.8.0/test/test_prase_it.py`

 * *Files identical despite different names*

