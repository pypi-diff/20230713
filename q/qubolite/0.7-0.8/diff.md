# Comparing `tmp/qubolite-0.7.tar.gz` & `tmp/qubolite-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubolite-0.7.tar", last modified: Mon Mar 20 15:46:50 2023, max compression
+gzip compressed data, was "qubolite-0.8.tar", last modified: Thu Jul 13 13:34:23 2023, max compression
```

## Comparing `qubolite-0.7.tar` & `qubolite-0.8.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-03-20 15:46:50.501943 qubolite-0.7/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4018 2023-03-20 15:46:50.501943 qubolite-0.7/PKG-INFO
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     3613 2023-03-16 16:09:49.000000 qubolite-0.7/README.md
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      673 2023-03-17 13:26:28.000000 qubolite-0.7/pyproject.toml
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-03-20 15:46:50.501943 qubolite-0.7/qubolite/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      164 2023-03-16 16:20:05.000000 qubolite-0.7/qubolite/__init__.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5401 2023-03-20 11:15:32.000000 qubolite-0.7/qubolite/_c_utils.c
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      965 2023-03-16 13:49:12.000000 qubolite-0.7/qubolite/bitvec.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2952 2023-03-16 16:16:22.000000 qubolite-0.7/qubolite/bounds.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4088 2022-07-29 21:00:45.000000 qubolite-0.7/qubolite/embedding.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2329 2023-03-16 16:15:26.000000 qubolite-0.7/qubolite/misc.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8825 2023-03-17 10:33:51.000000 qubolite-0.7/qubolite/qubo.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5945 2023-03-13 13:34:31.000000 qubolite-0.7/qubolite/sampling.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2287 2023-03-16 14:34:07.000000 qubolite-0.7/qubolite/solving.py
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-03-20 15:46:50.501943 qubolite-0.7/qubolite.egg-info/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4018 2023-03-20 15:46:50.000000 qubolite-0.7/qubolite.egg-info/PKG-INFO
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      368 2023-03-20 15:46:50.000000 qubolite-0.7/qubolite.egg-info/SOURCES.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)        1 2023-03-20 15:46:50.000000 qubolite-0.7/qubolite.egg-info/dependency_links.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      107 2023-03-20 15:46:50.000000 qubolite-0.7/qubolite.egg-info/requires.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)       18 2023-03-20 15:46:50.000000 qubolite-0.7/qubolite.egg-info/top_level.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)       38 2023-03-20 15:46:50.501943 qubolite-0.7/setup.cfg
--rwxr-xr-x   0 smuecke   (1000) smuecke   (1000)      836 2023-03-16 13:49:12.000000 qubolite-0.7/setup.py
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-13 13:34:23.548317 qubolite-0.8/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5231 2023-07-13 13:34:23.548317 qubolite-0.8/PKG-INFO
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4722 2023-07-13 08:34:09.000000 qubolite-0.8/README.md
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      850 2023-07-13 08:34:09.000000 qubolite-0.8/pyproject.toml
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-13 13:34:23.548317 qubolite-0.8/qubolite/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      205 2023-07-13 11:56:09.000000 qubolite-0.8/qubolite/__init__.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5873 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/_c_utils.c
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    10472 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/_heuristics.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2487 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/_misc.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6153 2023-07-13 08:49:00.000000 qubolite-0.8/qubolite/bitvec.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4689 2023-07-13 12:40:40.000000 qubolite-0.8/qubolite/bounds.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     9413 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/compression.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8161 2023-07-13 12:23:13.000000 qubolite-0.8/qubolite/embedding.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    21656 2023-07-13 12:48:30.000000 qubolite-0.8/qubolite/qubo.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    11257 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/sampling.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6740 2023-07-13 12:48:17.000000 qubolite-0.8/qubolite/solving.py
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-13 13:34:23.548317 qubolite-0.8/qubolite.egg-info/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5231 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/PKG-INFO
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      417 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/SOURCES.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)        1 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/dependency_links.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      185 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/requires.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)       18 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/top_level.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)       38 2023-07-13 13:34:23.548317 qubolite-0.8/setup.cfg
+-rwxr-xr-x   0 smuecke   (1000) smuecke   (1000)      836 2023-07-13 08:34:09.000000 qubolite-0.8/setup.py
```

### Comparing `qubolite-0.7/PKG-INFO` & `qubolite-0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-Metadata-Version: 2.1
-Name: qubolite
-Version: 0.7
-Summary: Toolbox for quadratic binary optimization
-Author-email: Sascha Mücke <sascha.muecke@tu-dortmund.de>
-Project-URL: Homepage, https://github.com/smuecke/qubolite
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: roof_dual
-Provides-Extra: kendall_tau
-Provides-Extra: all
-
 # qubolite
 
 A light-weight toolbox for working with QUBO instances in NumPy.
 
 
