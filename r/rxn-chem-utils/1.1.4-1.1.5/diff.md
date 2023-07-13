# Comparing `tmp/rxn-chem-utils-1.1.4.tar.gz` & `tmp/rxn-chem-utils-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-chem-utils-1.1.4.tar", last modified: Fri Feb 10 14:49:29 2023, max compression
+gzip compressed data, was "rxn-chem-utils-1.1.5.tar", last modified: Thu Jul 13 15:21:36 2023, max compression
```

## Comparing `rxn-chem-utils-1.1.4.tar` & `rxn-chem-utils-1.1.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.908933 rxn-chem-utils-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-10 14:49:29.908933 rxn-chem-utils-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-10 14:49:29.908933 rxn-chem-utils-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.904933 rxn-chem-utils-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.900933 rxn-chem-utils-1.1.4/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.904933 rxn-chem-utils-1.1.4/src/rxn/chemutils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/extended_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/multicomponent_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/reaction_combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/reaction_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/reaction_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.904933 rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/combine_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/smiles_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/smiles_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/src/rxn/chemutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.908933 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-10 14:49:29.000000 rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:49:29.908933 rxn-chem-utils-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_extended_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_multicomponent_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_reaction_combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_reaction_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_smiles_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_smiles_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-10 14:49:20.000000 rxn-chem-utils-1.1.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.366419 rxn-chem-utils-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.366419 rxn-chem-utils-1.1.5/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.370420 rxn-chem-utils-1.1.5/src/rxn/chemutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/extended_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/multicomponent_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.370420 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/combine_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_extended_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_multicomponent_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_reaction_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_reaction_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_smiles_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_smiles_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_utils.py
```

### Comparing `rxn-chem-utils-1.1.4/LICENSE` & `rxn-chem-utils-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/PKG-INFO` & `rxn-chem-utils-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-chem-utils
-Version: 1.1.4
+Version: 1.1.5
 Summary: Chemistry-related utilities
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `rxn-chem-utils-1.1.4/README.md` & `rxn-chem-utils-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/setup.cfg` & `rxn-chem-utils-1.1.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	= src
 packages = find_namespace:
 python_requires = >= 3.6
 zip_safe = False
 include_package_data = True
 install_requires = 
 	attrs>=21.2.0
-	click>=7.0
+	click>=7.0,<8.1.4
 	rxn-utils>=1.1.9
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 rxn.chemutils =
```

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/conversion.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/conversion.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/exceptions.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/extended_reaction_smiles.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/extended_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/miscellaneous.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/multicomponent_smiles.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/multicomponent_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/reaction_combiner.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_combiner.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/reaction_equation.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_equation.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/reaction_smiles.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/canonicalize.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/canonicalize.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,25 @@
     "--invalid_placeholder",
     type=str,
     help=(
         "If specified, the given value will be the output for invalid input SMILES. "
         "By default, an exception is raised in such cases."
     ),
 )
+@click.option(
+    "--sort_compounds",
+    "-s",
+    is_flag=True,
+    help="If specified, the compounds will be sorted after canonicalization.",
+)
 def main(
-    input_file: TextIO, output_file: TextIO, invalid_placeholder: Optional[str]
+    input_file: TextIO,
+    output_file: TextIO,
+    invalid_placeholder: Optional[str],
+    sort_compounds: bool,
 ) -> None:
     """
     Canonicalize SMILES strings (molecules, sets of molecules, or reactions).
 
     The script will read strings either from stdin, or from a file given as the
     first argument, and write to stdout, or from a file given as the second
     argument.
@@ -31,15 +40,15 @@
     setup_console_logger()
 
     for line in input_file:
         smiles = line.strip()
 
         # Canonicalize the SMILES, handle exception if needed
         try:
-            canonical = canonicalize_any(smiles)
+            canonical = canonicalize_any(smiles, sort_molecules=sort_compounds)
         except Exception:
             if invalid_placeholder is None:
                 raise
             canonical = invalid_placeholder
 
         output_file.write(f"{canonical}\n")
```

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/combine_reaction.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/combine_reaction.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/detokenize.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/detokenize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/scripts/tokenize.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/tokenize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/smiles_augmenter.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/smiles_randomization.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_randomization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/tokenization.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/tokenization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn/chemutils/utils.py` & `rxn-chem-utils-1.1.5/src/rxn/chemutils/utils.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/PKG-INFO` & `rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-chem-utils
-Version: 1.1.4
+Version: 1.1.5
 Summary: Chemistry-related utilities
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `rxn-chem-utils-1.1.4/src/rxn_chem_utils.egg-info/SOURCES.txt` & `rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_conversion.py` & `rxn-chem-utils-1.1.5/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_extended_reaction_smiles.py` & `rxn-chem-utils-1.1.5/tests/test_extended_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_miscellaneous.py` & `rxn-chem-utils-1.1.5/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_multicomponent_smiles.py` & `rxn-chem-utils-1.1.5/tests/test_multicomponent_smiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     assert canonicalize_multicomponent_smiles("C.OCC.C(C)O") == "C.CCO.CCO"
 
     # Canonicalizing an empty string is valid - since this is a valid multi-component SMILES
     assert canonicalize_multicomponent_smiles("") == ""
 
     # with fragment bond; may fail if fragment bond not specified
     assert (
-        canonicalize_multicomponent_smiles("C.[Na+]~[H-].O", fragment_bond="~")
-        == "C.[H-]~[Na+].O"
+        canonicalize_multicomponent_smiles("C.[H-]~[F-]~[Mg+2].O", fragment_bond="~")
+        == "C.[F-]~[H-]~[Mg+2].O"
     )
     with pytest.raises(InvalidSmiles):
-        _ = canonicalize_multicomponent_smiles("C.[Na+]~[H-].O")
+        _ = canonicalize_multicomponent_smiles("C.[H-]~[F-]~[Mg+2].O")
 
     # possibility to check valence or not
     assert (
         canonicalize_multicomponent_smiles("C.CF(C).O", check_valence=False)
         == "C.CFC.O"
     )
     with pytest.raises(InvalidSmiles):
```

### Comparing `rxn-chem-utils-1.1.4/tests/test_rdkit_utils.py` & `rxn-chem-utils-1.1.5/tests/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_reaction_combiner.py` & `rxn-chem-utils-1.1.5/tests/test_reaction_combiner.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_reaction_equation.py` & `rxn-chem-utils-1.1.5/tests/test_reaction_equation.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_reaction_smiles.py` & `rxn-chem-utils-1.1.5/tests/test_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_smiles_augmenter.py` & `rxn-chem-utils-1.1.5/tests/test_smiles_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_smiles_randomization.py` & `rxn-chem-utils-1.1.5/tests/test_smiles_randomization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_tokenization.py` & `rxn-chem-utils-1.1.5/tests/test_tokenization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.4/tests/test_utils.py` & `rxn-chem-utils-1.1.5/tests/test_utils.py`

 * *Files identical despite different names*

