# Comparing `tmp/gpforecaster-0.3.84.tar.gz` & `tmp/gpforecaster-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpforecaster-0.3.84.tar", last modified: Thu Jul 13 17:30:58 2023, max compression
+gzip compressed data, was "gpforecaster-0.3.9.tar", last modified: Thu Dec 22 10:07:29 2022, max compression
```

## Comparing `gpforecaster-0.3.84.tar` & `gpforecaster-0.3.9.tar`

### file list

```diff
@@ -1,43 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.024580 gpforecaster-0.3.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 17:30:58.024580 gpforecaster-0.3.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.020580 gpforecaster-0.3.84/gpforecaster/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.020580 gpforecaster-0.3.84/gpforecaster/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/model/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    38038 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/model/gpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/model/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/model/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/model/mlls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.020580 gpforecaster-0.3.84/gpforecaster/results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/results/calculate_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.024580 gpforecaster-0.3.84/gpforecaster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_calculate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_model_results_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_model_results_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_results_partial_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_run_model_with_sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_sparse_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_store_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_svg_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/tests/test_tourism_gpf_with_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.024580 gpforecaster-0.3.84/gpforecaster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.024580 gpforecaster-0.3.84/gpforecaster/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/gpforecaster/visualization/plot_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:58.020580 gpforecaster-0.3.84/gpforecaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 17:30:57.000000 gpforecaster-0.3.84/gpforecaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-13 17:30:57.000000 gpforecaster-0.3.84/gpforecaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:30:57.000000 gpforecaster-0.3.84/gpforecaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-13 17:30:57.000000 gpforecaster-0.3.84/gpforecaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 17:30:57.000000 gpforecaster-0.3.84/gpforecaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:30:58.024580 gpforecaster-0.3.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-13 17:30:43.000000 gpforecaster-0.3.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.678177 gpforecaster-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2022-12-22 10:07:29.678177 gpforecaster-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.674177 gpforecaster-0.3.9/gpforecaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.674177 gpforecaster-0.3.9/gpforecaster/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/model/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/model/gpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/model/mean_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.678177 gpforecaster-0.3.9/gpforecaster/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/results/calculate_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.678177 gpforecaster-0.3.9/gpforecaster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/tests/test_calculate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/tests/test_model_results_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/tests/test_model_results_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/tests/test_tourism_gpf_with_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.678177 gpforecaster-0.3.9/gpforecaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/gpforecaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.674177 gpforecaster-0.3.9/gpforecaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2022-12-22 10:07:29.000000 gpforecaster-0.3.9/gpforecaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2022-12-22 10:07:29.000000 gpforecaster-0.3.9/gpforecaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 10:07:29.000000 gpforecaster-0.3.9/gpforecaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-22 10:07:29.000000 gpforecaster-0.3.9/gpforecaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-22 10:07:29.000000 gpforecaster-0.3.9/gpforecaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 10:07:29.678177 gpforecaster-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2022-12-22 10:07:18.000000 gpforecaster-0.3.9/setup.py
```

### Comparing `gpforecaster-0.3.84/PKG-INFO` & `gpforecaster-0.3.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.84
+Version: 0.3.9
 Summary: Hierarchical time series forecasting model using Gaussian Processes
-Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
-License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENCE
 
 A package that allows you to forecast time series datasets with some type of hierarchical structure. The algorithm is implementedusing PyTorch
-
```

### Comparing `gpforecaster-0.3.84/gpforecaster/tests/test_early_stopping.py` & `gpforecaster-0.3.9/gpforecaster/tests/test_calculate_results.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import unittest
-from gpforecaster.model.gpf import GPF
 import tsaugmentation as tsag
-import timeit
+from gpforecaster.model.gpf import GPF
+import shutil
 
 
 class TestModel(unittest.TestCase):
