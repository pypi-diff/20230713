# Comparing `tmp/nyaggle-0.1.5.tar.gz` & `tmp/nyaggle-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nyaggle-0.1.5.tar", last modified: Sat Oct 30 12:27:36 2021, max compression
+gzip compressed data, was "nyaggle-0.1.6.tar", last modified: Thu Jul 13 14:58:22 2023, max compression
```

## Comparing `nyaggle-0.1.5.tar` & `nyaggle-0.1.6.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-10-30 12:27:25.000000 nyaggle-0.1.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-30 12:27:36.000000 nyaggle-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6919 2021-10-30 12:27:25.000000 nyaggle-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-10-30 12:27:25.000000 nyaggle-0.1.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-30 12:27:25.000000 nyaggle-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2021-10-30 12:27:36.000000 nyaggle-0.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/hyper_parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/hyper_parameters/catboost.py
--rw-r--r--   0 runner    (1001) docker     (121)     7557 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/hyper_parameters/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (121)    17152 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/hyper_parameters/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/hyper_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/hyper_parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/feature/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/feature/nlp/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7179 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/nlp/bert.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/groupby.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/feature/category_encoder/
--rw-r--r--   0 runner    (1001) docker     (121)     7615 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/category_encoder/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/category_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature/base.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/validation/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17454 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/validation/split.py
--rw-r--r--   0 runner    (1001) docker     (121)     9751 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/validation/cross_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3716 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/validation/adversarial_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/ensemble/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/ensemble/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/ensemble/stacking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/ensemble/averaging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/feature_store/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6606 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/feature_store/feature_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/experiment/
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/experiment/auto_prep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/experiment/hyperparameter_tuner.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14916 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)    15954 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/experiment/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle/util/
--rw-r--r--   0 runner    (1001) docker     (121)     3571 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/util/traits.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/util/plot_importance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2021-10-30 12:27:25.000000 nyaggle-0.1.5/nyaggle/util/submission.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-30 12:27:36.000000 nyaggle-0.1.5/nyaggle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-30 12:27:25.000000 nyaggle-0.1.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-10-30 12:27:25.000000 nyaggle-0.1.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:36.000000 nyaggle-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 12:27:25.000000 nyaggle-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-10-30 12:27:25.000000 nyaggle-0.1.5/tests/conftest.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1062 2023-07-10 14:23:05.000000 nyaggle-0.1.6/LICENSE
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       53 2023-07-10 14:23:05.000000 nyaggle-0.1.6/MANIFEST.in
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     7536 2023-07-13 14:58:22.344094 nyaggle-0.1.6/PKG-INFO
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     6966 2023-07-10 15:36:11.000000 nyaggle-0.1.6/README.md
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/docs/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       25 2023-07-10 14:23:05.000000 nyaggle-0.1.6/docs/requirements.txt
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       40 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/__init__.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/ensemble/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      110 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/ensemble/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     5503 2023-07-10 15:36:11.000000 nyaggle-0.1.6/nyaggle/ensemble/averaging.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      133 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/ensemble/common.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     4134 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/ensemble/stacking.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1225 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/environment.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/experiment/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      167 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/experiment/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     2696 2023-07-10 15:36:11.000000 nyaggle-0.1.6/nyaggle/experiment/auto_prep.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)    14916 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/experiment/experiment.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     3497 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/experiment/hyperparameter_tuner.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)    15954 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/experiment/run.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/feature/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)        0 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/feature/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      123 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/feature/base.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/feature/category_encoder/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       95 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/feature/category_encoder/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     7617 2023-07-10 15:36:11.000000 nyaggle-0.1.6/nyaggle/feature/category_encoder/target_encoder.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     4376 2023-07-13 14:48:36.000000 nyaggle-0.1.6/nyaggle/feature/groupby.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/feature/nlp/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       60 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/feature/nlp/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     7176 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/feature/nlp/bert.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/feature_store/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      106 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/feature_store/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     6606 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/feature_store/feature_store.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/hyper_parameters/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       88 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/hyper_parameters/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1403 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/hyper_parameters/catboost.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)    17152 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/hyper_parameters/lightgbm.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     2567 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/hyper_parameters/parameters.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     7557 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/hyper_parameters/xgboost.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/testing/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       35 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/testing/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     2531 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/testing/util.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/util/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      174 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/util/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1861 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/util/plot_importance.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1875 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/util/submission.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     3571 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/util/traits.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle/validation/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      262 2023-07-13 14:48:31.000000 nyaggle-0.1.6/nyaggle/validation/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     3716 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/validation/adversarial_validate.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     9751 2023-07-10 14:23:05.000000 nyaggle-0.1.6/nyaggle/validation/cross_validate.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)    17451 2023-07-10 15:36:11.000000 nyaggle-0.1.6/nyaggle/validation/split.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       22 2023-07-13 14:48:36.000000 nyaggle-0.1.6/nyaggle/version.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/nyaggle.egg-info/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     7536 2023-07-13 14:58:22.000000 nyaggle-0.1.6/nyaggle.egg-info/PKG-INFO
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1422 2023-07-13 14:58:22.000000 nyaggle-0.1.6/nyaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)        1 2023-07-13 14:58:22.000000 nyaggle-0.1.6/nyaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      177 2023-07-13 14:58:22.000000 nyaggle-0.1.6/nyaggle.egg-info/requires.txt
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       14 2023-07-13 14:58:22.000000 nyaggle-0.1.6/nyaggle.egg-info/top_level.txt
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       74 2023-07-13 14:48:36.000000 nyaggle-0.1.6/requirements-dev.txt
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      122 2023-07-10 15:36:11.000000 nyaggle-0.1.6/requirements.txt
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)       38 2023-07-13 14:58:22.344094 nyaggle-0.1.6/setup.cfg
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)     1622 2023-07-13 14:48:36.000000 nyaggle-0.1.6/setup.py
+drwxr-xr-x   0 nyanp     (1000) nyanp     (1000)        0 2023-07-13 14:58:22.344094 nyaggle-0.1.6/tests/
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)        0 2023-07-10 14:23:05.000000 nyaggle-0.1.6/tests/__init__.py
+-rw-r--r--   0 nyanp     (1000) nyanp     (1000)      331 2023-07-10 14:23:05.000000 nyaggle-0.1.6/tests/conftest.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nyaggle-0.1.5/setup.py` & `nyaggle-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         'matplotlib',
         'more-itertools',
         'numpy',
         'optuna>=1.0.0',
         'pandas',
         'pyarrow',
         'seaborn',
-        'sklearn',
+        'scikit-learn',
         'tqdm',
         'transformers>=2.3.0',
     ],
 
     extras_require={
         'all': ['catboost>=0.17', 'lightgbm', 'xgboost', 'torch', 'mlflow']
     },
@@ -51,12 +51,13 @@
     url='https://github.com/nyanp/nyaggle',
     description='Code for Kaggle and Offline Competitions.',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     keywords='nyaggle kaggle',
     classifiers=[
         'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ]
 )
