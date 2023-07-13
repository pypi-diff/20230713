# Comparing `tmp/conda_inject-1.0.1.tar.gz` & `tmp/conda_inject-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda_inject-1.0.1.tar", max compression
+gzip compressed data, was "conda_inject-1.0.2.tar", max compression
```

## Comparing `conda_inject-1.0.1.tar` & `conda_inject-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-07-12 12:54:43.877317 conda_inject-1.0.1/LICENSE
--rw-r--r--   0        0        0      197 2023-07-12 12:54:43.877317 conda_inject-1.0.1/README.md
--rw-r--r--   0        0        0     4463 2023-07-12 12:54:43.877317 conda_inject-1.0.1/conda_inject/__init__.py
--rw-r--r--   0        0        0      805 2023-07-12 12:54:43.877317 conda_inject-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 conda_inject-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-13 07:40:58.145798 conda_inject-1.0.2/LICENSE
+-rw-r--r--   0        0        0      197 2023-07-13 07:40:58.145798 conda_inject-1.0.2/README.md
+-rw-r--r--   0        0        0     4463 2023-07-13 07:40:58.145798 conda_inject-1.0.2/conda_inject/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-13 07:40:58.145798 conda_inject-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 conda_inject-1.0.2/PKG-INFO
```

### Comparing `conda_inject-1.0.1/LICENSE` & `conda_inject-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_inject-1.0.1/conda_inject/__init__.py` & `conda_inject-1.0.2/conda_inject/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_inject-1.0.1/pyproject.toml` & `conda_inject-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Johannes Köster <johannes.koester@uni-due.de>"]
 description = "Helper functions for injecting a conda environment into the current python environment (by modifying sys.path, without actually changing the current python environment)."
 name = "conda-inject"
 packages = [{include = "conda_inject"}]
 readme = "README.md"
-version = "1.0.1"
+version = "1.0.2"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
@@ -23,9 +23,7 @@
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*"]
 
 [tool.coverage.report]
 fail_under = 0
 
-[tool.poetry.scripts]
-yte = "yte:main"
```

### Comparing `conda_inject-1.0.1/PKG-INFO` & `conda_inject-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-inject
-Version: 1.0.1
+Version: 1.0.2
 Summary: Helper functions for injecting a conda environment into the current python environment (by modifying sys.path, without actually changing the current python environment).
 Author: Johannes Köster
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

