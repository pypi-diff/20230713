# Comparing `tmp/golfy-1.9.3.tar.gz` & `tmp/golfy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.9.3.tar", last modified: Wed Jul 12 21:33:56 2023, max compression
+gzip compressed data, was "golfy-2.0.0.tar", last modified: Thu Jul 13 18:50:09 2023, max compression
```

## Comparing `golfy-1.9.3.tar` & `golfy-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.525096 golfy-1.9.3/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.9.3/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     3658 2023-07-12 21:33:56.524983 golfy-1.9.3/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     2932 2023-07-12 21:27:59.000000 golfy-1.9.3/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.523220 golfy-1.9.3/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      693 2023-07-12 21:28:41.000000 golfy-1.9.3/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.9.3/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)    17960 2023-07-12 20:55:06.000000 golfy-1.9.3/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4264 2023-07-12 21:30:39.000000 golfy-1.9.3/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6810 2023-07-12 19:40:02.000000 golfy-1.9.3/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11274 2023-07-12 20:19:16.000000 golfy-1.9.3/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4177 2023-07-12 19:26:25.000000 golfy-1.9.3/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.9.3/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.9.3/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.9.3/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.523787 golfy-1.9.3/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     3658 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      479 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.9.3/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.9.3/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-12 21:33:56.525127 golfy-1.9.3/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.524730 golfy-1.9.3/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.9.3/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      538 2023-07-12 20:35:22.000000 golfy-1.9.3/tests/test_find_best_solution.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-1.9.3/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-1.9.3/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.353192 golfy-2.0.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.0.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     4385 2023-07-13 18:50:09.353036 golfy-2.0.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     3659 2023-07-13 17:17:58.000000 golfy-2.0.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.350406 golfy-2.0.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-13 17:18:12.000000 golfy-2.0.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.0.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.0.0/golfy/design.py
+-rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.0.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8844 2023-07-13 17:28:25.000000 golfy-2.0.0/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.0.0/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.0.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.0.0/golfy/simulation.py
+-rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.0.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.0.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.0.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.351034 golfy-2.0.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     4385 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      562 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-13 18:50:09.000000 golfy-2.0.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.0.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.0.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-13 18:50:09.353232 golfy-2.0.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-13 18:50:09.352593 golfy-2.0.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.0.0/tests/test_best_design_for_pool_budget.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.0.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.0.0/tests/test_find_best_design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.0.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.0.0/tests/test_optimize.py
+-rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.0.0/tests/test_simulation.py
```

### Comparing `golfy-1.9.3/LICENSE` & `golfy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.9.3/PKG-INFO` & `golfy-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.9.3
+Version: 2.0.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -29,63 +29,75 @@
 
 ```sh
 pip install scikit-learn
 ```
 
 ## Usage
 
-### High level API
+Assignments of peptides to pools are called `golfy.Design` objects, which can be constructed and optimized using several different strategies.
 
-Assignments of peptides to pools are called `golfy.Solution` objects, which can be constructed and optimized using several different strategies. You can
-ignore most of the implementation details by just calling `find_best_solution`, which tries multiple different initialization strategies to create multiple solutions,
-optimizes each one, and returns the solution which fewest constraint violations and fewest number of total pools.
+### Designs for single round ESLIpot experiments
+
+If all you care about is finding the best design for a fixed number of peptides and a maximum number of pools (eg 96 wells on a plate) then use thing function:
+
+```python
+from golfy import best_design_for_pool_budget
+
+design = best_design_for_pool_budget(num_peptides=200, max_pools=96)
+```
+
+It will loop over a very large configuration space, try to make the best design for each configuration, simulate ELISpot counts under a simplistic model, and score each design by its ability to deconvolve hits out of pooled results in a single round of experimentation (without a second round of validation for individual peptides).
+
+### More control over design parameters
+
+If you want to control parameters such as the number of replicates or the maximum peptides per pool, you can call `find_best_design`, which tries multiple different initialization strategies to create multiple designs, optimizes each one, and returns the design which fewest constraint violations and fewest number of total pools.
 
 ```python
-from golfy import find_best_solution
+from golfy import find_best_design
 
-s = find_best_solution(
+design = find_best_design(
     num_peptides=100,
     max_peptides_per_pool=5,
     num_replicates=3,
     invalid_neighbors=[(0,1), (1,2)],
     preferred_neighbors=[(0,3),(1,5)],
     allow_extra_pools=False,
     verbose=False)
 ```
 
