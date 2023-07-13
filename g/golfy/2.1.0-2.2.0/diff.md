# Comparing `tmp/golfy-2.1.0.tar.gz` & `tmp/golfy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-2.1.0.tar", last modified: Thu Jul 13 19:10:27 2023, max compression
+gzip compressed data, was "golfy-2.2.0.tar", last modified: Thu Jul 13 21:46:01 2023, max compression
```

## Comparing `golfy-2.1.0.tar` & `golfy-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:10:27.769613 golfy-2.1.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.1.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 19:10:27.769502 golfy-2.1.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.1.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:10:27.768147 golfy-2.1.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-13 19:09:47.000000 golfy-2.1.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.1.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.1.0/golfy/design.py
--rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.1.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8853 2023-07-13 19:08:41.000000 golfy-2.1.0/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.1.0/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.1.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.1.0/golfy/simulation.py
--rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.1.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.1.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.1.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:10:27.768681 golfy-2.1.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 19:10:27.000000 golfy-2.1.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      562 2023-07-13 19:10:27.000000 golfy-2.1.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-13 19:10:27.000000 golfy-2.1.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 19:10:27.000000 golfy-2.1.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 19:10:27.000000 golfy-2.1.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.1.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.1.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-13 19:10:27.769644 golfy-2.1.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 19:10:27.769359 golfy-2.1.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.1.0/tests/test_best_design_for_pool_budget.py
--rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.1.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.1.0/tests/test_find_best_design.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.1.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.1.0/tests/test_optimize.py
--rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.1.0/tests/test_simulation.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.758552 golfy-2.2.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.2.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 21:46:01.758401 golfy-2.2.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.2.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.755200 golfy-2.2.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-13 21:43:52.000000 golfy-2.2.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.2.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.2.0/golfy/design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2455 2023-07-13 19:55:22.000000 golfy-2.2.0/golfy/evaluation.py
+-rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.2.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8071 2023-07-13 21:43:37.000000 golfy-2.2.0/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.2.0/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.2.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.2.0/golfy/simulation.py
+-rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.2.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.2.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.2.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.755943 golfy-2.2.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      582 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 21:46:01.000000 golfy-2.2.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.2.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.2.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-13 21:46:01.758591 golfy-2.2.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 21:46:01.757978 golfy-2.2.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.2.0/tests/test_best_design_for_pool_budget.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.2.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.2.0/tests/test_find_best_design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.2.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.2.0/tests/test_optimize.py
+-rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.2.0/tests/test_simulation.py
```

### Comparing `golfy-2.1.0/LICENSE` & `golfy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/PKG-INFO` & `golfy-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.1.0
+Version: 2.2.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-2.1.0/README.md` & `golfy-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/__init__.py` & `golfy-2.2.0/golfy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     simulate_elispot_counts,
     simulate_any_hits_per_pool,
     simulate_number_hits_per_pool,
 )
 from .types import SpotCounts
 from .validity import is_valid, count_violations, violations_per_replicate
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 __all__ = [
     "__version__",
     "find_best_design",
     "best_design_for_pool_budget",
     "Design",
     "init",
```

### Comparing `golfy-2.1.0/golfy/deconvolution.py` & `golfy-2.2.0/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/design.py` & `golfy-2.2.0/golfy/design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/initialization.py` & `golfy-2.2.0/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/merging.py` & `golfy-2.2.0/golfy/merging.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/optimization.py` & `golfy-2.2.0/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/simulation.py` & `golfy-2.2.0/golfy/simulation.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/util.py` & `golfy-2.2.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy/validity.py` & `golfy-2.2.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/golfy.egg-info/PKG-INFO` & `golfy-2.2.0/golfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.1.0
+Version: 2.2.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-2.1.0/golfy.egg-info/SOURCES.txt` & `golfy-2.2.0/golfy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 golfy/__init__.py
 golfy/deconvolution.py
 golfy/design.py
+golfy/evaluation.py
 golfy/initialization.py
 golfy/main.py
 golfy/merging.py
 golfy/optimization.py
 golfy/simulation.py
 golfy/types.py
 golfy/util.py
```

### Comparing `golfy-2.1.0/pyproject.toml` & `golfy-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/tests/test_deconvolution.py` & `golfy-2.2.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/tests/test_find_best_design.py` & `golfy-2.2.0/tests/test_find_best_design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/tests/test_init.py` & `golfy-2.2.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `golfy-2.1.0/tests/test_simulation.py` & `golfy-2.2.0/tests/test_simulation.py`

 * *Files identical despite different names*

