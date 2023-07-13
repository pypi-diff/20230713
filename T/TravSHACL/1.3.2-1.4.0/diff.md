# Comparing `tmp/TravSHACL-1.3.2.tar.gz` & `tmp/TravSHACL-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TravSHACL-1.3.2.tar", last modified: Sun Jul  9 12:56:41 2023, max compression
+gzip compressed data, was "TravSHACL-1.4.0.tar", last modified: Thu Jul 13 12:18:34 2023, max compression
```

## Comparing `TravSHACL-1.3.2.tar` & `TravSHACL-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.602640 TravSHACL-1.3.2/TravSHACL/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/TravSHACL.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.602640 TravSHACL-1.3.2/TravSHACL/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/constraints/SPARQLConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.602640 TravSHACL-1.3.2/TravSHACL/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/core/GraphTraversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/core/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/core/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/core/ShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/TravSHACL/rule_based_validation/
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/rule_based_validation/InstancesRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    33764 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/rule_based_validation/Validation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/rule_based_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/TravSHACL/sparql/
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/TravSHACL/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/utils/ValidationStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/utils/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/TravSHACL/utils/fileManagement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.602640 TravSHACL-1.3.2/TravSHACL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-09 12:56:41.000000 TravSHACL-1.3.2/TravSHACL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 12:56:41.000000 TravSHACL-1.3.2/TravSHACL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:56:41.000000 TravSHACL-1.3.2/TravSHACL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 12:56:41.000000 TravSHACL-1.3.2/TravSHACL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 12:56:41.000000 TravSHACL-1.3.2/TravSHACL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:56:41.606641 TravSHACL-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-09 12:56:29.000000 TravSHACL-1.3.2/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.216628 TravSHACL-1.4.0/TravSHACL/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/TravSHACL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.216628 TravSHACL-1.4.0/TravSHACL/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/SPARQLConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/GraphTraversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29359 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/ShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/rule_based_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/rule_based_validation/InstancesRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/rule_based_validation/Validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/rule_based_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/ValidationStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/fileManagement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.216628 TravSHACL-1.4.0/TravSHACL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/tests/test_cases.py
```

### Comparing `TravSHACL-1.3.2/LICENSE` & `TravSHACL-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/PKG-INFO` & `TravSHACL-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.3.2
+Version: 1.4.0
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.3.2.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.0.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/SDM-TIB/Trav-SHACL/actions/workflows/test.yml/badge.svg)](https://github.com/SDM-TIB/Trav-SHACL/actions/workflows/test.yml)
 [![Latest Release](http://img.shields.io/github/release/SDM-TIB/Trav-SHACL.svg?logo=github)](https://github.com/SDM-TIB/Trav-SHACL/releases)
 [![Docker Image](https://img.shields.io/badge/Docker%20Image-sdmtib/travshacl-blue?logo=Docker)](https://hub.docker.com/r/sdmtib/travshacl)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
```

### Comparing `TravSHACL-1.3.2/README.md` & `TravSHACL-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/TravSHACL.py` & `TravSHACL-1.4.0/TravSHACL/TravSHACL.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/constraints/Constraint.py` & `TravSHACL-1.4.0/TravSHACL/constraints/Constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 __author__ = 'Monica Figuera and Philipp D. Rohde'
 
 
 class Constraint:
     """Base class for all constraints."""
 
     def __init__(self, id_=None, is_pos=None, satisfied=None, datatype=None, value=None,
-                 shape_ref=None, target_def=None, path=None):
+                 shape_ref=None, target_def=None, path=None, options=None, raw_or=None):
         """
         Base constructor for all constraints.
 
         :param id_: name of the constraint
         :param is_pos: true if it is a positive constraint, false otherwise
         :param satisfied: indicates whether the constraint is satisfied, should be unknown at creation
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         :param path: the path associated with this constraint, e.g., a predicate
+        :param options: gets the options to be used in or_operation
+        :param raw_or: contains the specific constraints for or in the shapes graph
         """
         self.id = id_
         self.isPos = is_pos
         self.satisfied = satisfied
-
+        self.options = options
+        self.raw_or = raw_or
         self.datatype = datatype
         self.value = value
         self.shapeRef = shape_ref
         self.target = target_def
 
         self.variables = []
         self.path = path
@@ -42,20 +45,24 @@
 
     def get_id(self):
         return self.id
 
     def get_is_pos(self):
         return self.isPos
 
+    def get_options(self):
+        return self.options
+
     @staticmethod
     def generate_variables(var_generator, type_, number_of_variables):
         """Generates variable names for the SPARQL queries of the constraint."""
         vars_ = []
-        for elem in range(number_of_variables):
-            vars_.append(var_generator.generate_variable(type_))
+        if number_of_variables:
+            for elem in range(number_of_variables):
+                vars_.append(var_generator.generate_variable(type_))
 
         return vars_
 
     def get_variables(self):
         return self.variables
 
     def compute_rule_pattern_body(self):
```

### Comparing `TravSHACL-1.3.2/TravSHACL/constraints/MaxOnlyConstraint.py` & `TravSHACL-1.4.0/TravSHACL/constraints/MaxOnlyConstraint.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from TravSHACL.utils.VariableGenerator import VariableType
 from TravSHACL.constraints.Constraint import Constraint
 
 
 class MaxOnlyConstraint(Constraint):
     """This class represents max constraints, i.e., a constraint for the maximal occurrence of a path."""
 
-    def __init__(self, var_generator, id_, path, max_, is_pos, datatype=None, value=None, shape_ref=None, target_def=None):
+    def __init__(self, var_generator, id_, path, max_, is_pos, options, raw_or, datatype=None, value=None, shape_ref=None, target_def=None):
         """
         Creates a new max constraint.
 
         :param var_generator: variable generator instance
         :param id_: name of the constraint
         :param path: the path associated with this constraint, e.g., a predicate
         :param max_: the maximal occurrence allowed
         :param is_pos: true if it is a positive constraint, false otherwise
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         """
-        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path)
+        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, options, raw_or)
         self.varGenerator = var_generator
         self.min = -1
         self.max = max_
         self.variables = self.compute_variables()
 
     def compute_variables(self):
         """Computes variable names for the SPARQL queries of the constraint."""
```

### Comparing `TravSHACL-1.3.2/TravSHACL/constraints/MinMaxConstraint.py` & `TravSHACL-1.4.0/TravSHACL/constraints/MinMaxConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/constraints/MinOnlyConstraint.py` & `TravSHACL-1.4.0/TravSHACL/constraints/MinOnlyConstraint.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from TravSHACL.utils.VariableGenerator import VariableType
 from TravSHACL.constraints.Constraint import Constraint
 
 
 class MinOnlyConstraint(Constraint):
     """This class represents min constraints, i.e., a constraint for the minimal occurrence of a path."""
 
-    def __init__(self, var_generator, id_, path, min_, is_pos, datatype=None, value=None, shape_ref=None, target_def=None):
+    def __init__(self, var_generator, id_, path, min_, is_pos, options, raw_or, datatype=None, value=None, shape_ref=None, target_def=None):
         """
         Creates a new min constraint.
 
         :param var_generator: variable generator instance
         :param id_: name of the constraint
         :param path: the path associated with this constraint, e.g., a predicate
         :param min_: the minimal occurrence allowed
         :param is_pos: true if it is a positive constraint, false otherwise
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         """
-        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path)
+        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, options, raw_or)
         self.varGenerator = var_generator
         self.min = min_
         self.max = -1
         self.variables = self.compute_variables()
 
     def compute_variables(self):
         """Computes variable names for the SPARQL queries of the constraint."""