-    def setUp(self):
-        self.data = tsag.preprocessing.PreprocessDatasets("prison", freq='Q').apply_preprocess()
-        self.n = self.data["predict"]["n"]
-        self.s = self.data["train"]["s"]
-        self.gpf = GPF("prison", self.data, log_dir="..")
 
-    def test_early_stopping_fn(self):
-        self.gpf.val_losses = [5.1, 5.2, 4.9, 5.0, 5.1, 5.2]
-        res = self.gpf.early_stopping(self.gpf.val_losses, 2)
-        self.assertTrue(res)
+    def setUp(self):
+        self.data = tsag.preprocessing.PreprocessDatasets('prison').apply_preprocess()
+        self.n = self.data['predict']['n']
+        self.s = self.data['train']['s']
+        shutil.rmtree("./data/original_datasets")
+        self.gpf = GPF('prison', self.data)
 
+    def test_calculate_metrics_dict(self):
+        model, like = self.gpf.train(n_iterations=100)
+        samples = self.gpf.predict(model, like)
+        res = self.gpf.metrics(samples)
+        self.assertLess(res['mase']['bottom'], 2.5)
```

### Comparing `gpforecaster-0.3.84/gpforecaster/tests/test_model_results_police.py` & `gpforecaster-0.3.9/gpforecaster/tests/test_model_results_police.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 from gpforecaster.model.gpf import GPF
 import shutil
 
 
 class TestModel(unittest.TestCase):
 
     def setUp(self):
-        self.data = tsag.preprocessing.PreprocessDatasets('police', top=10, freq='D').apply_preprocess()
+        self.data = tsag.preprocessing.PreprocessDatasets('police', top=10).apply_preprocess()
         self.n = self.data['predict']['n']
         self.s = self.data['train']['s']
         shutil.rmtree("./data/original_datasets")
         self.gpf = GPF('police', self.data, log_dir="..")
 
+    def test_correct_train(self):
+        model, like = self.gpf.train(n_iterations=10)
+        self.assertIsNotNone(model)
+
     def test_predict_shape(self):
-        model, like = self.gpf.train(epochs=10)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        self.assertTrue(preds[0].shape == (self.n, self.s))
+        model, like = self.gpf.train(n_iterations=10)
+        samples = self.gpf.predict(model, like)
+        self.assertTrue(samples.shape == (self.n, self.s, 500))
```

### Comparing `gpforecaster-0.3.84/gpforecaster/tests/test_model_results_prison.py` & `gpforecaster-0.3.9/gpforecaster/tests/test_early_stopping.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,37 @@
-import pickle
 import unittest
-
-import tsaugmentation as tsag
-
 from gpforecaster.model.gpf import GPF
-
+import tsaugmentation as tsag
+import timeit
 
 class TestModel(unittest.TestCase):
     def setUp(self):
-        self.data = tsag.preprocessing.PreprocessDatasets(
-            "prison", freq='Q'
-        ).apply_preprocess()
+        self.data = tsag.preprocessing.PreprocessDatasets("prison").apply_preprocess()
         self.n = self.data["predict"]["n"]
         self.s = self.data["train"]["s"]
