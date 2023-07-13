# Comparing `tmp/evodcinv-2.1.0.tar.gz` & `tmp/evodcinv-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodcinv-2.1.0.tar", last modified: Mon Jun  5 20:03:30 2023, max compression
+gzip compressed data, was "evodcinv-2.1.1.tar", last modified: Thu Jul 13 07:09:36 2023, max compression
```

## Comparing `evodcinv-2.1.0.tar` & `evodcinv-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.826051 evodcinv-2.1.0/
--rw-rw-rw-   0        0        0     1546 2023-05-28 06:48:01.000000 evodcinv-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     7013 2023-06-05 20:03:30.826051 evodcinv-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5989 2023-06-05 19:59:55.000000 evodcinv-2.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.797313 evodcinv-2.1.0/evodcinv/
--rw-rw-rw-   0        0        0        5 2023-06-05 18:07:27.000000 evodcinv-2.1.0/evodcinv/VERSION
--rw-rw-rw-   0        0        0      159 2023-06-05 18:08:41.000000 evodcinv-2.1.0/evodcinv/__about__.py
--rw-rw-rw-   0        0        0      305 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/__init__.py
--rw-rw-rw-   0        0        0      110 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_common.py
--rw-rw-rw-   0        0        0     4332 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_curve.py
--rw-rw-rw-   0        0        0      224 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.819531 evodcinv-2.1.0/evodcinv/_io/
--rw-rw-rw-   0        0        0      104 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/__init__.py
--rw-rw-rw-   0        0        0     2672 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.821536 evodcinv-2.1.0/evodcinv/_io/h5/
--rw-rw-rw-   0        0        0      150 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/h5/__init__.py
--rw-rw-rw-   0        0        0     1328 2023-06-05 18:11:52.000000 evodcinv-2.1.0/evodcinv/_io/h5/_h5.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.823536 evodcinv-2.1.0/evodcinv/_io/json/
--rw-rw-rw-   0        0        0      156 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/json/__init__.py
--rw-rw-rw-   0        0        0     1497 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_io/json/_json.py
--rw-rw-rw-   0        0        0     2009 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_layer.py
--rw-rw-rw-   0        0        0    13304 2023-06-05 18:11:52.000000 evodcinv-2.1.0/evodcinv/_model.py
--rw-rw-rw-   0        0        0      641 2023-05-28 06:48:01.000000 evodcinv-2.1.0/evodcinv/_progress.py
--rw-rw-rw-   0        0        0    17413 2023-06-05 18:11:52.000000 evodcinv-2.1.0/evodcinv/_result.py
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.817371 evodcinv-2.1.0/evodcinv.egg-info/
--rw-rw-rw-   0        0        0     7013 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 20:03:30.000000 evodcinv-2.1.0/evodcinv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-05-28 06:48:01.000000 evodcinv-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1271 2023-06-05 20:03:30.838564 evodcinv-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 20:03:30.825043 evodcinv-2.1.0/tests/
--rw-rw-rw-   0        0        0      166 2023-05-28 06:48:01.000000 evodcinv-2.1.0/tests/test_model.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.491620 evodcinv-2.1.1/
+-rw-rw-rw-   0        0        0     1546 2023-05-28 06:48:01.000000 evodcinv-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7013 2023-07-13 07:09:36.491620 evodcinv-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5989 2023-06-05 19:59:55.000000 evodcinv-2.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.456959 evodcinv-2.1.1/evodcinv/
+-rw-rw-rw-   0        0        0        5 2023-07-13 06:46:10.000000 evodcinv-2.1.1/evodcinv/VERSION
+-rw-rw-rw-   0        0        0      159 2023-06-05 18:08:41.000000 evodcinv-2.1.1/evodcinv/__about__.py
+-rw-rw-rw-   0        0        0      305 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_common.py
+-rw-rw-rw-   0        0        0     4332 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_curve.py
+-rw-rw-rw-   0        0        0      224 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.484066 evodcinv-2.1.1/evodcinv/_io/
+-rw-rw-rw-   0        0        0      104 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_io/__init__.py
+-rw-rw-rw-   0        0        0     2672 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_io/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.486631 evodcinv-2.1.1/evodcinv/_io/h5/
+-rw-rw-rw-   0        0        0      150 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_io/h5/__init__.py
+-rw-rw-rw-   0        0        0     1328 2023-06-05 18:11:52.000000 evodcinv-2.1.1/evodcinv/_io/h5/_h5.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.488635 evodcinv-2.1.1/evodcinv/_io/json/
+-rw-rw-rw-   0        0        0      156 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_io/json/__init__.py
+-rw-rw-rw-   0        0        0     1497 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_io/json/_json.py
+-rw-rw-rw-   0        0        0     2009 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_layer.py
+-rw-rw-rw-   0        0        0    14972 2023-07-13 07:03:57.000000 evodcinv-2.1.1/evodcinv/_model.py
+-rw-rw-rw-   0        0        0      641 2023-05-28 06:48:01.000000 evodcinv-2.1.1/evodcinv/_progress.py
+-rw-rw-rw-   0        0        0    17418 2023-07-12 20:48:54.000000 evodcinv-2.1.1/evodcinv/_result.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.481057 evodcinv-2.1.1/evodcinv.egg-info/
+-rw-rw-rw-   0        0        0     7013 2023-07-13 07:09:36.000000 evodcinv-2.1.1/evodcinv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-07-13 07:09:36.000000 evodcinv-2.1.1/evodcinv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:09:36.000000 evodcinv-2.1.1/evodcinv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-07-13 07:09:36.000000 evodcinv-2.1.1/evodcinv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 07:09:36.000000 evodcinv-2.1.1/evodcinv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-05-28 06:48:01.000000 evodcinv-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1271 2023-07-13 07:09:36.499124 evodcinv-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 07:09:36.489620 evodcinv-2.1.1/tests/
+-rw-rw-rw-   0        0        0      822 2023-07-13 06:53:32.000000 evodcinv-2.1.1/tests/test_model.py
```

### Comparing `evodcinv-2.1.0/LICENSE` & `evodcinv-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/PKG-INFO` & `evodcinv-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodcinv
-Version: 2.1.0
+Version: 2.1.1
 Summary: Inversion of dispersion curves using Evolutionary Algorithms
 Home-page: https://github.com/keurfonluu/evodcinv
 Author: Keurfon Luu
 License: BSD 3-Clause License
 Project-URL: Code, https://github.com/keurfonluu/evodcinv
 Project-URL: Issues, https://github.com/keurfonluu/evodcinv/issues
 Platform: any