```

### Comparing `TravSHACL-1.3.2/TravSHACL/constraints/SPARQLConstraint.py` & `TravSHACL-1.4.0/TravSHACL/constraints/SPARQLConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/core/GraphTraversal.py` & `TravSHACL-1.4.0/TravSHACL/core/GraphTraversal.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/core/RulePattern.py` & `TravSHACL-1.4.0/TravSHACL/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/core/Shape.py` & `TravSHACL-1.4.0/TravSHACL/core/Shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,45 @@
 from TravSHACL.sparql.QueryGenerator import QueryGenerator
 
 
 class Shape:
     """This class represents a SHACL shape."""
 
     def __init__(self, id_, target_def, target_type, target_query, constraints, constraints_id, referenced_shapes,
-                 use_selective_queries, max_split_size, order_by_in_queries, include_sparql_prefixes, prefixes=None):
+                 use_selective_queries, max_split_size, order_by_in_queries, include_sparql_prefixes, flag,
+                 prefixes=None):
         """
         Creates a new Shape instance representing a SHACL shape that needs to be evaluated.
 
         :param id_: the name of the shape
         :param target_def: target definition of the shape
         :param target_type: indicates the target type of the shape, e.g., class or node
         :param target_query: target query of the shape
         :param constraints: the constraints belonging to the shape
         :param constraints_id: the constraint ids
         :param referenced_shapes: a list of shapes that is referenced from this shape
         :param use_selective_queries: indicates whether selective queries are used
         :param max_split_size: maximum number of instances per query
         :param order_by_in_queries: indicates whether to use the ORDER BY clause
         :param include_sparql_prefixes: indicates whether to include SPARQL prefixes in queries for the shape
+        :param flag: indicates if there is an 'or' operation to be executed
         """
         self.id = id_
         self.constraints = constraints
         self.constraintsId = constraints_id
         self.predicates = []
         self.targetDef = target_def
-        self.targetType = target_type          # Might be None
-        self.targetQuery = target_query        # Might be None
+        self.targetType = target_type  # Might be None
+        self.targetQuery = target_query  # Might be None
         self.targetQueryNoPref = target_query  # Might be None
         self.rulePattern = ()
         self.satisfied = None
         self.inDegree = None
         self.outDegree = None
+        self.flag = flag
 
         self.minQuery = None
         self.maxQueries = None
         self.predicates = []
         self.maxValidRefs = {}
         self.skippedQueriesIds = set()
 
@@ -120,29 +123,31 @@
             self.ORDERBYinQueries
         )
 
         self.queriesFilters = {}
         for ref in self.referencedShapes.keys():
             for c in self.constraints:
                 if c.path == self.referencedShapes[ref]:
-                    query_valid, query_invalid = self.QueryGenerator.generate_target_query('template_FILTER', [c], self.targetQueryNoPref, self.includePrefixes, self.ORDERBYinQueries)
+                    query_valid, query_invalid = self.QueryGenerator.generate_target_query('template_FILTER', [c],
+                                                                                           self.targetQueryNoPref,
+                                                                                           self.includePrefixes,
+                                                                                           self.ORDERBYinQueries)
                     ref_dict = {
                         'query_valid': query_valid,
                         'query_invalid': query_invalid,
                         'constraint': c
                     }
                     self.queriesFilters[ref] = ref_dict
 
     def compute_constraint_queries(self):
         """Computes all constraint queries for the shape."""
-        min_constraints = [c for c in self.constraints if c.min != -1]
+        min_constraints = [c for c in self.constraints if c.min != -1 and c.options is None]
         max_constraints = [c for c in self.constraints if c.max != -1]
 
         subquery = self.QueryGenerator.generate_local_subquery(min_constraints)
-
         # Build a unique set of triples (+ filter) for all min constraints
         min_id = self.constraintsId + '_pos'
         if len(min_constraints) > 0:
             self.minQuery = self.QueryGenerator.generate_query(
                 min_id,
                 [c for c in min_constraints if c.get_shape_ref() is not None],
                 self.useSelectiveQueries,
@@ -151,25 +156,25 @@
                 self.ORDERBYinQueries,
                 subquery
             )
 
         # Build one set of triples (+ filter) for each max constraint (only one max constraint per query is allowed)
         max_ids = [self.constraintsId + '_max_' + str(i) for i in range(1, len(max_constraints) + 1)]
         for i, max_c in enumerate(max_constraints):
-            self.maxConstrId[max_c] = self.constraintsId + '_max_' + str(i+1)
+            self.maxConstrId[max_c] = self.constraintsId + '_max_' + str(i + 1)
 
         i = itertools.count()
         self.maxQueries = [self.QueryGenerator.generate_query(
-                                max_ids[next(i)],
-                                [c],
-                                self.useSelectiveQueries,
-                                self.targetQueryNoPref,
-                                self.includePrefixes,
-                                self.ORDERBYinQueries,
-                                subquery) for c in max_constraints]
+            max_ids[next(i)],
+            [c],
+            self.useSelectiveQueries,
+            self.targetQueryNoPref,
+            self.includePrefixes,
+            self.ORDERBYinQueries,
+            subquery) for c in max_constraints]
 
         self.predicates = self.__compute_predicate_set(min_id, max_ids)
         self.__compute_max_queries_to_skip()
         self.__remove_unevaluated_max_queries()
         self.rulePattern = self.__compute_rule_pattern()
 
     def __compute_rule_pattern(self):
@@ -217,7 +222,13 @@
         self.maxQueries = list(filter(lambda q: q.get_id() not in self.skippedQueriesIds, self.maxQueries))
 
     def get_max_query_valid_refs(self):
         return self.maxValidRefs
 
     def get_prefix_string(self):
         return '\n'.join([''.join('PREFIX ' + key + ': ' + value) for (key, value) in self.prefixes.items()]) + '\n'
+
+    def get_or_query(self):
+        if True in self.flag:
+            return self.QueryGenerator.options_query(self.constraints, self.targetQuery, self.includePrefixes,
+                                                     self.ORDERBYinQueries)
+        return
```

### Comparing `TravSHACL-1.3.2/TravSHACL/core/ShapeParser.py` & `TravSHACL-1.4.0/TravSHACL/core/ShapeParser.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from TravSHACL.constraints.MinOnlyConstraint import MinOnlyConstraint
 
 QUERY_TARGET_QUERY = '''SELECT ?query WHERE {{
   <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> ;
       <http://www.w3.org/ns/shacl#targetQuery> ?query .
 }}'''
 
+
 class ShapeParser:
     """Used for parsing shape definitions from files to the internal representation."""
 
     def __init__(self):
         pass
 
     def parse_shapes_from_dir(self, path, shape_format, use_selective_queries, max_split_size, order_by_in_queries):
@@ -100,29 +101,31 @@
         constraints = self.parse_constraints(obj['constraintDef']['conjunctions'], target_def, id_)
 
         include_sparql_prefixes = self.abbreviated_syntax_used(constraints)
         prefixes = None
         if 'prefix' in obj.keys():
             prefixes = obj['prefix']
         referenced_shapes = self.shape_references(obj['constraintDef']['conjunctions'][0])
