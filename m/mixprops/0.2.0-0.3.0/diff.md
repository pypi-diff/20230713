# Comparing `tmp/mixprops-0.2.0.tar.gz` & `tmp/mixprops-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprops-0.2.0.tar", max compression
+gzip compressed data, was "mixprops-0.3.0.tar", max compression
```

## Comparing `mixprops-0.2.0.tar` & `mixprops-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-13 12:56:49.433042 mixprops-0.2.0/LICENSE
--rw-r--r--   0        0        0     1822 2023-07-13 12:56:49.433042 mixprops-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/cli.py
--rw-r--r--   0        0        0      205 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/constants.py
--rw-r--r--   0        0        0     9650 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/data/species_T_1000_6000.csv
--rw-r--r--   0        0        0     9140 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/data/species_T_200_1000.csv
--rw-r--r--   0        0        0      974 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/database.py
--rw-r--r--   0        0        0     4579 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/mixture.py
--rw-r--r--   0        0        0     1530 2023-07-13 12:57:09.254453 mixprops-0.2.0/mixprops/reference_conditions.py
--rw-r--r--   0        0        0     2399 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/species.py
--rw-r--r--   0        0        0      583 2023-07-13 12:56:49.433042 mixprops-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 mixprops-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 13:14:06.181738 mixprops-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2016 2023-07-13 13:14:06.181738 mixprops-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/__init__.py
+-rw-r--r--   0        0        0     1549 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/cli.py
+-rw-r--r--   0        0        0      205 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/constants.py
+-rw-r--r--   0        0        0     9650 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/data/species_T_1000_6000.csv
+-rw-r--r--   0        0        0     9140 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/data/species_T_200_1000.csv
+-rw-r--r--   0        0        0      974 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/database.py
+-rw-r--r--   0        0        0     4579 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/mixture.py
+-rw-r--r--   0        0        0     1530 2023-07-13 13:14:24.209764 mixprops-0.3.0/mixprops/reference_conditions.py
+-rw-r--r--   0        0        0     2399 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/species.py
+-rw-r--r--   0        0        0      585 2023-07-13 13:14:06.181738 mixprops-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 mixprops-0.3.0/PKG-INFO
```

### Comparing `mixprops-0.2.0/LICENSE` & `mixprops-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/README.md` & `mixprops-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # mixprops
 
 [![CI](https://github.com/oaarnikoivu/mixprops/workflows/CI/badge.svg)](https://github.com/oaarnikoivu/mixprops/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
+[![pypi](https://img.shields.io/pypi/v/mixprops)](https://pypi.org/project/mixprops/)
+[![versions](https://img.shields.io/pypi/pyversions/mixprops.svg)](https://github.com/oaarnikoivu/mixprops)
 [![license](https://img.shields.io/github/license/oaarnikoivu/mixprops.svg)](https://github.com/oaarnikoivu/mixprops/blob/main/LICENSE)
 
 Mixture properties calculator.
 
 ## Installation
 
 ### Python
```

### Comparing `mixprops-0.2.0/mixprops/cli.py` & `mixprops-0.3.0/mixprops/cli.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/mixprops/data/species_T_1000_6000.csv` & `mixprops-0.3.0/mixprops/data/species_T_1000_6000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/mixprops/data/species_T_200_1000.csv` & `mixprops-0.3.0/mixprops/data/species_T_200_1000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/mixprops/database.py` & `mixprops-0.3.0/mixprops/database.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/mixprops/mixture.py` & `mixprops-0.3.0/mixprops/mixture.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/mixprops/reference_conditions.py` & `mixprops-0.3.0/mixprops/reference_conditions.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/mixprops/species.py` & `mixprops-0.3.0/mixprops/species.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.2.0/pyproject.toml` & `mixprops-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "mixprops"
-version = "0.2.0"
+version = "0.3.0"
 description = "Mixture properties calculator"
 authors = ["Oliver Aarnikoivu <oliveraarnikoivu@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["mixprops/data/*.csv"]
 
 [tool.poetry.scripts]
 mixprops = "mixprops.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8.1"
 pydantic = "^2.0.2"
 pandas = "^2.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
```

### Comparing `mixprops-0.2.0/PKG-INFO` & `mixprops-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: mixprops
-Version: 0.2.0
+Version: 0.3.0
 Summary: Mixture properties calculator
 License: MIT
 Author: Oliver Aarnikoivu
 Author-email: oliveraarnikoivu@icloud.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # mixprops
 
 [![CI](https://github.com/oaarnikoivu/mixprops/workflows/CI/badge.svg)](https://github.com/oaarnikoivu/mixprops/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
+[![pypi](https://img.shields.io/pypi/v/mixprops)](https://pypi.org/project/mixprops/)
+[![versions](https://img.shields.io/pypi/pyversions/mixprops.svg)](https://github.com/oaarnikoivu/mixprops)
 [![license](https://img.shields.io/github/license/oaarnikoivu/mixprops.svg)](https://github.com/oaarnikoivu/mixprops/blob/main/LICENSE)
 
 Mixture properties calculator.
 
 ## Installation
 
 ### Python
```

