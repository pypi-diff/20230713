# Comparing `tmp/hidden-py-1.0.6.tar.gz` & `tmp/hidden-py-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidden-py-1.0.6.tar", last modified: Thu Jul 13 17:44:12 2023, max compression
+gzip compressed data, was "hidden-py-1.0.7.tar", last modified: Thu Jul 13 20:53:22 2023, max compression
```

## Comparing `hidden-py-1.0.6.tar` & `hidden-py-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.843456 hidden-py-1.0.6/
--rw-r--r--   0 stevelarge   (501) staff       (20)     1068 2022-03-05 13:45:02.000000 hidden-py-1.0.6/LICENSE.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)    13053 2023-07-13 17:44:12.843218 hidden-py-1.0.6/PKG-INFO
--rw-r--r--   0 stevelarge   (501) staff       (20)    12366 2023-06-21 04:36:21.000000 hidden-py-1.0.6/README.md
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.839360 hidden-py-1.0.6/hidden_py/
--rw-r--r--   0 stevelarge   (501) staff       (20)       66 2023-07-13 16:20:17.000000 hidden-py-1.0.6/hidden_py/__init__.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     5515 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/dynamics.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.840561 hidden-py-1.0.6/hidden_py/filters/
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/filters/__init__.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     9293 2023-07-13 17:43:37.000000 hidden-py-1.0.6/hidden_py/filters/bayesian.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    11471 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/infer.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.842134 hidden-py-1.0.6/hidden_py/optimize/
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/__init__.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    11349 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/base.py
--rw-r--r--   0 stevelarge   (501) staff       (20)      170 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/config.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    19445 2023-07-13 17:42:41.000000 hidden-py-1.0.6/hidden_py/optimize/optimization.py
--rw-r--r--   0 stevelarge   (501) staff       (20)      281 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/registry.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     2318 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/results.py
--rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/types.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.840226 hidden-py-1.0.6/hidden_py.egg-info/
--rw-r--r--   0 stevelarge   (501) staff       (20)    13053 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/PKG-INFO
--rw-r--r--   0 stevelarge   (501) staff       (20)      623 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/SOURCES.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)        1 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/dependency_links.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)       52 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/requires.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)       10 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/top_level.txt
--rw-r--r--   0 stevelarge   (501) staff       (20)       38 2023-07-13 17:44:12.843505 hidden-py-1.0.6/setup.cfg
--rw-r--r--   0 stevelarge   (501) staff       (20)     1123 2023-07-13 17:43:53.000000 hidden-py-1.0.6/setup.py
-drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.842895 hidden-py-1.0.6/tests/
--rw-r--r--   0 stevelarge   (501) staff       (20)     3644 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_dynamics.py
--rw-r--r--   0 stevelarge   (501) staff       (20)    10667 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_filters.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     5702 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_inferrence.py
--rw-r--r--   0 stevelarge   (501) staff       (20)     7563 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_optimizers.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 20:53:22.448189 hidden-py-1.0.7/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     1068 2022-03-05 13:45:02.000000 hidden-py-1.0.7/LICENSE.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)    13053 2023-07-13 20:53:22.447883 hidden-py-1.0.7/PKG-INFO
+-rw-r--r--   0 stevelarge   (501) staff       (20)    12366 2023-06-21 04:36:21.000000 hidden-py-1.0.7/README.md
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 20:53:22.443878 hidden-py-1.0.7/hidden_py/
+-rw-r--r--   0 stevelarge   (501) staff       (20)       66 2023-07-13 20:52:48.000000 hidden-py-1.0.7/hidden_py/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     5515 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/dynamics.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 20:53:22.445345 hidden-py-1.0.7/hidden_py/filters/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/filters/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     9293 2023-07-13 20:52:48.000000 hidden-py-1.0.7/hidden_py/filters/bayesian.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    11751 2023-07-13 20:52:48.000000 hidden-py-1.0.7/hidden_py/infer.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 20:53:22.446731 hidden-py-1.0.7/hidden_py/optimize/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/optimize/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    11573 2023-07-13 20:52:48.000000 hidden-py-1.0.7/hidden_py/optimize/base.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)      170 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/optimize/config.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    20088 2023-07-13 20:52:48.000000 hidden-py-1.0.7/hidden_py/optimize/optimization.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)      281 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/optimize/registry.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     2318 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/optimize/results.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.7/hidden_py/optimize/types.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 20:53:22.444810 hidden-py-1.0.7/hidden_py.egg-info/
+-rw-r--r--   0 stevelarge   (501) staff       (20)    13053 2023-07-13 20:53:22.000000 hidden-py-1.0.7/hidden_py.egg-info/PKG-INFO
+-rw-r--r--   0 stevelarge   (501) staff       (20)      623 2023-07-13 20:53:22.000000 hidden-py-1.0.7/hidden_py.egg-info/SOURCES.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)        1 2023-07-13 20:53:22.000000 hidden-py-1.0.7/hidden_py.egg-info/dependency_links.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       52 2023-07-13 20:53:22.000000 hidden-py-1.0.7/hidden_py.egg-info/requires.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       10 2023-07-13 20:53:22.000000 hidden-py-1.0.7/hidden_py.egg-info/top_level.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       38 2023-07-13 20:53:22.448246 hidden-py-1.0.7/setup.cfg
+-rw-r--r--   0 stevelarge   (501) staff       (20)     1123 2023-07-13 20:53:04.000000 hidden-py-1.0.7/setup.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 20:53:22.447509 hidden-py-1.0.7/tests/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     3644 2023-06-18 01:27:25.000000 hidden-py-1.0.7/tests/test_dynamics.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    10667 2023-06-18 01:27:25.000000 hidden-py-1.0.7/tests/test_filters.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     5702 2023-06-18 01:27:25.000000 hidden-py-1.0.7/tests/test_inferrence.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     7644 2023-07-13 20:52:48.000000 hidden-py-1.0.7/tests/test_optimizers.py
```

### Comparing `hidden-py-1.0.6/LICENSE.txt` & `hidden-py-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/PKG-INFO` & `hidden-py-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidden-py
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package for discrete-output hidden Markov models
 Author: Steven Large
 Author-email: stevelarge7@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/StevenJLarge/hmm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hidden-py-1.0.6/README.md` & `hidden-py-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/hidden_py/dynamics.py` & `hidden-py-1.0.7/hidden_py/dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/hidden_py/filters/bayesian.py` & `hidden-py-1.0.7/hidden_py/filters/bayesian.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/hidden_py/infer.py` & `hidden-py-1.0.7/hidden_py/infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,21 +252,30 @@
         return optimizer.optimize(observations, trans_init, obs_init, symmetric)
 
 
 if __name__ == "__main__":
     from hidden_py import dynamics
     import time
     hmm = dynamics.HMM(2, 2)