-A key parameter to `find_best_solution` is `allow_extra_pools`, which determines whether Golfy is allowed to expand the number of total pools beyond the minimum by the `ceil(num_peptides * num_replicates / max_peptides_per_pool)`. If Golfy cannot add extra pools then
-it may not be able to find a valid solution for every combination of parameters (but will still give you the solution with the least constraint violations that it could construct and optimize).
+A key parameter to `find_best_design` is `allow_extra_pools`, which determines whether Golfy is allowed to expand the number of total pools beyond the minimum by the `ceil(num_peptides * num_replicates / max_peptides_per_pool)`. If Golfy cannot add extra pools then
+it may not be able to find a valid solution for every combination of parameters (but will still give you the design with the least constraint violations that it could construct and optimize).
 
-### Initialization and optimization of solutions
+### Initialization and optimization of designs
 
-If you want more control over the way that solutions are initialized and optimized you can use the `golfy.init` and `golfy.optimize` functions directly.
+If you want more control over the way that desgins are initialized and optimized you can use the `golfy.init` and `golfy.optimize` functions directly.
 
 ```python
 
 from golfy import init, is_valid, optimize
 
 # create a random initial assignment of peptides to pools
 s = init(num_peptides=100, peptides_per_pool=5, num_replicates=3, strategy='random', allow_extra_pools=False)
 
-# the random assignment probably isn't yet a valid solution
+# the random assignment probably isn't yet a valid design
 assert not is_valid(s)
 
 # iteratively swap peptides which violate constraints until
 # a valid configuration is achieved
 optimize(s, allow_extra_pools=False)
 
 assert is_valid(s)
 ```
 
 ### Deconvolution of hit peptides from ELISpot counts
 
 ```python
 from golfy.deconvolution import create_linear_system, solve_linear_system
 
-# s is a golfy.Solution object containing the mapping of peptides to pools
+# s is a golfy.Design object containing the mapping of peptides to pools
 # counts is a dictionary from (replicate, pool) index pairs to ELISpot counts or activity values
 linear_system = create_linear_system(s, counts)
 
 # result type has an array of individual peptide activity estimates (result.activity_per_peptide)
 # and a set of high confidence hit peptides (result.high_confidence_peptides)
 result = solve_linear_system(linear_system)
 print(result.high_confidence_hits)
```

### Comparing `golfy-1.9.3/README.md` & `golfy-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,63 +12,75 @@
 
 ```sh
 pip install scikit-learn
 ```
 
 ## Usage
 
-### High level API
+Assignments of peptides to pools are called `golfy.Design` objects, which can be constructed and optimized using several different strategies.
 
-Assignments of peptides to pools are called `golfy.Solution` objects, which can be constructed and optimized using several different strategies. You can
-ignore most of the implementation details by just calling `find_best_solution`, which tries multiple different initialization strategies to create multiple solutions,
-optimizes each one, and returns the solution which fewest constraint violations and fewest number of total pools.
+### Designs for single round ESLIpot experiments
+
+If all you care about is finding the best design for a fixed number of peptides and a maximum number of pools (eg 96 wells on a plate) then use thing function:
+
+```python
+from golfy import best_design_for_pool_budget
+
+design = best_design_for_pool_budget(num_peptides=200, max_pools=96)
+```
+
+It will loop over a very large configuration space, try to make the best design for each configuration, simulate ELISpot counts under a simplistic model, and score each design by its ability to deconvolve hits out of pooled results in a single round of experimentation (without a second round of validation for individual peptides).
+
+### More control over design parameters
+
+If you want to control parameters such as the number of replicates or the maximum peptides per pool, you can call `find_best_design`, which tries multiple different initialization strategies to create multiple designs, optimizes each one, and returns the design which fewest constraint violations and fewest number of total pools.
 
 ```python
-from golfy import find_best_solution
+from golfy import find_best_design
 
-s = find_best_solution(
+design = find_best_design(
     num_peptides=100,
     max_peptides_per_pool=5,
     num_replicates=3,
     invalid_neighbors=[(0,1), (1,2)],
     preferred_neighbors=[(0,3),(1,5)],
     allow_extra_pools=False,
     verbose=False)
 ```
 