```

### Comparing `nyaggle-0.1.5/README.md` & `nyaggle-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 ![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/weekly_test/badge.svg)
 ![Python Versions](https://img.shields.io/pypi/pyversions/nyaggle.svg?logo=python&logoColor=white)
 ![Documentation Status](https://readthedocs.org/projects/nyaggle/badge/?version=latest)
 
 [**Documentation**](https://nyaggle.readthedocs.io/en/latest/index.html)
 | [**Slide (Japanese)**](https://docs.google.com/presentation/d/1jv3J7DISw8phZT4z9rqjM-azdrQ4L4wWJN5P-gKL6fA/edit?usp=sharing)
 
-**nyaggle** is a utility library for Kaggle and offline competitions, 
-particularly focused on experiment tracking, feature engineering and validation.
+**nyaggle** is an utility library for Kaggle and offline competitions. 
+It is particularly focused on experiment tracking, feature engineering, and validation.
 
 - **nyaggle.ensemble** - Averaging & stacking
 - **nyaggle.experiment** - Experiment tracking
 - **nyaggle.feature_store** - Lightweight feature storage using feather-format
 - **nyaggle.features** - sklearn-compatible features
 - **nyaggle.hyper_parameters** - Collection of GBDT hyper-parameters used in past Kaggle competitions
 - **nyaggle.validation** - Adversarial validation & sklearn-compatible CV splitters
 
 ## Installation
 
 You can install nyaggle via pip:
 
-```Shell
-$pip install nyaggle
+```bash
+pip install nyaggle
 ```
 
 ## Examples
 
 ### Experiment Tracking
 
-`run_experiment()` is an high-level API for experiment with cross validation.
+`run_experiment()` is a high-level API for experiments with cross validation.
 It outputs parameters, metrics, out of fold predictions, test predictions,
-feature importance and submission.csv under the specified directory.
+feature importance, and submission.csv under the specified directory.
 
-It can be combined with mlflow tracking.
+To enable mlflow tracking, include the optional `with_mlflow=True` parameter.
 
 ```python
 from sklearn.model_selection import train_test_split
 
 from nyaggle.experiment import run_experiment
 from nyaggle.testing import make_classification_df
 
@@ -51,15 +51,15 @@
 }
 
 result = run_experiment(params,
                         X_train,
                         y_train,
                         X_test)
 
-# You can get outputs that needed in data science competitions with 1 API
+# You can get outputs that are needed in data science competitions with 1 API
 
 print(result.test_prediction)  # Test prediction in numpy array
 print(result.oof_prediction)   # Out-of-fold prediction in numpy array
 print(result.models)           # Trained models for each fold
 print(result.importance)       # Feature importance for each fold
 print(result.metrics)          # Evalulation metrics for each fold
 print(result.time)             # Elapsed time
@@ -130,15 +130,15 @@
 # ... or just call fit_transform to concatenated data
 all.loc[:, cat_cols] = te.fit_transform(all[cat_cols], all[cat_cols])
 ```
 
 #### Text Vectorization using BERT
 
 You need to install pytorch to your virtual environment to use BertSentenceVectorizer. 
-MaCab and mecab-python3 are also required if you use Japanese BERT model.
+MaCab and mecab-python3 are also required if you use the Japanese BERT model.
 
 ```python
 import pandas as pd
 from nyaggle.feature.nlp import BertSentenceVectorizer
 
 
 train = pd.read_csv('train.csv')
@@ -179,15 +179,15 @@
 
 auc, importance = adversarial_validate(train, test, importance_type='gain')
 
 ```
 
 ### Validation Splitters
 
-nyaggle provides a set of validation splitters that compatible with sklean interface.
+nyaggle provides a set of validation splitters that are compatible with sklearn.
 
 ```python
 import pandas as pd
 from sklearn.model_selection import cross_validate, KFold
 from nyaggle.validation import TimeSeriesSplit, Take, Skip, Nth
 
 train = pd.read_csv('train.csv', parse_dates='dt')
```

### Comparing `nyaggle-0.1.5/PKG-INFO` & `nyaggle-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,240 +1,241 @@
 Metadata-Version: 2.1
 Name: nyaggle
-Version: 0.1.5
+Version: 0.1.6
 Summary: Code for Kaggle and Offline Competitions.
 Home-page: https://github.com/nyanp/nyaggle
 Author: nyanp
 Author-email: Noumi.Taiga@gmail.com
 License: MIT
-Description: # nyaggle
-        
-        ![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/Python%20package/badge.svg)
-        ![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/weekly_test/badge.svg)
-        ![Python Versions](https://img.shields.io/pypi/pyversions/nyaggle.svg?logo=python&logoColor=white)
-        ![Documentation Status](https://readthedocs.org/projects/nyaggle/badge/?version=latest)
-        
-        [**Documentation**](https://nyaggle.readthedocs.io/en/latest/index.html)
-        | [**Slide (Japanese)**](https://docs.google.com/presentation/d/1jv3J7DISw8phZT4z9rqjM-azdrQ4L4wWJN5P-gKL6fA/edit?usp=sharing)
-        
-        **nyaggle** is a utility library for Kaggle and offline competitions, 
-        particularly focused on experiment tracking, feature engineering and validation.
-        
-        - **nyaggle.ensemble** - Averaging & stacking
-        - **nyaggle.experiment** - Experiment tracking
-        - **nyaggle.feature_store** - Lightweight feature storage using feather-format
-        - **nyaggle.features** - sklearn-compatible features
-        - **nyaggle.hyper_parameters** - Collection of GBDT hyper-parameters used in past Kaggle competitions
-        - **nyaggle.validation** - Adversarial validation & sklearn-compatible CV splitters
-        
-        ## Installation
-        
-        You can install nyaggle via pip:
-        
-        ```Shell
-        $pip install nyaggle
-        ```
-        
-        ## Examples
-        
-        ### Experiment Tracking
-        
-        `run_experiment()` is an high-level API for experiment with cross validation.
-        It outputs parameters, metrics, out of fold predictions, test predictions,
-        feature importance and submission.csv under the specified directory.
-        
-        It can be combined with mlflow tracking.
-        
-        ```python
-        from sklearn.model_selection import train_test_split
-        
-        from nyaggle.experiment import run_experiment
-        from nyaggle.testing import make_classification_df
-        
-        X, y = make_classification_df()
-        X_train, X_test, y_train, y_test = train_test_split(X, y)
-        
-        params = {
-            'n_estimators': 1000,
-            'max_depth': 8
-        }
-        
-        result = run_experiment(params,
-                                X_train,
-                                y_train,
-                                X_test)
-        
-        # You can get outputs that needed in data science competitions with 1 API
-        
-        print(result.test_prediction)  # Test prediction in numpy array
-        print(result.oof_prediction)   # Out-of-fold prediction in numpy array
-        print(result.models)           # Trained models for each fold
-        print(result.importance)       # Feature importance for each fold
-        print(result.metrics)          # Evalulation metrics for each fold
-        print(result.time)             # Elapsed time
-        print(result.submission_df)    # The output dataframe saved as submission.csv
-        
-        # ...and all outputs have been saved under the logging directory (default: output/yyyymmdd_HHMMSS).
-        
-        
-        # You can use it with mlflow and track your experiments through mlflow-ui
-        result = run_experiment(params,
-                                X_train,
-                                y_train,
-                                X_test,
-                                with_mlflow=True)
-        ```
-        
-        nyaggle also has a low-level API which has similar interface to
-        [mlflow tracking](https://www.mlflow.org/docs/latest/tracking.html) and [wandb](https://www.wandb.com/).
-        
-        ```python
-        from nyaggle.experiment import Experiment
-        
-        with Experiment(logging_directory='./output/') as exp:
-            # log key-value pair as a parameter
-            exp.log_param('lr', 0.01)
-            exp.log_param('optimizer', 'adam')
-        
-            # log text
-            exp.log('blah blah blah')
-        
-            # log metric
-            exp.log_metric('CV', 0.85)
-        
-            # log numpy ndarray, pandas dafaframe and any artifacts
-            exp.log_numpy('predicted', predicted)
-            exp.log_dataframe('submission', sub, file_format='csv')
-            exp.log_artifact('path-to-your-file')
-        ```
-        
-        ### Feature Engineering
-        
-        #### Target Encoding with K-Fold
-        
-        ```python
-        import pandas as pd
-        import numpy as np
-        
-        from sklearn.model_selection import KFold
-        from nyaggle.feature.category_encoder import TargetEncoder
-        
-        
-        train = pd.read_csv('train.csv')
-        test = pd.read_csv('test.csv')
-        all = pd.concat([train, test]).copy()
-        
-        cat_cols = [c for c in train.columns if train[c].dtype == np.object]
-        target_col = 'y'
-        
-        kf = KFold(5)
-        
-        # Target encoding with K-fold
-        te = TargetEncoder(kf.split(train))
-        
-        # use fit/fit_transform to train data, then apply transform to test data
-        train.loc[:, cat_cols] = te.fit_transform(train[cat_cols], train[target_col])
-        test.loc[:, cat_cols] = te.transform(test[cat_cols])
-        
-        # ... or just call fit_transform to concatenated data
-        all.loc[:, cat_cols] = te.fit_transform(all[cat_cols], all[cat_cols])
-        ```
-        
-        #### Text Vectorization using BERT
-        
-        You need to install pytorch to your virtual environment to use BertSentenceVectorizer. 
-        MaCab and mecab-python3 are also required if you use Japanese BERT model.
-        
-        ```python
-        import pandas as pd
-        from nyaggle.feature.nlp import BertSentenceVectorizer
-        
-        
-        train = pd.read_csv('train.csv')
-        test = pd.read_csv('test.csv')
-        all = pd.concat([train, test]).copy()
-        
-        text_cols = ['body']
-        target_col = 'y'
-        group_col = 'user_id'
-        
-        
-        # extract BERT-based sentence vector
-        bv = BertSentenceVectorizer(text_columns=text_cols)
-        
-        text_vector = bv.fit_transform(train)
-        
-        
-        # BERT + SVD, with cuda
-        bv = BertSentenceVectorizer(text_columns=text_cols, use_cuda=True, n_components=40)
-        
-        text_vector_svd = bv.fit_transform(train)
-        
-        # Japanese BERT
-        bv = BertSentenceVectorizer(text_columns=text_cols, lang='jp')
-        
-        japanese_text_vector = bv.fit_transform(train)
-        ```
-        
-        
-        ### Adversarial Validation
-        
-        ```python
-        import pandas as pd
-        from nyaggle.validation import adversarial_validate
-        
-        train = pd.read_csv('train.csv')
-        test = pd.read_csv('test.csv')
-        
-        auc, importance = adversarial_validate(train, test, importance_type='gain')
-        
-        ```
-        
-        ### Validation Splitters
-        
-        nyaggle provides a set of validation splitters that compatible with sklean interface.
-        
-        ```python
-        import pandas as pd
-        from sklearn.model_selection import cross_validate, KFold
-        from nyaggle.validation import TimeSeriesSplit, Take, Skip, Nth
-        
-        train = pd.read_csv('train.csv', parse_dates='dt')
-        
-        # time-series split
-        ts = TimeSeriesSplit(train['dt'])
-        ts.add_fold(train_interval=('2019-01-01', '2019-01-10'), test_interval=('2019-01-10', '2019-01-20'))
-        ts.add_fold(train_interval=('2019-01-06', '2019-01-15'), test_interval=('2019-01-15', '2019-01-25'))
-        
-        cross_validate(..., cv=ts)
-        
-        # take the first 3 folds out of 10
-        cross_validate(..., cv=Take(3, KFold(10)))
-        
-        # skip the first 3 folds, and evaluate the remaining 7 folds
-        cross_validate(..., cv=Skip(3, KFold(10)))
-        
-        # evaluate 1st fold
-        cross_validate(..., cv=Nth(1, ts))
-        
-        ```
-        
-        ### Other Awesome Repositories
-        
-        Here is a list of awesome repositories that provide general utility functions for data science competitions.
-        Please let me know if you have another one :)
-        
-        - [jeongyoonlee/Kaggler](https://github.com/jeongyoonlee/Kaggler)
-        - [mxbi/mlcrate](https://github.com/mxbi/mlcrate)
-        - [analokmaus/kuma_utils](https://github.com/analokmaus/kuma_utils)
-        - [Far0n/kaggletils](https://github.com/Far0n/kaggletils)
-        - [MLWave/Kaggle-Ensemble-Guide](https://github.com/MLWave/Kaggle-Ensemble-Guide)
-        - [rushter/heamy](https://github.com/rushter/heamy)
-        
 Keywords: nyaggle kaggle
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: all
+License-File: LICENSE
+
+# nyaggle
+
+![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/Python%20package/badge.svg)
+![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/weekly_test/badge.svg)
+![Python Versions](https://img.shields.io/pypi/pyversions/nyaggle.svg?logo=python&logoColor=white)
+![Documentation Status](https://readthedocs.org/projects/nyaggle/badge/?version=latest)
+
+[**Documentation**](https://nyaggle.readthedocs.io/en/latest/index.html)
+| [**Slide (Japanese)**](https://docs.google.com/presentation/d/1jv3J7DISw8phZT4z9rqjM-azdrQ4L4wWJN5P-gKL6fA/edit?usp=sharing)
+
+**nyaggle** is an utility library for Kaggle and offline competitions. 
+It is particularly focused on experiment tracking, feature engineering, and validation.
+
+- **nyaggle.ensemble** - Averaging & stacking
+- **nyaggle.experiment** - Experiment tracking
+- **nyaggle.feature_store** - Lightweight feature storage using feather-format
+- **nyaggle.features** - sklearn-compatible features
+- **nyaggle.hyper_parameters** - Collection of GBDT hyper-parameters used in past Kaggle competitions
+- **nyaggle.validation** - Adversarial validation & sklearn-compatible CV splitters
+
+## Installation
+
+You can install nyaggle via pip:
+
+```bash
+pip install nyaggle
+```
+
+## Examples
+
+### Experiment Tracking
+
+`run_experiment()` is a high-level API for experiments with cross validation.
+It outputs parameters, metrics, out of fold predictions, test predictions,
+feature importance, and submission.csv under the specified directory.
+
+To enable mlflow tracking, include the optional `with_mlflow=True` parameter.
+
+```python
+from sklearn.model_selection import train_test_split
+
+from nyaggle.experiment import run_experiment
+from nyaggle.testing import make_classification_df
+
+X, y = make_classification_df()
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+params = {
+    'n_estimators': 1000,
+    'max_depth': 8
+}
+
+result = run_experiment(params,
+                        X_train,
+                        y_train,
+                        X_test)
+
+# You can get outputs that are needed in data science competitions with 1 API
+
+print(result.test_prediction)  # Test prediction in numpy array
+print(result.oof_prediction)   # Out-of-fold prediction in numpy array
+print(result.models)           # Trained models for each fold
+print(result.importance)       # Feature importance for each fold
+print(result.metrics)          # Evalulation metrics for each fold
+print(result.time)             # Elapsed time
+print(result.submission_df)    # The output dataframe saved as submission.csv
+
+# ...and all outputs have been saved under the logging directory (default: output/yyyymmdd_HHMMSS).
+
+
+# You can use it with mlflow and track your experiments through mlflow-ui
+result = run_experiment(params,
+                        X_train,
+                        y_train,
+                        X_test,
+                        with_mlflow=True)
+```
+
+nyaggle also has a low-level API which has similar interface to
+[mlflow tracking](https://www.mlflow.org/docs/latest/tracking.html) and [wandb](https://www.wandb.com/).
+
+```python
+from nyaggle.experiment import Experiment
+
+with Experiment(logging_directory='./output/') as exp:
+    # log key-value pair as a parameter
+    exp.log_param('lr', 0.01)
+    exp.log_param('optimizer', 'adam')
+
+    # log text
+    exp.log('blah blah blah')
+
+    # log metric
+    exp.log_metric('CV', 0.85)
+
+    # log numpy ndarray, pandas dafaframe and any artifacts
+    exp.log_numpy('predicted', predicted)
+    exp.log_dataframe('submission', sub, file_format='csv')
+    exp.log_artifact('path-to-your-file')
+```
+
+### Feature Engineering
+
+#### Target Encoding with K-Fold
+
+```python
+import pandas as pd
+import numpy as np
+
+from sklearn.model_selection import KFold
+from nyaggle.feature.category_encoder import TargetEncoder
+
+
+train = pd.read_csv('train.csv')
+test = pd.read_csv('test.csv')
+all = pd.concat([train, test]).copy()
+
+cat_cols = [c for c in train.columns if train[c].dtype == np.object]
+target_col = 'y'
+
+kf = KFold(5)
+
+# Target encoding with K-fold
+te = TargetEncoder(kf.split(train))
+
+# use fit/fit_transform to train data, then apply transform to test data
+train.loc[:, cat_cols] = te.fit_transform(train[cat_cols], train[target_col])
+test.loc[:, cat_cols] = te.transform(test[cat_cols])
+
+# ... or just call fit_transform to concatenated data
+all.loc[:, cat_cols] = te.fit_transform(all[cat_cols], all[cat_cols])
+```
+
+#### Text Vectorization using BERT
+
+You need to install pytorch to your virtual environment to use BertSentenceVectorizer. 
+MaCab and mecab-python3 are also required if you use the Japanese BERT model.
+
+```python
+import pandas as pd
+from nyaggle.feature.nlp import BertSentenceVectorizer
+
+
+train = pd.read_csv('train.csv')
+test = pd.read_csv('test.csv')
+all = pd.concat([train, test]).copy()
+
+text_cols = ['body']
+target_col = 'y'
+group_col = 'user_id'
+
+
+# extract BERT-based sentence vector
+bv = BertSentenceVectorizer(text_columns=text_cols)
+
+text_vector = bv.fit_transform(train)
+
+
+# BERT + SVD, with cuda
+bv = BertSentenceVectorizer(text_columns=text_cols, use_cuda=True, n_components=40)
+
+text_vector_svd = bv.fit_transform(train)
+
+# Japanese BERT
+bv = BertSentenceVectorizer(text_columns=text_cols, lang='jp')
+
+japanese_text_vector = bv.fit_transform(train)
+```
+
+
+### Adversarial Validation
+
+```python
+import pandas as pd
+from nyaggle.validation import adversarial_validate
+
+train = pd.read_csv('train.csv')
+test = pd.read_csv('test.csv')
+
+auc, importance = adversarial_validate(train, test, importance_type='gain')
+
+```
+
+### Validation Splitters
+
+nyaggle provides a set of validation splitters that are compatible with sklearn.
+
+```python
+import pandas as pd
+from sklearn.model_selection import cross_validate, KFold
+from nyaggle.validation import TimeSeriesSplit, Take, Skip, Nth
+
+train = pd.read_csv('train.csv', parse_dates='dt')
+
+# time-series split
+ts = TimeSeriesSplit(train['dt'])
+ts.add_fold(train_interval=('2019-01-01', '2019-01-10'), test_interval=('2019-01-10', '2019-01-20'))
+ts.add_fold(train_interval=('2019-01-06', '2019-01-15'), test_interval=('2019-01-15', '2019-01-25'))
+
+cross_validate(..., cv=ts)
+
+# take the first 3 folds out of 10
+cross_validate(..., cv=Take(3, KFold(10)))
+
+# skip the first 3 folds, and evaluate the remaining 7 folds
+cross_validate(..., cv=Skip(3, KFold(10)))
+
+# evaluate 1st fold
+cross_validate(..., cv=Nth(1, ts))
+
+```
+
+### Other Awesome Repositories
+
+Here is a list of awesome repositories that provide general utility functions for data science competitions.
+Please let me know if you have another one :)
+
+- [jeongyoonlee/Kaggler](https://github.com/jeongyoonlee/Kaggler)
+- [mxbi/mlcrate](https://github.com/mxbi/mlcrate)
+- [analokmaus/kuma_utils](https://github.com/analokmaus/kuma_utils)
+- [Far0n/kaggletils](https://github.com/Far0n/kaggletils)
+- [MLWave/Kaggle-Ensemble-Guide](https://github.com/MLWave/Kaggle-Ensemble-Guide)
+- [rushter/heamy](https://github.com/rushter/heamy)
```

### Comparing `nyaggle-0.1.5/nyaggle/hyper_parameters/catboost.py` & `nyaggle-0.1.6/nyaggle/hyper_parameters/catboost.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/hyper_parameters/xgboost.py` & `nyaggle-0.1.6/nyaggle/hyper_parameters/xgboost.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/hyper_parameters/lightgbm.py` & `nyaggle-0.1.6/nyaggle/hyper_parameters/lightgbm.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/hyper_parameters/parameters.py` & `nyaggle-0.1.6/nyaggle/hyper_parameters/parameters.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/testing/util.py` & `nyaggle-0.1.6/nyaggle/testing/util.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/feature/nlp/bert.py` & `nyaggle-0.1.6/nyaggle/feature/nlp/bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         return self.svd[col].fit_transform(emb)
 
     def _process(self, X: pd.DataFrame, func: Callable[[str, np.ndarray], Any]):
         is_pandas = isinstance(X, pd.DataFrame)
         X = convert_input(X)
 
         tqdm.pandas()
-        columns = self.text_columns or [c for c in X.columns if X[c].dtype == np.object]
+        columns = self.text_columns or [c for c in X.columns if X[c].dtype == object]
         non_text_columns = [c for c in X.columns if c not in columns]
 
         column_names = []
         processed = []
         for c in columns:
             emb = np.vstack(X[c].progress_apply(lambda x: self._process_text(x)))
             emb = func(c, emb)
```

### Comparing `nyaggle-0.1.5/nyaggle/feature/groupby.py` & `nyaggle-0.1.6/nyaggle/feature/groupby.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 # Copyright (c) 2020 Kota Yuhara (@wakamezake)
 # -----------------------------------------------------------------------------
 
 # Original work of aggregation:
 # https://github.com/pfnet-research/xfeat/blob/master/xfeat/helper.py
 # -----------------------------------------------------------------------------
 # MIT License
-# 
+#
 # Copyright (c) 2020 Preferred Networks, Inc.
-# 
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
-# 
+#
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
-# 
+#
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # -----------------------------------------------------------------------------
 
-
-from types import LambdaType, FunctionType
-from typing import List, Callable, Union, Tuple
+from inspect import isroutine
+from types import FunctionType, LambdaType
+from typing import Callable, List, Tuple, Union
 
 import pandas as pd
 from pandas.core.common import get_callable_name
 
 
 def _is_lambda_function(obj):
     """
@@ -67,28 +67,31 @@
             Input data frame.
         group_key:
             Used to determine the groups for the groupby.
         group_values:
             Used to aggregate values for the groupby.
         agg_methods:
             List of function or function names, e.g. ['mean', 'max', 'min', numpy.mean].
-            Do not use a lambda function because the name attribute of the lambda function cannot generate a unique string of column names in <lambda>.
+            Do not use a lambda function because the name attribute of the lambda
+            function cannot generate a unique string of column names in <lambda>.
     Returns:
         Tuple of output dataframe and new column names.
     """
     new_df = input_df.copy()
 
     new_cols = []
     for agg_method in agg_methods:
         if _is_lambda_function(agg_method):
             raise ValueError('Not supported lambda function.')
         elif isinstance(agg_method, str):
             pass
         elif isinstance(agg_method, FunctionType):
             pass
+        elif isroutine(agg_method):
+            pass
         else:
             raise ValueError('Supported types are: {} or {}.'
                              ' Got {} instead.'.format(str, Callable, type(agg_method)))
 
     for agg_method in agg_methods:
         for col in group_values:
             # only str or FunctionType
```

### Comparing `nyaggle-0.1.5/nyaggle/feature/category_encoder/target_encoder.py` & `nyaggle-0.1.6/nyaggle/feature/category_encoder/target_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             If False, these APIs always return a numpy array, similar to sklearn's API.
     """
 
     def __init__(self, cv: Optional[Union[Iterable, BaseCrossValidator]] = None,
                  groups: Optional[pd.Series] = None,
                  cols: List[str] = None,
                  drop_invariant: bool = False, handle_missing: str = 'value', handle_unknown: str = 'value',
-                 min_samples_leaf: int = 1, smoothing: float = 1.0, return_same_type: bool = True):
+                 min_samples_leaf: int = 20, smoothing: float = 10.0, return_same_type: bool = True):
         e = ce.TargetEncoder(cols=cols, drop_invariant=drop_invariant, return_df=True,
                              handle_missing=handle_missing,
                              handle_unknown=handle_unknown,
                              min_samples_leaf=min_samples_leaf, smoothing=smoothing)
 
         super().__init__(e, cv, return_same_type, groups)
```

### Comparing `nyaggle-0.1.5/nyaggle/validation/split.py` & `nyaggle-0.1.6/nyaggle/validation/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
             # -------
             splitx = np.argmin(losses)
             split_freq[splitx] = cand_freq[splitx]
             split_ratios[splitx] = cand_ratio[splitx]
             split_diffs[splitx] = cand_diffs[splitx]
             grouped_splitx.append(splitx)
 
-        test_folds = np.empty(n_samples, dtype=np.int)
+        test_folds = np.empty(n_samples, dtype=int)
         for group_idx, splitx in zip(sortx, grouped_splitx):
             idxs = group_idxs[group_idx]
             test_folds[idxs] = splitx
 
         return test_folds
 
     @staticmethod
```

### Comparing `nyaggle-0.1.5/nyaggle/validation/cross_validate.py` & `nyaggle-0.1.6/nyaggle/validation/cross_validate.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/validation/adversarial_validate.py` & `nyaggle-0.1.6/nyaggle/validation/adversarial_validate.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/environment.py` & `nyaggle-0.1.6/nyaggle/environment.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/ensemble/stacking.py` & `nyaggle-0.1.6/nyaggle/ensemble/stacking.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/ensemble/averaging.py` & `nyaggle-0.1.6/nyaggle/ensemble/averaging.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,36 +68,40 @@
 
     return EnsembleResult(average_test, average_oof, score)
 
 
 def averaging_opt(test_predictions: List[np.ndarray],
                   oof_predictions: Optional[List[np.ndarray]],
                   y: Optional[pd.Series],
-                  eval_func: Optional[Callable],
+                  eval_func: Optional[Callable[[np.ndarray, np.ndarray], float]],
                   higher_is_better: bool,
-                  weight_bounds: Tuple = (0, 1),
-                  rank_averaging: bool = False) -> EnsembleResult:
+                  weight_bounds: Tuple[float, float] = (0.0, 1.0),
+                  rank_averaging: bool = False,
+                  method: Optional[str] = None) -> EnsembleResult:
     """
-    Perform averaging with optimal weights using scipy.optimize
+    Perform averaging with optimal weights using scipy.optimize.
 
     Args:
         test_predictions:
             List of predicted values on test data.
         oof_predictions:
             List of predicted values on out-of-fold training data.
         y:
             Target value
         eval_func:
-            Evaluation metric used for calculating result score. Used only if ``oof_predictions`` and ``y`` are given.
+            Evaluation metric f(y_true, y_pred) used for calculating result score.
+            Used only if ``oof_predictions`` and ``y`` are given.
         higher_is_better:
             Determine the direction of optimize ``eval_func``.
         weight_bounds:
             Specify lower/upper bounds of each weight.
         rank_averaging:
             If ``True``, predictions will be converted to rank before averaging.
+        method:
+            Type of solver. If ``None``, SLSQP will be used.
     Returns:
         Namedtuple with following members
 
         * test_prediction:
             numpy array, Average prediction on test data.
         * oof_prediction:
             numpy array, Average prediction on Out-of-Fold validation data. ``None`` if ``oof_predictions`` = ``None``.
@@ -114,19 +118,24 @@
         return -oof_score if higher_is_better else oof_score
 
     weights = np.ones((len(test_predictions))) / len(test_predictions)
 
     if rank_averaging:
         test_predictions, oof_predictions = _to_rank(test_predictions, oof_predictions)
 
-    cons = ({'type': 'eq', 'fun': lambda w: 1 - sum(w)})
+    method = method or 'SLSQP'
+
+    if method in ['COBYLA', 'SLSQP', 'trust-constr']:
+        cons = ({'type': 'eq', 'fun': lambda w: 1 - sum(w)})
+    else:
+        cons = None
 
     bounds = [weight_bounds] * len(test_predictions)
 
-    result = minimize(_minimize, weights, method='SLSQP', constraints=cons, bounds=bounds)
+    result = minimize(_minimize, weights, method=method, constraints=cons, bounds=bounds)
 
     return averaging(test_predictions, oof_predictions, y, result['x'], eval_func)
 
 
 def _to_rank(test_predictions: List[np.ndarray], oof_predictions: Optional[List[np.ndarray]]):
     if oof_predictions is not None:
         oof_predictions = [stats.rankdata(oof) / len(oof) for oof in oof_predictions]
```

### Comparing `nyaggle-0.1.5/nyaggle/feature_store/feature_store.py` & `nyaggle-0.1.6/nyaggle/feature_store/feature_store.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/experiment/auto_prep.py` & `nyaggle-0.1.6/nyaggle/experiment/auto_prep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
-from pandas.api.types import is_integer_dtype, is_categorical
+from pandas.api.types import is_integer_dtype, is_categorical_dtype
 from sklearn.preprocessing import LabelEncoder
 
 
 def autoprep_gbdt(algorithm_type: str, X_train: pd.DataFrame, X_test: Optional[pd.DataFrame],
                   categorical_feature_to_treat: Optional[List[str]] = None) -> Tuple[pd.DataFrame, pd.DataFrame]:
     if categorical_feature_to_treat is None:
         categorical_feature_to_treat = [c for c in X_train.columns if X_train[c].dtype.name in ['object', 'category']]
@@ -20,15 +20,15 @@
     # https://catboost.ai/docs/concepts/faq.html#why-float-and-nan-values-are-forbidden-for-cat-features
     #
     # XGBoost:
     # All categorical column should be encoded beforehand.
 
     if algorithm_type == 'lgbm':
         # LightGBM can handle categorical dtype natively
-        categorical_feature_to_treat = [c for c in categorical_feature_to_treat if not is_categorical(X_train[c])]
+        categorical_feature_to_treat = [c for c in categorical_feature_to_treat if not is_categorical_dtype(X_train[c])]
 
     if algorithm_type == 'cat' and len(categorical_feature_to_treat) > 0:
         X_train = X_train.copy()
         X_test = X_test.copy() if X_test is not None else X_train.iloc[:1, :].copy()  # dummy
         for c in categorical_feature_to_treat:
             X_train[c], X_test[c] = _fill_na_by_unique_value(X_train[c], X_test[c])
 
@@ -45,14 +45,14 @@
             X_train[c] = concat[:len(X_train)]
             X_test[c] = concat[len(X_train):]
 
     return X_train, X_test
 
 
 def _fill_na_by_unique_value(strain: pd.Series, stest: Optional[pd.Series]) -> Tuple[pd.Series, pd.Series]:
-    if is_categorical(strain):
+    if is_categorical_dtype(strain):
         return strain.cat.codes, stest.cat.codes
     elif is_integer_dtype(strain.dtype):
         fillval = min(strain.min(), stest.min()) - 1
         return strain.fillna(fillval), stest.fillna(fillval)
     else:
         return strain.astype(str), stest.astype(str)
```

### Comparing `nyaggle-0.1.5/nyaggle/experiment/hyperparameter_tuner.py` & `nyaggle-0.1.6/nyaggle/experiment/hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/experiment/experiment.py` & `nyaggle-0.1.6/nyaggle/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/experiment/run.py` & `nyaggle-0.1.6/nyaggle/experiment/run.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/util/traits.py` & `nyaggle-0.1.6/nyaggle/util/traits.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/util/plot_importance.py` & `nyaggle-0.1.6/nyaggle/util/plot_importance.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle/util/submission.py` & `nyaggle-0.1.6/nyaggle/util/submission.py`

 * *Files identical despite different names*

### Comparing `nyaggle-0.1.5/nyaggle.egg-info/SOURCES.txt` & `nyaggle-0.1.6/nyaggle.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements.txt
 setup.py
 docs/requirements.txt
 nyaggle/__init__.py
```

### Comparing `nyaggle-0.1.5/nyaggle.egg-info/PKG-INFO` & `nyaggle-0.1.6/nyaggle.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,240 +1,241 @@
 Metadata-Version: 2.1
 Name: nyaggle
-Version: 0.1.5
+Version: 0.1.6
 Summary: Code for Kaggle and Offline Competitions.
 Home-page: https://github.com/nyanp/nyaggle
 Author: nyanp
 Author-email: Noumi.Taiga@gmail.com
 License: MIT
-Description: # nyaggle
-        
-        ![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/Python%20package/badge.svg)
-        ![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/weekly_test/badge.svg)
-        ![Python Versions](https://img.shields.io/pypi/pyversions/nyaggle.svg?logo=python&logoColor=white)
-        ![Documentation Status](https://readthedocs.org/projects/nyaggle/badge/?version=latest)
-        
-        [**Documentation**](https://nyaggle.readthedocs.io/en/latest/index.html)
-        | [**Slide (Japanese)**](https://docs.google.com/presentation/d/1jv3J7DISw8phZT4z9rqjM-azdrQ4L4wWJN5P-gKL6fA/edit?usp=sharing)
-        
-        **nyaggle** is a utility library for Kaggle and offline competitions, 
-        particularly focused on experiment tracking, feature engineering and validation.
-        
-        - **nyaggle.ensemble** - Averaging & stacking
-        - **nyaggle.experiment** - Experiment tracking
-        - **nyaggle.feature_store** - Lightweight feature storage using feather-format
-        - **nyaggle.features** - sklearn-compatible features
-        - **nyaggle.hyper_parameters** - Collection of GBDT hyper-parameters used in past Kaggle competitions
-        - **nyaggle.validation** - Adversarial validation & sklearn-compatible CV splitters
-        
-        ## Installation
-        
-        You can install nyaggle via pip:
-        
-        ```Shell
-        $pip install nyaggle
-        ```
-        
-        ## Examples
-        
-        ### Experiment Tracking
-        
-        `run_experiment()` is an high-level API for experiment with cross validation.
-        It outputs parameters, metrics, out of fold predictions, test predictions,
-        feature importance and submission.csv under the specified directory.
-        
-        It can be combined with mlflow tracking.
-        
-        ```python
-        from sklearn.model_selection import train_test_split
-        
-        from nyaggle.experiment import run_experiment
-        from nyaggle.testing import make_classification_df
-        
-        X, y = make_classification_df()
-        X_train, X_test, y_train, y_test = train_test_split(X, y)
-        
-        params = {
-            'n_estimators': 1000,
-            'max_depth': 8
-        }
-        
-        result = run_experiment(params,
-                                X_train,
-                                y_train,
-                                X_test)
-        
-        # You can get outputs that needed in data science competitions with 1 API
-        
-        print(result.test_prediction)  # Test prediction in numpy array
-        print(result.oof_prediction)   # Out-of-fold prediction in numpy array
-        print(result.models)           # Trained models for each fold
-        print(result.importance)       # Feature importance for each fold
-        print(result.metrics)          # Evalulation metrics for each fold
-        print(result.time)             # Elapsed time
-        print(result.submission_df)    # The output dataframe saved as submission.csv
-        
-        # ...and all outputs have been saved under the logging directory (default: output/yyyymmdd_HHMMSS).
-        
-        
-        # You can use it with mlflow and track your experiments through mlflow-ui
-        result = run_experiment(params,
-                                X_train,
-                                y_train,
-                                X_test,
-                                with_mlflow=True)
-        ```
-        
-        nyaggle also has a low-level API which has similar interface to
-        [mlflow tracking](https://www.mlflow.org/docs/latest/tracking.html) and [wandb](https://www.wandb.com/).
-        
-        ```python
-        from nyaggle.experiment import Experiment
-        
-        with Experiment(logging_directory='./output/') as exp:
-            # log key-value pair as a parameter
-            exp.log_param('lr', 0.01)
-            exp.log_param('optimizer', 'adam')
-        
-            # log text
-            exp.log('blah blah blah')
-        
-            # log metric
-            exp.log_metric('CV', 0.85)
-        
-            # log numpy ndarray, pandas dafaframe and any artifacts
-            exp.log_numpy('predicted', predicted)
-            exp.log_dataframe('submission', sub, file_format='csv')
-            exp.log_artifact('path-to-your-file')
-        ```
-        
-        ### Feature Engineering
-        
-        #### Target Encoding with K-Fold
-        
-        ```python
-        import pandas as pd
-        import numpy as np
-        
-        from sklearn.model_selection import KFold
-        from nyaggle.feature.category_encoder import TargetEncoder
-        
-        
-        train = pd.read_csv('train.csv')
-        test = pd.read_csv('test.csv')
-        all = pd.concat([train, test]).copy()
-        
-        cat_cols = [c for c in train.columns if train[c].dtype == np.object]
-        target_col = 'y'
-        
-        kf = KFold(5)
-        
-        # Target encoding with K-fold
-        te = TargetEncoder(kf.split(train))
-        
-        # use fit/fit_transform to train data, then apply transform to test data
-        train.loc[:, cat_cols] = te.fit_transform(train[cat_cols], train[target_col])
-        test.loc[:, cat_cols] = te.transform(test[cat_cols])
-        
-        # ... or just call fit_transform to concatenated data
-        all.loc[:, cat_cols] = te.fit_transform(all[cat_cols], all[cat_cols])
-        ```
-        
-        #### Text Vectorization using BERT
-        
-        You need to install pytorch to your virtual environment to use BertSentenceVectorizer. 
-        MaCab and mecab-python3 are also required if you use Japanese BERT model.
-        
-        ```python
-        import pandas as pd
-        from nyaggle.feature.nlp import BertSentenceVectorizer
-        
-        
-        train = pd.read_csv('train.csv')
-        test = pd.read_csv('test.csv')
-        all = pd.concat([train, test]).copy()
-        
-        text_cols = ['body']
-        target_col = 'y'
-        group_col = 'user_id'
-        
-        
-        # extract BERT-based sentence vector
-        bv = BertSentenceVectorizer(text_columns=text_cols)
-        
-        text_vector = bv.fit_transform(train)
-        
-        
-        # BERT + SVD, with cuda
-        bv = BertSentenceVectorizer(text_columns=text_cols, use_cuda=True, n_components=40)
-        
-        text_vector_svd = bv.fit_transform(train)
-        
-        # Japanese BERT
-        bv = BertSentenceVectorizer(text_columns=text_cols, lang='jp')
-        
-        japanese_text_vector = bv.fit_transform(train)
-        ```
-        
-        
-        ### Adversarial Validation
-        
-        ```python
-        import pandas as pd
-        from nyaggle.validation import adversarial_validate
-        
-        train = pd.read_csv('train.csv')
-        test = pd.read_csv('test.csv')
-        
-        auc, importance = adversarial_validate(train, test, importance_type='gain')
-        
-        ```
-        
-        ### Validation Splitters
-        
-        nyaggle provides a set of validation splitters that compatible with sklean interface.
-        
-        ```python
-        import pandas as pd
-        from sklearn.model_selection import cross_validate, KFold
-        from nyaggle.validation import TimeSeriesSplit, Take, Skip, Nth
-        
-        train = pd.read_csv('train.csv', parse_dates='dt')
-        
-        # time-series split
-        ts = TimeSeriesSplit(train['dt'])
-        ts.add_fold(train_interval=('2019-01-01', '2019-01-10'), test_interval=('2019-01-10', '2019-01-20'))
-        ts.add_fold(train_interval=('2019-01-06', '2019-01-15'), test_interval=('2019-01-15', '2019-01-25'))
-        
-        cross_validate(..., cv=ts)
-        
-        # take the first 3 folds out of 10
-        cross_validate(..., cv=Take(3, KFold(10)))
-        
-        # skip the first 3 folds, and evaluate the remaining 7 folds
-        cross_validate(..., cv=Skip(3, KFold(10)))
-        
-        # evaluate 1st fold
-        cross_validate(..., cv=Nth(1, ts))
-        
-        ```
-        
-        ### Other Awesome Repositories
-        
-        Here is a list of awesome repositories that provide general utility functions for data science competitions.
-        Please let me know if you have another one :)
-        
-        - [jeongyoonlee/Kaggler](https://github.com/jeongyoonlee/Kaggler)
-        - [mxbi/mlcrate](https://github.com/mxbi/mlcrate)
-        - [analokmaus/kuma_utils](https://github.com/analokmaus/kuma_utils)
-        - [Far0n/kaggletils](https://github.com/Far0n/kaggletils)
-        - [MLWave/Kaggle-Ensemble-Guide](https://github.com/MLWave/Kaggle-Ensemble-Guide)
-        - [rushter/heamy](https://github.com/rushter/heamy)
-        
 Keywords: nyaggle kaggle
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: all
+License-File: LICENSE
+
+# nyaggle
+
+![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/Python%20package/badge.svg)
+![GitHub Actions CI Status](https://github.com/nyanp/nyaggle/workflows/weekly_test/badge.svg)
+![Python Versions](https://img.shields.io/pypi/pyversions/nyaggle.svg?logo=python&logoColor=white)
+![Documentation Status](https://readthedocs.org/projects/nyaggle/badge/?version=latest)
+
+[**Documentation**](https://nyaggle.readthedocs.io/en/latest/index.html)
+| [**Slide (Japanese)**](https://docs.google.com/presentation/d/1jv3J7DISw8phZT4z9rqjM-azdrQ4L4wWJN5P-gKL6fA/edit?usp=sharing)
+
+**nyaggle** is an utility library for Kaggle and offline competitions. 
+It is particularly focused on experiment tracking, feature engineering, and validation.
+
+- **nyaggle.ensemble** - Averaging & stacking
+- **nyaggle.experiment** - Experiment tracking
+- **nyaggle.feature_store** - Lightweight feature storage using feather-format
+- **nyaggle.features** - sklearn-compatible features
+- **nyaggle.hyper_parameters** - Collection of GBDT hyper-parameters used in past Kaggle competitions
+- **nyaggle.validation** - Adversarial validation & sklearn-compatible CV splitters
+
+## Installation
+
+You can install nyaggle via pip:
+
+```bash
+pip install nyaggle
+```
+
+## Examples
+
+### Experiment Tracking
+
+`run_experiment()` is a high-level API for experiments with cross validation.
+It outputs parameters, metrics, out of fold predictions, test predictions,
+feature importance, and submission.csv under the specified directory.
+
+To enable mlflow tracking, include the optional `with_mlflow=True` parameter.
+
+```python
+from sklearn.model_selection import train_test_split
+
+from nyaggle.experiment import run_experiment
+from nyaggle.testing import make_classification_df
+
+X, y = make_classification_df()
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+params = {
+    'n_estimators': 1000,
+    'max_depth': 8
+}
+
+result = run_experiment(params,
+                        X_train,
+                        y_train,
+                        X_test)
+
+# You can get outputs that are needed in data science competitions with 1 API
+
+print(result.test_prediction)  # Test prediction in numpy array
+print(result.oof_prediction)   # Out-of-fold prediction in numpy array
+print(result.models)           # Trained models for each fold
+print(result.importance)       # Feature importance for each fold
+print(result.metrics)          # Evalulation metrics for each fold
+print(result.time)             # Elapsed time
+print(result.submission_df)    # The output dataframe saved as submission.csv
+
+# ...and all outputs have been saved under the logging directory (default: output/yyyymmdd_HHMMSS).
+
+
+# You can use it with mlflow and track your experiments through mlflow-ui
+result = run_experiment(params,
+                        X_train,
+                        y_train,
+                        X_test,
+                        with_mlflow=True)
+```
+
+nyaggle also has a low-level API which has similar interface to
+[mlflow tracking](https://www.mlflow.org/docs/latest/tracking.html) and [wandb](https://www.wandb.com/).
+
+```python
+from nyaggle.experiment import Experiment
+
+with Experiment(logging_directory='./output/') as exp:
+    # log key-value pair as a parameter
+    exp.log_param('lr', 0.01)
+    exp.log_param('optimizer', 'adam')
+
+    # log text
+    exp.log('blah blah blah')
+
+    # log metric
+    exp.log_metric('CV', 0.85)
+
+    # log numpy ndarray, pandas dafaframe and any artifacts
+    exp.log_numpy('predicted', predicted)
+    exp.log_dataframe('submission', sub, file_format='csv')
+    exp.log_artifact('path-to-your-file')
+```
+
+### Feature Engineering
+
+#### Target Encoding with K-Fold
+
+```python
+import pandas as pd
+import numpy as np
+
+from sklearn.model_selection import KFold
+from nyaggle.feature.category_encoder import TargetEncoder
+
+
+train = pd.read_csv('train.csv')
+test = pd.read_csv('test.csv')
+all = pd.concat([train, test]).copy()
+
+cat_cols = [c for c in train.columns if train[c].dtype == np.object]
+target_col = 'y'
+
+kf = KFold(5)
+
+# Target encoding with K-fold
+te = TargetEncoder(kf.split(train))
+
+# use fit/fit_transform to train data, then apply transform to test data
+train.loc[:, cat_cols] = te.fit_transform(train[cat_cols], train[target_col])
+test.loc[:, cat_cols] = te.transform(test[cat_cols])
+
+# ... or just call fit_transform to concatenated data
+all.loc[:, cat_cols] = te.fit_transform(all[cat_cols], all[cat_cols])
+```
+
+#### Text Vectorization using BERT
+
+You need to install pytorch to your virtual environment to use BertSentenceVectorizer. 
+MaCab and mecab-python3 are also required if you use the Japanese BERT model.
+
+```python
+import pandas as pd
+from nyaggle.feature.nlp import BertSentenceVectorizer
+
+
+train = pd.read_csv('train.csv')
+test = pd.read_csv('test.csv')
+all = pd.concat([train, test]).copy()
+
+text_cols = ['body']
+target_col = 'y'
+group_col = 'user_id'
+
+
+# extract BERT-based sentence vector
+bv = BertSentenceVectorizer(text_columns=text_cols)
+
+text_vector = bv.fit_transform(train)
+
+
+# BERT + SVD, with cuda
+bv = BertSentenceVectorizer(text_columns=text_cols, use_cuda=True, n_components=40)
+
+text_vector_svd = bv.fit_transform(train)
+
+# Japanese BERT
+bv = BertSentenceVectorizer(text_columns=text_cols, lang='jp')
+
+japanese_text_vector = bv.fit_transform(train)
+```
+
+
+### Adversarial Validation
+
+```python
+import pandas as pd
+from nyaggle.validation import adversarial_validate
+
+train = pd.read_csv('train.csv')
+test = pd.read_csv('test.csv')
+
+auc, importance = adversarial_validate(train, test, importance_type='gain')
+
+```
+
+### Validation Splitters
+
+nyaggle provides a set of validation splitters that are compatible with sklearn.
+
+```python
+import pandas as pd
+from sklearn.model_selection import cross_validate, KFold
+from nyaggle.validation import TimeSeriesSplit, Take, Skip, Nth
+
+train = pd.read_csv('train.csv', parse_dates='dt')
+
+# time-series split
+ts = TimeSeriesSplit(train['dt'])
+ts.add_fold(train_interval=('2019-01-01', '2019-01-10'), test_interval=('2019-01-10', '2019-01-20'))
+ts.add_fold(train_interval=('2019-01-06', '2019-01-15'), test_interval=('2019-01-15', '2019-01-25'))
+
+cross_validate(..., cv=ts)
+
+# take the first 3 folds out of 10
+cross_validate(..., cv=Take(3, KFold(10)))
+
+# skip the first 3 folds, and evaluate the remaining 7 folds
+cross_validate(..., cv=Skip(3, KFold(10)))
+
+# evaluate 1st fold
+cross_validate(..., cv=Nth(1, ts))
+
+```
+
+### Other Awesome Repositories
+
+Here is a list of awesome repositories that provide general utility functions for data science competitions.
+Please let me know if you have another one :)
+
+- [jeongyoonlee/Kaggler](https://github.com/jeongyoonlee/Kaggler)
+- [mxbi/mlcrate](https://github.com/mxbi/mlcrate)
+- [analokmaus/kuma_utils](https://github.com/analokmaus/kuma_utils)
+- [Far0n/kaggletils](https://github.com/Far0n/kaggletils)
+- [MLWave/Kaggle-Ensemble-Guide](https://github.com/MLWave/Kaggle-Ensemble-Guide)
+- [rushter/heamy](https://github.com/rushter/heamy)
```

