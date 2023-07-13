# Comparing `tmp/sail-0.6.3.tar.gz` & `tmp/sail-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sail-0.6.3.tar", last modified: Sun Jul  9 22:40:16 2023, max compression
+gzip compressed data, was "sail-0.6.4.tar", last modified: Thu Jul 13 21:26:49 2023, max compression
```

## Comparing `sail-0.6.3.tar` & `sail-0.6.4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.576851 sail-0.6.3/
--rw-r--r--   0 dhaval     (501) staff       (20)     1088 2023-06-24 15:16:23.000000 sail-0.6.3/LICENSE
--rw-r--r--   0 dhaval     (501) staff       (20)     4972 2023-07-09 22:40:16.576953 sail-0.6.3/PKG-INFO
--rw-r--r--   0 dhaval     (501) staff       (20)     3859 2023-06-27 22:14:03.000000 sail-0.6.3/README.md
--rw-r--r--   0 dhaval     (501) staff       (20)     1202 2023-06-24 15:16:23.000000 sail-0.6.3/pyproject.toml
--rw-r--r--   0 dhaval     (501) staff       (20)      836 2023-07-09 22:40:16.577308 sail-0.6.3/setup.cfg
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.558366 sail-0.6.3/src/
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.561637 sail-0.6.3/src/sail/
--rw-r--r--   0 dhaval     (501) staff       (20)      226 2023-07-09 22:39:47.000000 sail-0.6.3/src/sail/__init__.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.563290 sail-0.6.3/src/sail/drift_detection/
--rw-r--r--   0 dhaval     (501) staff       (20)     3336 2023-07-09 00:54:44.000000 sail-0.6.3/src/sail/drift_detection/drift_detector.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.563898 sail-0.6.3/src/sail/model_selector/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/model_selector/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4781 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/model_selector/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2082 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/model_selector/holdout_best_model.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2283 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/model_selector/prequential_best_model.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.564236 sail-0.6.3/src/sail/models/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/__init__.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.565217 sail-0.6.3/src/sail/models/auto_ml/
--rw-r--r--   0 dhaval     (501) staff       (20)       44 2023-07-09 00:54:44.000000 sail-0.6.3/src/sail/models/auto_ml/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     7535 2023-07-09 22:10:12.000000 sail-0.6.3/src/sail/models/auto_ml/auto_pipeline.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8222 2023-07-09 22:05:59.000000 sail-0.6.3/src/sail/models/auto_ml/base_strategy.py
--rw-r--r--   0 dhaval     (501) staff       (20)     7352 2023-07-09 22:05:45.000000 sail-0.6.3/src/sail/models/auto_ml/pipeline_strategy.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2709 2023-06-30 13:08:15.000000 sail-0.6.3/src/sail/models/auto_ml/searcher.py
--rw-r--r--   0 dhaval     (501) staff       (20)    20211 2023-07-09 21:47:50.000000 sail-0.6.3/src/sail/models/auto_ml/tune.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1346 2023-06-28 14:12:38.000000 sail-0.6.3/src/sail/models/base.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.566122 sail-0.6.3/src/sail/models/ensemble/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/ensemble/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     9275 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/ensemble/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4153 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/ensemble/distAggregateClassifier.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3648 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/ensemble/distAggregateRegressor.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3907 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/ensemble/distEWARegressor.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.566902 sail-0.6.3/src/sail/models/keras/
--rw-r--r--   0 dhaval     (501) staff       (20)       52 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/keras/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2525 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/keras/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8953 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/keras/oselm.py
--rw-r--r--   0 dhaval     (501) staff       (20)    13781 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/keras/wglstm.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.568230 sail-0.6.3/src/sail/models/native/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)    23813 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4277 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/ielm.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2162 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/isvm.py
--rw-r--r--   0 dhaval     (501) staff       (20)    14132 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/lasvm.py
--rw-r--r--   0 dhaval     (501) staff       (20)    12348 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/learn_pp.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2901 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/native/robust_iml.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.570072 sail-0.6.3/src/sail/models/river/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)       75 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/anomaly.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1073 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3020 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/ensemble.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4351 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/forest.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3340 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/linear_model.py
--rw-r--r--   0 dhaval     (501) staff       (20)      930 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/naive_bayes.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1574 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/river/neighbors.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.570934 sail-0.6.3/src/sail/models/sklearn/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/sklearn/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)      888 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/sklearn/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)       80 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/sklearn/cluster.py
--rw-r--r--   0 dhaval     (501) staff       (20)      399 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/sklearn/linear_model.py
--rw-r--r--   0 dhaval     (501) staff       (20)      143 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/sklearn/naive_bayes.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.573961 sail-0.6.3/src/sail/models/torch/
--rw-r--r--   0 dhaval     (501) staff       (20)       90 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1324 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1807 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/data.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2020 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/fcn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2107 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/fcn_classification.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8676 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/inceptiontime.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1499 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/layers.py
--rw-r--r--   0 dhaval     (501) staff       (20)      985 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/light_lstm.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1813 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/lstm.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2430 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/lstm_fcn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1146 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/nn.py
--rw-r--r--   0 dhaval     (501) staff       (20)    12028 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/onn_hbp.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8576 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/os_cnn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4170 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/rnn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3159 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/rocket.py
--rw-r--r--   0 dhaval     (501) staff       (20)     7826 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/tcn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2018 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/models/torch/utils.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.574254 sail-0.6.3/src/sail/pipeline/
--rw-r--r--   0 dhaval     (501) staff       (20)       34 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/pipeline/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8960 2023-07-09 00:54:44.000000 sail-0.6.3/src/sail/pipeline/pipeline.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.574624 sail-0.6.3/src/sail/transfomers/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/base.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.575209 sail-0.6.3/src/sail/transfomers/river/
--rw-r--r--   0 dhaval     (501) staff       (20)      265 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/river/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2908 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/river/feature_extraction.py
--rw-r--r--   0 dhaval     (501) staff       (20)      961 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/river/feature_selection.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3697 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/river/preprocessing.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.575343 sail-0.6.3/src/sail/transfomers/sklearn/
--rw-r--r--   0 dhaval     (501) staff       (20)     2105 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/transfomers/sklearn/preprocessing.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.576444 sail-0.6.3/src/sail/utils/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/utils/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1009 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/utils/logging.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2024 2023-07-09 21:40:46.000000 sail-0.6.3/src/sail/utils/progress_bar.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2053 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/utils/ray_utils.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4401 2023-07-09 00:54:44.000000 sail-0.6.3/src/sail/utils/scorer.py
--rw-r--r--   0 dhaval     (501) staff       (20)      908 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/utils/serialization.py
--rw-r--r--   0 dhaval     (501) staff       (20)      241 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/utils/stats.py
--rw-r--r--   0 dhaval     (501) staff       (20)      794 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/utils/ts_utils.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.576718 sail-0.6.3/src/sail/visualisation/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/visualisation/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2453 2023-06-24 15:16:23.000000 sail-0.6.3/src/sail/visualisation/ts_plot.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-09 22:40:16.563053 sail-0.6.3/src/sail.egg-info/
--rw-r--r--   0 dhaval     (501) staff       (20)     4972 2023-07-09 22:40:16.000000 sail-0.6.3/src/sail.egg-info/PKG-INFO
--rw-r--r--   0 dhaval     (501) staff       (20)     2960 2023-07-09 22:40:16.000000 sail-0.6.3/src/sail.egg-info/SOURCES.txt
--rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-09 22:40:16.000000 sail-0.6.3/src/sail.egg-info/dependency_links.txt
--rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-05 11:44:37.000000 sail-0.6.3/src/sail.egg-info/not-zip-safe
--rw-r--r--   0 dhaval     (501) staff       (20)      695 2023-07-09 22:40:16.000000 sail-0.6.3/src/sail.egg-info/requires.txt
--rw-r--r--   0 dhaval     (501) staff       (20)        5 2023-07-09 22:40:16.000000 sail-0.6.3/src/sail.egg-info/top_level.txt
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.327736 sail-0.6.4/
+-rw-r--r--   0 dhaval     (501) staff       (20)     1088 2023-07-12 19:00:43.000000 sail-0.6.4/LICENSE
+-rw-r--r--   0 dhaval     (501) staff       (20)     4825 2023-07-13 21:26:49.327831 sail-0.6.4/PKG-INFO
+-rw-r--r--   0 dhaval     (501) staff       (20)     3721 2023-07-12 19:01:03.000000 sail-0.6.4/README.md
+-rw-r--r--   0 dhaval     (501) staff       (20)     1202 2023-07-12 19:00:43.000000 sail-0.6.4/pyproject.toml
+-rw-r--r--   0 dhaval     (501) staff       (20)      794 2023-07-13 21:26:49.328193 sail-0.6.4/setup.cfg
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.310467 sail-0.6.4/src/
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.313265 sail-0.6.4/src/sail/
+-rw-r--r--   0 dhaval     (501) staff       (20)      226 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/__init__.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.314779 sail-0.6.4/src/sail/drift_detection/
+-rw-r--r--   0 dhaval     (501) staff       (20)     3336 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/drift_detection/drift_detector.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.315681 sail-0.6.4/src/sail/model_selector/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4781 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2082 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/holdout_best_model.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2283 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/prequential_best_model.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.316086 sail-0.6.4/src/sail/models/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/__init__.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.317408 sail-0.6.4/src/sail/models/auto_ml/
+-rw-r--r--   0 dhaval     (501) staff       (20)       44 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/auto_ml/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    13943 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/auto_pipeline.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     7896 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/base_strategy.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     7033 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/pipeline_strategy.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2709 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/auto_ml/searcher.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    20259 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/tune.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1346 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/base.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.318491 sail-0.6.4/src/sail/models/ensemble/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     9275 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4153 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/distAggregateClassifier.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3648 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/distAggregateRegressor.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3907 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/distEWARegressor.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.319111 sail-0.6.4/src/sail/models/keras/
+-rw-r--r--   0 dhaval     (501) staff       (20)       52 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2525 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8953 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/oselm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    13781 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/wglstm.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.320187 sail-0.6.4/src/sail/models/native/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    23089 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/native/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4277 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/ielm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2162 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/isvm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    14132 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/lasvm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    12455 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/native/learn_pp.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2901 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/robust_iml.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.321442 sail-0.6.4/src/sail/models/river/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)       75 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/anomaly.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1073 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3020 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/ensemble.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4351 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/forest.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3340 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/linear_model.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      930 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/naive_bayes.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1574 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/neighbors.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.322392 sail-0.6.4/src/sail/models/sklearn/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      888 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)       80 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/cluster.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      399 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/linear_model.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      143 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/naive_bayes.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.324989 sail-0.6.4/src/sail/models/torch/
+-rw-r--r--   0 dhaval     (501) staff       (20)       90 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1324 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1807 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/data.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2020 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/fcn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2107 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/fcn_classification.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8676 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/inceptiontime.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1499 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/layers.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      985 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/light_lstm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1813 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/lstm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2430 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/lstm_fcn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1146 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/nn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    12028 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/onn_hbp.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8576 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/os_cnn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4170 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/rnn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3159 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/rocket.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     7826 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/tcn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2018 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/utils.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.325273 sail-0.6.4/src/sail/pipeline/
+-rw-r--r--   0 dhaval     (501) staff       (20)       34 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/pipeline/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    11789 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/pipeline/pipeline.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.325529 sail-0.6.4/src/sail/transfomers/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/base.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.326045 sail-0.6.4/src/sail/transfomers/river/
+-rw-r--r--   0 dhaval     (501) staff       (20)      265 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2908 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/feature_extraction.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      961 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/feature_selection.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3697 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/preprocessing.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.326182 sail-0.6.4/src/sail/transfomers/sklearn/
+-rw-r--r--   0 dhaval     (501) staff       (20)     2105 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/sklearn/preprocessing.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.327339 sail-0.6.4/src/sail/utils/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1034 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/logging.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2024 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/progress_bar.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2053 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/ray_utils.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4863 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/scorer.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1478 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/serialization.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      241 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/stats.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      794 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/ts_utils.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.327579 sail-0.6.4/src/sail/visualisation/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/visualisation/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2453 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/visualisation/ts_plot.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.314441 sail-0.6.4/src/sail.egg-info/
+-rw-r--r--   0 dhaval     (501) staff       (20)     4825 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/PKG-INFO
+-rw-r--r--   0 dhaval     (501) staff       (20)     2960 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/SOURCES.txt
+-rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/dependency_links.txt
+-rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/not-zip-safe
+-rw-r--r--   0 dhaval     (501) staff       (20)      653 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/requires.txt
+-rw-r--r--   0 dhaval     (501) staff       (20)        5 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/top_level.txt
```

### Comparing `sail-0.6.3/LICENSE` & `sail-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/PKG-INFO` & `sail-0.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sail
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python package for streaming data and incremental learning
 Author-email: Dhaval Salwala <dhaval.vinodbhai.salwala@ibm.com>, Seshu Tirupathi <seshutir@ie.ibm.com>
 License: MIT
 Project-URL: repository, https://github.com/IBM/sail
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
-Provides-Extra: tensorflow_arm64
+Provides-Extra: tfarm64
 Provides-Extra: pytorch
 Provides-Extra: river
 Provides-Extra: ray
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: examples
 Provides-Extra: all