+        valid_flag = [False]   # for json files, the 'or' operations can be implemented starting from here
 
         if target_def is not None:
             target_query = target_def['query']
 
             target_def_copy = target_def.copy()
             del target_def_copy['query']
             target_type = list(target_def_copy.keys())[0]
 
             if urlparse(target_def[target_type]).netloc != '':  # if the target node is a url, add '<>' to it
                 target_def = '<' + target_def[target_type] + '>'
             else:
                 target_def = target_def[target_type]
 
         return Shape(name, target_def, target_type, target_query, constraints, id_, referenced_shapes,
-                     use_selective_queries, max_split_size, order_by_in_queries, include_sparql_prefixes, prefixes)
+                     use_selective_queries, max_split_size, order_by_in_queries, include_sparql_prefixes,
+                     valid_flag, prefixes)
 
     def parse_ttl(self, filename, use_selective_queries, max_split_size, order_by_in_queries):
         """
         Parses a particular file and converts its content into the internal representation of a SHACL shape.
 
         :param filename: the path to the shapes file
         :param use_selective_queries: indicates whether selective queries are used
@@ -161,19 +164,34 @@
                 for res in g_file.query(QUERY_TARGET_QUERY.format(shape=name)):
                     target_query = str(res[0])
                 if target_query is None:
                     target_query = 'SELECT ?x WHERE { ?x a <' + target_def + '> }'  # come up with a query for this
                     if urlparse(target_def).netloc != '':  # if the target node is a url, add '<>' to it
                         target_def = '<' + target_def + '>'
 
-            cons_dict = self.parse_all_const(g_file, name=name, target_def=target_def, target_type=target_type, query=queries)
-
+            cons_dict = self.parse_all_const(g_file, name=name, target_def=target_def, target_type=target_type,
+                                             query=queries)
             const_array = list(cons_dict.values())  # change the format to an array
-            constraints = self.parse_constraints_ttl(const_array, target_def, id_)
 
+            #valid_flag = [entry['flag'] for entry in const_array if entry['flag']]
+            valid_flag = []
+            for entry in const_array:
+                if 'flag' in entry.keys():
+                    valid_flag.append(entry['flag'])
+
+            if True in valid_flag:
+                var_generator = VariableGenerator()
+                valid_options = self.parse_or_constraint(var_generator, const_array, id_ + "_c",
+                                                         target_def)  # remember you removed +str(i + 1) in id_ used
+                valid_raw = self.extract_only_or(const_array)
+            else:
+                valid_options = None
+                valid_raw = None
+
+            constraints = self.parse_constraints_ttl(const_array, target_def, id_, valid_options, valid_raw)
             include_sparql_prefixes = self.abbreviated_syntax_used(constraints)
             prefixes = None
             referenced_shapes = self.shape_references(const_array)
 
             # helps to navigate the shape.__compute_target_queries function
             referenced_shape = {'<' + key + '>': '<' + referenced_shapes[key] + '>'
                                 for key in referenced_shapes.keys()
@@ -182,15 +200,16 @@
             # to helps to navigate the ShapeSchema.compute_edges function
             if urlparse(name).netloc != '':
                 name_ = '<' + name + '>'
             else:
                 name_ = name
 
             shapes.append(Shape(name_, target_def, target_type, target_query, constraints, id_, referenced_shape,
-                     use_selective_queries, max_split_size, order_by_in_queries, include_sparql_prefixes, prefixes))
+                                use_selective_queries, max_split_size, order_by_in_queries, include_sparql_prefixes,
+                                valid_flag, prefixes))
 
         return shapes
 
     @staticmethod
     def abbreviated_syntax_used(constraints):
         """
         Run after parsingConstraints.
@@ -247,16 +266,24 @@
         QUERY_CONSTRAINTS = '''SELECT ?constraint WHERE {{
           <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> .
           <{shape}> <http://www.w3.org/ns/shacl#property> ?constraint .
         }}
         '''
 
         QUERY_CONSTRAINT_DETAILS = '''SELECT ?p ?o WHERE {{
-          ?s ?p ?o .
-          FILTER( str(?s) = "{constraint}" )
+            {{
+                ?s ?p ?o .
+                FILTER( str(?s) = "{constraint}" )
+                FILTER( ?p != <http://www.w3.org/ns/shacl#path> || !isBlank(?o) )
+            }} UNION {{
+                ?s <http://www.w3.org/ns/shacl#path>/<http://www.w3.org/ns/shacl#inversePath> ?o .
+                BIND(<http://www.w3.org/ns/shacl#path> AS ?p)
+                BIND(CONCAT('^', str(?o)) AS ?o)
+                FILTER( str(?s) = "{constraint}" )
+            }}
         }}'''
 
         QUERY_QVS_REF_1 = '''SELECT ?shape_ref WHERE {{
               ?s <http://www.w3.org/ns/shacl#node> ?shape_ref .
               FILTER ( str(?s) = "{qvs}" )
             }}'''
 
@@ -267,46 +294,75 @@
 
         QUERY_SPARQL_CONSTRAINTS = '''SELECT ?constraint ?query WHERE {{
           <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> .
           <{shape}> <http://www.w3.org/ns/shacl#sparql> ?constraint .
           ?constraint <http://www.w3.org/ns/shacl#select> ?query .
         }}
         '''
-        return QUERY_SHAPES, QUERY_TARGET_1, QUERY_TARGET_2, QUERY_CONSTRAINTS, QUERY_CONSTRAINT_DETAILS, QUERY_QVS_REF_1, QUERY_QVS_REF_2, QUERY_SPARQL_CONSTRAINTS
+
+        QUERY_OR = '''SELECT ?constraint WHERE {{
+                                  <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> .
+                                  <{shape}> <http://www.w3.org/ns/shacl#or> ?constraint .
+                                }}
+                                '''
+        return QUERY_SHAPES, QUERY_TARGET_1, QUERY_TARGET_2, QUERY_CONSTRAINTS, QUERY_CONSTRAINT_DETAILS, \
+               QUERY_QVS_REF_1, QUERY_QVS_REF_2, QUERY_SPARQL_CONSTRAINTS, QUERY_OR
+
+    @staticmethod
+    def extract_only_or(or_constraint):
+        or_raw = []
+        for option in or_constraint:
+            keys = list(option['or'].keys())
+            grouping = []
+            for key in keys:
+                grouping.append(option['or'][key])
+            or_raw.append(grouping)
+        return or_raw
 
     def get_res(self, filename, name, query):
         """
 
         :param query: List of queries
         :param name: name of the Shape
         :param filename: shape file in ttl format
         :return: valid response from query execution
         """
         exp_dict = collections.defaultdict(list)
-        for constraint in filename.query(query[3].format(shape=name)):
-            constraint_id = constraint[0]
-
-            for detail in filename.query(query[4].format(constraint=constraint_id)):
-
-                if isinstance(detail.asdict()['o'], rdflib.term.BNode):
-                    qv_type = detail.asdict()['p']
-                    qvs = detail.asdict()['o']
-                    if len(filename.query(query[5].format(qvs=qvs))) != 0:
-                        for shape_ref in filename.query(query[5].format(qvs=qvs)):
-                            # dict_1 = [qv_type, ['shape', str(shape_ref.asdict()['shape_ref'])]]
-                            dict_1 = [qv_type, str(shape_ref.asdict()['shape_ref'])]
-                        exp_dict[str(constraint_id)].append(dict_1.copy())
+        if filename.query(query[3].format(shape=name)):
+            for constraint in filename.query(query[3].format(shape=name)):
+                constraint_id = constraint[0]
+
+                for detail in filename.query(query[4].format(constraint=constraint_id)):
+
+                    if isinstance(detail.asdict()['o'], rdflib.term.BNode):
+                        qv_type = detail.asdict()['p']
+                        qvs = detail.asdict()['o']
+                        if len(filename.query(query[5].format(qvs=qvs))) != 0:
+                            for shape_ref in filename.query(query[5].format(qvs=qvs)):
+                                # dict_1 = [qv_type, ['shape', str(shape_ref.asdict()['shape_ref'])]]
+                                dict_1 = [qv_type, str(shape_ref.asdict()['shape_ref'])]
+                            exp_dict[str(constraint_id)].append(dict_1.copy())
+                        else:
+                            for shape_ref in filename.query(query[6].format(qvs=qvs)):
+                                dict_1 = [qv_type, ['value', str(shape_ref.asdict()['shape_ref'])]]
+                            exp_dict[str(constraint_id)].append(dict_1.copy())
                     else:
