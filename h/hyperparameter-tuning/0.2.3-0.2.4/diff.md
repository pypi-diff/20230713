# Comparing `tmp/hyperparameter-tuning-0.2.3.tar.gz` & `tmp/hyperparameter-tuning-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameter-tuning-0.2.3.tar", last modified: Sat May 13 09:35:14 2023, max compression
+gzip compressed data, was "hyperparameter-tuning-0.2.4.tar", last modified: Thu Jul 13 11:02:00 2023, max compression
```

## Comparing `hyperparameter-tuning-0.2.3.tar` & `hyperparameter-tuning-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 09:35:14.429966 hyperparameter-tuning-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-13 09:35:14.429966 hyperparameter-tuning-0.2.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2420 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 09:35:14.421966 hyperparameter-tuning-0.2.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/requirements/plotting.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 09:35:14.429966 hyperparameter-tuning-0.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 09:35:14.421966 hyperparameter-tuning-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 09:35:14.425966 hyperparameter-tuning-0.2.3/src/hpt/
--rwxr-xr-x   0 runner    (1001) docker     (123)      149 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/binarize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8965 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/evaluation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7252 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/thresholding_evaluation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11728 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 09:35:14.425966 hyperparameter-tuning-0.2.3/src/hpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/classpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/fairness_criteria.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5473 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/load_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3518 2023-05-13 09:35:03.000000 hyperparameter-tuning-0.2.3/src/hpt/utils/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 09:35:14.429966 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-13 09:35:14.000000 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-13 09:35:14.000000 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 09:35:14.000000 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 09:35:14.000000 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-13 09:35:14.000000 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-13 09:35:14.000000 hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:02:00.197348 hyperparameter-tuning-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-13 11:02:00.197348 hyperparameter-tuning-0.2.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2498 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:02:00.193349 hyperparameter-tuning-0.2.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/requirements/plotting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:02:00.197348 hyperparameter-tuning-0.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:02:00.193349 hyperparameter-tuning-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:02:00.197348 hyperparameter-tuning-0.2.4/src/hpt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      149 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/binarize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8972 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/evaluation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7252 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/thresholding_evaluation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12095 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:02:00.197348 hyperparameter-tuning-0.2.4/src/hpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/classpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/fairness_criteria.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5473 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/load_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3518 2023-07-13 11:01:35.000000 hyperparameter-tuning-0.2.4/src/hpt/utils/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:02:00.197348 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-13 11:02:00.000000 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 11:02:00.000000 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:02:00.000000 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:02:00.000000 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-13 11:02:00.000000 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 11:02:00.000000 hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/top_level.txt
```

### Comparing `hyperparameter-tuning-0.2.3/LICENSE` & `hyperparameter-tuning-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/PKG-INFO` & `hyperparameter-tuning-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter-tuning
-Version: 0.2.3
+Version: 0.2.4
 Summary: A minimal framework for running hyperparameter tuning
 Home-page: https://github.com/AndreFCruz/hpt
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,hyperparameter,tuning,fairness
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -47,22 +47,25 @@
 ## Getting started
 
 ```py
 from hpt.tuner import ObjectiveFunction, OptunaTuner
 
 obj_func = ObjectiveFunction(
     X_train, y_train, X_test, y_test,
-    hyperparameter_space=HYPERPARAM_SPACE_PATH,
-    eval_metric='accuracy',
+    hyperparameter_space=HYPERPARAM_SPACE_PATH,    # path to YAML file
+    eval_metric="accuracy",
     s_train=s_train,
     s_val=s_test,
     threshold=0.50,
 )
 
-tuner = OptunaTuner(obj_func) # NOTE: can pass other useful study kwargs here (e.g. storage)
+tuner = OptunaTuner(
+    objective_function=obj_func,
+    direction="maximize",    # NOTE: can pass other useful study kwargs here (e.g. storage)
+)
 
 # Then just run optimize as you would for an optuna.Study object
 tuner.optimize(n_trials=20, n_jobs=4)
 
 # Results are stored in tuner.results
 tuner.results
 ```
```

### Comparing `hyperparameter-tuning-0.2.3/README.md` & `hyperparameter-tuning-0.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 ## Getting started
 
 ```py
 from hpt.tuner import ObjectiveFunction, OptunaTuner
 
 obj_func = ObjectiveFunction(
     X_train, y_train, X_test, y_test,
-    hyperparameter_space=HYPERPARAM_SPACE_PATH,
-    eval_metric='accuracy',
+    hyperparameter_space=HYPERPARAM_SPACE_PATH,    # path to YAML file
+    eval_metric="accuracy",
     s_train=s_train,
     s_val=s_test,
     threshold=0.50,
 )
 
-tuner = OptunaTuner(obj_func) # NOTE: can pass other useful study kwargs here (e.g. storage)
+tuner = OptunaTuner(
+    objective_function=obj_func,
+    direction="maximize",    # NOTE: can pass other useful study kwargs here (e.g. storage)
+)
 
 # Then just run optimize as you would for an optuna.Study object
 tuner.optimize(n_trials=20, n_jobs=4)
 
 # Results are stored in tuner.results
 tuner.results
 ```
