# Comparing `tmp/mixprops-0.1.2.tar.gz` & `tmp/mixprops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprops-0.1.2.tar", max compression
+gzip compressed data, was "mixprops-0.1.3.tar", max compression
```

## Comparing `mixprops-0.1.2.tar` & `mixprops-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-12 10:20:34.054298 mixprops-0.1.2/LICENSE
--rw-r--r--   0        0        0     1625 2023-07-13 11:49:58.033066 mixprops-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-12 21:02:04.206492 mixprops-0.1.2/mixprops/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-13 11:31:11.459290 mixprops-0.1.2/mixprops/cli.py
--rw-r--r--   0        0        0      205 2023-07-12 21:02:04.207071 mixprops-0.1.2/mixprops/constants.py
--rw-r--r--   0        0        0     9650 2023-07-12 21:02:04.206111 mixprops-0.1.2/mixprops/data/species_T_1000_6000.csv
--rw-r--r--   0        0        0     9140 2023-07-12 21:02:04.206306 mixprops-0.1.2/mixprops/data/species_T_200_1000.csv
--rw-r--r--   0        0        0      889 2023-07-13 11:47:45.466919 mixprops-0.1.2/mixprops/database.py
--rw-r--r--   0        0        0     4579 2023-07-13 11:31:11.459651 mixprops-0.1.2/mixprops/mixture.py
--rw-r--r--   0        0        0     1530 2023-07-13 11:29:50.025842 mixprops-0.1.2/mixprops/reference_conditions.py
--rw-r--r--   0        0        0     2399 2023-07-12 21:02:04.207674 mixprops-0.1.2/mixprops/species.py
--rw-r--r--   0        0        0      541 2023-07-13 11:56:49.415669 mixprops-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 mixprops-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-12 10:20:34.054298 mixprops-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1625 2023-07-13 11:49:58.033066 mixprops-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 21:02:04.206492 mixprops-0.1.3/mixprops/__init__.py
+-rw-r--r--   0        0        0     1549 2023-07-13 11:31:11.459290 mixprops-0.1.3/mixprops/cli.py
+-rw-r--r--   0        0        0      205 2023-07-12 21:02:04.207071 mixprops-0.1.3/mixprops/constants.py
+-rw-r--r--   0        0        0     9650 2023-07-12 21:02:04.206111 mixprops-0.1.3/mixprops/data/species_T_1000_6000.csv
+-rw-r--r--   0        0        0     9140 2023-07-12 21:02:04.206306 mixprops-0.1.3/mixprops/data/species_T_200_1000.csv
+-rw-r--r--   0        0        0      974 2023-07-13 12:03:04.940500 mixprops-0.1.3/mixprops/database.py
+-rw-r--r--   0        0        0     4579 2023-07-13 12:03:15.454754 mixprops-0.1.3/mixprops/mixture.py
+-rw-r--r--   0        0        0     1530 2023-07-13 12:03:16.318927 mixprops-0.1.3/mixprops/reference_conditions.py
+-rw-r--r--   0        0        0     2399 2023-07-12 21:02:04.207674 mixprops-0.1.3/mixprops/species.py
+-rw-r--r--   0        0        0      530 2023-07-13 12:03:53.370194 mixprops-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 mixprops-0.1.3/PKG-INFO
```

### Comparing `mixprops-0.1.2/LICENSE` & `mixprops-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/README.md` & `mixprops-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/mixprops/cli.py` & `mixprops-0.1.3/mixprops/cli.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/mixprops/data/species_T_1000_6000.csv` & `mixprops-0.1.3/mixprops/data/species_T_1000_6000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/mixprops/data/species_T_200_1000.csv` & `mixprops-0.1.3/mixprops/data/species_T_200_1000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/mixprops/database.py` & `mixprops-0.1.3/mixprops/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 from typing import List
 
 import pandas as pd
 
 from mixprops.species import Species
 
-DATA_PATH = "mixprops/data"
+MODULE_PATH = os.path.dirname(os.path.abspath(__file__))
+DATA_PATH = os.path.join(MODULE_PATH, "data")
 
 
 class SpeciesNotFoundException(Exception):
     def __init__(self, name: str):
         self.message = f"Species {name} not found"
         super().__init__(self.message)
```

### Comparing `mixprops-0.1.2/mixprops/mixture.py` & `mixprops-0.1.3/mixprops/mixture.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/mixprops/reference_conditions.py` & `mixprops-0.1.3/mixprops/reference_conditions.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/mixprops/species.py` & `mixprops-0.1.3/mixprops/species.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.2/pyproject.toml` & `mixprops-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [tool.poetry]
 name = "mixprops"
-version = "0.1.2"
+version = "0.1.3"
 description = "Mixture properties calculator"
 authors = ["Oliver Aarnikoivu <oliveraarnikoivu@icloud.com>"]
 license = "MIT"
 readme = "README.md"
-include = [
-    { path = "mixprops/data"},
-]
+include = ["mixprops/data/*.csv"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0.2"
 pandas = "^2.0.3"
```

### Comparing `mixprops-0.1.2/PKG-INFO` & `mixprops-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprops
-Version: 0.1.2
+Version: 0.1.3
 Summary: Mixture properties calculator
 License: MIT
 Author: Oliver Aarnikoivu
 Author-email: oliveraarnikoivu@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