+<img src="qubolite.png"  width="100" height="100">
+
+
 ## Installation
 
 ```
 pip install qubolite
 ```
 
 This package was created using Python 3.10, but runs with Python >= 3.8.
@@ -32,14 +22,18 @@
 installed. This can be done with `pip install igraph` or by installing qubolite with 
 `pip install qubolite[roof_dual]`.
 
 Using the function `qubolite.ordering_distance()` requires the Kendall-τ measure from the
 [scipy](https://scipy.org/) library which can be installed by `pip install scipy` or by installing 
 qubolite with `pip install qubolite[kendall_tau]`.
 
+For exemplary QUBO embeddings (e.g. clustering or subset sum), the 
+[scikit-learn](https://scikit-learn.org/) library is required. It can be installed by either using 
+`pip install scikit-learn` or installing qubolite with `pip install qubolite[embeddings]`.
+
 If you would like to install all optional dependencies you can use `pip install qubolite[all]` for
 achieving this.
 
 ## Usage Examples
 
 By design, `qubolite` is a shallow wrapper around `numpy` arrays, which represent QUBO parameters.
 The core class is `qubo`, which receives a `numpy.ndarray` of size `(n, n)`.
@@ -64,14 +58,33 @@
 >>> Q(x)
 7.488225478498116
 >>> xs = np.random.random((5,8)) < 0.5
 >>> Q(xs)
 array([5.81642745, 4.41380893, 11.3391062, 4.34253921, 6.07799747])
 ```
 
+### Solving
+
+The submodule `solving` contains several methods to obtain the minimizing bit vector or energy value of a given QUBO instance, both exact and approximative.
+
+```
+>>> from qubolite.solving import brute_force
+>>> x_min, value = brute_force(Q, return_value=True)
+>>> x_min
+array([1., 1., 1., 0., 1., 0., 0., 0.])
+>>> value
+-3.394893116198653
+```
+
+The method `brute_force` is implemented efficiently in C and parallelized with OpenMP.
+Still, for instances with more than 30 variables take a long time to solve this way.
+
+## Documentation
+
+The complete API documentation can be found [here](https://smuecke.github.com/qubolite).
 
 ## Version Log
 
 * **0.2** Added problem embeddings (binary clustering, subset sum problem)
 * **0.3** Added `QUBOSample` class and sampling methods `full` and `gibbs`
 * **0.4** Renamed `QUBOSample` to `BinarySample`; added methods for saving and loading QUBO and Sample instances
 * **0.5** Moved `gibbs` to `mcmc` and implemented true Gibbs sampling as `gibbs`; added `numba` as dependency
@@ -84,7 +97,8 @@
     * **0.6.5** complete empirical prob. vector can be returned from `BinarySample`
     * **0.6.6** fixed spectral gap implementation
     * **0.6.7** moved `brute_force` to new sub-module `solving`; added some approximate solving methods
     * **0.6.8** added `bitvec` sub-module; `dynamic_range` now uses bits by default, changed `bits=False` to `decibel=False`; removed scipy from requirements
     * **0.6.9** new, more memory-efficient save format
     * **0.6.10** fixed requirements in `setup.py`; fixed size estimation in `qubo.save()`
 * **0.7** Added more efficient brute-force implementation using C extension; added optional dependencies for calculating bounds and ordering distance
+* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction
```

### Comparing `qubolite-0.7/pyproject.toml` & `qubolite-0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,17 +3,18 @@
     "setuptools>=61.0",
     "numpy>=1.23.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qubolite"
-version = "0.7"
+version = "0.8"
 authors = [
-    { name = "Sascha Mücke", email="sascha.muecke@tu-dortmund.de" }
+    { name = "Sascha Mücke", email="sascha.muecke@tu-dortmund.de" },
+    { name = "Thore Gerlach", email="thore.gerlach@iais.fraunhofer.de" }
 ]
 description = "Toolbox for quadratic binary optimization"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
@@ -27,11 +28,18 @@
 [project.optional-dependencies]
 roof_dual = [
     "igraph>=0.10.4"
 ]
 kendall_tau = [
     "scipy>=1.10.1"
 ]
+embedding = [
+    "scikit-learn>=1.2.2"
+]
+compression = [
+    "portion>=2.4.0"
+]
 all = [
     "igraph>=0.10.4",
+    "portion>=2.4.0",
     "scipy>=1.10.1"
 ]
```

### Comparing `qubolite-0.7/qubolite/_c_utils.c` & `qubolite-0.8/qubolite/_c_utils.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 #include <Python.h>
 #include <math.h>
 #include <numpy/arrayobject.h>
+#include <numpy/random/bitgen.h>
+#include <numpy/random/distributions.h>
 #include <omp.h>
 
 typedef unsigned char bit;
 
+bitgen_t *B = 0;
+
+
 void print_bits(bit *x, size_t n) {
     for (size_t i=0; i<n; ++i)
         printf("%d ", x[i]);
     printf("\n");
 }
 
 double qubo_score(double **qubo, bit *x, size_t n) {
@@ -160,14 +165,28 @@
     PyTuple_SetItem(tup, 1, min_val0_obj);
     PyTuple_SetItem(tup, 2, min_val1_obj);
     if (PyErr_Occurred())
         return NULL;
     return tup;
 }
 
+
+/* ################################################
+ * Gibbs sampling
+ * ################################################ */
+
+int gibbs_sample(double **qubo, bit *state, size_t burn_in, double temp) {
+    return -1;
+}
+
+
+/* ################################################
+ * Python module def                              
+ * ################################################ */
+
 static PyMethodDef methods[] = {
     {"brute_force", py_brute_force, METH_VARARGS, "Solves QUBO the hard way"},
     {NULL, NULL, 0, NULL}
 };
 
 static struct PyModuleDef module = {
     PyModuleDef_HEAD_INIT, "_c_utils",
```

### Comparing `qubolite-0.7/qubolite/misc.py` & `qubolite-0.8/qubolite/_misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 from hashlib   import md5
 from importlib import import_module
 from sys       import stderr
 
 import numpy as np
-from numpy.random import RandomState
 
 from .bitvec import all_bitvectors_array
 
 
 # make warning message more minialistic
 def _custom_showwarning(message, *args, file=None, **kwargs):
     (file or stderr).write(f'Warning: {str(message)}\n')
@@ -38,24 +37,28 @@
 
 def warn_size(n: int, limit: int=30):
     if n > limit:
         warn(f'This operation may take a very long time for n>{limit}.')
 
 
 def get_random_state(state=None):
-    if isinstance(state, RandomState):
-        return state
     if state is None:
-        return RandomState()
+        return np.random.default_rng()
+    if isinstance(state, np.random._generator.Generator):
+        return state
+    if isinstance(state, np.random.RandomState):
+        # for compatibility
+        seed = state.randint(1<<31)
+        return np.random.default_rng(seed)
     try:
         seed = int(state)
     except ValueError:
         # use hash digest when seed is a (non-numerical) string
         seed = int(md5(state.encode('utf-8')).hexdigest(), 16) & 0xffffffff
-    return RandomState(seed)
+    return np.random.default_rng(seed)
 
 
 def set_suffix(filename, suffix):
     s = suffix.strip(' .')
     if filename.lower().endswith('.'+s.lower()):
         return filename
     else:
```

### Comparing `qubolite-0.7/setup.py` & `qubolite-0.8/setup.py`

 * *Files identical despite different names*

