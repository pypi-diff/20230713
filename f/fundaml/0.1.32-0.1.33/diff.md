# Comparing `tmp/fundaml-0.1.32.tar.gz` & `tmp/fundaml-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundaml-0.1.32.tar", max compression
+gzip compressed data, was "fundaml-0.1.33.tar", max compression
```

## Comparing `fundaml-0.1.32.tar` & `fundaml-0.1.33.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1069 2023-07-09 20:13:04.215596 fundaml-0.1.32/LICENSE
--rw-r--r--   0        0        0     2314 2023-07-09 20:13:04.219596 fundaml-0.1.32/README.md
--rw-r--r--   0        0        0     1614 2023-07-09 20:25:29.405250 fundaml-0.1.32/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-09 20:13:04.587599 fundaml-0.1.32/src/fundaml/__init__.py
--rw-r--r--   0        0        0     1058 2023-07-09 20:13:04.587599 fundaml-0.1.32/src/fundaml/eda.py
--rw-r--r--   0        0        0     1400 2023-07-09 20:13:04.587599 fundaml-0.1.32/src/fundaml/models.py
--rw-r--r--   0        0        0     1032 2023-07-09 20:13:04.587599 fundaml-0.1.32/src/fundaml/scores.py
--rw-r--r--   0        0        0    17645 2023-07-09 20:13:04.587599 fundaml-0.1.32/src/fundaml/trainers.py
--rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 fundaml-0.1.32/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-13 13:27:54.203014 fundaml-0.1.33/LICENSE
+-rw-r--r--   0        0        0     2284 2023-07-13 13:27:54.203014 fundaml-0.1.33/README.md
+-rw-r--r--   0        0        0     1614 2023-07-13 13:40:01.281395 fundaml-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/eda.py
+-rw-r--r--   0        0        0     1400 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/models.py
+-rw-r--r--   0        0        0     1032 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/scores.py
+-rw-r--r--   0        0        0    17645 2023-07-13 13:27:54.567020 fundaml-0.1.33/src/fundaml/trainers.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.33/PKG-INFO
```

### Comparing `fundaml-0.1.32/LICENSE` & `fundaml-0.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.32/README.md` & `fundaml-0.1.33/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 
-`fundaml` was created by Tony Zoght. It is licensed under the terms of the MIT license.
+`fundaml` is licensed under the terms of the MIT license.
 
 ## Credits
 
 `fundaml` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
 
 
 ## Code Coverage
```

### Comparing `fundaml-0.1.32/pyproject.toml` & `fundaml-0.1.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fundaml"
-version = "0.1.32"
+version = "0.1.33"
 description = "A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks."
 authors = ["Tony Zoght"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `fundaml-0.1.32/src/fundaml/eda.py` & `fundaml-0.1.33/src/fundaml/eda.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.32/src/fundaml/models.py` & `fundaml-0.1.33/src/fundaml/models.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.32/src/fundaml/scores.py` & `fundaml-0.1.33/src/fundaml/scores.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.32/src/fundaml/trainers.py` & `fundaml-0.1.33/src/fundaml/trainers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.32/PKG-INFO` & `fundaml-0.1.33/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundaml
-Version: 0.1.32
+Version: 0.1.33
 Summary: A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks.
 License: MIT
 Author: Tony Zoght
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -48,15 +48,15 @@
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 
-`fundaml` was created by Tony Zoght. It is licensed under the terms of the MIT license.
+`fundaml` is licensed under the terms of the MIT license.
 
 ## Credits
 
 `fundaml` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
 
 
 ## Code Coverage
```