```

### Comparing `evodcinv-2.1.0/README.rst` & `evodcinv-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_curve.py` & `evodcinv-2.1.1/evodcinv/_curve.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_io/_helpers.py` & `evodcinv-2.1.1/evodcinv/_io/_helpers.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_io/h5/_h5.py` & `evodcinv-2.1.1/evodcinv/_io/h5/_h5.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_io/json/_json.py` & `evodcinv-2.1.1/evodcinv/_io/json/_json.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_layer.py` & `evodcinv-2.1.1/evodcinv/_layer.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_model.py` & `evodcinv-2.1.1/evodcinv/_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from disba import DispersionError, Ellipticity, surf96
 from disba._common import ifunc
 from stochopy.optimize import minimize
+from stochopy.optimize._common import lhs
 
 from ._common import itype
 from ._curve import Curve
 from ._helpers import nafe_drake
 from ._layer import Layer
 from ._progress import ProgressBar
 from ._result import InversionResult
@@ -92,14 +93,15 @@
 
     def configure(
         self,
         optimizer="cpso",
         misfit="rmse",
         density="nafe-drake",
         normalize_weights=True,
+        increasing_velocity=False,
         extra_terms=None,
         dc=0.001,
         dt=0.01,
         optimizer_args=None,
     ):
         """
         Configure misfit function to minimize.
@@ -126,21 +128,23 @@
         density : str or callable, optional, default 'nafe-drake'
             Function to evaluate density. If callable, must be in the form ``f(vp)``, where ``vp`` is the P-wave velocity (in km/s). If str, should be one of:
 
              - 'nafe-drake'
 
         normalize_weights : bool, optional, default True
             If `True`, weights associated to individual misfit terms are normalized.
-        extra_terms : sequence of callable, optional, default True
+        increasing_velocity : bool, optional, default True
+            If `True`, optimize for increasing velocity models. Note that a penalty term is added to `extra_terms`.
+        extra_terms : sequence of callable or None, optional, default None
             Additional misfit terms. Must be a sequence of callables.
         dc : scalar, optional, default 0.001
             Phase velocity increment for root finding.
         dt : scalar, optional, default 0.01
             Frequency increment (%) for calculating group velocity.
-        optimizer_args : dict, optional, default None
+        optimizer_args : dict or None, optional, default None
             A dictionary of solver options. All methods accept the following generic options:
 
              - maxiter (int): maximum number of iterations to perform
              - popsize (int): total population size
              - seed (int or None): seed for random number generator
 
             See :mod:`stochopy`'s documentation for more options.
@@ -185,14 +189,15 @@
         self._configuration = {
             "optimizer": optimizer,
             "misfit": misfit,
             "density": density,
             "dc": dc,
             "dt": dt,
             "normalize_weights": normalize_weights,
+            "increasing_velocity": increasing_velocity,
             "extra_terms": extra_terms,
             "optimizer_args": optimizer_args,
         }
 
     def invert(self, curves, maxrun=1, split_results=False):
         """
         Invert model.
