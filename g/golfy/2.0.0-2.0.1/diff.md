# Comparing `tmp/golfy-2.0.0.tar.gz` & `tmp/golfy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-2.0.0.tar", last modified: Thu Jul 13 18:50:09 2023, max compression
+gzip compressed data, was "golfy-2.0.1.tar", last modified: Thu Jul 13 19:03:51 2023, max compression
```

## Comparing `golfy-2.0.0.tar` & `golfy-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.353192 golfy-2.0.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.0.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     4385 2023-07-13 18:50:09.353036 golfy-2.0.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     3659 2023-07-13 17:17:58.000000 golfy-2.0.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.350406 golfy-2.0.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-13 17:18:12.000000 golfy-2.0.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.0.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.0.0/golfy/design.py
--rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.0.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8844 2023-07-13 17:28:25.000000 golfy-2.0.0/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.0.0/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.0.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.0.0/golfy/simulation.py
--rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.0.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.0.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.0.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.351034 golfy-2.0.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     4385 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      562 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.0.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.0.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-13 18:50:09.353232 golfy-2.0.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.352593 golfy-2.0.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.0.0/tests/test_best_design_for_pool_budget.py
--rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.0.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.0.0/tests/test_find_best_design.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.0.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.0.0/tests/test_optimize.py
--rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.0.0/tests/test_simulation.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:03:51.101746 golfy-2.0.1/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.0.1/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 19:03:51.101371 golfy-2.0.1/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.0.1/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:03:51.092622 golfy-2.0.1/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-13 19:03:05.000000 golfy-2.0.1/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.0.1/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.0.1/golfy/design.py
+-rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.0.1/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8844 2023-07-13 17:28:25.000000 golfy-2.0.1/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.0.1/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.0.1/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.0.1/golfy/simulation.py
+-rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.0.1/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.0.1/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.0.1/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:03:51.093363 golfy-2.0.1/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 19:03:51.000000 golfy-2.0.1/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      562 2023-07-13 19:03:51.000000 golfy-2.0.1/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-13 19:03:51.000000 golfy-2.0.1/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 19:03:51.000000 golfy-2.0.1/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 19:03:51.000000 golfy-2.0.1/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.0.1/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.0.1/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-13 19:03:51.101840 golfy-2.0.1/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:03:51.101110 golfy-2.0.1/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.0.1/tests/test_best_design_for_pool_budget.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.0.1/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.0.1/tests/test_find_best_design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.0.1/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.0.1/tests/test_optimize.py
+-rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.0.1/tests/test_simulation.py
```

### Comparing `golfy-2.0.0/LICENSE` & `golfy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/PKG-INFO` & `golfy-2.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# golfy
+# Golfy
 