-                        for shape_ref in filename.query(query[6].format(qvs=qvs)):
-                            dict_1 = [qv_type, ['value', str(shape_ref.asdict()['shape_ref'])]]
-                        exp_dict[str(constraint_id)].append(dict_1.copy())
-                else:
-                    #detail_dict = detail.asdict()
-                    dict_2 = [str(detail['p']), str(detail['o'])]
-                    exp_dict[str(constraint_id)].append(dict_2.copy())
+                        # detail_dict = detail.asdict()
+                        dict_2 = [str(detail['p']), str(detail['o'])]
+                        exp_dict[str(constraint_id)].append(dict_2.copy())
+
+        if filename.query(query[8].format(shape=name)):
+            for constraint in filename.query(query[8].format(shape=name)):
+                constraint_id = filename.items(constraint[0])
+                dict_or = collections.defaultdict(list)
+                for item in constraint_id:
+                    for detail in filename.query(query[4].format(constraint=item.toPython())):
+                        dict_3 = [str(detail['p']), str(detail['o'])]
+                        dict_or[str(item)].append(dict_3.copy())
+                exp_dict[str(constraint_id)].append(dict_or.copy())
 
         return exp_dict
 
     def parse_all_const(self, filename, name, target_def, target_type, query):
         """
 
         :param query: List of queries
@@ -336,114 +392,247 @@
                     trav_dict['min'] = None
                     trav_dict['max'] = None
                     trav_dict['value'] = None
                     trav_dict['path'] = None
                     trav_dict['shape'] = None
                     trav_dict['datatype'] = None
                     trav_dict['negated'] = None
+                    trav_dict['or'] = {}
+                    trav_dict['flag'] = False
 
-                    for i in dv:
-                        if 'path' in str(i[0]).lower():
-                            trav_dict['path'] = str(i[1])
-
-                        if 'min' in str(i[0]).lower():
-                            trav_dict['min'] = str(i[1])
-
-                        if 'max' in str(i[0]).lower():
-                            trav_dict['max'] = str(i[1])
-
-                        if 'datatype' in str(i[0]).lower():
-                            trav_dict['datatype'] = str(i[1])
-
-                        if 'valueshape' in str(i[0]).lower():
-                            trav_dict['shape'] = str(i[1])
-#                            if 'value' in str(i[1][0]).lower():
-#                                trav_dict['value'] = str(i[1][1])
-#                            if 'shape' in str(i[1][0]).lower():
-#                                trav_dict['shape'] = str(i[1][1])
+                    if "Graph.items" not in dk:
+                        for i in dv:
+                            if 'path' in str(i[0]).lower():
+                                trav_dict['path'] = str(i[1])
+
+                            if 'min' in str(i[0]).lower():
+                                trav_dict['min'] = str(i[1])
+
+                            if 'max' in str(i[0]).lower():
+                                trav_dict['max'] = str(i[1])
+
+                            if 'datatype' in str(i[0]).lower():
+                                trav_dict['datatype'] = str(i[1])
+
+                            if 'valueshape' in str(i[0]).lower():
+                                trav_dict['shape'] = str(i[1])
+                            #                            if 'value' in str(i[1][0]).lower():
+                            #                                trav_dict['value'] = str(i[1][1])
+                            #                            if 'shape' in str(i[1][0]).lower():
+                            #                                trav_dict['shape'] = str(i[1][1])
 
-                        if 'not' in str(i[0]).lower():
-                            trav_dict['negated'] = str(i[1])
+                            if 'not' in str(i[0]).lower():
+                                trav_dict['negated'] = str(i[1])
 
-                exp_dict[str(dk)] = trav_dict.copy()
+                    else:
+                        trav_dict['flag'] = True
+                        for options in dv:
+                            for i_or, j_or in options.items():
+                                trav_dict['or'][i_or] = {}
+                                for j_sub in j_or:
+                                    if 'path' in str(j_sub[0]).lower():
+                                        trav_dict['or'][i_or]['path'] = str(j_sub[1])
+                                    if 'max' in str(j_sub[0]).lower():
+                                        trav_dict['or'][i_or]['max'] = str(j_sub[1])
+                                        # trav_dict['max'] = str(sub_option[1])
+                                    if 'min' in str(j_sub[0]).lower():
+                                        trav_dict['or'][i_or]['min'] = str(j_sub[1])
 
+                exp_dict[str(dk)] = trav_dict.copy()
         return exp_dict
 
     def parse_constraints(self, array, target_def, constraints_id):
         """
         Parses all constraints of a shape.
 
         :param array: list of constraints belonging to the shape
         :param target_def: the target definition of the shape
         :param constraints_id: suffix for the constraint IDs
         :return: list of constraints in internal constraint representation
         """
         var_generator = VariableGenerator()
         constraints = []
-        [constraints.extend(self.parse_constraint(var_generator, array[0][i], constraints_id + '_c' + str(i + 1), target_def)) for i in range(len(array[0]))]
+        options = None
+        [constraints.extend(self.parse_constraint(var_generator, array[0][i], constraints_id + '_c' + str(i + 1),
+                                                  target_def, options)) for i in range(len(array[0]))]
         return constraints
 
-    def parse_constraints_ttl(self, array, target_def, constraints_id):
+    def parse_constraints_ttl(self, array, target_def, constraints_id, options, raw_or):
         """
         Parses all constraints of a shape.
 
         :param array: list of constraints belonging to the shape
         :param target_def: the target definition of the shape
         :param constraints_id: suffix for the constraint IDs
+        :param options: option to be used in or_operations
+        :param raw_or: raw form for 'or' query response
         :return: list of constraints in internal constraint representation
         """
         var_generator = VariableGenerator()
         constraints = []
-        [constraints.extend(self.parse_constraint(var_generator, array[i], constraints_id + '_c' + str(i + 1), target_def)) for i in range(len(array))]
+        if not options:
+            [constraints.extend(
+                self.parse_constraint(var_generator, array[i], constraints_id + '_c' + str(i + 1), target_def
+                                      )) for i in range(len(array))]
+        else:
+            [constraints.extend(
+                self.parse_constraint(var_generator, array[i], constraints_id + '_c' + str(i + 1), target_def,
+                                      options[i], raw_or[i])) for i in range(len(array))]
         return constraints
 
     @staticmethod
-    def parse_constraint(var_generator, obj, id_, target_def):
+    def parse_constraint(var_generator, obj, id_, target_def, options=None, raw_or=None):
         """
         Parses one constraint to the internal representation.
 
         :param var_generator: reference to the VariableGenerator instance for variable generation for SPARQL queries
         :param obj: the constraint in its original representation
         :param id_: suffix for the constraint ID
         :param target_def: the target definition of the associated shape