-        self.res_type = 'fitpred'
-        self.res_measure = 'mean'
-        self.input_dir = './results/gpf/'
-        self.gpf = GPF("tourism", self.data, input_dir=self.input_dir)
-
-    def test_correct_train(self):
-        model, like = self.gpf.train(epochs=10)
-        self.assertIsNotNone(model)
-
-    def test_predict_shape(self):
-        model, like = self.gpf.train(epochs=10)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        self.assertTrue(preds[0].shape == (self.n, self.s))
-
-    def test_results_interval(self):
-        model, like = self.gpf.train(epochs=100)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        res = self.gpf.metrics(preds[0], preds[1])
-        self.assertLess(res["mase"]["bottom"], 40)
-
-    def test_wall_time(self):
-        model, like = self.gpf.train(epochs=10)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        res = self.gpf.metrics(preds[0], preds[1])
-        self.assertLess(res["wall_time"]["wall_time_total"], 100)
-
-    def test_output_results(self):
-        model, like = self.gpf.train(epochs=10)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        res = self.gpf.metrics(preds[0], preds[1])
-        self.gpf.store_results(res, res_type=self.res_type, res_measure=self.res_measure)
-        with open(
-            f"{self.gpf.input_dir}results_{self.res_type}_{self.res_measure}_gp_{self.gpf.gp_type}_cov_{self.gpf.dataset}_{self.gpf.model_version}.pickle",
-            "rb",
-        ) as handle:
-            output_res = pickle.load(file=handle)
-        self.assertIsNotNone(output_res["mase"]["bottom"])
+        self.gpf = GPF("prison", self.data, log_dir="..")
+
+    def test_early_stopping_fn(self):
+        self.gpf.val_losses = [5.1, 5.2, 4.9, 5.0, 5.1, 5.2]
+        res = self.gpf.early_stopping(2)
+        self.assertTrue(res)
+
+    def test_early_stopping(self):
+        model, like = self.gpf.train(n_iterations=500, track_mem=True)
+        self.gpf.plot_losses()
+        self.assertEqual(len(self.gpf.losses), 500)
+
+    def test_early_stopping_w_patience(self):
+        model, like = self.gpf.train(n_iterations=200, patience=4, track_mem=True)
+        self.gpf.plot_losses()
+        self.assertEqual(len(self.gpf.losses), 131)
+
+    def test_compare_execution_times(self):
+        n_iter = 100
+        elapsed_time_es = timeit.timeit(lambda: self.gpf.train(n_iterations=n_iter, verbose=False), number=1)
+        print(f"Elapsed time with Early Stopping: {elapsed_time_es} seconds")
+        elapsed_time = timeit.timeit(lambda: self.gpf.train(n_iterations=n_iter, early_stopping=False, verbose=False), number=1)
+        print(f"Elapsed time: {elapsed_time} seconds")
+
+    def test_without_early_stopping(self):
+        model, like = self.gpf.train(n_iterations=500, early_stopping=False, track_mem=True)
+        self.assertEqual(len(self.gpf.losses), 500)
```

### Comparing `gpforecaster-0.3.84/gpforecaster/tests/test_tourism_gpf_with_local_file.py` & `gpforecaster-0.3.9/gpforecaster/tests/test_tourism_gpf_with_local_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,35 +3,50 @@
 from gpforecaster.model.gpf import GPF
 import shutil
 
 
 class TestModel(unittest.TestCase):
 
     def setUp(self):
-        self.preproc = tsag.preprocessing.PreprocessDatasets('tourism', test_size=228*10, freq='M')
+        self.preproc = tsag.preprocessing.PreprocessDatasets('tourism', test_size=228*10)
         self.data = self.preproc._tourism()
         self.n = self.data['predict']['n']
         self.s = self.data['train']['s']
-        self.gpf = GPF(dataset='tourism', groups=self.data)
+        self.gpf = GPF(dataset='tourism', groups=self.data,
+                       store_prediction_samples=True,
+                       store_prediction_points=True)
 
     def test_results_mean_and_prediction_interval(self):
-        model, like = self.gpf.train(epochs=10)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        res = self.gpf.metrics(preds[0], preds[1])
+        model, like = self.gpf.train(n_iterations=10)
+        samples = self.gpf.predict(model, like)
+        res = self.gpf.metrics(samples)
 
         # Test shape of results
         self.assertTrue(res['mase']['bottom_ind'].shape == (self.s, ))
         self.assertTrue(res['CRPS']['bottom_ind'].shape == (self.s, ))
         self.assertTrue(res['rmse']['bottom_ind'].shape == (self.s, ))
 