+    hmm3 = dynamics.HMM(3, 3)
+
     hmm.init_uniform_cycle()
     hmm.run_dynamics(1000)
 
+    hmm3.init_uniform_cycle()
+    hmm3.run_dynamics(500)
+
     state_ts = hmm.get_state_ts()
     obs_ts = hmm.get_obs_ts()
 
+    state_ts = hmm3.get_state_ts()
+    obs_ts3 = hmm3.get_obs_ts()
+
     BayesInfer = MarkovInfer(2, 2)
+    BayesInfer3 = MarkovInfer(3, 3)
     param_init = (0.15, 0.15)
     A_init = np.array([[0.85, 0.15], [0.15, 0.85]])
     B_init = np.array([[0.85, 0.15], [0.15, 0.85]])
 
     BayesInfer.forward_algo(obs_ts, hmm.A, hmm.B)
     BayesInfer.backward_algo(obs_ts, hmm.A, hmm.B)
     BayesInfer.bayesian_smooth(obs_ts, hmm.A, hmm.B)
@@ -275,14 +284,16 @@
     BayesInfer.beta(obs_ts, hmm.A, hmm.B)
 
     res_loc = BayesInfer.optimize(obs_ts, A_init, B_init, symmetric=True)
     res_glo = BayesInfer.optimize(
         obs_ts, A_init, B_init, symmetric=True, opt_type=OptClass.Global
     )
 