@@ -43,15 +43,15 @@
 
 ## Documentation
 
 See the [**SAIL Wiki**](https://github.com/IBM/sail/wiki) for full documentation, installation guide, operational details and other information.
 
 ## Architecture
 
-### SAIL Pipeline 
+### SAIL Pipeline
 
 ![Architecture](architecture.png)
 
 ### SAIL Model Framework
 
 ![Architecture](model_framework.png)
 
@@ -86,20 +86,14 @@
 - ray
 - dev
 - tests
 - examples : to run notebooks and examples
 - all : all of the above
 - all_arm64 : Apple ARM64 version all of the above
 
-Sail has an additional dependency on Scikit-Multiflow which can be installed as follows:
-
-```sh
-pip install scikit-multiflow==0.5.3
-```
-
 ## ✍️ Examples and Notebooks
 
 Examples and notebooks are located in the `examples` and `notebook` respectively. Please run the below command to install the necessary packages to run examples.
 
 ```sh
 pip install -e ".[examples]"
 ```
```

### Comparing `sail-0.6.3/README.md` & `sail-0.6.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ## Documentation
 
 See the [**SAIL Wiki**](https://github.com/IBM/sail/wiki) for full documentation, installation guide, operational details and other information.
 
 ## Architecture
 
-### SAIL Pipeline 
+### SAIL Pipeline
 
 ![Architecture](architecture.png)
 
 ### SAIL Model Framework
 
 ![Architecture](model_framework.png)
 
@@ -55,20 +55,14 @@
 - ray
 - dev
 - tests
 - examples : to run notebooks and examples
 - all : all of the above
 - all_arm64 : Apple ARM64 version all of the above
 
-Sail has an additional dependency on Scikit-Multiflow which can be installed as follows:
-
-```sh
-pip install scikit-multiflow==0.5.3
-```
-
 ## ✍️ Examples and Notebooks
 
 Examples and notebooks are located in the `examples` and `notebook` respectively. Please run the below command to install the necessary packages to run examples.
 
 ```sh
 pip install -e ".[examples]"
 ```
```

### Comparing `sail-0.6.3/pyproject.toml` & `sail-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/setup.cfg` & `sail-0.6.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [options]
 install_requires = 
 	logzero
 	dill
 	tqdm
-	numpy==1.23.*
+	numpy>=1.23
 	scipy>=1.10
 	pandas>=2.0
 	matplotlib>=3.5.2
 	scikit-learn>=1.2
 
 [options.extras_require]
 tensorflow = 
 	tensorflow>=2.7,<=2.10
-	scikeras>=0.10
+	scikeras
 	tensorflow-addons
-tensorflow_arm64 = 
-	tensorflow-macos>=2.7,<=2.10
-	scikeras==0.11.*
+tfarm64 = 
+	tensorflow-macos>=2.7,<2.10
+	scikeras
 	tensorflow-addons
 pytorch = 
-	torch==2.0.*
-	skorch==0.14.*
+	torch>=2.0
+	skorch
 river = 
 	river==0.14.*
 ray = 
-	ray==2.4.*
+	ray>=2.0,<2.5
 	hyperopt
 	tune_sklearn
 dev = 
 	black
 	pylint
 tests = 
 	pytest
@@ -47,15 +47,15 @@
 	sail[pytorch]
 	sail[river]
 	sail[ray]
 	sail[dev]
 	sail[examples]
 	sail[tests]
 all_arm64 = 
-	sail[tensorflow_arm64]
+	sail[tfarm64]
 	sail[pytorch]
 	sail[river]
 	sail[ray]
 	sail[dev]
 	sail[examples]
 	sail[tests]
```

### Comparing `sail-0.6.3/src/sail/drift_detection/drift_detector.py` & `sail-0.6.4/src/sail/drift_detection/drift_detector.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/model_selector/base.py` & `sail-0.6.4/src/sail/model_selector/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/model_selector/holdout_best_model.py` & `sail-0.6.4/src/sail/model_selector/holdout_best_model.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/model_selector/prequential_best_model.py` & `sail-0.6.4/src/sail/model_selector/prequential_best_model.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/auto_ml/base_strategy.py` & `sail-0.6.4/src/sail/models/auto_ml/base_strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,14 +98,20 @@
         self.incremental_training = incremental_training
 
     def action_separator(self):
         print(
             ">>>--------------------------------------------------------------------------------------------"
         )
 
+    def set_current_action(self, current_action: PipelineAction):
+        self.pipeline_actions.current_action_node = current_action
+
+    def get_current_action(self):
+        return self.pipeline_actions.current_action_node
+
     def next(self, X, y=None, tune_params={}, **fit_params):
         if self.pipeline_actions.current_action == PipelineActionType.DATA_COLLECTION:
             self._collect_data_for_parameter_tuning(X, y)
 
         if (
             self.pipeline_actions.current_action
             == PipelineActionType.FIND_BEST_PIPELINE
@@ -117,47 +123,35 @@
         ):
             self._find_best_pipeline(warm_start=True, **fit_params)
         elif (
             self.pipeline_actions.current_action
             == PipelineActionType.SCORE_AND_DETECT_DRIFT
         ):
             self.action_separator()
-            y_preds = self._best_pipeline.predict(X)
             if self.incremental_training:
-                score = self._best_pipeline._scorer._eval_progressive_score(
-                    y_preds, y, detached=True
-                )
+                score = self._best_pipeline.progressive_score(X, y, detached=True)
             else:
                 score = self._best_pipeline.score(X, y)
 
-            if not self._detect_drift(score, y_preds, y) and self.incremental_training:
+            y_pred = self._best_pipeline.predict(X)
+            if not self._detect_drift(score, y_pred, y) and self.incremental_training:
                 self._partial_fit_pipeline(X, y, **fit_params)
         elif (
             self.pipeline_actions.current_action
             == PipelineActionType.PARTIAL_FIT_PIPELINE
         ):
             self.action_separator()
             self._partial_fit_pipeline(X, y, **fit_params)
         elif (
             self.pipeline_actions.current_action == PipelineActionType.PARTIAL_FIT_MODEL
         ):
             self.action_separator()
-            # if self.incremental_training:
-            #     y_preds = self._best_pipeline.predict(X)
-            #     self._best_pipeline._scorer._eval_progressive_score(
-            #         y_preds, y, verbose=0
-            #     )
             self._partial_fit_model(X, y, **fit_params)
         elif self.pipeline_actions.current_action == PipelineActionType.FIT_MODEL:
             self.action_separator()
-            # if self.incremental_training:
-            #     y_preds = self._best_pipeline.predict(X)
-            #     self._best_pipeline._scorer._eval_progressive_score(
-            #         y_preds, y, verbose=0
-            #     )
             self._fit_model(X, y, **fit_params)
 
     def _collect_data_for_parameter_tuning(self, X, y):
         if not hasattr(self, "_input_X"):
             self._input_X = X
             self._input_y = y
         else:
@@ -189,34 +183,34 @@
             fit_result = self.search_method.fit(
                 X=self._input_X,
                 y=self._input_y,
                 warm_start=warm_start,
                 tune_params=tune_params,
                 **fit_params,
             )
-        except:
+        except Exception as e:
+            LOGGER.debug(e)
             LOGGER.info("Pipeline tuning failed. Disconnecting Ray cluster...")
         finally:
             ray.shutdown()
         LOGGER.info("Pipeline tuning completed. Disconnecting Ray cluster...")
 
         # set best estimator and fit results
         self._best_pipeline = fit_result.best_estimator_
-        self._best_pipeline.log_verbose = 1
+        self._best_pipeline.verbosity = 1
         self._fit_result = fit_result
         LOGGER.info(f"Found best params: {fit_result.best_params}")
 
         # housekeeping
         del self.__dict__["_input_X"]
         del self.__dict__["_input_y"]
 
         self.pipeline_actions.next()
 
     def _partial_fit_pipeline(self, X, y, **fit_params):
-        LOGGER.debug("Partially fitting best pipeline.")
         self._best_pipeline.partial_fit(X, y, **fit_params)
 
     def _partial_fit_model(self, X, y, **fit_params):
         self._best_pipeline.fit_final_estimator(
             X, y, warm_start=True, verbose=1, **fit_params
         )
         self.pipeline_actions.next()
```

### Comparing `sail-0.6.3/src/sail/models/auto_ml/pipeline_strategy.py` & `sail-0.6.4/src/sail/models/auto_ml/pipeline_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,16 +199,7 @@
             PipelineActionType.PARTIAL_FIT_PIPELINE,
             next=PipelineActionType.PARTIAL_FIT_PIPELINE,
         )
 
         LOGGER.info(
             f"Pipeline Strategy [{self.__class__.__name__}] created with actions: {self.pipeline_actions.get_actions()}"
         )
-
-    def _detect_drift(self, *args):
-        if self.drift_detector.detect_drift(*args):
-            LOGGER.info(
-                "Drift Detected in the data. SAIL AutoML will re-start from scratch on the next train()"
-            )
-            self.pipeline_actions.next()
-            return True
-        return False
```

### Comparing `sail-0.6.3/src/sail/models/auto_ml/searcher.py` & `sail-0.6.4/src/sail/models/auto_ml/searcher.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/auto_ml/tune.py` & `sail-0.6.4/src/sail/models/auto_ml/tune.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,28 +70,25 @@
         "pipeline_auto_early_stop": False,
         "keep_best_configurations": 1,
     }
     defined_loggers = ["csv", "json"]
 
     def __init__(
         self,
-        *args,
         num_cpus_per_trial=1,
         num_gpus_per_trial=0,
         keep_best_configurations=1,
         cluster_address=None,
         **kwargs,
     ):
