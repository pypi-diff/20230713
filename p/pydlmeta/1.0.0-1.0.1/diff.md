# Comparing `tmp/pydlmeta-1.0.0.tar.gz` & `tmp/pydlmeta-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlmeta-1.0.0.tar", last modified: Wed Jul 12 03:18:15 2023, max compression
+gzip compressed data, was "pydlmeta-1.0.1.tar", last modified: Thu Jul 13 03:27:14 2023, max compression
```

## Comparing `pydlmeta-1.0.0.tar` & `pydlmeta-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 03:18:15.045098 pydlmeta-1.0.0/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1077 2023-07-12 03:18:15.045098 pydlmeta-1.0.0/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      900 2023-07-12 03:17:21.000000 pydlmeta-1.0.0/README.md
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 03:18:15.041098 pydlmeta-1.0.0/pydlmeta/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:40:59.000000 pydlmeta-1.0.0/pydlmeta/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      234 2023-07-12 03:15:30.000000 pydlmeta-1.0.0/pydlmeta/config.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4619 2023-07-12 03:13:09.000000 pydlmeta-1.0.0/pydlmeta/dtype_map.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 03:18:15.045098 pydlmeta-1.0.0/pydlmeta/identifier/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:49:38.000000 pydlmeta-1.0.0/pydlmeta/identifier/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     7418 2023-07-12 03:13:09.000000 pydlmeta-1.0.0/pydlmeta/identifier/dataset.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    10974 2023-07-12 03:13:09.000000 pydlmeta-1.0.0/pydlmeta/identifier/model.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2018 2023-07-11 03:49:38.000000 pydlmeta-1.0.0/pydlmeta/identifier/types.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    16534 2023-07-12 03:13:09.000000 pydlmeta-1.0.0/pydlmeta/meta.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      567 2023-07-12 03:15:30.000000 pydlmeta-1.0.0/pydlmeta/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 03:18:15.045098 pydlmeta-1.0.0/pydlmeta.egg-info/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1077 2023-07-12 03:18:15.000000 pydlmeta-1.0.0/pydlmeta.egg-info/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      413 2023-07-12 03:18:15.000000 pydlmeta-1.0.0/pydlmeta.egg-info/SOURCES.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-12 03:18:15.000000 pydlmeta-1.0.0/pydlmeta.egg-info/dependency_links.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      132 2023-07-12 03:18:15.000000 pydlmeta-1.0.0/pydlmeta.egg-info/requires.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        9 2023-07-12 03:18:15.000000 pydlmeta-1.0.0/pydlmeta.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-12 03:18:15.045098 pydlmeta-1.0.0/setup.cfg
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1253 2023-07-12 03:15:17.000000 pydlmeta-1.0.0/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      904 2023-07-13 03:25:48.000000 pydlmeta-1.0.1/README.md
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/pydlmeta/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:40:59.000000 pydlmeta-1.0.1/pydlmeta/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      234 2023-07-12 03:15:30.000000 pydlmeta-1.0.1/pydlmeta/config.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4619 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/dtype_map.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/pydlmeta/identifier/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:49:38.000000 pydlmeta-1.0.1/pydlmeta/identifier/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7418 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/identifier/dataset.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    10974 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/identifier/model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2018 2023-07-11 03:49:38.000000 pydlmeta-1.0.1/pydlmeta/identifier/types.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    16534 2023-07-12 03:13:09.000000 pydlmeta-1.0.1/pydlmeta/meta.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      567 2023-07-12 03:15:30.000000 pydlmeta-1.0.1/pydlmeta/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/pydlmeta.egg-info/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      413 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/SOURCES.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/dependency_links.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       80 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/requires.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        9 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/pydlmeta.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-13 03:27:14.677203 pydlmeta-1.0.1/setup.cfg
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1253 2023-07-13 03:27:14.000000 pydlmeta-1.0.1/setup.py
```

### Comparing `pydlmeta-1.0.0/PKG-INFO` & `pydlmeta-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pydlmeta
-Version: 1.0.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: Apache License 2.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # PyDLmeta
 
 Features: identify the model type belong to which deep learning framework
 and extract the meta data if possible. The meta data includes input/output
 name and shape of the model.
 
 The supported formats are:
@@ -24,15 +15,15 @@
 - Caffe model directory: *.caffemodel/ *.prototxt
 
 - Openvino IR directory: *.xml/ *.bin
 
 # Installation
 - Create a Python 3.8 environment and activate it.
 ```
-git clone --depth 1 -b develop --recursive git@github.com:skymizer/pydlmeta.git
+git clone --depth 1 -b develop --recursive https://github.com/skymizer/pydlmeta.git
 (cd pydlmeta && python3 -m pip install -e .)
 ```
 
 # Usage
 
 — Retrieve the metadata of the model
 ```
@@ -40,9 +31,8 @@
 res = retrieve_model_metadata("/path/to/your/model")
 ```
 
 - Identify model format
 ```
 from pydlmeta.identifier.model import identify
 model_format = identify(model_path)
-```
-
+```
```

### Comparing `pydlmeta-1.0.0/pydlmeta/dtype_map.py` & `pydlmeta-1.0.1/pydlmeta/dtype_map.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.0/pydlmeta/identifier/dataset.py` & `pydlmeta-1.0.1/pydlmeta/identifier/dataset.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.0/pydlmeta/identifier/model.py` & `pydlmeta-1.0.1/pydlmeta/identifier/model.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.0/pydlmeta/identifier/types.py` & `pydlmeta-1.0.1/pydlmeta/identifier/types.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.0/pydlmeta/meta.py` & `pydlmeta-1.0.1/pydlmeta/meta.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.0/pydlmeta/utils.py` & `pydlmeta-1.0.1/pydlmeta/utils.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.0/pydlmeta.egg-info/PKG-INFO` & `pydlmeta-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlmeta
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # PyDLmeta
@@ -24,15 +24,15 @@
 - Caffe model directory: *.caffemodel/ *.prototxt
 
 - Openvino IR directory: *.xml/ *.bin
 
 # Installation
 - Create a Python 3.8 environment and activate it.
 ```
-git clone --depth 1 -b develop --recursive git@github.com:skymizer/pydlmeta.git
+git clone --depth 1 -b develop --recursive https://github.com/skymizer/pydlmeta.git
 (cd pydlmeta && python3 -m pip install -e .)
 ```
 
 # Usage
 
 — Retrieve the metadata of the model
 ```
```

### Comparing `pydlmeta-1.0.0/setup.py` & `pydlmeta-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="pydlmeta",
-    version="1.0.0",
+    version="1.0.1",
     license="Apache License 2.0",
     long_description=README, # without this pypi upload will raise warning
     long_description_content_type="text/markdown",  # without this pypi upload will raise warning
     packages=find_packages(),
     package_data={"pydlmeta": ["*"]},
     dependency_links=[
         "https://download.pytorch.org/whl/torch_stable.html",
```