-Heuristic solver for peptide pool assignments. Golfy attempts to map peptides to pools with a fixed specified "coverage" (number of pools that each peptide occurs in) while avoiding having any pair of peptides occur in a pool twice.
+Golfy is a heuristic solver for experimental designs using pools of peptides, such as [combinatorial ELISpot epitope mapping](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0147812). Golfy constructs experimental designs which assign peptides to pools with a fixed specified "coverage" (number of pools that each peptide occurs in) while trying to avoid having any pair of peptides occur together in a pool more than once. 
+
+More formally, Golfy is a collection of heuristic search techniques for [partially balanced incomplete block designs](https://www.jstor.org/stable/40383923), where *block design* means that it's an experimental design where peptides are tested in groups, *incomplete* means that each block is smaller than the full set of peptides, and *partially balanced* means that a pair of peptides can occur together in a group 0 or 1 times. 
+
+Golfy also includes a deconvolution algorithm which attempts to find a sparse set of "hit peptides" to best explain ELISpot counts observed after using a Golfy generated experimental design. 
 
 ## Installation
 
 ```sh
 pip install golfy
 ```
```

### Comparing `golfy-2.0.0/README.md` & `golfy-2.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-# golfy
+# Golfy
 
-Heuristic solver for peptide pool assignments. Golfy attempts to map peptides to pools with a fixed specified "coverage" (number of pools that each peptide occurs in) while avoiding having any pair of peptides occur in a pool twice.
+Golfy is a heuristic solver for experimental designs using pools of peptides, such as [combinatorial ELISpot epitope mapping](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0147812). Golfy constructs experimental designs which assign peptides to pools with a fixed specified "coverage" (number of pools that each peptide occurs in) while trying to avoid having any pair of peptides occur together in a pool more than once. 
+
+More formally, Golfy is a collection of heuristic search techniques for [partially balanced incomplete block designs](https://www.jstor.org/stable/40383923), where *block design* means that it's an experimental design where peptides are tested in groups, *incomplete* means that each block is smaller than the full set of peptides, and *partially balanced* means that a pair of peptides can occur together in a group 0 or 1 times. 
+
+Golfy also includes a deconvolution algorithm which attempts to find a sparse set of "hit peptides" to best explain ELISpot counts observed after using a Golfy generated experimental design. 
 
 ## Installation
 
 ```sh
 pip install golfy
 ```
```

### Comparing `golfy-2.0.0/golfy/__init__.py` & `golfy-2.0.1/golfy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     simulate_elispot_counts,
     simulate_any_hits_per_pool,
     simulate_number_hits_per_pool,
 )
 from .types import SpotCounts
 from .validity import is_valid, count_violations, violations_per_replicate
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 __all__ = [
     "__version__",
     "find_best_design",
     "best_design_for_pool_budget",
     "Design",
     "init",
```

### Comparing `golfy-2.0.0/golfy/deconvolution.py` & `golfy-2.0.1/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/design.py` & `golfy-2.0.1/golfy/design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/initialization.py` & `golfy-2.0.1/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/main.py` & `golfy-2.0.1/golfy/main.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/merging.py` & `golfy-2.0.1/golfy/merging.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/optimization.py` & `golfy-2.0.1/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/simulation.py` & `golfy-2.0.1/golfy/simulation.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/util.py` & `golfy-2.0.1/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy/validity.py` & `golfy-2.0.1/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/golfy.egg-info/PKG-INFO` & `golfy-2.0.1/golfy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# golfy
+# Golfy
 
-Heuristic solver for peptide pool assignments. Golfy attempts to map peptides to pools with a fixed specified "coverage" (number of pools that each peptide occurs in) while avoiding having any pair of peptides occur in a pool twice.
+Golfy is a heuristic solver for experimental designs using pools of peptides, such as [combinatorial ELISpot epitope mapping](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0147812). Golfy constructs experimental designs which assign peptides to pools with a fixed specified "coverage" (number of pools that each peptide occurs in) while trying to avoid having any pair of peptides occur together in a pool more than once. 
+
+More formally, Golfy is a collection of heuristic search techniques for [partially balanced incomplete block designs](https://www.jstor.org/stable/40383923), where *block design* means that it's an experimental design where peptides are tested in groups, *incomplete* means that each block is smaller than the full set of peptides, and *partially balanced* means that a pair of peptides can occur together in a group 0 or 1 times. 
+
+Golfy also includes a deconvolution algorithm which attempts to find a sparse set of "hit peptides" to best explain ELISpot counts observed after using a Golfy generated experimental design. 
 
 ## Installation
 
 ```sh
 pip install golfy
 ```
```

### Comparing `golfy-2.0.0/golfy.egg-info/SOURCES.txt` & `golfy-2.0.1/golfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/pyproject.toml` & `golfy-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/tests/test_deconvolution.py` & `golfy-2.0.1/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/tests/test_find_best_design.py` & `golfy-2.0.1/tests/test_find_best_design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/tests/test_init.py` & `golfy-2.0.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `golfy-2.0.0/tests/test_simulation.py` & `golfy-2.0.1/tests/test_simulation.py`

 * *Files identical despite different names*