-A key parameter to `find_best_solution` is `allow_extra_pools`, which determines whether Golfy is allowed to expand the number of total pools beyond the minimum by the `ceil(num_peptides * num_replicates / max_peptides_per_pool)`. If Golfy cannot add extra pools then
-it may not be able to find a valid solution for every combination of parameters (but will still give you the solution with the least constraint violations that it could construct and optimize).
+A key parameter to `find_best_design` is `allow_extra_pools`, which determines whether Golfy is allowed to expand the number of total pools beyond the minimum by the `ceil(num_peptides * num_replicates / max_peptides_per_pool)`. If Golfy cannot add extra pools then
+it may not be able to find a valid solution for every combination of parameters (but will still give you the design with the least constraint violations that it could construct and optimize).
 
-### Initialization and optimization of solutions
+### Initialization and optimization of designs
 
-If you want more control over the way that solutions are initialized and optimized you can use the `golfy.init` and `golfy.optimize` functions directly.
+If you want more control over the way that desgins are initialized and optimized you can use the `golfy.init` and `golfy.optimize` functions directly.
 
 ```python
 
 from golfy import init, is_valid, optimize
 
 # create a random initial assignment of peptides to pools
 s = init(num_peptides=100, peptides_per_pool=5, num_replicates=3, strategy='random', allow_extra_pools=False)
 
-# the random assignment probably isn't yet a valid solution
+# the random assignment probably isn't yet a valid design
 assert not is_valid(s)
 
 # iteratively swap peptides which violate constraints until
 # a valid configuration is achieved
 optimize(s, allow_extra_pools=False)
 
 assert is_valid(s)
 ```
 
 ### Deconvolution of hit peptides from ELISpot counts
 
 ```python
 from golfy.deconvolution import create_linear_system, solve_linear_system
 
-# s is a golfy.Solution object containing the mapping of peptides to pools
+# s is a golfy.Design object containing the mapping of peptides to pools
 # counts is a dictionary from (replicate, pool) index pairs to ELISpot counts or activity values
 linear_system = create_linear_system(s, counts)
 
 # result type has an array of individual peptide activity estimates (result.activity_per_peptide)
 # and a set of high confidence hit peptides (result.high_confidence_peptides)
 result = solve_linear_system(linear_system)
 print(result.high_confidence_hits)
```

### Comparing `golfy-1.9.3/golfy/initialization.py` & `golfy-2.0.0/golfy/initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 import math
 from typing import Optional, Literal
 
 import numpy as np
 
-from .solution import Solution
+from .design import Design
 from .types import PeptidePairList, Replicate, Peptide
 from .util import pairs_to_dict, transitive_closure
 from .validity import count_violations
 
 
 def _pools_per_replicate(
     num_peptides: int,
@@ -61,78 +61,80 @@
     max_peptides_per_pool: int,
     num_replicates: int,
     num_pools_per_replicate: dict[Replicate, int],
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     allow_extra_pools: bool = False,
     verbose: bool = False,
-) -> Solution:
+) -> Design:
     replicate_to_pool_to_peptides = {}
     for i in range(num_replicates):
         peptide_array = np.arange(num_peptides)
         np.random.shuffle(peptide_array)
         pool_assignments = {}
         replicate_to_pool_to_peptides[i] = pool_assignments
         num_pools = num_pools_per_replicate[i]
         peptides_per_pool = int(np.ceil(num_peptides / num_pools))
         for j in range(num_pools):
             start_idx = peptides_per_pool * j
             end_idx = peptides_per_pool * (j + 1)
             pool_assignments[j] = peptide_array[start_idx:end_idx]
 