+        # Test shape of predictions
+        # Number of prediction samples for the bottom time series (n_points, n_series, n_samples)
+        self.assertTrue(res['predictions']['samples']['bottom'].shape == (self.n, self.s, 500))
+        self.assertTrue(res['predictions']['points']['bottom'].shape == (self.data['h'], self.s))
+        # Number of prediction samples for the total time series
+        self.assertTrue(res['predictions']['samples']['total'].shape == (self.n, 500))
+        self.assertTrue(res['predictions']['points']['total'].shape == (self.data['h'],))
+        # Test number of objects predicted and stored
+        self.assertTrue(len(res['predictions']['samples']) == 12)
+        self.assertTrue(len(res['predictions']['points']) == 12)
+
     def test_results_mean_and_prediction_interval_without_storing_results(self):
-        self.gpf = GPF(dataset='tourism', groups=self.data)
-        model, like = self.gpf.train(epochs=10)
-        preds, preds_scaled = self.gpf.predict(model, like)
-        res = self.gpf.metrics(preds[0], preds[1])
+        self.gpf = GPF(dataset='tourism', groups=self.data,
+                       store_prediction_samples=False,
+                       store_prediction_points=False)
+        model, like = self.gpf.train(n_iterations=10)
+        samples = self.gpf.predict(model, like)
+        res = self.gpf.metrics(samples)
 
         # Test shape of results
         self.assertTrue(res['mase']['bottom_ind'].shape == (self.s, ))
         self.assertTrue(res['CRPS']['bottom_ind'].shape == (self.s, ))
         self.assertTrue(res['rmse']['bottom_ind'].shape == (self.s, ))
 
         # Test shape of predictions
```

### Comparing `gpforecaster-0.3.84/gpforecaster.egg-info/PKG-INFO` & `gpforecaster-0.3.9/gpforecaster.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.84
+Version: 0.3.9
 Summary: Hierarchical time series forecasting model using Gaussian Processes
-Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
-License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENCE
 
 A package that allows you to forecast time series datasets with some type of hierarchical structure. The algorithm is implementedusing PyTorch
-
```

### Comparing `gpforecaster-0.3.84/gpforecaster.egg-info/SOURCES.txt` & `gpforecaster-0.3.9/gpforecaster.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-LICENCE
 README.md
 setup.py
 gpforecaster/__init__.py
 gpforecaster.egg-info/PKG-INFO
 gpforecaster.egg-info/SOURCES.txt
 gpforecaster.egg-info/dependency_links.txt
 gpforecaster.egg-info/requires.txt
 gpforecaster.egg-info/top_level.txt
 gpforecaster/model/__init__.py
 gpforecaster/model/gp.py
 gpforecaster/model/gpf.py
-gpforecaster/model/hyperparameter_tuning.py
 gpforecaster/model/mean_functions.py
-gpforecaster/model/mlls.py
 gpforecaster/results/__init__.py
 gpforecaster/results/calculate_metrics.py
 gpforecaster/tests/__init__.py
 gpforecaster/tests/test_calculate_results.py
 gpforecaster/tests/test_early_stopping.py
-gpforecaster/tests/test_hyperparameter_tuning.py
 gpforecaster/tests/test_model_results_police.py
 gpforecaster/tests/test_model_results_prison.py
-gpforecaster/tests/test_results_partial_data.py
-gpforecaster/tests/test_run_model_with_sampled_dataset.py
-gpforecaster/tests/test_sparse_gps.py
-gpforecaster/tests/test_store_results.py
-gpforecaster/tests/test_svg_gps.py
 gpforecaster/tests/test_tourism_gpf_with_local_file.py
 gpforecaster/utils/__init__.py
-gpforecaster/utils/logger.py
-gpforecaster/visualization/__init__.py
-gpforecaster/visualization/plot_predictions.py
+gpforecaster/utils/logger.py
```

### Comparing `gpforecaster-0.3.84/setup.py` & `gpforecaster-0.3.9/setup.py`

 * *Files identical despite different names*

