# Comparing `tmp/mixprops-0.1.3.tar.gz` & `tmp/mixprops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprops-0.1.3.tar", max compression
+gzip compressed data, was "mixprops-0.2.0.tar", max compression
```

## Comparing `mixprops-0.1.3.tar` & `mixprops-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-12 10:20:34.054298 mixprops-0.1.3/LICENSE
--rw-r--r--   0        0        0     1625 2023-07-13 11:49:58.033066 mixprops-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-12 21:02:04.206492 mixprops-0.1.3/mixprops/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-13 11:31:11.459290 mixprops-0.1.3/mixprops/cli.py
--rw-r--r--   0        0        0      205 2023-07-12 21:02:04.207071 mixprops-0.1.3/mixprops/constants.py
--rw-r--r--   0        0        0     9650 2023-07-12 21:02:04.206111 mixprops-0.1.3/mixprops/data/species_T_1000_6000.csv
--rw-r--r--   0        0        0     9140 2023-07-12 21:02:04.206306 mixprops-0.1.3/mixprops/data/species_T_200_1000.csv
--rw-r--r--   0        0        0      974 2023-07-13 12:03:04.940500 mixprops-0.1.3/mixprops/database.py
--rw-r--r--   0        0        0     4579 2023-07-13 12:03:15.454754 mixprops-0.1.3/mixprops/mixture.py
--rw-r--r--   0        0        0     1530 2023-07-13 12:03:16.318927 mixprops-0.1.3/mixprops/reference_conditions.py
--rw-r--r--   0        0        0     2399 2023-07-12 21:02:04.207674 mixprops-0.1.3/mixprops/species.py
--rw-r--r--   0        0        0      530 2023-07-13 12:03:53.370194 mixprops-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 mixprops-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 12:56:49.433042 mixprops-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1822 2023-07-13 12:56:49.433042 mixprops-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/__init__.py
+-rw-r--r--   0        0        0     1549 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/cli.py
+-rw-r--r--   0        0        0      205 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/constants.py
+-rw-r--r--   0        0        0     9650 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/data/species_T_1000_6000.csv
+-rw-r--r--   0        0        0     9140 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/data/species_T_200_1000.csv
+-rw-r--r--   0        0        0      974 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/database.py
+-rw-r--r--   0        0        0     4579 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/mixture.py
+-rw-r--r--   0        0        0     1530 2023-07-13 12:57:09.254453 mixprops-0.2.0/mixprops/reference_conditions.py
+-rw-r--r--   0        0        0     2399 2023-07-13 12:56:49.433042 mixprops-0.2.0/mixprops/species.py
+-rw-r--r--   0        0        0      583 2023-07-13 12:56:49.433042 mixprops-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 mixprops-0.2.0/PKG-INFO
```

### Comparing `mixprops-0.1.3/LICENSE` & `mixprops-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/README.md` & `mixprops-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,34 @@
 [![CI](https://github.com/oaarnikoivu/mixprops/workflows/CI/badge.svg)](https://github.com/oaarnikoivu/mixprops/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![license](https://img.shields.io/github/license/oaarnikoivu/mixprops.svg)](https://github.com/oaarnikoivu/mixprops/blob/main/LICENSE)
 
 Mixture properties calculator.
 
 ## Installation
 
+### Python
+
 ```bash
 pip install mixprops
 ```
 
+### CLI
+
+Follow instructions from [pipx](https://github.com/pypa/pipx) to install `pipx`.
+
+```bash
+pipx install git+https://github.com/oaarnikoivu/mixprops.git
+```
+
 ## Usage
 
 ### Python
 
 ```python
+from mixprops.mixture import Mixture
 from mixprops.reference_conditions import ReferenceConditions
 
 mixture = Mixture(
     species=[("O2", 0.21), ("N2", 0.79)],
     reference_conditions=ReferenceConditions(
         absolute_pressure_unit="Pa",
         absolute_pressure=101325,
@@ -30,15 +41,15 @@
 print(mixture.specific_heat_capacity)
 # 1011.338752
 ```
 
 ### CLI
 
 ```bash
-poetry run python main.py \
+mixprops \
     -rc 101325,25 \
     -u Pa,C \
     -s O2,N2 \
     -sc 0.21,0.79
 ```
 
 - rc = Reference conditions -> Absolute pressure,temperature
```

### Comparing `mixprops-0.1.3/mixprops/cli.py` & `mixprops-0.2.0/mixprops/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 
 from mixprops.mixture import Mixture
 from mixprops.reference_conditions import ReferenceConditions
 
 
-def run():
+def cli():
     parser = argparse.ArgumentParser(description="Mixture properties calculator.")
     parser.add_argument(
         "-rc",
         "--conditions",
         type=str,
         required=True,
         help="Reference conditions values.",
```

### Comparing `mixprops-0.1.3/mixprops/data/species_T_1000_6000.csv` & `mixprops-0.2.0/mixprops/data/species_T_1000_6000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/mixprops/data/species_T_200_1000.csv` & `mixprops-0.2.0/mixprops/data/species_T_200_1000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/mixprops/database.py` & `mixprops-0.2.0/mixprops/database.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/mixprops/mixture.py` & `mixprops-0.2.0/mixprops/mixture.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/mixprops/reference_conditions.py` & `mixprops-0.2.0/mixprops/reference_conditions.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/mixprops/species.py` & `mixprops-0.2.0/mixprops/species.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.3/pyproject.toml` & `mixprops-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "mixprops"
-version = "0.1.3"
+version = "0.2.0"
 description = "Mixture properties calculator"
 authors = ["Oliver Aarnikoivu <oliveraarnikoivu@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["mixprops/data/*.csv"]
 
+[tool.poetry.scripts]
+mixprops = "mixprops.cli:cli"
+
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0.2"
 pandas = "^2.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `mixprops-0.1.3/PKG-INFO` & `mixprops-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprops
-Version: 0.1.3
+Version: 0.2.0
 Summary: Mixture properties calculator
 License: MIT
 Author: Oliver Aarnikoivu
 Author-email: oliveraarnikoivu@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,23 +18,34 @@
 [![CI](https://github.com/oaarnikoivu/mixprops/workflows/CI/badge.svg)](https://github.com/oaarnikoivu/mixprops/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![license](https://img.shields.io/github/license/oaarnikoivu/mixprops.svg)](https://github.com/oaarnikoivu/mixprops/blob/main/LICENSE)
 
 Mixture properties calculator.
 
 ## Installation
 
+### Python
+
 ```bash
 pip install mixprops
 ```
 
+### CLI
+
+Follow instructions from [pipx](https://github.com/pypa/pipx) to install `pipx`.
+
+```bash
+pipx install git+https://github.com/oaarnikoivu/mixprops.git
+```
+
 ## Usage
 
 ### Python
 
 ```python
+from mixprops.mixture import Mixture
 from mixprops.reference_conditions import ReferenceConditions
 
 mixture = Mixture(
     species=[("O2", 0.21), ("N2", 0.79)],
     reference_conditions=ReferenceConditions(
         absolute_pressure_unit="Pa",
         absolute_pressure=101325,
@@ -45,15 +56,15 @@
 print(mixture.specific_heat_capacity)
 # 1011.338752
 ```
 
 ### CLI
 
 ```bash
-poetry run python main.py \
+mixprops \
     -rc 101325,25 \
     -u Pa,C \
     -s O2,N2 \
     -sc 0.21,0.79
 ```
 
 - rc = Reference conditions -> Absolute pressure,temperature
```