+        :param options: contains Constraints for or_operation
+        :param raw_or: contains only the raw form of the options for the 'or' operation
         :return: constraint in internal representation
         """
         min_ = obj.get('min')
         max_ = obj.get('max')
         shape_ref = obj.get('shape')
         datatype = obj.get('datatype')
         value = obj.get('value')
         path = obj.get('path')
         negated = obj.get('negated')
         query = obj.get('sparql')
 
+        if path is not None and str(path).startswith('^'):
+            is_inverse_path = True
+            path = str(path)[1:]
+        else:
+            is_inverse_path = False
+
         o_min = None if (min_ is None) else int(min_)
         o_max = None if (max_ is None) else int(max_)
         o_shape_ref = None if (shape_ref is None) else str(shape_ref)
         o_datatype = None if (datatype is None) else str(datatype)
         o_value = None if (value is None) else str(value)
         o_path = None if (path is None) else str(path)
         o_neg = True if (negated is None) else not negated  # True means it is a positive constraint
         o_query = None if (query is None) else str(query)
 
         if path is not None and urlparse(path).netloc != '':  # if the predicate is a url, add '<>' to it
             o_path = '<' + path + '>'
+        if is_inverse_path:
+            o_path = '^' + o_path
 
-        if urlparse(shape_ref).netloc != '' and shape_ref is not None:  # if the shape reference is a url, add '<>' to it
+        if urlparse(
+                shape_ref).netloc != '' and shape_ref is not None:  # if the shape reference is a url, add '<>' to it
             o_shape_ref = '<' + shape_ref + '>'
 
         if urlparse(value).netloc != '' and value is not None:  # if the value reference is a url, add '<>' to it
             o_value = '<' + value + '>'
 
         if urlparse(datatype).netloc != '' and datatype is not None:  # if the data type is a url, add '<>' to it
             o_datatype = '<' + datatype + '>'
 
         if o_path is not None:
             if o_min is not None:
                 if o_max is not None:
-                    #return MinMaxConstraint(var_generator, id_, o_path, o_min, o_max, o_neg, o_datatype, o_value, o_shape_ref, target_def)
-                    return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, o_datatype, o_value, o_shape_ref, target_def), MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, o_datatype, o_value, o_shape_ref, target_def)]
-                return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, o_datatype, o_value, o_shape_ref, target_def)]
+                    # return MinMaxConstraint(var_generator, id_, o_path, o_min, o_max, o_neg, o_datatype, o_value, o_shape_ref, target_def)
+                    return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype,
+                                              o_value, o_shape_ref, target_def),
+                            MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype,
+                                              o_value, o_shape_ref, target_def)]
+                return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype,
+                                          o_value, o_shape_ref, target_def)]
             if o_max is not None:
-                return [MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, o_datatype, o_value, o_shape_ref, target_def)]
+                return [MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype,
+                                          o_value, o_shape_ref, target_def)]
         elif o_query is not None:
             return [SPARQLConstraint(id_, o_neg, o_query)]
+        elif o_path is None:
+            return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value,
+                                      o_shape_ref, target_def)]
+
+    @staticmethod
+    def parse_or_constraint(var_generator, objs, id_, target_def):
+        """
+        Parses one constraint to the internal representation.
+
+        :param var_generator: reference to the VariableGenerator instance for variable generation for SPARQL queries
+        :param objs: the constraint in its original representation
+        :param id_: suffix for the constraint ID
+        :param target_def: the target definition of the associated shape
+        :return: constraint in internal representation
+        """
+        constraint_list = []
+        options = None
+        raw_or = None
+        for obj in objs:
+            shape_ref = obj.get("shape")
+            datatype = obj.get("datatype")
+            value = obj.get("value")
+            negated = obj.get("negated")
+            query = obj.get('sparql')
+
+            keys = list(obj['or'].keys())
+            or_constraints = []
+            for key in keys:
+                min_ = None
+                max_ = None
+                path = None
+                for key_, value_ in obj['or'][key].items():
+                    if key_ == 'path':
+                        path = value_
+                    if key_ == 'max':
+                        max_ = value_
+                    if key_ == 'min':
+                        min_ = value_
+
+                o_min = None if (min_ is None) else int(min_)
+                o_max = None if (max_ is None) else int(max_)
+                o_shape_ref = None if (shape_ref is None) else str(shape_ref)
+                o_datatype = None if (datatype is None) else str(datatype)
+                o_value = None if (value is None) else str(value)
+                o_path = None if (path is None) else str(path)
+                o_neg = True if (negated is None) else not negated
+                o_query = None if (query is None) else str(query)           # not used in this implementation
+
+                if path is not None and str(path).startswith('^'):
+                    is_inverse_path = True
+                    path = str(path)[1:]
+                else:
+                    is_inverse_path = False
+
+                if urlparse(path).netloc != '':  # if the predicate is a url, add '<>' to it
+                    o_path = '<' + path + '>'
+                if is_inverse_path:
+                    o_path = '^' + o_path
+
+                if urlparse(
+                        shape_ref).netloc != '' and shape_ref is not None:  # if shape reference is a url, add '<>' to it
+                    o_shape_ref = '<' + shape_ref + '>'
+
+                if urlparse(
+                        value).netloc != '' and value is not None:  # if the value reference is a url, add '<>' to it
+                    o_value = '<' + value + '>'
+
+                if urlparse(
+                        datatype).netloc != '' and datatype is not None:  # if the data type is a url, add '<>' to it
+                    o_datatype = '<' + datatype + '>'
+
+                if o_path is not None:
+                    if o_min is not None:
+                        if o_max is not None:
+                            constraint = [
+                                MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype,
+                                                  o_value, o_shape_ref, target_def),
+                                MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype,
+                                                  o_value, o_shape_ref, target_def)]
+                        else:
+                            constraint = MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or,
+                                                           o_datatype, o_value, o_shape_ref, target_def)
+                    else:
+                        if o_max is not None:
+                            constraint = MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options,  raw_or,
+                                                           o_datatype, o_value, o_shape_ref, target_def)
+
+                    or_constraints.append(constraint)
+            constraint_list.append(or_constraints.copy() if or_constraints else None)
+        return constraint_list
```

### Comparing `TravSHACL-1.3.2/TravSHACL/core/ShapeSchema.py` & `TravSHACL-1.4.0/TravSHACL/core/ShapeSchema.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/rule_based_validation/InstancesRetrieval.py` & `TravSHACL-1.4.0/TravSHACL/rule_based_validation/InstancesRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,36 @@
 
         self.stats.update_log('\nelapsed: ' + str(end - start) + ' ms\n')
         self.stats.record_query_exec_time(end - start)
         self.stats.record_query()
         self.stats.update_log('\nNumber of targets retrieved: ' + str(len(bindings)))
         return {(shape.id, b['x']['value'], True) for b in bindings}
 
+    def extract_options(self, shape):
+        """
+        Retrieves answers from the SPARQL endpoint.
+        When a network of shapes has only 'some' targets, a shape without a target class returns no new bindings
+
+        :param shape: focus shape being evaluated
+        :return: set containing target literals (stored in the form of built-in python tuples)
+        """
+        query = shape.get_or_query()  # or_query is formed in the shape class
+        if not query:
+            return
+        self.stats.update_log(''.join(['\nEvaluating OR_options query for ', shape.id, ':\n', query]))
+        start = time.time() * 1000.0
+        bindings = self.endpoint.run_query(query)['results']['bindings']
+        end = time.time() * 1000.0
+
+        self.stats.update_log('\nelapsed: ' + str(end - start) + ' ms\n')
+        self.stats.record_query_exec_time(end - start)
+        self.stats.record_query()
+        self.stats.update_log('\nNumber of options retrieved: ' + str(len(bindings)))
+        return {(shape.id, b['x']['value'], True) for b in bindings}
+
     def extract_targets_with_filter(self, shape, filtering_shape):
         """
         Retrieves more selective query answers by separating early invalidated targets from the still pending ones.
 
         :param shape: focus shape being evaluated
         :param filtering_shape: referenced shape used to filter query, or None
         :return: two sets containing all targets of 'shape': pending targets to validate and directly invalidated targets