-    return Solution(
+    return Design(
         num_peptides=num_peptides,
         max_peptides_per_pool=max_peptides_per_pool,
         num_replicates=num_replicates,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
         assignments=replicate_to_pool_to_peptides,
+        allow_extra_pools=allow_extra_pools,
     )
 
 
 def _singleton_init(
     num_peptides: int,
     max_peptides_per_pool: int,
     num_replicates: int,
     num_pools_per_replicate: dict[Replicate, int],
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     allow_extra_pools: bool = False,
     verbose: bool = False,
-) -> Solution:
+) -> Design:
     """
     Initialize every peptide to be in its own pool
     """
 
     replicate_to_pool_to_peptides = {}
     for i in range(num_replicates):
         pool_to_peptides = {}
         for p in range(num_peptides):
             pool_to_peptides[p] = np.array([p])
         replicate_to_pool_to_peptides[i] = pool_to_peptides
-    return Solution(
+    return Design(
         num_peptides=num_peptides,
         max_peptides_per_pool=max_peptides_per_pool,
         num_replicates=num_replicates,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
         assignments=replicate_to_pool_to_peptides,
+        allow_extra_pools=allow_extra_pools,
     )
 
 
 def _valid_init(
     num_peptides: int,
     max_peptides_per_pool: int,
     num_replicates: int,
     num_pools_per_replicate: dict[Replicate, int],
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     allow_extra_pools: bool = False,
     verbose: bool = False,
-) -> Solution:
+) -> Design:
     peptide_to_invalid = pairs_to_dict(invalid_neighbors)
     peptide_to_preferred = transitive_closure(pairs_to_dict(preferred_neighbors))
     if verbose:
         print("[_valid_init] Invalid neighbors: %s" % (peptide_to_invalid,))
         print("[_valid_init] Preferred neighbors: %s" % (peptide_to_preferred,))
 
     replicate_to_pool_to_peptides = {}
@@ -230,34 +232,35 @@
                     )
                 make_new_pool(peptide)
 
         replicate_to_pool_to_peptides[i] = {
             pool_idx: np.array(sorted(peptides))
             for (pool_idx, peptides) in pool_to_peptides.items()
         }
-    return Solution(
+    return Design(
         num_peptides=num_peptides,
         max_peptides_per_pool=max_peptides_per_pool,
         num_replicates=num_replicates,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
         assignments=replicate_to_pool_to_peptides,
+        allow_extra_pools=allow_extra_pools,
     )
 
 
 def _greedy_init(
     num_peptides: int,
     max_peptides_per_pool: int,
     num_replicates: int,
     num_pools_per_replicate: dict[Replicate, int],
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     allow_extra_pools: bool = False,
     verbose: bool = False,
-) -> Solution:
+) -> Design:
     peptide_to_invalid = pairs_to_dict(invalid_neighbors)
     peptide_to_preferred = transitive_closure(pairs_to_dict(preferred_neighbors))
     if verbose:
         print("[_greedy_init] Invalid neighbors: %s" % (peptide_to_invalid,))
         print("[_greedy_init] Preferred neighbors: %s" % (peptide_to_preferred,))
 
     replicate_to_pool_to_peptides = {}
@@ -362,35 +365,36 @@
                     raise ValueError("Unable to create valid configuration")
 
         replicate_to_pool_to_peptides[i] = {
             pool_idx: np.array(sorted(peptides))
             for (pool_idx, peptides) in pool_to_peptides.items()
         }
 