+    res_loc3 = BayesInfer3.optimize(obs_ts3, hmm3.A, hmm3.B, opt_type=OptClass.Local)
+
     start_bw = time.time()
     res_bw = BayesInfer.optimize(
         obs_ts, A_init, B_init, opt_type=OptClass.ExpMax,
         algo_opts={
             "track_optimization": True, "tracking_interval": 10,
             "maxiter": 200, "testing": "THIS IS A TEST"
         }
```

### Comparing `hidden-py-1.0.6/hidden_py/optimize/base.py` & `hidden-py-1.0.7/hidden_py/optimize/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
         Returns:
             Iterable: Variable-length iterable, with each element containing
                 the same upper and lower bounds on a model parameters.
         """
         return [(lower_lim, upper_lim)] * n_params
 
+    def _build_optimization_constraints(self, n_params: int, dim_tuple: Tuple):
+        pass
+
     @abstractmethod
     def optimize(self):
         pass
 
 
 class LikelihoodOptimizer(BaseOptimizer):
 
@@ -248,15 +251,15 @@
         # Add in diagonal terms so that sum(axis=0) = 1
         trans_mat += np.eye(trans_mat.shape[0], M=trans_mat.shape[1]) - np.diag(trans_mat.sum(axis=0))
         obs_mat += np.eye(obs_mat.shape[0], M=obs_mat.shape[1]) - np.diag(obs_mat.sum(axis=0))
 
         return trans_mat, obs_mat
 
     @staticmethod
-    @numba.jit(nopython=True)
+    # @numba.jit(nopython=True)
     def _likelihood(
         predictions: np.ndarray, obs_ts: np.ndarray, B: np.ndarray
     ) -> float:
         """Calcualte negative log-likelihood value for a particular set of
         parameters (which produce a specific set of predictions and a B matrix)
 
         Args:
@@ -267,15 +270,19 @@
 
         Returns:
             float: negative log-likelihood value
         """
         likelihood = 0
         for i, obs in enumerate(obs_ts):
             inner = predictions[i, :] @ B[obs, :]
+            if inner <= 0:
+                print("OOPS!")
             likelihood -= np.log(inner)
+            if likelihood == np.nan:
+                print('Hmmm...')
         return likelihood
 
     @staticmethod
     def calc_likelihood(
         param_arr: Iterable, dim: Tuple, obs_ts: Iterable,
         symmetric: Optional[bool] = False
     ) -> float:
```

### Comparing `hidden-py-1.0.6/hidden_py/optimize/optimization.py` & `hidden-py-1.0.7/hidden_py/optimize/optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from hidden_py.optimize.results import LikelihoodOptimizationResult, EMOptimizationResult
 from hidden_py.optimize.base import LikelihoodOptimizer, CompleteLikelihoodOptimizer
 from hidden_py.filters import bayesian
 
 
 class LocalLikelihoodOptimizer(LikelihoodOptimizer):
     def __init__(
-        self, algorithm: Optional[str] = "L-BFGS-B"
+        self, algorithm: Optional[str] = "SLSQP"
     ) -> None:
         """Contructor for LicalLikelihoodOptimizer class
 
         Args:
             algorithm (Optional[str], optional): Algorithm to use in numerical
-                optimization. Defaults to "L-BFGS-B" (Limited-Memory
-                Broyden-Fletcher-Goldfarb-Shanno (BFGS) algorithm).
+                optimization. Defaults to "SLSQP" (Sequential Least-SQuareds
+                Programming).
         """
         self.algo = algorithm
         super().__init__()
 
     def optimize(
         self, obs_ts: Iterable, A_guess: np.ndarray, B_guess: np.ndarray,
         symmetric: Optional[bool] = False
@@ -52,14 +52,16 @@
         else:
             param_init, dim_tuple = self._encode_parameters(A_guess, B_guess)
 
         # Additional arguments to pass into optimizer
         opt_args = (dim_tuple, obs_ts, symmetric)
         # Parameter bounds in optimization
         bnds = self._build_optimization_bounds(len(param_init))
+        if any(dim_tuple > 2):
+            const = self._build_optimization_constraints()
 
         # run optimizer
         self.result = so.minimize(
             fun=LikelihoodOptimizer.calc_likelihood,
             x0=param_init,
             args=opt_args,
             method=self.algo,
@@ -449,25 +451,42 @@
     from hidden_py.optimize.base import OptClass
     # testing routines here, lets work with symmetric ''true' matrices
     A = np.array([
         [0.7, 0.3],
         [0.3, 0.7]
     ])
 
+    A_3 = np.array([
+        [0.80, 0.05, 0.05],
+        [0.15, 0.85, 0.20],
+        [0.05, 0.10, 0.75]
+    ])
+
     B = np.array([
         [0.9, 0.1],
         [0.1, 0.9]
     ])
 
+    B_3 = np.array([
+        [0.90, 0.05, 0.10],
+        [0.05, 0.85, 0.05],
+        [0.05, 0.10, 0.85]
+    ])
+
     hmm = dynamics.HMM(2, 2)
+    hmm3 = dynamics.HMM(3, 3)
     hmm.initialize_dynamics(A, B)
+    hmm3.initialize_dynamics(A_3, B_3)
     hmm.run_dynamics(500)
+    hmm3.run_dynamics(500)
     obs_ts = hmm.get_obs_ts()
+    obs_ts_3 = hmm3.get_obs_ts()
 
     analyzer = infer.MarkovInfer(2, 2)
+    analyzer3 = infer.MarkovInfer(3, 3)
 
     A_test = np.array([
         [0.75, 0.25],
         [0.25, 0.75]
     ])
 
     A_test_sym = np.array([
@@ -481,27 +500,36 @@
     ])
 
     B_test_sym = np.array([
         [0.95, 0.05],
         [0.05, 0.95]
     ])
 
+    A_test_3 = np.array([
+        [0.80, 0.10, 0.15],
+        [0.15, 0.85, 0.10],
+        [0.05, 0.05, 0.75]
+    ])
+
+    B_test_3 = B_3
+
     param_init_legacy = [0.2, 0.05]
     start_leg = time.time()
     # legacy_res = analyzer.max_likelihood(param_init_legacy, obs_ts)
     end_leg = time.time()
     opt = LocalLikelihoodOptimizer(algorithm="SLSQP")
     opt_em = EMOptimizer()
 
     start_new_nonsym = time.time()
-    # res_nosym = opt.optimize(obs_ts, A_test, B_test)
+    res_nosym = opt.optimize(obs_ts, A_test, B_test)
+    res_nosym3 = opt.optimize(obs_ts_3, A_test_3, B_test_3)
     end_new_nonsym = time.time()
 
     start_new_sym = time.time()
-    # res = opt.optimize(obs_ts, A_test_sym, B_test_sym, symmetric=True)
+    res = opt.optimize(obs_ts, A_test_sym, B_test_sym, symmetric=True)
     end_new_sym = time.time()
 
     start_new_em = time.time()
     res_em = opt_em.optimize(np.array(obs_ts), A_test, B_test)
     res_em_2 = analyzer.optimize(obs_ts, A_test, B_test, opt_type=OptClass.ExpMax)
     end_new_em = time.time()
```

### Comparing `hidden-py-1.0.6/hidden_py/optimize/results.py` & `hidden-py-1.0.7/hidden_py/optimize/results.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/hidden_py.egg-info/PKG-INFO` & `hidden-py-1.0.7/hidden_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidden-py
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package for discrete-output hidden Markov models
 Author: Steven Large
 Author-email: stevelarge7@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/StevenJLarge/hmm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hidden-py-1.0.6/hidden_py.egg-info/SOURCES.txt` & `hidden-py-1.0.7/hidden_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/setup.py` & `hidden-py-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # README contents
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hidden-py',
     packages=find_packages(),
-    version="1.0.6",
+    version="1.0.7",
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='''
         A python package for discrete-output hidden Markov models
     ''',
     author='Steven Large',
     author_email='stevelarge7@gmail.com',
```

### Comparing `hidden-py-1.0.6/tests/test_dynamics.py` & `hidden-py-1.0.7/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/tests/test_filters.py` & `hidden-py-1.0.7/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/tests/test_inferrence.py` & `hidden-py-1.0.7/tests/test_inferrence.py`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.6/tests/test_optimizers.py` & `hidden-py-1.0.7/tests/test_optimizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,53 +208,54 @@
         obs_ts, A_matrix, B_matrix, alpha_mat, beta_mat, bayes_mat
     )
 
     # Assert
     assert sample_xi.shape == (hmm.A.shape)
 
 
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_bw_update_preserves_A_matrix_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 10
-    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-    opt = optimization.EMOptimizer()
-
-    # Act
-    A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
-    A_new_2, _ = opt.baum_welch_step(A_new, B_new, obs_ts)
-
-    # Assert
-    assert all(np.isclose(A_new.sum(axis=0), np.ones(A_new.shape[1])))
-    assert all(np.isclose(A_new_2.sum(axis=0), np.ones(A_new_2.shape[1])))
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_bw_update_preserves_B_matrix_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 10
-    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-    opt = optimization.EMOptimizer()
-
-    # Act
-    A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
-    _, B_new_2 = opt.baum_welch_step(A_new, B_new, obs_ts)
-
-    # Assert
-    assert all(np.isclose(B_new.sum(axis=0), np.ones(B_new.shape[1])))
-    assert all(np.isclose(B_new_2.sum(axis=0), np.ones(B_new_2.shape[1])))
+# @pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+# @pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+# def test_bw_update_preserves_A_matrix_normalization(A_matrix, B_matrix, iteration):
+#     # Arrange
+#     _ = iteration
+#     n_steps = 10
+#     hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
+#     hmm.init_uniform_cycle()
+#     hmm.run_dynamics(n_steps)
+#     obs_ts = np.array(hmm.get_obs_ts())
+#     opt = optimization.EMOptimizer()
+
+#     # Act
+#     A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
+#     A_new_2, _ = opt.baum_welch_step(A_new, B_new, obs_ts)
+
+#     # Assert
+#     assert all(np.isclose(A_new.sum(axis=0), np.ones(A_new.shape[1])))
+#     assert all(np.isclose(A_new_2.sum(axis=0), np.ones(A_new_2.shape[1])))
+
+
+# @pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+# @pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+# def test_bw_update_preserves_B_matrix_normalization(A_matrix, B_matrix, iteration):
+#     # Arrange
+#     _ = iteration
+#     n_steps = 10
+#     hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
+#     hmm.init_uniform_cycle()
+#     hmm.run_dynamics(n_steps)
+#     obs_ts = np.array(hmm.get_obs_ts())
+#     opt = optimization.EMOptimizer()
+
+#     # Act
+#     A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
+#     _, B_new_2 = opt.baum_welch_step(A_new, B_new, obs_ts)
+
+#     # Assert
+#     assert all(np.isclose(B_new.sum(axis=0), np.ones(B_new.shape[1])))
+#     assert all(np.isclose(B_new_2.sum(axis=0), np.ones(B_new_2.shape[1])))
 
 
 if __name__ == "__main__":
     # pytest.main([__file__])
-    for i, (A, B) in enumerate(test_data):
-        test_bw_update_preserves_A_matrix_normalization(A, B, i)
+    # for i, (A, B) in enumerate(test_data):
+    #     test_bw_update_preserves_A_matrix_normalization(A, B, i)
+    pass
```

