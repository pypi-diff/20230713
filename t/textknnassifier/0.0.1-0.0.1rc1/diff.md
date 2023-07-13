# Comparing `tmp/textknnassifier-0.0.1.tar.gz` & `tmp/textknnassifier-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textknnassifier-0.0.1.tar", max compression
+gzip compressed data, was "textknnassifier-0.0.1rc1.tar", max compression
```

## Comparing `textknnassifier-0.0.1.tar` & `textknnassifier-0.0.1rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    26190 2023-07-13 19:54:47.282577 textknnassifier-0.0.1/LICENSE
--rw-r--r--   0        0        0     2395 2023-07-13 19:54:47.282577 textknnassifier-0.0.1/README.md
--rw-r--r--   0        0        0      942 2023-07-13 19:54:47.282577 textknnassifier-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 19:54:47.282577 textknnassifier-0.0.1/src/textknnassifier/__init__.py
--rw-r--r--   0        0        0     4626 2023-07-13 19:54:47.282577 textknnassifier-0.0.1/src/textknnassifier/classifier.py
--rw-r--r--   0        0        0     1276 2023-07-13 19:54:47.282577 textknnassifier-0.0.1/src/textknnassifier/compressor.py
--rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 textknnassifier-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    26190 2023-07-13 19:31:04.763576 textknnassifier-0.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     2395 2023-07-13 19:31:04.763576 textknnassifier-0.0.1rc1/README.md
+-rw-r--r--   0        0        0      945 2023-07-13 19:31:04.763576 textknnassifier-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 19:31:04.763576 textknnassifier-0.0.1rc1/src/textknnassifier/__init__.py
+-rw-r--r--   0        0        0     4626 2023-07-13 19:31:04.763576 textknnassifier-0.0.1rc1/src/textknnassifier/classifier.py
+-rw-r--r--   0        0        0     1276 2023-07-13 19:31:04.763576 textknnassifier-0.0.1rc1/src/textknnassifier/compressor.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 textknnassifier-0.0.1rc1/PKG-INFO
```

### Comparing `textknnassifier-0.0.1/LICENSE` & `textknnassifier-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `textknnassifier-0.0.1/README.md` & `textknnassifier-0.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `textknnassifier-0.0.1/pyproject.toml` & `textknnassifier-0.0.1rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textknnassifier"
-version = "0.0.1"
+version = "0.0.1rc1"
 description = "TextKNNClassifier is a k-nearest neighbors classifier for text data. It uses a compression algorithm to compute the distance between texts and predicts the label of a test entry based on the labels of the k-nearest neighbors in the training data."
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "textknnassifier", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `textknnassifier-0.0.1/src/textknnassifier/classifier.py` & `textknnassifier-0.0.1rc1/src/textknnassifier/classifier.py`

 * *Files identical despite different names*

### Comparing `textknnassifier-0.0.1/src/textknnassifier/compressor.py` & `textknnassifier-0.0.1rc1/src/textknnassifier/compressor.py`

 * *Files identical despite different names*

### Comparing `textknnassifier-0.0.1/PKG-INFO` & `textknnassifier-0.0.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textknnassifier
-Version: 0.0.1
+Version: 0.0.1rc1
 Summary: TextKNNClassifier is a k-nearest neighbors classifier for text data. It uses a compression algorithm to compute the distance between texts and predicts the label of a test entry based on the labels of the k-nearest neighbors in the training data.
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