```

### Comparing `hyperparameter-tuning-0.2.3/setup.py` & `hyperparameter-tuning-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/binarize.py` & `hyperparameter-tuning-0.2.4/src/hpt/binarize.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/evaluation.py` & `hyperparameter-tuning-0.2.4/src/hpt/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     confidence_percentiles = [low_percentile, 100 - low_percentile]
 
     for m in all_metrics:
         metric_values = [r[m] for r in results]
 
         bt_mean[m] = statistics.mean(metric_values)
         bt_stdev[m] = statistics.stdev(metric_values)
-        bt_percentiles[m] = np.percentile(metric_values, confidence_percentiles)
+        bt_percentiles[m] = tuple(np.percentile(metric_values, confidence_percentiles))
 
     # Construct DF with results
 
     return join_dictionaries(*(
         {
             f"{metric}_bootstrap": bt_mean[metric],
             f"{metric}_stdev_bootstrap": bt_stdev[metric],
```

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/suggest.py` & `hyperparameter-tuning-0.2.4/src/hpt/suggest.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/thresholding_evaluation.py` & `hyperparameter-tuning-0.2.4/src/hpt/thresholding_evaluation.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/tuner.py` & `hyperparameter-tuning-0.2.4/src/hpt/tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     # NOTE: I don't love this constructor API, feels cluttered
     def __init__(
             self,
             X_train,
             y_train,
             X_val,
             y_val,
+            *,
             hyperparameter_space: Union[str, dict],
             eval_metric: str,
             s_train = None,
             s_val = None,
             X_test = None,
             y_test = None,
             s_test = None,
@@ -180,14 +181,20 @@
         self.hyperparameter_space = hyperparameter_space
         if isinstance(hyperparameter_space, (str, Path)):
             self.hyperparameter_space = load_hyperparameter_space(str(hyperparameter_space))
 
         self.eval_metric = eval_metric
         self.other_eval_metric = other_eval_metric
         self.alpha = alpha
+        if self.other_eval_metric is None:
+            self.alpha = 1.0
+            logging.warning(
+                f"Setting `alpha={self.alpha}` as no secondary evaluation "
+                f"metric was provided (`other_eval_metric={self.other_eval_metric}`)."
+            )
         assert alpha is None or (0 <= alpha <= 1)
 
         # Running custom evaluation function
         if eval_func is not None:
             self.eval_func = eval_func
 
         # Using the default evaluation function with the provided threshold target
@@ -331,21 +338,23 @@
     """
 
     def __init__(
             self,
             objective_function: Callable[[BaseTrial], float],
             sampler: Optional[samplers.BaseSampler] = None,
             seed: int = 42,
+            direction: str = "maximize",
             **study_kwargs,
         ):
 
         self.objective_function = objective_function
         self.seed = seed
         self.study = optuna.create_study(
             sampler=(sampler or samplers.RandomSampler(self.seed)),
+            direction=direction,
             **study_kwargs,
         )
 
     @property
     def results(self):
         return self.objective_function.results
```

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/utils/classpath.py` & `hyperparameter-tuning-0.2.4/src/hpt/utils/classpath.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/utils/dict.py` & `hyperparameter-tuning-0.2.4/src/hpt/utils/dict.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/utils/fairness_criteria.py` & `hyperparameter-tuning-0.2.4/src/hpt/utils/fairness_criteria.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/utils/load_yaml.py` & `hyperparameter-tuning-0.2.4/src/hpt/utils/load_yaml.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hpt/utils/trial.py` & `hyperparameter-tuning-0.2.4/src/hpt/utils/trial.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/PKG-INFO` & `hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter-tuning
-Version: 0.2.3
+Version: 0.2.4
 Summary: A minimal framework for running hyperparameter tuning
 Home-page: https://github.com/AndreFCruz/hpt
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,hyperparameter,tuning,fairness
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -47,22 +47,25 @@
 ## Getting started
 
 ```py
 from hpt.tuner import ObjectiveFunction, OptunaTuner
 
 obj_func = ObjectiveFunction(
     X_train, y_train, X_test, y_test,
-    hyperparameter_space=HYPERPARAM_SPACE_PATH,
-    eval_metric='accuracy',
+    hyperparameter_space=HYPERPARAM_SPACE_PATH,    # path to YAML file
+    eval_metric="accuracy",
     s_train=s_train,
     s_val=s_test,
     threshold=0.50,
 )
 
-tuner = OptunaTuner(obj_func) # NOTE: can pass other useful study kwargs here (e.g. storage)
+tuner = OptunaTuner(
+    objective_function=obj_func,
+    direction="maximize",    # NOTE: can pass other useful study kwargs here (e.g. storage)
+)
 
 # Then just run optimize as you would for an optuna.Study object
 tuner.optimize(n_trials=20, n_jobs=4)
 
 # Results are stored in tuner.results
 tuner.results
 ```
```

### Comparing `hyperparameter-tuning-0.2.3/src/hyperparameter_tuning.egg-info/SOURCES.txt` & `hyperparameter-tuning-0.2.4/src/hyperparameter_tuning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

