# Comparing `tmp/mixprops-0.1.0.tar.gz` & `tmp/mixprops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprops-0.1.0.tar", max compression
+gzip compressed data, was "mixprops-0.1.1.tar", max compression
```

## Comparing `mixprops-0.1.0.tar` & `mixprops-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-12 10:20:34.054298 mixprops-0.1.0/LICENSE
--rw-r--r--   0        0        0     1566 2023-07-13 11:31:11.458922 mixprops-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 21:02:04.206492 mixprops-0.1.0/mixprops/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-13 11:31:11.459290 mixprops-0.1.0/mixprops/cli.py
--rw-r--r--   0        0        0      205 2023-07-12 21:02:04.207071 mixprops-0.1.0/mixprops/constants.py
--rw-r--r--   0        0        0      880 2023-07-13 11:19:38.159584 mixprops-0.1.0/mixprops/database.py
--rw-r--r--   0        0        0     4579 2023-07-13 11:31:11.459651 mixprops-0.1.0/mixprops/mixture.py
--rw-r--r--   0        0        0     1530 2023-07-13 11:29:50.025842 mixprops-0.1.0/mixprops/reference_conditions.py
--rw-r--r--   0        0        0     2399 2023-07-12 21:02:04.207674 mixprops-0.1.0/mixprops/species.py
--rw-r--r--   0        0        0      496 2023-07-13 06:29:20.145042 mixprops-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2039 1970-01-01 00:00:00.000000 mixprops-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-12 10:20:34.054298 mixprops-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1574 2023-07-13 11:48:28.257044 mixprops-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 21:02:04.206492 mixprops-0.1.1/mixprops/__init__.py
+-rw-r--r--   0        0        0     1549 2023-07-13 11:31:11.459290 mixprops-0.1.1/mixprops/cli.py
+-rw-r--r--   0        0        0      205 2023-07-12 21:02:04.207071 mixprops-0.1.1/mixprops/constants.py
+-rw-r--r--   0        0        0     9650 2023-07-12 21:02:04.206111 mixprops-0.1.1/mixprops/data/species_T_1000_6000.csv
+-rw-r--r--   0        0        0     9140 2023-07-12 21:02:04.206306 mixprops-0.1.1/mixprops/data/species_T_200_1000.csv
+-rw-r--r--   0        0        0      889 2023-07-13 11:47:45.466919 mixprops-0.1.1/mixprops/database.py
+-rw-r--r--   0        0        0     4579 2023-07-13 11:31:11.459651 mixprops-0.1.1/mixprops/mixture.py
+-rw-r--r--   0        0        0     1530 2023-07-13 11:29:50.025842 mixprops-0.1.1/mixprops/reference_conditions.py
+-rw-r--r--   0        0        0     2399 2023-07-12 21:02:04.207674 mixprops-0.1.1/mixprops/species.py
+-rw-r--r--   0        0        0      496 2023-07-13 11:49:22.205226 mixprops-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2047 1970-01-01 00:00:00.000000 mixprops-0.1.1/PKG-INFO
```

### Comparing `mixprops-0.1.0/LICENSE` & `mixprops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.0/README.md` & `mixprops-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 - `viscosity` - Viscosity (kg/m-s)
 - `conductivity` - Thermal conductivity (W/m-K)
 - `speed_of_sound` - Speed of sound (m/s)
 - `adiabatic_index` - Adiabatic index
 
 ### Supported species
 
-For the supported species, see the `.csv` files in the `data/` directory.
+For the supported species, see the `.csv` files in the `mixprops/data` directory.
```

### Comparing `mixprops-0.1.0/mixprops/cli.py` & `mixprops-0.1.1/mixprops/cli.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.0/mixprops/database.py` & `mixprops-0.1.1/mixprops/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 import pandas as pd
 
 from mixprops.species import Species
 
-DATA_PATH = "data"
+DATA_PATH = "mixprops/data"
 
 
 class SpeciesNotFoundException(Exception):
     def __init__(self, name: str):
         self.message = f"Species {name} not found"
         super().__init__(self.message)
```

### Comparing `mixprops-0.1.0/mixprops/mixture.py` & `mixprops-0.1.1/mixprops/mixture.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.0/mixprops/reference_conditions.py` & `mixprops-0.1.1/mixprops/reference_conditions.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.0/mixprops/species.py` & `mixprops-0.1.1/mixprops/species.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.1.0/PKG-INFO` & `mixprops-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprops
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mixture properties calculator
 License: MIT
 Author: Oliver Aarnikoivu
 Author-email: oliveraarnikoivu@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -63,9 +63,9 @@
 - `viscosity` - Viscosity (kg/m-s)
 - `conductivity` - Thermal conductivity (W/m-K)
 - `speed_of_sound` - Speed of sound (m/s)
 - `adiabatic_index` - Adiabatic index
 
 ### Supported species
 
-For the supported species, see the `.csv` files in the `data/` directory.
+For the supported species, see the `.csv` files in the `mixprops/data` directory.
```