```

### Comparing `TravSHACL-1.3.2/TravSHACL/rule_based_validation/Validation.py` & `TravSHACL-1.4.0/TravSHACL/rule_based_validation/Validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,28 @@
             for target in invalid:
                 self.register_target(target, 'violated', next_focus_shape_name, shapes_state)
                 shapes_state[next_focus_shape_name]['inferred'].add((target[0], target[1], not target[2]))
                 shapes_state[next_focus_shape_name]['remaining_targets_count'] -= 1
         else:
             pending = self.InstRetrieval.extract_targets(next_focus_shape)
 
+        # checking for 'or' constraint
+        if next_focus_shape.flag:
+            invalid_pending = []
+            pending_val = self.InstRetrieval.extract_options(next_focus_shape)
+            for target in pending:
+                if pending_val:
+                    if target not in pending_val:
+                        invalid_pending.append(target)
+                        self.register_target(target, "violated", next_focus_shape_name, shapes_state)
+                        shapes_state[next_focus_shape_name]['inferred'].add((target[0], target[1], not target[2]))
+                        shapes_state[next_focus_shape_name]['remaining_targets_count'] -= 1
+
+            pending = [target for target in pending if target not in invalid_pending]
+
         # check the SPARQL constraints
         sparql_constraints = next_focus_shape.get_sparql_constraints()
         if len(sparql_constraints) > 0:
             for constraint in sparql_constraints:
                 violations = self.InstRetrieval.execute_sparql_constraint(
                     constraint_id=constraint.id,
                     query_str=constraint.query,
@@ -264,15 +278,14 @@
         query_rp_head = q_rule_pattern.head
         query_rp_body = q_rule_pattern.body
         shape_rp_head = s_rule_pattern.head
         shape_rp_body = s_rule_pattern.body
 
         q_body_ref_shapes = [preds_to_shapes[pattern[0]] for pattern in query_rp_body]
         s_body_ref_shapes = [preds_to_shapes[pattern[0]] for pattern in shape_rp_body]
-
         shape_max_refs = shape.get_max_query_valid_refs()
         inter_constr_count = {}
         new_rules_count = 0
         rules_directly_inferred = 0
 
         for query_str in self.InstRetrieval.rewrite_constraint_query(shape, q, filtering_shape, q_type, self.selectivity_enabled):
             start = time.time() * 1000.0
@@ -602,20 +615,18 @@
                     if i != 0:
                         output_ttl += ' ,'
                     output_ttl += '\n    [ a  sh:ValidationResult ;\n' +\
                                   '      sh:resultSeverity  sh:Violation ;\n' +\
                                   '      sh:focusNode  <' + violation[1] + '> ;\n' +\
                                   '      sh:sourceShape  ' + violation[0] + ' ]'
 
-            output_ttl = '@prefix sh: <http://www.w3.org/ns/shacl#> . \n\n' + output_ttl + ' .'
-
+            output_ttl = '@prefix sh: <http://www.w3.org/ns/shacl#> . \n\n' + output_ttl + ' .'            
             validation_report = fileManagement.open_file(self.output_dir_name, 'validationReport.ttl')
             validation_report.write(output_ttl)
             fileManagement.close_file(validation_report)
-
         return output
 
 
 class ValidationState:
     """This class is responsible for keeping track of the validation state."""
 
     def __init__(self, shapes_dict):
```

### Comparing `TravSHACL-1.3.2/TravSHACL/sparql/QueryGenerator.py` & `TravSHACL-1.4.0/TravSHACL/sparql/QueryGenerator.py`

 * *Files 22% similar despite different names*

```diff
@@ -128,14 +128,57 @@
             '    ?' + focus_var + ' ' + ref_path + ' ?inst .\n  }\n',
             '}\nGROUP BY ?' + focus_var, '\nORDER BY ?' + focus_var if include_order_by else ''
         ])
         return Query(None, None, query)
 
     # CONSTRAINT QUERIES #
 
+    def options_query(self, constraint, target_query, include_prefixes, include_order_by):
+        """
+        Generates a target query including a VALUES clause to filter based on valid instances.
+
+        :param constraint: constraint that refers to this target query
+        :param target_query: target query string parsed from the input file
+        :param include_prefixes: indicates whether or not prefixes should be included in the query
+        :param include_order_by: indicates whether or not the ORDER BY clause will be added
+        :return: target query with VALUES clause
+        """
+        prefixes = self.shape.get_prefix_string() if include_prefixes else ''
+        focus_var = VariableGenerator.get_focus_node_var()
+        target_node = get_target_node_statement(target_query)
+        query_top = ''.join([prefixes, " SELECT DISTINCT ?" + focus_var + " WHERE {\n"])
+        query_down = " ORDER BY ?" + focus_var if include_order_by else ''
+        or_union = self.get_or_query(constraint, target_node)
+        return query_top + or_union + '}' + query_down
+
+    @staticmethod
+    def get_or_query(constraints_, target_node_statement):
+        """
+        used to generate and combine triples required for 'or' operations
+
+        :param constraints_: constraint to be evaluated as 'or'
+        :param target_node_statement: statement for the target node
+        :return: a set of unions that can be used in a query for initial validation
+        """
+        or_constraints = [c for c in constraints_ if c.get_shape_ref() is None]  # unsure validity with 'get_shape_ref'
+
+        builder = QueryBuilder('tmp', None, VariableGenerator.get_focus_node_var(), False)
+        or_value = 1  # used for differentiating between the constraints of different options of each or_operation
+        for c in or_constraints:
+            if c.options:
+                or_affix = 1   # not in use yet but can be used if there are more than one constraint in an or_option
+                for option in c.options:
+                    if isinstance(option, MaxOnlyConstraint):
+                        builder.build_clause(option, or_value, or_affix, True)
+                    else:
+                        builder.build_clause(option, or_value, or_affix, False)
+                    or_affix += 1
+                or_value += 1
+        return builder.build_union(target_node_statement, VariableGenerator.get_focus_node_var())
+
     def generate_query(self, id_, constraints, is_selective, target_query,
                        include_prefixes, include_order_by, subquery=None):
         """
         Generates a constraint query.
 
         :param id_: internal query/constraint name
         :param constraints: a list of constraints that refer to this constraint query
@@ -184,15 +227,14 @@
         if len(local_pos_constraints) == 0:
             return None  # optional empty
 
         builder = QueryBuilder('tmp', None, VariableGenerator.get_focus_node_var(), False)
 
         for c in local_pos_constraints:
             builder.build_clause(c)
-
         return builder.get_sparql(False, True)
 
 
 class QueryBuilder:
     """This class is responsible for actually building SPARQL queries for constraints."""
 
     def __init__(self, id_, subquery, projected_variables, is_selective, target_query=None,
@@ -210,14 +252,17 @@
         :param prefix_string: prefix string for the queries being built
         """
         self.id = id_
         self.subquery = subquery
         self.projected_variables = projected_variables
         self.filters = []
         self.triples = []
+        self.union_triples = []
+        self.max_dict = {}
+        self.or_triples = []
 
         self.include_selectivity = is_selective
         self.target_query = target_query
         self.constraints = constraints
         self.include_ORDERBY = include_order_by
         self.inter_shape_refs = {}
         self.prefix_string = prefix_string