-    return Solution(
+    return Design(
         num_peptides=num_peptides,
         max_peptides_per_pool=max_peptides_per_pool,
         num_replicates=num_replicates,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
         assignments=replicate_to_pool_to_peptides,
+        allow_extra_pools=allow_extra_pools,
     )
 
 
 def init(
     num_peptides: int = 100,
     max_peptides_per_pool: int = 5,
     num_replicates: int = 3,
     num_pools_per_replicate: Optional[int | dict[Replicate, int]] = None,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     strategy: Literal["greedy", "random", "valid", "singleton"] = "greedy",
     allow_extra_pools: bool = False,
     verbose: bool = False,
-) -> Solution:
+) -> Design:
     """
     Initialize a Solution for a given configuration
 
     Args
     ----
     num_peptides
         number of peptides (default: 100)
```

### Comparing `golfy-1.9.3/golfy/merging.py` & `golfy-2.0.0/golfy/merging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 
-from .solution import Solution
+from .design import Design
 from .types import Replicate, Pool, Peptide
 from .util import pairs_to_dict, transitive_closure
 
 
 def _make_peptide_to_invalid_excluding_replicate(
-    s: Solution,
+    s: Design,
 ) -> dict[Replicate, dict[Peptide, set[Peptide]]]:
     peptide_to_invalid = pairs_to_dict(s.invalid_neighbors)
     peptide_to_invalid_excluding_replicate = {
         replicate_idx: {
             peptide: peptide_to_invalid.get(peptide, set()).copy()
             for peptide in range(s.num_peptides)
         }
@@ -35,15 +35,15 @@
                             ].add(other_peptide)
                             peptide_to_invalid_excluding_replicate[replicate_idx][
                                 other_peptide
                             ].add(peptide)
     return peptide_to_invalid_excluding_replicate
 
 
-def merge_small_pools(s: Solution, verbose: bool = False) -> int:
+def merge_small_pools(s: Design, verbose: bool = False) -> int:
     num_merged = 0
 
     peptide_to_preferred = transitive_closure(pairs_to_dict(s.preferred_neighbors))
     peptide_to_invalid_excluding_replicate = (
         _make_peptide_to_invalid_excluding_replicate(s)
     )
 
@@ -142,15 +142,15 @@
                     break
 
     # just in case we ended up with any empty pools, remove them from the solution
     s.remove_empty_pools()
     return num_merged
 
 
-def cleanup(s: Solution, verbose: bool = True, max_iters=1000) -> int:
+def cleanup(s: Design, verbose: bool = True, max_iters=1000) -> int:
     total_num_merged = 0
     prev_num_pools = s.num_pools()
 
     for iter_idx in range(max_iters):
         num_merged = merge_small_pools(s)
         total_num_merged += num_merged
         num_pools = s.num_pools()
```

### Comparing `golfy-1.9.3/golfy/optimization.py` & `golfy-2.0.0/golfy/optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections import defaultdict
 import random
 import time
 
 import numpy as np
 
 from .merging import cleanup
-from .solution import Solution
+from .design import Design
 from .types import SwapCandidateList, ReplicateToNeighborDict, Replicate, Pool, Peptide
 from .validity import violations_per_replicate, is_valid, count_violations
 from .util import pairs_to_dict
 
 
 def find_violating_peptides(
-    s: Solution,
+    s: Design,
 ) -> tuple[SwapCandidateList, ReplicateToNeighborDict]:
     replicate_to_pool_to_peptides = s.assignments
     # treat invalid pairs as if they've already been neighbors in a previous round
     peptide_to_neighbors = pairs_to_dict(s.invalid_neighbors)
     needs_swap = []
     replicate_to_neighbor_dict = {}
     for replicate_idx, pool_to_peptides in replicate_to_pool_to_peptides.items():
@@ -41,15 +41,15 @@
 ) -> dict[Replicate, tuple[Pool, Peptide]]:
     result = defaultdict(list)
     for replicate_idx, pool_idx, peptide in swap_candidates:
         result[replicate_idx].append((pool_idx, peptide))
     return result
 
 
-def improve_solution(s: Solution, verbose: bool = False):
+def improve_solution(s: Design, verbose: bool = False):
     replicate_to_pool_to_peptides = s.assignments
     replicate_to_peptide_to_pool = s.replicate_to_peptide_to_pool_dict()
 
     needs_swap, replicate_to_neighbor_dict = find_violating_peptides(s)
 
     random.shuffle(needs_swap)
 
@@ -177,15 +177,15 @@
                     swapped_pools.add(pool_idx_a)
                     swapped_pools.add(pool_idx_b)
                     swapped_peptides.add(peptide_a)
                     swapped_peptides.add(peptide_b)
 
 
 def optimize(
-    s: Solution,
+    s: Design,
     max_iters: int = 2000,
     verbose: bool = False,
     allow_extra_pools: bool = True,
     return_history: bool = False,
 ) -> bool:
     """
     Iteratively update solution by randomly swapping a violating peptide with a random other peptide
```

### Comparing `golfy-1.9.3/golfy/solution.py` & `golfy-2.0.0/golfy/design.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,56 @@
 from collections import defaultdict
-from dataclasses import dataclass
-import numpy as np
+from dataclasses import dataclass, field
 from typing import Iterable, Mapping
 