@@ -228,14 +233,15 @@
             "maxiter": 100,
             "popsize": 10,
             "seed": None,
         }
         _optimizer_args.update(optimizer_args)
 
         maxiter = _optimizer_args["maxiter"]
+        popsize = _optimizer_args["popsize"]
 
         # Overwrite options
         constraints = {
             "cmaes": "Penalize",
             "cpso": "Shrink",
             "de": "Random",
             "pso": "Shrink",
@@ -257,26 +263,64 @@
             [
                 [layer.thickness for layer in self._layers[:-1]],
                 [layer.velocity_s for layer in self._layers],
                 [layer.poisson for layer in self._layers],
             ]
         )
 
+        # Increasing velocity models
+        if self._configuration["increasing_velocity"]:
+            # Sample thickness and Poisson's ratio
+            idx = np.concatenate(
+                (
+                    np.arange(self.n_layers - 1),
+                    np.arange(2 * self.n_layers, 3 * self.n_layers) - 1,
+                )
+            )
+            dnu0 = lhs(popsize, idx.size, bounds[idx])
+
+            # Sample S-wave velocity
+            v0 = [np.random.uniform(*self._layers[0].velocity_s, size=popsize).tolist()]
+
+            for layer in self._layers[1:]:
+                vmin, vmax = layer.velocity_s
+                tmp = [np.random.uniform(max(v, vmin), vmax) for v in v0[-1]]
+                v0.append(tmp)
+
+            v0 = np.transpose(v0)
+
+            # Initial population
+            x0 = np.column_stack(
+                (dnu0[:, : self.n_layers - 1], v0, dnu0[:, self.n_layers - 1 :])
+            )
+
+            # Penalty term
+            def constraint(x):
+                vs = x[self.n_layers - 1 : 2 * self.n_layers - 1]
+
+                return 0.0 if (vs[1:] >= vs[:-1]).all() else np.Inf
+
+            self._configuration["extra_terms"].append(constraint)
+
+        else:
+            x0 = None
+
         results = []
         for i in range(maxrun):
             prefix = f"Run {i + 1:<{len(str(maxiter)) - 1}d}"
             with ProgressBar(prefix, max=maxiter) as bar:
 
                 def callback(X, res):
                     bar.misfit = res.fun
                     bar.next()
 
                 x = minimize(
                     func,
                     bounds,
+                    x0=x0,
                     method=method,
                     options=_optimizer_args,
                     callback=callback,
                 )
 
             # Parse output
             popsize = x.xall.shape[1]
```

### Comparing `evodcinv-2.1.0/evodcinv/_progress.py` & `evodcinv-2.1.1/evodcinv/_progress.py`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/evodcinv/_result.py` & `evodcinv-2.1.1/evodcinv/_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
         :class:`evodcinv.InversionResult`
             Inversion results with models that satisfy the threshold criterion.
 
         """
         idx = ~np.isinf(self.misfits) if value is None else self.misfits <= value
 
         return InversionResult(
-            xs=self.xs,
+            xs=self.xs[idx],
             models=self.models[idx],
             misfits=self.misfits[idx],
             global_misfits=self.global_misfits,
             maxiter=self.maxiter,
             popsize=self.popsize,
         )
```

### Comparing `evodcinv-2.1.0/evodcinv.egg-info/PKG-INFO` & `evodcinv-2.1.1/evodcinv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodcinv
-Version: 2.1.0
+Version: 2.1.1
 Summary: Inversion of dispersion curves using Evolutionary Algorithms
 Home-page: https://github.com/keurfonluu/evodcinv
 Author: Keurfon Luu
 License: BSD 3-Clause License
 Project-URL: Code, https://github.com/keurfonluu/evodcinv
 Project-URL: Issues, https://github.com/keurfonluu/evodcinv/issues
 Platform: any
```

### Comparing `evodcinv-2.1.0/evodcinv.egg-info/SOURCES.txt` & `evodcinv-2.1.1/evodcinv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evodcinv-2.1.0/setup.cfg` & `evodcinv-2.1.1/setup.cfg`

 * *Files identical despite different names*