@@ -228,14 +273,115 @@
         No subject is needed as in a constraint query all triple patterns share the same subject.
 
         :param path: predicate of the triple pattern
         :param obj: object of the triple pattern
         """
         self.triples.append('?' + VariableGenerator.get_focus_node_var() + ' ' + path + ' ' + obj + '.')
 
+    def add_union_triples(self, path, obj, val_1, val_2, maxonly: bool = False, card: int = -1):
+        """
+        Adds a triple pattern to the constraint query.
+        No subject is needed as in a constraint query all triple patterns share the same subject.
+
+        :param path: predicate of the triple pattern
+        :param obj: object of the triple pattern
+        :param val_1: for union grouping(general)
+        :param val_2: for local union grouping
+        :param maxonly: tells if the constraint is maxonly
+        :param card: cardinality restriction of the constraint to be added
+        """
+        if maxonly:
+            self.union_triples.append(str(val_1) + '#' + str(val_2) + '#max#' + str(card) + '#?' +
+                                      VariableGenerator.get_focus_node_var() + ' ' + path + ' ' + obj + '.')
+        else:
+            self.union_triples.append(str(val_1) + '#' + str(val_2) + '#min#' + str(card) + '#?' +
+                                      VariableGenerator.get_focus_node_var() + ' ' + path + ' ' + obj + '.')
+
+    def union_with_filters(self, union_list):
+        union_list_to_keep = []
+        for filter_ in self.filters:
+            filter_union = []
+            for entry in union_list:
+                if entry.rsplit(' ', 1)[1].split('.')[0] in filter_:
+                    filter_union.append(entry)
+                else:
+                    union_list_to_keep.append(entry)
+            if filter_union:
+                union_list_to_keep.append('{' + self.__get_projection_string() + ' WHERE {\n' + '\n'.join(filter_union)
+                                          + '\nFILTER( \n' + filter_ + ') \n }}')
+        return union_list_to_keep
+
+    def build_union(self, target_node_statement: str, focus_node_var: str):
+        """
+        Builds a union pattern
+        No subject is needed as in a constraint query all triple patterns share the same subject.
+
+        """
+        if self.union_triples is []:
+            return
+        else:
+            grouping = []
+            for entry in self.union_triples:
+                group_number = entry.split('#', 3)[0]
+                if group_number not in grouping:
+                    grouping.append(group_number)
+
+            for group in grouping:
+                current_group = []
+                for entry in self.union_triples:
+                    if entry.split('#', 3)[0] == group:
+                        if entry.split('#', 3)[2] == 'min':
+                            current_group.append(self.cardinality_graph_pattern(target_node_statement, focus_node_var,
+                                                           entry.split('#', 4)[4], False, entry.split('#', 4)[3]))
+                        if entry.split('#', 3)[2] == 'max':
+                            current_group.append(self.cardinality_graph_pattern(target_node_statement, focus_node_var,
+                                                           entry.split('#', 4)[4], True, entry.split('#', 4)[3]))
+                        # self.triples.remove(entry.split('#', 2)[2])
+                    # entry.split('#', 2)[1] can be used for grouping if there are more than just the path constraint
+                # print(current_group)
+                if len(self.filters) > 0:
+                    current_group = self.union_with_filters(current_group)
+
+                self.triples.append(self.union_group(current_group))
+        return '\n'.join(self.triples)
+
+    @staticmethod
+    def cardinality_graph_pattern(target_node_statement: str, focus_node_var: str,
+                                  triple_pattern: str, max_: bool, card: int):
+        """
+        Creates a subquery for cardinality constraints to be used in OR constraints.
+
+        :param target_node_statement: The statement for the target node of the constraint
+        :param focus_node_var: The variable for the focus node (usually x)
+        :param triple_pattern: The triple pattern of the cardinality constraint
+        :param max_: Indicates whether the constraint is a max cardinality constraint
+        :param card: The cardinality restriction of the constraint
+        """
+        cgp = '{ SELECT DISTINCT ?' + focus_node_var + ' WHERE {\n' + target_node_statement + ' .\n'
+        if max_:
+            cgp += 'OPTIONAL { ' + triple_pattern + '}'
+        else:
+            cgp += triple_pattern
+        cgp += '\n}\nGROUP BY ?' + focus_node_var + '\nHAVING (COUNT(DISTINCT ?' + triple_pattern.split('?', 2)[2][:-1] + ') '
+        if max_:
+            cgp += '<= '
+        else:
+            cgp += '>= '
+        cgp += str(card) + ') }'
+        return cgp
+
+    @staticmethod
+    def union_group(triples_to_join):
+        """
+        Add a filter based on a datatype.
+
+        :param triples_to_join: list containing triples that should observe unions
+        """
+        return '\n UNION \n'.join(triples_to_join)
+
     def add_datatype_filter(self, variable, datatype, is_pos):
         """
         Add a filter based on a datatype.
 
         :param variable: the variable the filter should be added for
         :param datatype: the expected datatype
         :param is_pos: indicated whether this is a positive constraint
@@ -262,48 +408,54 @@
         :param is_subquery: indicates whether the query is considered to be a sub-query
         :return: the SPARQL query as a string
         """
         if is_subquery:
             return self.__get_query(False)  # create subquery
 
         prefixes = self.prefix_string if include_prefixes else ''
+        if isinstance(self.subquery, str):
+            if self.subquery == '':
+                self.subquery = None
         outer_query_closing_braces = ''.join(['}\n' if self.subquery is not None else '',
                                               '}' if self.get_triple_patterns() != '' and self.subquery is not None else '',
                                               '}' if self.get_triple_patterns() != '' else ''])
+
         selective_closing_braces = '}}' if self.include_selectivity and self.target_query is not None else ''
 
-        if len(self.constraints) == 1 and isinstance(self.constraints[0], MaxOnlyConstraint) and self.constraints[0].get_shape_ref() is None:
+        if len(self.constraints) == 1 and isinstance(self.constraints[0], MaxOnlyConstraint) and self.constraints[
+            0].get_shape_ref() is None:
             target_node = ''
             if self.include_selectivity and self.target_query is not None:
                 target_node = get_target_node_statement(self.target_query) + '.\n'
 
             if self.constraints[0].get_value() is not None:
                 pred = self.constraints[0].path
                 obj = self.constraints[0].get_value()
                 return ''.join([prefixes,
                                 self.__get_projection_string(),
                                 ' WHERE {\n', target_node,
                                 '?', VariableGenerator.get_focus_node_var(), ' ', pred, ' ', obj, '.\n}',
                                 ' ORDER BY ?' + VariableGenerator.get_focus_node_var() if self.include_ORDERBY else ''])
             else:
-                return ''.join([prefixes,
-                                self.__get_projection_string(),
-                                ' WHERE {\n', target_node,
-                                self.triples[0], '\n} GROUP BY ?',
-                                VariableGenerator.get_focus_node_var(),
-                                ' HAVING (COUNT(DISTINCT ?', self.triples[0].rsplit('?', 1)[1][:-1], ') >= ', str(self.constraints[0].max + 1), ')',
-                                ' ORDER BY ?' + VariableGenerator.get_focus_node_var() if self.include_ORDERBY else ''])
-
+                if self.triples:
+                    return ''.join([prefixes,
+                                    self.__get_projection_string(),
+                                    ' WHERE {\n', target_node,
+                                    self.triples[0], '\n} GROUP BY ?',
+                                    VariableGenerator.get_focus_node_var(),
+                                    ' HAVING (COUNT(DISTINCT ?', self.triples[0].rsplit('?', 1)[1][:-1], ') >= ',
+                                    str(self.constraints[0].max + 1), ')',
+                                    ' ORDER BY ?' + VariableGenerator.get_focus_node_var() if self.include_ORDERBY else ''])
         query = ''.join([prefixes,
-                        self.__get_selective(),
-                        self.__get_query(include_prefixes),
-                        self.subquery if self.subquery is not None else '',
-                        outer_query_closing_braces,
-                        selective_closing_braces,
-                        ' ORDER BY ?' + VariableGenerator.get_focus_node_var() if self.include_ORDERBY else ''])
+                         self.__get_selective(),
+                         self.__get_query(include_prefixes),
+                         self.subquery if self.subquery is not None else '',
+                         outer_query_closing_braces,
+                         selective_closing_braces,
+                         ' ORDER BY ?' + VariableGenerator.get_focus_node_var() if self.include_ORDERBY else ''])
         return query
 
     def __get_query(self, include_prefixes):
         """
         Internal method of the QueryBuilder to generate the SPARQL query string.
 
         :param include_prefixes: indicates whether prefixes should be included in the query