+import numpy as np
+
 from .types import PeptidePairList, Replicate, Pool, Peptide
 
 
 @dataclass
 class Spec:
     num_peptides: int
     max_peptides_per_pool: int
     num_replicates: int
+    allow_extra_pools: bool
     invalid_neighbors: PeptidePairList
     preferred_neighbors: PeptidePairList
 
+    def to_tuple(self):
+        return (
+            self.num_peptides,
+            self.max_peptides_per_pool,
+            self.num_replicates,
+            self.allow_extra_pools,
+            tuple(sorted(self.invalid_neighbors)),
+            tuple(sorted(self.preferred_neighbors)),
+        )
+
+    def __eq__(self, other):
+        return isinstance(other, Spec) and self.to_tuple() == other.to_tuple()
+
+    def __hash__(self):
+        return hash(self.to_tuple())
+
 
 @dataclass
-class Solution(Spec):
+class Design(Spec):
     assignments: Mapping[Replicate, Mapping[Pool, Iterable[Peptide]]]
 
+    def to_spec(self) -> Spec:
+        return Spec(
+            num_peptides=self.num_peptides,
+            max_peptides_per_pool=self.max_peptides_per_pool,
+            num_replicates=self.num_replicates,
+            allow_extra_pools=self.allow_extra_pools,
+            invalid_neighbors=self.invalid_neighbors,
+            preferred_neighbors=self.preferred_neighbors,
+        )
+
     def move_peptide(
         self,
         replicate_idx: Replicate,
         old_pool_idx: Pool,
         peptide: Peptide,
         new_pool_idx: Pool,
     ):
```

### Comparing `golfy-1.9.3/golfy/util.py` & `golfy-2.0.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.3/golfy/validity.py` & `golfy-2.0.0/golfy/validity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .solution import Solution
+from .design import Design
 from .types import Replicate, Pool, Peptide, Mapping
 from .util import pairs_to_dict
 
 
 def violations_per_replicate(
-    s: Solution,
+    s: Design,
     error_on_duplicate=True,
     error_on_extra=True,
     error_on_missing=True,
     verbose=False,
 ) -> Mapping[Replicate, int]:
     replicate_to_violations = {}
 