-        super(SAILTuneGridSearchCV, self).__init__(*args, **kwargs)
+        super(SAILTuneGridSearchCV, self).__init__(**kwargs)
         self.keep_best_configurations = keep_best_configurations
         self.cluster_address = cluster_address
-        self.resources_per_trial = {
-            "cpu": num_cpus_per_trial,
-            "gpu": num_gpus_per_trial,
-        }
+        self.num_cpus_per_trial = num_cpus_per_trial
+        self.num_gpus_per_trial = num_gpus_per_trial
 
     def fit(
         self, X, y=None, warm_start=False, groups=None, tune_params=None, **fit_params
     ):
         self.warm_start = warm_start
         return super().fit(X, y, groups, tune_params, **fit_params)
 
@@ -171,16 +168,18 @@
         run_args = dict(
             scheduler=self.early_stopping_,
             reuse_actors=True,
             verbose=self.verbose,
             stop=stopper,
             config=config,
             fail_fast="raise",
-            resources_per_trial=self.resources_per_trial,
-            # local_dir=self.local_dir,
+            resources_per_trial={
+                "cpu": self.num_cpus_per_trial,
+                "gpu": self.num_gpus_per_trial,
+            },
             trial_dirname_creator=lambda trial: f"Trail_{trial.trial_id}",
             name="SAILAutoML_Experiment" + "_" + time.strftime("%d-%m-%Y_%H:%M:%S"),
             callbacks=resolve_logger_callbacks(self.loggers, self.defined_loggers),
             time_budget_s=self.time_budget_s,
             metric=self._metric_name,
             mode=self.mode,
         )