@@ -312,14 +464,17 @@
         temp_string = ''
         if include_prefixes:
             if '_pos' in self.id or '_max_' in self.id:
                 # add VALUES clause to external query
                 temp_string = '$filter_clause_to_add$'
 
         triple_patterns = self.get_triple_patterns()
+        if isinstance(self.subquery, str):
+            if self.subquery == '':
+                self.subquery = None
         if triple_patterns != '':
             return ''.join([self.__get_projection_string(),
                             ' WHERE {\n',
                             temp_string,
                             triple_patterns,
                             '\n', '{\n' if self.subquery is not None else ''])
         else:
@@ -376,49 +531,66 @@
 
         :param variables: list of variables to add cardinality filters for
         """
         for i in range(0, len(variables)):
             for j in range(i + 1, len(variables)):
                 self.filters.append('?' + variables[i] + ' != ?' + variables[j])
 
-    def build_clause(self, c):
+    def build_clause(self, c, or_value: int = 0, or_affix: int = 0, maxonly: bool = False):
         """
         Adds the necessary information to the QueryBuilder for a given constraint.
 
         :param c: the constraint to be included in the query
+        :param or_value: used in the case of multiple 'or' for triple grouping
+        :param or_affix: used in the case of more than one or triple within an option in an 'or' operation
+        :param maxonly: tells if the constraint is maxonly
         """
         variables = c.get_variables()
+        if c.raw_or:            # the use of raw_or is highly debatable. Only important with or_constraint within property in shapes_graph
+            self.or_triples = ['<' + entry['path'] + '>' for entry in c.raw_or]
+        if not maxonly:
+            if isinstance(c, Constraint):
+                path = c.path
+                if path not in self.or_triples:
+                    if c.get_value() is not None:  # if there is fixed value for the object
+                        if or_value > 0:
+                            self.add_union_triples(path, c.get_value(), or_value, or_affix)
+                        else:
+                            self.add_triple(path, c.get_value())
+                        return
+
+                    if or_value > 0:
+                        v = variables[0]
+                        self.add_union_triples(path, '?' + v, or_value, or_affix, card=c.min)
+                    else:
+                        for v in variables:
+                            if c.get_shape_ref() is not None:  # if there is an existing reference to another shape
+                                self.inter_shape_refs[v] = c.get_shape_ref()
+                                self.triples.append('\n$inter_shape_type_to_add$')
+                            self.add_triple(path, '?' + v)
+
+            if c.get_value() is not None:
+                self.add_constant_filter(
+                    variables.iterator().next(),
+                    c.get_value().get(),
+                    c.get_is_pos()
+                )
+
+            if c.get_datatype() is not None:
+                for v in variables:
+                    self.add_datatype_filter(v, c.get_datatype(), c.get_is_pos())
 
-        if isinstance(c, Constraint):
-            path = c.path
+            if len(variables) > 1 and or_value == 0:
+                self.add_cardinality_filter(variables)
 
-            if c.get_value() is not None:  # if there is fixed value for the object
-                self.add_triple(path, c.get_value())
-                return
-
-            for v in variables:
-                if c.get_shape_ref() is not None:  # if there is an existing reference to another shape
-                    self.inter_shape_refs[v] = c.get_shape_ref()
-                    self.triples.append('\n$inter_shape_type_to_add$')
-
-                self.add_triple(path, '?' + v)
-
-        if c.get_value() is not None:
-            self.add_constant_filter(
-                variables.iterator().next(),
-                c.get_value().get(),
-                c.get_is_pos()
-            )
-
-        if c.get_datatype() is not None:
-            for v in variables:
-                self.add_datatype_filter(v, c.get_datatype(), c.get_is_pos())
-
-        if len(variables) > 1:
-            self.add_cardinality_filter(variables)
+        else:
+            if isinstance(c, Constraint):
+                path = c.path
+                v = variables[0]        # this limits the use of max_constraints
+                self.add_union_triples(path, '?' + v, or_value, or_affix, True, card=c.max)
 
     def build_query(self, rule_pattern, include_prefixes):
         """
         Generate a Query object based on the current state of the QueryBuilder.
 
         :param rule_pattern: the query rule pattern associated with the query
         :param include_prefixes: indicates whether prefixes should be included in the query
```

### Comparing `TravSHACL-1.3.2/TravSHACL/sparql/SPARQLEndpoint.py` & `TravSHACL-1.4.0/TravSHACL/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/utils/ValidationStats.py` & `TravSHACL-1.4.0/TravSHACL/utils/ValidationStats.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/utils/VariableGenerator.py` & `TravSHACL-1.4.0/TravSHACL/utils/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL/utils/fileManagement.py` & `TravSHACL-1.4.0/TravSHACL/utils/fileManagement.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/TravSHACL.egg-info/PKG-INFO` & `TravSHACL-1.4.0/TravSHACL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.3.2
+Version: 1.4.0
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.3.2.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.0.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/SDM-TIB/Trav-SHACL/actions/workflows/test.yml/badge.svg)](https://github.com/SDM-TIB/Trav-SHACL/actions/workflows/test.yml)
 [![Latest Release](http://img.shields.io/github/release/SDM-TIB/Trav-SHACL.svg?logo=github)](https://github.com/SDM-TIB/Trav-SHACL/releases)
 [![Docker Image](https://img.shields.io/badge/Docker%20Image-sdmtib/travshacl-blue?logo=Docker)](https://hub.docker.com/r/sdmtib/travshacl)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
```

### Comparing `TravSHACL-1.3.2/TravSHACL.egg-info/SOURCES.txt` & `TravSHACL-1.4.0/TravSHACL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.2/setup.py` & `TravSHACL-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     author='Mónica Figuera, Philipp D. Rohde',
     author_email='philipp.rohde@tib.eu',
     url='https://github.com/SDM-TIB/Trav-SHACL',
     download_url='https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v' + version + '.tar.gz',
     description='A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['SPARQLWrapper==2.0.0', 'rdflib>=6.1.1'],
-    python_requires='>=3.7',
+    install_requires=['SPARQLWrapper>=2.0.0', 'rdflib>=6.1.1'],
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 5 - Production/Stable ',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research'
       ]
 )
```

### Comparing `TravSHACL-1.3.2/tests/test_cases.py` & `TravSHACL-1.4.0/tests/test_cases.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 @pytest.mark.parametrize('graph_traversal', ['DFS', 'BFS'])
 @pytest.mark.parametrize('selective', [True, False])
 @pytest.mark.parametrize('shape_format', ['JSON', 'SHACL'])
 @pytest.mark.parametrize('endpoint', [TEST_ENDPOINT, TEST_GRAPH])
 def test_case(file, selective, graph_traversal, prio_target, prio_degree, prio_number, shape_format, endpoint):
     if 'sparql' in file and shape_format == 'JSON':
         pytest.skip('SPARQL constraints in JSON format are not implemented.')
+    if 'or_constraint' in file and shape_format == 'JSON':
+        pytest.skip('OR constraints in JSON format are not implemented.')
 
     with open(file, 'r') as f:
         test_definition = json.load(f)
 
     schema_dir = test_definition['schemaDir']
     gt_valid = sorted(test_definition['groundTruth']['valid'])
     gt_invalid = sorted(test_definition['groundTruth']['invalid'])
```

