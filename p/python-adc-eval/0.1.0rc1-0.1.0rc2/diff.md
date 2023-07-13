# Comparing `tmp/python-adc-eval-0.1.0rc1.tar.gz` & `tmp/python-adc-eval-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-adc-eval-0.1.0rc1.tar", last modified: Thu Jul 13 20:09:13 2023, max compression
+gzip compressed data, was "python-adc-eval-0.1.0rc2.tar", last modified: Thu Jul 13 20:48:54 2023, max compression
```

## Comparing `python-adc-eval-0.1.0rc1.tar` & `python-adc-eval-0.1.0rc2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:09:13.967065 python-adc-eval-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 20:08:56.000000 python-adc-eval-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 20:08:56.000000 python-adc-eval-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-13 20:09:13.967065 python-adc-eval-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-13 20:08:56.000000 python-adc-eval-0.1.0rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-13 20:08:56.000000 python-adc-eval-0.1.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:09:13.967065 python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-13 20:09:13.000000 python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 20:09:13.000000 python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:09:13.000000 python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 20:09:13.000000 python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:09:13.000000 python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 20:08:56.000000 python-adc-eval-0.1.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:09:13.967065 python-adc-eval-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/adc_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/setup.cfg
```

### Comparing `python-adc-eval-0.1.0rc1/LICENSE` & `python-adc-eval-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.0rc1/PKG-INFO` & `python-adc-eval-0.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
```

### Comparing `python-adc-eval-0.1.0rc1/README.rst` & `python-adc-eval-0.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.0rc1/pyproject.toml` & `python-adc-eval-0.1.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=68.0", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-adc-eval"
-version = "0.1.0rc1"
+version = "0.1.0rc2"
 license = {text = "MIT"}
 description = "ADC Evaluation Library"
 readme = "README.rst"
 authors = [{name = "Kevin Fronczak", email = "kfronczak@gmail.com"}]
 keywords = ["adc", "analog-to-digital", "evaluation", "eval", "spectrum"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -29,15 +29,15 @@
 "Bug Reports" = "https://github.com/fronzbot/python-adc-eval/issues"
 
 [tool.setuptools]
 platforms = ["any"]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-include = ["src/*"]
+include = ["adc_eval*"]
 
 [tool.ruff]
 select = [
     "C",  # complexity
     "D",  # docstrings
     "E",  # pydocstyle
     "F",  # pyflakes/autoflake
```

### Comparing `python-adc-eval-0.1.0rc1/python_adc_eval.egg-info/PKG-INFO` & `python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
```