@@ -211,15 +210,15 @@
                 )
             )
 
         run_args = self._override_run_args_with_tune_params(run_args, tune_params)
 
         # Currently, there is a bug where a tqdm logger instance is left unhandled during the Ray Tune. Also, it is an overkill to log Pipeline Training for Distributed Cross Validation. Hence, turning off the verbosity for `SAILPipeline`. This does not affect the Ray Tune logs which can be set via verbose field of tune.run.
         for estimator in estimator_list:
-            estimator.log_verbose = 0
+            estimator.verbosity = 0
 
         trainable = tune.with_parameters(
             trainable,
             X=X,
             y=y,
             estimator_list=estimator_list,
             fit_params=fit_params,
@@ -254,28 +253,25 @@
         "pipeline_auto_early_stop": False,
         "keep_best_configurations": 1,
     }
     defined_loggers = ["csv", "json"]
 
     def __init__(
         self,
-        *args,
         num_cpus_per_trial=1,
         num_gpus_per_trial=0,
         keep_best_configurations=1,
         cluster_address=None,
         **kwargs,
     ):
-        super(SAILTuneSearchCV, self).__init__(*args, **kwargs)
+        super(SAILTuneSearchCV, self).__init__(**kwargs)
         self.keep_best_configurations = keep_best_configurations
         self.cluster_address = cluster_address
-        self.resources_per_trial = {
-            "cpu": num_cpus_per_trial,
-            "gpu": num_gpus_per_trial,
-        }
+        self.num_cpus_per_trial = num_cpus_per_trial
+        self.num_gpus_per_trial = num_gpus_per_trial
 
     def fit(
         self, X, y=None, warm_start=False, groups=None, tune_params=None, **fit_params
     ):
         self.warm_start = warm_start
         return super().fit(X, y, groups, tune_params, **fit_params)
 
@@ -339,15 +335,18 @@
             scheduler=self.early_stopping_,
             reuse_actors=True,
             verbose=self.verbose,
             stop=stopper,
             num_samples=self.n_trials,
             config=config,
             fail_fast="raise",
-            resources_per_trial=self.resources_per_trial,
+            resources_per_trial={
+                "cpu": self.num_cpus_per_trial,
+                "gpu": self.num_gpus_per_trial,
+            },
             local_dir=self.local_dir,
             name="SAILAutoML_Experiment" + "_" + time.strftime("%d-%m-%Y_%H:%M:%S"),
             callbacks=resolve_logger_callbacks(self.loggers, self.defined_loggers),
             time_budget_s=self.time_budget_s,
             metric=self._metric_name,
             mode=self.mode,
         )
@@ -484,15 +483,15 @@
             search_algo = ConcurrencyLimiter(search_algo, max_concurrent=self.n_jobs)
             run_args["search_alg"] = search_algo
 
         run_args = self._override_run_args_with_tune_params(run_args, tune_params)
 
         # Currently, there is a bug where a tqdm logger instance is left unhandled during the Ray Tune. Also, it is an overkill to log Pipeline Training for Distributed Cross Validation. Hence, turning off the verbosity for `SAILPipeline`. This does not affect the Ray Tune logs which can be set via verbose field of tune.run.
         for estimator in estimator_list:
-            estimator.log_verbose = 0
+            estimator.verbosity = 0
 
         trainable = tune.with_parameters(
             trainable, X=X, y=y, estimator_list=estimator_list, fit_params=fit_params
         )
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message="fail_fast='raise' " "detected.")
```

### Comparing `sail-0.6.3/src/sail/models/base.py` & `sail-0.6.4/src/sail/models/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/ensemble/base.py` & `sail-0.6.4/src/sail/models/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/ensemble/distAggregateClassifier.py` & `sail-0.6.4/src/sail/models/ensemble/distAggregateClassifier.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/ensemble/distAggregateRegressor.py` & `sail-0.6.4/src/sail/models/ensemble/distAggregateRegressor.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/ensemble/distEWARegressor.py` & `sail-0.6.4/src/sail/models/ensemble/distEWARegressor.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/keras/base.py` & `sail-0.6.4/src/sail/models/keras/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/keras/oselm.py` & `sail-0.6.4/src/sail/models/keras/oselm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/keras/wglstm.py` & `sail-0.6.4/src/sail/models/keras/wglstm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/native/base.py` & `sail-0.6.4/src/sail/models/native/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """ Base class for all estimators in sail """
 
 # Almost all the code taken from scikit-multiflow
 # https://github.com/scikit-multiflow/scikit-multiflow/blob/a7e316d/src/skmultiflow/core/base.py
 
-from abc import ABCMeta, abstractmethod
-
 import copy
-import warnings
-from collections import defaultdict
 import inspect
 import re
+import warnings
+from abc import ABCMeta, abstractmethod
+from collections import defaultdict
+
+import sklearn
 
+sklearn.set_config(print_changed_only=False)
 import numpy as np