@@ -66,15 +66,15 @@
                             violations += 1
                         peptide_to_neighbors[p1].add(p2)
         replicate_to_violations[replicate_idx] = violations
     return replicate_to_violations
 
 
 def count_violations(
-    s: Solution,
+    s: Design,
     error_on_duplicate=True,
     error_on_extra=True,
     error_on_missing=True,
     verbose=False,
 ) -> int:
     return sum(
         violations_per_replicate(
@@ -84,15 +84,15 @@
             error_on_missing=error_on_missing,
             verbose=verbose,
         ).values()
     )
 
 
 def is_valid(
-    s: Solution,
+    s: Design,
     error_on_duplicate=True,
     error_on_extra=True,
     error_on_missing=True,
     verbose=False,
 ) -> bool:
     return (
         count_violations(
```

### Comparing `golfy-1.9.3/golfy.egg-info/PKG-INFO` & `golfy-2.0.0/golfy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.9.3
+Version: 2.0.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -29,63 +29,75 @@
 
 ```sh
 pip install scikit-learn
 ```
 
 ## Usage
 
-### High level API
+Assignments of peptides to pools are called `golfy.Design` objects, which can be constructed and optimized using several different strategies.
 
-Assignments of peptides to pools are called `golfy.Solution` objects, which can be constructed and optimized using several different strategies. You can
-ignore most of the implementation details by just calling `find_best_solution`, which tries multiple different initialization strategies to create multiple solutions,
-optimizes each one, and returns the solution which fewest constraint violations and fewest number of total pools.
+### Designs for single round ESLIpot experiments
+
+If all you care about is finding the best design for a fixed number of peptides and a maximum number of pools (eg 96 wells on a plate) then use thing function:
+
+```python
+from golfy import best_design_for_pool_budget
+
+design = best_design_for_pool_budget(num_peptides=200, max_pools=96)
+```
+
+It will loop over a very large configuration space, try to make the best design for each configuration, simulate ELISpot counts under a simplistic model, and score each design by its ability to deconvolve hits out of pooled results in a single round of experimentation (without a second round of validation for individual peptides).
+
+### More control over design parameters
+
+If you want to control parameters such as the number of replicates or the maximum peptides per pool, you can call `find_best_design`, which tries multiple different initialization strategies to create multiple designs, optimizes each one, and returns the design which fewest constraint violations and fewest number of total pools.
 
 ```python
-from golfy import find_best_solution
+from golfy import find_best_design
 
-s = find_best_solution(
+design = find_best_design(
     num_peptides=100,
     max_peptides_per_pool=5,
     num_replicates=3,
     invalid_neighbors=[(0,1), (1,2)],
     preferred_neighbors=[(0,3),(1,5)],
     allow_extra_pools=False,
     verbose=False)
 ```
 
-A key parameter to `find_best_solution` is `allow_extra_pools`, which determines whether Golfy is allowed to expand the number of total pools beyond the minimum by the `ceil(num_peptides * num_replicates / max_peptides_per_pool)`. If Golfy cannot add extra pools then
-it may not be able to find a valid solution for every combination of parameters (but will still give you the solution with the least constraint violations that it could construct and optimize).
+A key parameter to `find_best_design` is `allow_extra_pools`, which determines whether Golfy is allowed to expand the number of total pools beyond the minimum by the `ceil(num_peptides * num_replicates / max_peptides_per_pool)`. If Golfy cannot add extra pools then
+it may not be able to find a valid solution for every combination of parameters (but will still give you the design with the least constraint violations that it could construct and optimize).
 
-### Initialization and optimization of solutions
+### Initialization and optimization of designs
 
-If you want more control over the way that solutions are initialized and optimized you can use the `golfy.init` and `golfy.optimize` functions directly.
+If you want more control over the way that desgins are initialized and optimized you can use the `golfy.init` and `golfy.optimize` functions directly.
 
 ```python
 
 from golfy import init, is_valid, optimize
 
 # create a random initial assignment of peptides to pools
 s = init(num_peptides=100, peptides_per_pool=5, num_replicates=3, strategy='random', allow_extra_pools=False)
 
-# the random assignment probably isn't yet a valid solution
+# the random assignment probably isn't yet a valid design
 assert not is_valid(s)
 
 # iteratively swap peptides which violate constraints until
 # a valid configuration is achieved
 optimize(s, allow_extra_pools=False)
 
 assert is_valid(s)
 ```
 
 ### Deconvolution of hit peptides from ELISpot counts
 
 ```python
 from golfy.deconvolution import create_linear_system, solve_linear_system
 
-# s is a golfy.Solution object containing the mapping of peptides to pools
+# s is a golfy.Design object containing the mapping of peptides to pools
 # counts is a dictionary from (replicate, pool) index pairs to ELISpot counts or activity values
 linear_system = create_linear_system(s, counts)
 
 # result type has an array of individual peptide activity estimates (result.activity_per_peptide)
 # and a set of high confidence hit peptides (result.high_confidence_peptides)
 result = solve_linear_system(linear_system)
 print(result.high_confidence_hits)
```

### Comparing `golfy-1.9.3/pyproject.toml` & `golfy-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.9.3/tests/test_find_best_solution.py` & `golfy-2.0.0/tests/test_find_best_design.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from golfy import find_best_solution
+from golfy import find_best_design
 
 
-def test_find_best_solution_allow_extra_pools():
-    s = find_best_solution(100, 20, 3, allow_extra_pools=True)
+def test_find_best_design_allow_extra_pools():
+    s = find_best_design(100, 20, 3, allow_extra_pools=True)
     assert s.num_peptides == 100
     assert s.num_replicates == 3
     assert s.max_peptides_per_pool == 20
     assert s.num_pools() > 15
 
 
-def test_find_best_solution_no_extra_pools():
-    s = find_best_solution(100, 20, 3, allow_extra_pools=False)
+def test_find_best_design_no_extra_pools():
+    s = find_best_design(100, 20, 3, allow_extra_pools=False)
     assert s.num_peptides == 100
     assert s.num_replicates == 3
     assert s.max_peptides_per_pool == 20
     assert s.num_pools() == 15
```

### Comparing `golfy-1.9.3/tests/test_init.py` & `golfy-2.0.0/tests/test_init.py`

 * *Files identical despite different names*