+from sklearn.utils._pprint import _EstimatorPrettyPrinter
 
 __version__ = "0.1.0"
 
 _DEFAULT_TAGS = {
     "non_deterministic": False,
     "requires_positive_data": False,
     "X_types": ["2darray"],
@@ -240,16 +243,14 @@
         return self
 
     def __repr__(self, N_CHAR_MAX=700):
         # N_CHAR_MAX is the (approximate) maximum number of non-blank
         # characters to render. We pass it as an optional parameter to ease
         # the tests.
 
-        from skmultiflow.utils._pprint import _EstimatorPrettyPrinter
-
         N_MAX_ELEMENTS_TO_SHOW = 30  # number of elements to show in sequences
 
         # use ellipsis for sequences with a lot of elements
         pp = _EstimatorPrettyPrinter(
             compact=True,
             indent=1,
             indent_at_name=True,
@@ -294,31 +295,15 @@
     def __getstate__(self):
         try:
             state = super().__getstate__()
         except AttributeError:
             state = self.__dict__.copy()
         return state
 
-        # if type(self).__module__.startswith('skmultiflow.'):
-        #     return dict(state.items(), _skmultiflow_version=__version__)
-        # else:
-        #     return state
-
     def __setstate__(self, state):
-        if type(self).__module__.startswith("skmultiflow."):
-            pickle_version = state.pop("_skmultiflow_version", "pre-0.18")
-            if pickle_version != __version__:
-                warnings.warn(
-                    "Trying to unpickle estimator {0} from version {1} when "
-                    "using version {2}. This might lead to breaking code or "
-                    "invalid results. Use at your own risk.".format(
-                        self.__class__.__name__, pickle_version, __version__
-                    ),
-                    UserWarning,
-                )
         try:
             super().__setstate__(state)
         except AttributeError:
             self.__dict__.update(state)
 
     def _get_tags(self):
         collected_tags = {}
```

### Comparing `sail-0.6.3/src/sail/models/native/ielm.py` & `sail-0.6.4/src/sail/models/native/ielm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/native/isvm.py` & `sail-0.6.4/src/sail/models/native/isvm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/native/lasvm.py` & `sail-0.6.4/src/sail/models/native/lasvm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/native/learn_pp.py` & `sail-0.6.4/src/sail/models/native/learn_pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 # Most of the code from https://github.com/scikit-multiflow/scikit-multiflow/blob/a7e316d/src/skmultiflow/meta/learn_pp.py#L24
 import copy
 import numpy as np
 from sklearn.tree import DecisionTreeClassifier
 from sail.models.native import BaseSailObject, ClassifierMixin, MetaEstimatorMixin
-from skmultiflow.utils import check_random_state
 import warnings
+from sklearn.utils import check_random_state
 
 
-def LearnPP(base_estimator=DecisionTreeClassifier(), error_threshold=0.5, n_estimators=30, n_ensembles=10,
-            window_size=100, random_state=None):     # pragma: no cover
-    warnings.warn("'LearnPP' has been renamed to 'LearnPPClassifier' in v0.5.0.\n"
-                  "The old name will be removed in v0.7.0", category=FutureWarning)
-    return LearnPPClassifier(base_estimator=base_estimator,
-                             error_threshold=error_threshold,
-                             n_estimators=n_estimators,
-                             n_ensembles=n_ensembles,
-                             window_size=window_size,
-                             random_state=random_state)
+def LearnPP(
+    base_estimator=DecisionTreeClassifier(),
+    error_threshold=0.5,
+    n_estimators=30,
+    n_ensembles=10,
+    window_size=100,
+    random_state=None,
+):  # pragma: no cover
+    warnings.warn(
+        "'LearnPP' has been renamed to 'LearnPPClassifier' in v0.5.0.\n"
+        "The old name will be removed in v0.7.0",
+        category=FutureWarning,
+    )
+    return LearnPPClassifier(
+        base_estimator=base_estimator,
+        error_threshold=error_threshold,
+        n_estimators=n_estimators,
+        n_ensembles=n_ensembles,
+        window_size=window_size,
+        random_state=random_state,
+    )
 
 
 class LearnPPClassifier(BaseSailObject, ClassifierMixin, MetaEstimatorMixin):
-    """ Learn++ ensemble classifier.
+    """Learn++ ensemble classifier.
 
     Learn++ [1]_  does not require access to previously used data during
     subsequent incremental learning steps. At the same time, it does not
     forget previously acquired knowledge. Learn++ utilizes an ensemble of
     classifiers by generating multiple hypotheses using training data
     sampled according to carefully tailored distributions.
 
@@ -32,15 +43,15 @@
     ----------
     .. [1] Polikar, Robi and Upda, Lalita and Upda, Satish S and Honavar, Vasant.
        Learn++: An Incremental Learning Algorithm for Supervised Neural Networks.
        IEEE Transactions on Systems Man and Cybernetics Part C (Applications and Reviews), 2002.
 
     Parameters
     ----------
-    base_estimator: skmultiflow.core.BaseSKMObject or sklearn.BaseEstimator (default=DecisionTreeClassifier)
+    base_estimator: sklearn.BaseEstimator (default=DecisionTreeClassifier)
         Each member of the ensemble is an instance of the base estimator.
     n_estimators: int (default=30)
         The number of classifiers per ensemble
     n_ensembles: int (default=10)
         The number of ensembles to keep.
     window_size: int (default=100)
         The size of the training window (batch), in other words, how many instances are kept for training.
@@ -72,20 +83,23 @@
 
     Examples
     --------
     Learn++ classifier performance: 0.9555
 
     """
 
-    def __init__(self, base_estimator=DecisionTreeClassifier(),
-                 error_threshold=0.5,
-                 n_estimators=30,
-                 n_ensembles=10,
-                 window_size=100,
-                 random_state=None):
+    def __init__(
+        self,
+        base_estimator=DecisionTreeClassifier(),
+        error_threshold=0.5,
+        n_estimators=30,
+        n_ensembles=10,
+        window_size=100,
+        random_state=None,
+    ):
         super().__init__()
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.ensembles = []
         self.ensemble_weights = []
         self.classes = None
         self.n_ensembles = n_ensembles
@@ -100,15 +114,15 @@
         self.ensembles = []
         self.ensemble_weights = []
         self.X_batch = []
         self.y_batch = []
         self.random = check_random_state(self.random_state)
 
     def partial_fit(self, X, y, classes=None, sample_weight=None):
-        """ Partially (incrementally) fit the model.
+        """Partially (incrementally) fit the model.
 
         Parameters
         ----------
         X : numpy.ndarray of shape (n_samples, n_features)
             The features to train the model.
 
         y: numpy.ndarray of shape (n_samples)
@@ -133,15 +147,17 @@
         -------
         LearnPPClassifier
             self
         """
 
         if self.classes is None:
             if classes is None:
-                raise RuntimeError("Should pass the classes in the first partial_fit call")
+                raise RuntimeError(
+                    "Should pass the classes in the first partial_fit call"
+                )
             else:
                 self.classes = classes
 
         if classes is not None and self.classes is not None:
             if set(classes) == set(self.classes):
                 pass
             else:
@@ -178,15 +194,14 @@
             sum_dt = np.sum(Dt)
             if sum_dt == 0:  # Early stop in case all instances are correctly classified
                 break
             Dt = Dt / sum_dt
 
             total_error = 1.0
             while total_error >= self.error_threshold:
-
                 # create training and testing subsets according to Dt
                 train_size = int(m / 2)
                 test_size = int(m / 2)
                 train_items_index = self._get_item(items_index, Dt, train_size)
                 test_items_index = self._get_item(items_index, Dt, test_size)
 
                 X_train = X[train_items_index]
@@ -202,29 +217,34 @@
                     ensemble[t].fit(X_train, y_train)
                 except NotImplementedError:
                     ensemble[t].partial_fit(X_train, y_train)
 
                 # predict on the data
                 y_predict = ensemble[t].predict(X_test)
 
-                total_error = self.__compute_error(Dt[test_items_index], y_test, y_predict)
+                total_error = self.__compute_error(
+                    Dt[test_items_index], y_test, y_predict
+                )
 
                 if total_error < self.error_threshold:
-
                     norm_error = total_error / (1 - total_error)
                     normalized_errors[t] = norm_error
 
                     # predict using all hypothesis in the ensemble with majority votes
-                    y_predict_composite = self.__majority_vote(X, t + 1, ensemble, normalized_errors)
+                    y_predict_composite = self.__majority_vote(
+                        X, t + 1, ensemble, normalized_errors
+                    )
 
                     total_error = self.__compute_error(Dt, y, y_predict_composite)
                     if total_error < self.error_threshold:
                         normalize_composite_error = total_error / (1 - total_error)
                         if t < self.n_estimators - 1:
-                            Dt[y_predict_composite == y] = Dt[y_predict_composite == y] * normalize_composite_error
+                            Dt[y_predict_composite == y] = (
+                                Dt[y_predict_composite == y] * normalize_composite_error
+                            )
 
                 if total_error > self.error_threshold:
                     patience += 1
                 else:
                     patience = 0
                 if patience > 1000:
                     raise RuntimeError("Your base estimator is too weak")
@@ -259,15 +279,15 @@
         return res
 
     def __majority_vote(self, X, t, ensemble, normalized_errors):
         res = self.__vote_proba(X, t, ensemble, normalized_errors)
         return np.argmax(res, axis=1)
 
     def predict_proba(self, X):
-        """ Predicts the probability of each sample belonging to each one of the
+        """Predicts the probability of each sample belonging to each one of the
         known classes.
 
         Parameters
         ----------
         X: numpy.ndarray of shape (n_samples, n_features)
             A matrix of the samples we want to predict.
 
@@ -280,19 +300,21 @@
             the probability that the i-th sample of X belongs to a certain label.
 
         """
         votes = np.zeros((len(X), len(self.classes)))
         for i in range(len(self.ensembles)):
             ensemble = self.ensembles[i]
             ensemble_weight = self.ensemble_weights[i]
-            votes += np.array(self.__vote_proba(X, len(ensemble), ensemble, ensemble_weight))
+            votes += np.array(
+                self.__vote_proba(X, len(ensemble), ensemble, ensemble_weight)
+            )
         return votes
 
     def predict(self, X):
-        """ Predict classes for the passed data.
+        """Predict classes for the passed data.
 
         Parameters
         ----------
         X : numpy.ndarray of shape (n_samples, n_features)
             The set of data samples to predict the labels for.
 
         Returns
@@ -306,8 +328,10 @@
         with their weights to find the most likely prediction for the sample matrix X.
 
         """
         votes = self.predict_proba(X)
         return np.argmax(votes, axis=1)
 
     def _get_item(self, items, items_weights, number_of_items):
-        return self.random.choice(items, number_of_items, p=items_weights).astype(np.int32)
+        return self.random.choice(items, number_of_items, p=items_weights).astype(
+            np.int32
+        )
```

### Comparing `sail-0.6.3/src/sail/models/native/robust_iml.py` & `sail-0.6.4/src/sail/models/native/robust_iml.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/river/base.py` & `sail-0.6.4/src/sail/models/river/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/river/ensemble.py` & `sail-0.6.4/src/sail/models/river/ensemble.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/river/forest.py` & `sail-0.6.4/src/sail/models/river/forest.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/river/linear_model.py` & `sail-0.6.4/src/sail/models/river/linear_model.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/river/naive_bayes.py` & `sail-0.6.4/src/sail/models/river/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/river/neighbors.py` & `sail-0.6.4/src/sail/models/river/neighbors.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/sklearn/base.py` & `sail-0.6.4/src/sail/models/sklearn/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/base.py` & `sail-0.6.4/src/sail/models/torch/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/data.py` & `sail-0.6.4/src/sail/models/torch/data.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/fcn.py` & `sail-0.6.4/src/sail/models/torch/fcn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/fcn_classification.py` & `sail-0.6.4/src/sail/models/torch/fcn_classification.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/inceptiontime.py` & `sail-0.6.4/src/sail/models/torch/inceptiontime.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/layers.py` & `sail-0.6.4/src/sail/models/torch/layers.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/light_lstm.py` & `sail-0.6.4/src/sail/models/torch/light_lstm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/lstm.py` & `sail-0.6.4/src/sail/models/torch/lstm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/lstm_fcn.py` & `sail-0.6.4/src/sail/models/torch/lstm_fcn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/nn.py` & `sail-0.6.4/src/sail/models/torch/nn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/onn_hbp.py` & `sail-0.6.4/src/sail/models/torch/onn_hbp.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/os_cnn.py` & `sail-0.6.4/src/sail/models/torch/os_cnn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/rnn.py` & `sail-0.6.4/src/sail/models/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/rocket.py` & `sail-0.6.4/src/sail/models/torch/rocket.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/tcn.py` & `sail-0.6.4/src/sail/models/torch/tcn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/models/torch/utils.py` & `sail-0.6.4/src/sail/models/torch/utils.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/pipeline/pipeline.py` & `sail-0.6.4/src/sail/pipeline/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,86 @@
 import os
 import shutil
-import uuid
 from typing import Any, List, Tuple
+
+import numpy as np
+import pandas as pd
 from sklearn import utils
 from sklearn.base import clone
 from sklearn.pipeline import Pipeline
 from sklearn.utils import _print_elapsed_time
 
 from sail.utils.logging import configure_logger
 from sail.utils.progress_bar import SAILProgressBar
 from sail.utils.scorer import SAILModelScorer
 from sail.utils.serialization import load_obj, save_obj
 
-LOGGER = configure_logger()
+LOGGER = configure_logger(logger_name="SAILPipeline")
 
 
 class SAILPipeline(Pipeline):
     def __init__(
         self,
         steps: List[Tuple[str, Any]],
         scoring=None,
-        verbose: int = 1,
+        verbosity: int = 1,
     ):
         """[summary]
 
         Args:
             steps (list, optional): List of steps for the pipeline, required. Each step is a tuple containing a string, representing the name of a step, and a python object for the step.
             scoring: pipeline score metric
             verbosity: verbosity level for training logs. 0 (No logs) is default.
         """
         super(SAILPipeline, self).__init__(steps, verbose=False)
-        self._uuid = uuid.uuid4()
         self.scoring = scoring
-        self._scorer = SAILModelScorer(
-            scoring=scoring, estimator=steps[-1][1], is_pipeline=True
+        self._scorer = self._validate_and_get_scorer(scoring, steps[-1][1])
+        self.verbosity = verbosity
+
+    def _validate_and_get_scorer(self, scoring, estimator):
+        if scoring is None:
+            estimator_type = (
+                None if estimator == "passthrough" else estimator._estimator_type
+            )
+            assert (
+                estimator_type is not None
+            ), "SAILPipeline.scoring cannot be None when the estimator is set to passthrough in SAILPipeline.steps."
+
+        return SAILModelScorer(
+            scoring=scoring,
+            estimator_type=None
+            if estimator == "passthrough"
+            else estimator._estimator_type,
+            pipeline_mode=True,
         )
-        self.log_verbose = verbose
 
     @property
-    def progressive_score(self):
-        return self._scorer.progressive_score
+    def get_progressive_score(self):
+        return self._scorer.get_progressive_score
 
     def score(self, X, y, sample_weight=1.0):
         y_preds = self.predict(X)
-        score = self._scorer.score(y_preds, y, sample_weight, verbose=self.log_verbose)
-        return score
+        if isinstance(y, pd.Series):
+            y = y.to_numpy()
+        return self._scorer.score(y, y_preds, sample_weight, verbose=self.verbosity)
+
+    def progressive_score(self, X, y, sample_weight=1.0, detached=False, verbose=1):
+        y_pred = self.predict(X)
+        if isinstance(y, pd.Series):
+            y = y.to_numpy()
+        return self._scorer.progressive_score(
+            y, y_pred, sample_weight, detached, verbose
+        )
 
     def fit(self, X, y=None, **fit_params):
         self._fit(X, y, warm_start=False, **fit_params)
 
     def partial_fit(self, X, y=None, **fit_params):
         if self.__sklearn_is_fitted__():
-            y_preds = self.predict(X)
-            self._scorer._eval_progressive_score(y_preds, y, verbose=0)
+            self.progressive_score(X, y, verbose=0)
         self._fit(X, y, warm_start=True, **fit_params)
 
     def _fit(self, X, y=None, warm_start=None, **fit_params):
         Xh = X.copy()
         yh = y.copy()
         fit_params_steps = self._check_fit_params(**fit_params)
         # shallow copy of steps - this should really be steps_
@@ -71,23 +95,22 @@
             elif hasattr(transformer, "fit_transform"):
                 transformed_X = transformer.fit_transform(X, y, **fit_params)
             else:
                 transformed_X = transformer.fit(X, y, **fit_params).transform(X)
             return transformed_X, transformer
 
         fit_transform_one_cached = memory.cache(_fit_transform_one)
-
         with SAILProgressBar(
             steps=len(list(self._iter(with_final=True, filter_passthrough=True))),
             desc=f"SAIL Pipeline Partial fit" if warm_start else f"SAIL Pipeline fit",
             params={
                 "Batch Size": X.shape[0],
             },
             format="pipeline_training",
-            verbose=self.log_verbose,
+            verbose=self.verbosity,
         ) as progress:
             for step_idx, name, transformer in self._iter(
                 with_final=False, filter_passthrough=True
             ):
                 progress.append_desc(f"[{name}]")
                 if transformer is None or transformer == "passthrough":
                     with _print_elapsed_time("Pipeline", self._log_message(step_idx)):
@@ -123,15 +146,15 @@
                     )
                 progress.update()
 
             # update score for fit() call.
             if not warm_start:
                 progress.update_params("Score", self.score(Xh, yh))
             else:
-                progress.update_params("P_Score", self.progressive_score)
+                progress.update_params("P_Score", self.get_progressive_score)
 
         return self
 
     def fit_final_estimator(
         self, X, y, warm_start=False, verbose=0, **fit_params_steps
     ):
         with SAILProgressBar(
@@ -152,40 +175,40 @@
             if warm_start:
                 if not hasattr(self._final_estimator, "partial_fit"):
                     raise AttributeError(
                         f"Final Estimator: '{self.steps[-1][0]}' does not implement partial_fit()."
                     )
                 self._final_estimator.partial_fit(X, y, **fit_params_last_step)
                 progress.update()
-                progress.update_params("P_Score", self.progressive_score)
+                progress.update_params("P_Score", self.get_progressive_score)
             else:
                 if not hasattr(self._final_estimator, "fit"):
                     raise AttributeError(
                         f"Final Estimator '{self.steps[-1][0]}' does not implement fit()."
                     )
                 if "classes" in fit_params_last_step:
                     fit_params_last_step.pop("classes")
                 self._final_estimator.fit(X, y, **fit_params_last_step)
                 progress.update()
                 progress.update_params("Score", self.score(X, y))
 
-    def save(self, model_folder, overwrite=True) -> str:
+    def save(self, model_folder, name="sail_pipeline", overwrite=True) -> str:
         """
         Parameters:
         -----------
         model_folder: str
             location to save the model
         overwrite: bool (False)
             if True and model_folder already exists, it will be delted and recreated
 
         Returns
         -------
         saved_location: str
         """
-        save_location = os.path.join(model_folder, "sail_pipeline")
+        save_location = os.path.join(model_folder, name)
         if not overwrite and os.path.exists(save_location):
             raise Exception(
                 f"{save_location} already exists, specify overwrite=True to replace contents"
             )
         else:
             # delete old folder to avoid unwanted file overlaps
             if os.path.exists(save_location) and os.path.isdir(save_location):
@@ -193,35 +216,84 @@
 
             LOGGER.info(f"making directory tree {save_location}")
             os.makedirs(save_location, exist_ok=True)
             if not os.path.exists(save_location):
                 raise Exception(f"target directory {save_location} can not be created!")
 
         # -------------------------------------------
-        # explicity save all the steps
+        # explicity save all the steps and steps names
         # -------------------------------------------
-        for i, (name, step) in enumerate(self.steps):
+        for i, (step_name, step) in enumerate(self.steps):
             save_obj(
-                obj=step, location=os.path.join(save_location, "steps"), file_name=name
+                obj=step,
+                location=os.path.join(save_location, "steps"),
+                file_name=step_name,
+            )
+        save_obj(
+            obj=[step_name for (step_name, _) in self.steps],
+            location=os.path.join(save_location, "steps"),
+            file_name="steps_meta",
+            serialize_type="json",
+        )
+
+        # -------------------------------------------
+        # save scorer progressive state if present
+        # -------------------------------------------
+        if hasattr(self._scorer, "_y_true"):
+            np.savez(
+                os.path.join(save_location, "scorer_state"),
+                y_true=self._scorer._y_true,
+                y_pred=self._scorer._y_pred,
             )
 
-        # save the complete pipeline which internally calls __getstate__ to
-        # remove unpickled objects
-        save_obj(obj=self, location=save_location, file_name="pipeline")
+        # -------------------------------------------
+        # save rest of the params
+        # -------------------------------------------
+        params = self.get_params(deep=False)
+        params.pop("steps")
+        save_obj(
+            obj=params,
+            location=save_location,
+            file_name="params",
+        )
 
         return save_location
 
     @classmethod
-    def load(cls, model_folder):
-        load_location = os.path.join(model_folder, "sail_pipeline")
-        # load pipeline
-        sail_pipeline = load_obj(location=load_location, file_name="pipeline")
-
-        # load steps to pipeline
-        for i, (name, _) in enumerate(sail_pipeline.steps):
-            step_obj = load_obj(
-                location=os.path.join(load_location, "steps"), file_name=name
-            )
+    def load(cls, model_folder, name="sail_pipeline"):
+        load_location = os.path.join(model_folder, name)
 
-            sail_pipeline.steps[i] = (name, step_obj)
+        # -------------------------------------------
+        # Load steps to add to sail pipeline
+        # -------------------------------------------
+        steps = []
+        steps_location = os.path.join(load_location, "steps")
+        steps_meta = load_obj(
+            location=steps_location,
+            file_name="steps_meta",
+            serialize_type="json",
+        )
+        for step_name in steps_meta:
+            step_obj = load_obj(location=steps_location, file_name=step_name)
+            steps.append((step_name, step_obj))
+
+        # -------------------------------------------
+        # Load params
+        # -------------------------------------------
+        params = load_obj(location=load_location, file_name="params")
+
+        # -------------------------------------------
+        # create pipeline
+        # -------------------------------------------
+        sail_pipeline = SAILPipeline(steps=steps, **params)
+
+        # -------------------------------------------
+        # Pre-load progressive scorer state from initial_points if present.
+        # -------------------------------------------
+        if os.path.exists(os.path.join(load_location, "scorer_state.npz")):
+            initial_points = np.load(os.path.join(load_location, "scorer_state.npz"))
+            sail_pipeline._scorer.progressive_score(
+                initial_points["y_true"], initial_points["y_pred"], verbose=1
+            )
+            initial_points.close()
 
         return sail_pipeline
```

### Comparing `sail-0.6.3/src/sail/transfomers/river/feature_extraction.py` & `sail-0.6.4/src/sail/transfomers/river/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/transfomers/river/feature_selection.py` & `sail-0.6.4/src/sail/transfomers/river/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/transfomers/river/preprocessing.py` & `sail-0.6.4/src/sail/transfomers/river/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/transfomers/sklearn/preprocessing.py` & `sail-0.6.4/src/sail/transfomers/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/utils/logging.py` & `sail-0.6.4/src/sail/utils/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import logging
 import logzero
 import sail
 
 
-def configure_logger(logger_name: str = "", logging_level=sail.get_logging_level()):
+def configure_logger(
+    package_name: str = "SAIL",
+    logger_name: str = "",
+    logging_level=sail.get_logging_level(),
+):
     if logger_name:
         logger_name = " (" + logger_name + ")"
 
     info_log_format = (
         "%(color)s[%(asctime)s:%(msecs)d] - %(levelname)s - "
-        + sail.__package_name__
+        + package_name
         + logger_name
         + " : "
         "%(end_color)s%(message)s"
     )
     rest_log_format = (
         "%(color)s[%(asctime)s:%(msecs)d] - %(levelname)s - "
-        + sail.__package_name__
+        + package_name
         + logger_name
         + " "
         "%(module)s:%(funcName)s:%(lineno)d%(end_color)s %(message)s"
     )
 
     logging_level = logging.getLevelName(logging_level)
     if logging.INFO == logging_level:
```

### Comparing `sail-0.6.3/src/sail/utils/progress_bar.py` & `sail-0.6.4/src/sail/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/utils/ray_utils.py` & `sail-0.6.4/src/sail/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/utils/scorer.py` & `sail-0.6.4/src/sail/utils/scorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,57 @@
+import copy
 import importlib
 import inspect
 import sys
-import copy
+
+import numpy as np
+
 import river
 from river import metrics
+from sympy import public
 
 from sail.utils.progress_bar import SAILProgressBar
 
 
 class SAILModelScorer:
-    def __init__(self, scoring, estimator=None, is_pipeline=False) -> None:
+    def __init__(
+        self,
+        scoring=None,
+        estimator_type=None,
+        sample_weight=1.0,
+        pipeline_mode=False,
+    ) -> None:
         self.scoring = scoring
-        self.estimator = estimator
-        self.is_pipeline = is_pipeline
-        self._scorer = self._resolve_scoring(scoring, estimator)
+        self.estimator_type = estimator_type
+        self.sample_weight = sample_weight
+        self.pipeline_mode = pipeline_mode
+        self._metric = self._resolve_scoring(scoring, estimator_type)
+        self._scorer_type = "Pipeline" if self.pipeline_mode else "Model"
 
     @property
-    def progressive_score(self):
-        return self._scorer.get()
+    def get_progressive_score(self):
+        return self._metric.get()
 
     def get_default_scorer(self, estimator_type):
         if estimator_type == "classifier":
             return metrics.Accuracy()
         elif estimator_type == "regressor":
             return metrics.R2()
         elif estimator_type == "clusterer":
             return metrics.Completeness()
         else:
             raise Exception(
                 "Invalid Estimator type. Last step in the pipeline can only be a regressor, classifier or clusterer"
             )
 
-    def _resolve_scoring(self, scoring, estimator):
+    def _resolve_scoring(self, scoring, estimator_type):
+        assert not (
+            scoring == estimator_type == None
+        ), "Either scoring or estimator_type must be a non null value."
         if scoring is None:
-            estimator_type = (
-                None if estimator == "passthrough" else estimator._estimator_type
-            )
-            assert (
-                estimator_type is not None
-            ), "SAILPipeline.scoring cannot be None when the estimator is set to passthrough in SAILPipeline."
             return self.get_default_scorer(estimator_type)
         try:
             if isinstance(scoring, str):
                 module = importlib.import_module("river.metrics")
                 _scoring_class = getattr(module, scoring)
                 return _scoring_class()
             elif isinstance(scoring, metrics.base.Metric):
@@ -70,52 +79,63 @@
                 if isinstance(scoring, str)
                 else scoring.__class__.__name__
             )
             raise AttributeError(
                 f"Method '{method_name}' is not available in river.metrics. Scoring must be a str or an instance of the {river.metrics.__all__}."
             )
 
-    def score(self, y_preds, y_true, sample_weight=1.0, verbose=1):
-        desc_type = "Pipeline" if self.is_pipeline else "Model"
+    def score(self, y_true, y_pred, sample_weight=None, verbose=1):
         with SAILProgressBar(
-            steps=len(y_preds),
-            desc=f"SAIL {desc_type} Score",
+            steps=len(y_pred),
+            desc=f"SAIL {self._scorer_type} Score",
             params={
-                "Metric": self._scorer.__class__.__qualname__,
-                "Batch Size": len(y_preds),
+                "Metric": self._metric.__class__.__qualname__,
+                "Batch Size": len(y_pred),
             },
             format="scoring",
             verbose=verbose,
         ) as progress:
-            scorer = self._resolve_scoring(self.scoring, self.estimator)
-            for v1, v2 in zip(y_true, y_preds):
+            scorer = self._resolve_scoring(self.scoring, self.estimator_type)
+            if not sample_weight:
+                sample_weight = self.sample_weight
+            for v1, v2 in zip(y_true, y_pred):
                 scorer.update(v1, v2, sample_weight)
                 progress.update()
             progress.update_params("Score", scorer.get())
         return scorer.get()
 
-    def _eval_progressive_score(
-        self, y_preds, y_true, sample_weight=1.0, detached=False, verbose=1
+    def progressive_score(
+        self, y_true, y_pred, sample_weight=None, detached=False, verbose=1
     ):
-        desc_type = "Pipeline" if self.is_pipeline else "Model"
         with SAILProgressBar(
-            steps=len(y_preds),
-            desc=f"SAIL {desc_type} Progressive Score",
+            steps=len(y_pred),
+            desc=f"SAIL {self._scorer_type} Progressive Score",
             params={
-                "Metric": self._scorer.__class__.__qualname__,
-                "Batch Size": len(y_preds),
+                "Metric": self._metric.__class__.__qualname__,
+                "Batch Size": len(y_pred),
             },
             format="scoring",
             verbose=verbose,
         ) as progress:
+            if not hasattr(self, "_y_true"):
+                self._y_true = y_true
+                self._y_pred = y_pred
+            else:
+                self._y_true = np.hstack((self._y_true, y_true))
+                self._y_pred = np.hstack((self._y_pred, y_pred))
+
+            if not sample_weight:
+                sample_weight = self.sample_weight
+
             if detached:
-                scorer = copy.deepcopy(self._scorer)
+                scorer = copy.deepcopy(self._metric)
             else:
-                scorer = self._scorer
-            for v1, v2 in zip(y_true, y_preds):
+                scorer = self._metric
+
+            for v1, v2 in zip(y_true, y_pred):
                 scorer.update(v1, v2, sample_weight)
                 progress.update()
             progress.update_params("P_Score", scorer.get())
         return scorer.get()
 
     def clear(self):
-        self._scorer = self._resolve_scoring()
+        self._metric = self._resolve_scoring(self.scoring, self.estimator_type)
```

### Comparing `sail-0.6.3/src/sail/utils/ts_utils.py` & `sail-0.6.4/src/sail/utils/ts_utils.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail/visualisation/ts_plot.py` & `sail-0.6.4/src/sail/visualisation/ts_plot.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail.egg-info/PKG-INFO` & `sail-0.6.4/src/sail.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sail
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python package for streaming data and incremental learning
 Author-email: Dhaval Salwala <dhaval.vinodbhai.salwala@ibm.com>, Seshu Tirupathi <seshutir@ie.ibm.com>
 License: MIT
 Project-URL: repository, https://github.com/IBM/sail
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
-Provides-Extra: tensorflow_arm64
+Provides-Extra: tfarm64
 Provides-Extra: pytorch
 Provides-Extra: river
 Provides-Extra: ray
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: examples
 Provides-Extra: all
@@ -43,15 +43,15 @@
 
 ## Documentation
 
 See the [**SAIL Wiki**](https://github.com/IBM/sail/wiki) for full documentation, installation guide, operational details and other information.
 
 ## Architecture
 
-### SAIL Pipeline 
+### SAIL Pipeline
 
 ![Architecture](architecture.png)
 
 ### SAIL Model Framework
 
 ![Architecture](model_framework.png)
 
@@ -86,20 +86,14 @@
 - ray
 - dev
 - tests
 - examples : to run notebooks and examples
 - all : all of the above
 - all_arm64 : Apple ARM64 version all of the above
 
-Sail has an additional dependency on Scikit-Multiflow which can be installed as follows:
-
-```sh
-pip install scikit-multiflow==0.5.3
-```
-
 ## ✍️ Examples and Notebooks
 
 Examples and notebooks are located in the `examples` and `notebook` respectively. Please run the below command to install the necessary packages to run examples.
 
 ```sh
 pip install -e ".[examples]"
 ```
```

### Comparing `sail-0.6.3/src/sail.egg-info/SOURCES.txt` & `sail-0.6.4/src/sail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sail-0.6.3/src/sail.egg-info/requires.txt` & `sail-0.6.4/src/sail.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 logzero
 dill
 tqdm
-numpy==1.23.*
+numpy>=1.23
 scipy>=1.10
 pandas>=2.0
 matplotlib>=3.5.2
 scikit-learn>=1.2
 
 [all]
 sail[tensorflow]
@@ -13,15 +13,15 @@
 sail[river]
 sail[ray]
 sail[dev]
 sail[examples]
 sail[tests]
 
 [all_arm64]
-sail[tensorflow_arm64]
+sail[tfarm64]
 sail[pytorch]
 sail[river]
 sail[ray]
 sail[dev]
 sail[examples]
 sail[tests]
 
@@ -34,33 +34,33 @@
 plotly
 nbformat
 seaborn
 gdown
 liac-arff
 
 [pytorch]
-torch==2.0.*
-skorch==0.14.*
+torch>=2.0
+skorch
 
 [ray]
-ray==2.4.*
+ray<2.5,>=2.0
 hyperopt
 tune_sklearn
 
 [river]
 river==0.14.*
 
 [tensorflow]
 tensorflow<=2.10,>=2.7
-scikeras>=0.10
-tensorflow-addons
-
-[tensorflow_arm64]
-tensorflow-macos<=2.10,>=2.7
-scikeras==0.11.*
+scikeras
 tensorflow-addons
 
 [tests]
 pytest
 nbmake
 pytest-xdist
 pytest-console-scripts
+
+[tfarm64]
+tensorflow-macos<2.10,>=2.7
+scikeras
+tensorflow-addons
```

