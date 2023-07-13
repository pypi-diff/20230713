# Comparing `tmp/autogluon.timeseries-0.8.3b20230712.tar.gz` & `tmp/autogluon.timeseries-0.8.3b20230713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.8.3b20230712.tar", last modified: Wed Jul 12 09:04:42 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.8.3b20230713.tar", last modified: Thu Jul 13 09:04:36 2023, max compression
```

## Comparing `autogluon.timeseries-0.8.3b20230712.tar` & `autogluon.timeseries-0.8.3b20230713.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.876404 autogluon.timeseries-0.8.3b20230712/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.876404 autogluon.timeseries-0.8.3b20230712/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49409 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48405 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.884404 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-12 09:04:00.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:42.880404 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:42.000000 autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.222730 autogluon.timeseries-0.8.3b20230713/
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-13 09:04:36.222730 autogluon.timeseries-0.8.3b20230713/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:04:36.222730 autogluon.timeseries-0.8.3b20230713/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.214730 autogluon.timeseries-0.8.3b20230713/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.214730 autogluon.timeseries-0.8.3b20230713/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.218730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.222730 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-13 09:03:54.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:36.214730 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:04:36.000000 autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.8.3b20230712/PKG-INFO` & `autogluon.timeseries-0.8.3b20230713/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.8.3b20230712
+Version: 0.8.3b20230713
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.8.3b20230712/setup.py` & `autogluon.timeseries-0.8.3b20230713/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Frequency string (cf. gluonts frequency strings) describing the frequency
         of the time series data. For example, "H" for hourly or "D" for daily data.
     prediction_length: int
         Length of the prediction horizon, i.e., the number of time steps the model
         is fit to forecast.
     name : str, default = None
         Name of the subdirectory inside path where model will be saved.
-        The final model directory will be path+name+os.path.sep()
+        The final model directory will be os.path.join(path, name)
         If None, defaults to the model's class name: self.__class__.__name__
     metadata: CovariateMetadata
         A mapping of different covariate types known to autogluon.timeseries to column names
         in the data set.
     eval_metric : str, default
         Metric by which predictions will be ultimately evaluated on test data.
         This only impacts `model.score()`, as eval_metric is not used during training.
@@ -114,15 +114,15 @@
     def __repr__(self) -> str:
         return self.name
 
     def save(self, path: str = None, verbose=True) -> str:
         # Save self._oof_predictions as a separate file, not model attribute
         if self._oof_predictions is not None:
             save_pkl.save(
-                path=os.path.join(self.path + "utils", self._oof_filename),
+                path=os.path.join(self.path, "utils", self._oof_filename),
                 object=self._oof_predictions,
                 verbose=verbose,
             )
         oof_predictions = self._oof_predictions
         self._oof_predictions = None
         save_path = super().save(path=path, verbose=verbose)
         self._oof_predictions = oof_predictions
@@ -136,15 +136,15 @@
         if load_oof and model._oof_predictions is None:
             model._oof_predictions = cls.load_oof_predictions(path=path, verbose=verbose)
         return model
 
     @classmethod
     def load_oof_predictions(cls, path: str, verbose: bool = True) -> TimeSeriesDataFrame:
         """Load the cached OOF predictions from disk."""
-        return load_pkl.load(path=os.path.join(path + "utils", cls._oof_filename), verbose=verbose)
+        return load_pkl.load(path=os.path.join(path, "utils", cls._oof_filename), verbose=verbose)
 
     def get_oof_predictions(self):
         if self._oof_predictions is None:
             self._oof_predictions = self.load_oof_predictions(self.path)
         return self._oof_predictions
 
     def _initialize(self, **kwargs) -> None:
@@ -397,15 +397,15 @@
         search_space = self._get_search_space()
 
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(self, train_data, val_data, time_limit=hpo_executor.time_limit)
 
-        self.set_contexts(os.path.abspath(self.path) + os.path.sep)
+        self.set_contexts(os.path.abspath(self.path))
         directory = self.path
         dataset_train_filename = "dataset_train.pkl"
         train_path = os.path.join(self.path, dataset_train_filename)
         save_pkl.save(path=train_path, object=train_data)
 
         dataset_val_filename = "dataset_val.pkl"
         val_path = os.path.join(self.path, dataset_val_filename)
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """Runs a single trial of a hyperparameter tuning. Replaces
     `core.models.abstract.model_trial.model_trial` for timeseries models.
     """
     try:
         model = init_model(
             args, model_cls, init_params, backend=hpo_executor.executor_type, is_bagged_model=is_bagged_model
         )
-        model.set_contexts(path_context=model.path_root + model.name + os.path.sep)
+        model.set_contexts(path_context=os.path.join(model.path_root, model.name))
 
         train_data = load_pkl.load(train_path)
         val_data = load_pkl.load(val_path)
 
         eval_metric = model.eval_metric
 
         model = fit_and_save_model(
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         X_train, y_train = self._get_features_dataframe(train_subset, last_k_values=max_rows_per_item)
         X_val, y_val = self._get_features_dataframe(
             val_subset, last_k_values=min(self.prediction_length, max_rows_per_item)
         )
 
         estimator = TabularEstimator(
             predictor_init_kwargs={
-                "path": self.path + os.sep + "point_predictor",
+                "path": os.path.join(self.path, "point_predictor"),
                 "problem_type": ag.constants.REGRESSION,
                 "eval_metric": self.TIMESERIES_METRIC_TO_TABULAR_METRIC[self.eval_metric],
                 "verbosity": verbosity - 2,
             },
             predictor_fit_kwargs={
                 "tuning_data": pd.concat([X_val, y_val], axis=1),
                 "time_limit": time_limit,
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module including wrappers for PyTorch implementations of models in GluonTS
 """
 import logging
+import os
 import shutil
 from datetime import timedelta
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Type
 
 import gluonts
 import numpy as np
@@ -111,15 +112,15 @@
         # which breaks training
         self.callbacks = []
         return super().save(path, **kwargs)
 
     @classmethod
     def load(cls, path: str, reset_paths: bool = True, verbose: bool = True) -> "AbstractGluonTSModel":
         with torch_warning_filter():
-            model = load_pkl.load(path=path + cls.model_file_name, verbose=verbose)
+            model = load_pkl.load(path=os.path.join(path, cls.model_file_name), verbose=verbose)
             if reset_paths:
                 model.set_contexts(path)
             model.gts_predictor = GluonTSPyTorchPredictor.deserialize(Path(path) / cls.gluonts_model_path)
         return model
 
     @staticmethod
     def _distribution_to_quantile_forecast(
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         return save_path
 
     @classmethod
     def load(
         cls, path: str, reset_paths: bool = True, load_oof: bool = False, verbose: bool = True
     ) -> AbstractTimeSeriesModel:
         model = super().load(path=path, reset_paths=reset_paths, load_oof=load_oof, verbose=verbose)
-        most_recent_model_path = model.path + os.sep + cls._most_recent_model_folder + os.sep
+        most_recent_model_path = os.path.join(model.path, cls._most_recent_model_folder)
         model.most_recent_model = model.model_base_type.load(
             most_recent_model_path,
             reset_paths=reset_paths,
             verbose=verbose,
         )
         return model
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import pprint
 import time
 import warnings
 from typing import Any, Dict, List, Optional, Type, Union
 
 import pandas as pd
 
@@ -671,15 +672,15 @@
 
     def score(self, data: Union[TimeSeriesDataFrame, pd.DataFrame], **kwargs):
         """See, :meth:`~autogluon.timeseries.TimeSeriesPredictor.evaluate`."""
         return self.evaluate(data, **kwargs)
 
     @classmethod
     def _load_version_file(cls, path: str) -> str:
-        version_file_path = path + cls._predictor_version_file_name
+        version_file_path = os.path.join(path, cls._predictor_version_file_name)
         version = load_str.load(path=version_file_path)
         return version
 
     @classmethod
     def load(cls, path: str, require_version_match: bool = True) -> "TimeSeriesPredictor":
         """Load an existing ``TimeSeriesPredictor`` from given ``path``.
 
@@ -701,47 +702,47 @@
             raise ValueError("`path` cannot be None or empty in load().")
         path = setup_outputdir(path, warn_if_exist=False)
 
         try:
             version_saved = cls._load_version_file(path=path)
         except:
             logger.warning(
-                f'WARNING: Could not find version file at "{path + cls._predictor_version_file_name}".\n'
+                f'WARNING: Could not find version file at "{os.path.join(path, cls._predictor_version_file_name)}".\n'
                 f"This means that the predictor was fit in a version `<=0.7.0`."
             )
             version_saved = "Unknown (Likely <=0.7.0)"
 
         check_saved_predictor_version(
             version_current=current_ag_version,
             version_saved=version_saved,
             require_version_match=require_version_match,
             logger=logger,
         )
 
         logger.info(f"Loading predictor from path {path}")
         learner = AbstractLearner.load(path)
-        predictor = load_pkl.load(path=learner.path + cls.predictor_file_name)
+        predictor = load_pkl.load(path=os.path.join(learner.path, cls.predictor_file_name))
         predictor._learner = learner
         predictor.path = learner.path
         return predictor
 
     def _save_version_file(self):
         version_file_contents = current_ag_version
-        version_file_path = self.path + self._predictor_version_file_name
+        version_file_path = os.path.join(self.path, self._predictor_version_file_name)
         save_str.save(path=version_file_path, data=version_file_contents, verbose=False)
 
     def save(self) -> None:
         """Save this predictor to file in directory specified by this Predictor's ``path``.
 
         Note that :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit` already saves the predictor object automatically
         (we do not recommend modifying the Predictor object yourself as it tracks many trained models).
         """
         tmp_learner = self._learner
         self._learner = None
-        save_pkl.save(path=tmp_learner.path + self.predictor_file_name, object=self)
+        save_pkl.save(path=os.path.join(tmp_learner.path, self.predictor_file_name), object=self)
         self._learner = tmp_learner
         self._save_version_file()
 
     def info(self) -> Dict[str, Any]:
         """Returns a dictionary of objects each describing an attribute of the training process and trained models."""
         return self._learner.get_info(include_model_info=True)
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 class SimpleAbstractTrainer:
     trainer_file_name = "trainer.pkl"
     trainer_info_name = "info.pkl"
     trainer_info_json_name = "info.json"
 
     def __init__(self, path: str, low_memory: bool, save_data: bool, *args, **kwargs):
         self.path = path
-        self.path = PathConverter.to_relative(self.path)
         self.reset_paths = False
 
         self.low_memory = low_memory
         self.save_data = save_data
 
         self.models = {}
         self.model_graph = nx.DiGraph()
@@ -84,54 +83,47 @@
 
         return max(performances_list, key=lambda i: i[1])[0]
 
     def get_model_attribute(self, model: Union[str, AbstractModel], attribute: str):
         """Get a member attribute for given model from the `model_graph`."""
         if not isinstance(model, str):
             model = model.name
+        if attribute == "path":
+            return os.path.join(*self.model_graph.nodes[model][attribute])
         return self.model_graph.nodes[model][attribute]
 
     def set_model_attribute(self, model: Union[str, AbstractModel], attribute: str, val):
         """Set a member attribute for given model in the `model_graph`."""
         if not isinstance(model, str):
             model = model.name
         self.model_graph.nodes[model][attribute] = val
 
     @property
     def path_root(self) -> str:
-        return self.path.rsplit(os.path.sep, maxsplit=2)[0] + os.path.sep
+        return os.path.dirname(self.path)
 
     @property
     def path_utils(self) -> str:
-        return self.path_root + "utils" + os.path.sep
+        return os.path.join(self.path_root, "utils")
 
     @property
     def path_data(self) -> str:
-        return self.path_utils + "data" + os.path.sep
+        return os.path.join(self.path_utils, "data")
 
     @property
     def path_pkl(self) -> str:
-        return self.path + self.trainer_file_name
+        return os.path.join(self.path, self.trainer_file_name)
 
     def set_contexts(self, path_context: str) -> None:
-        self.path, model_paths = self.create_contexts(path_context)
-        for model, path in model_paths.items():
-            self.set_model_attribute(model=model, attribute="path", val=path)
+        self.path = self.create_contexts(path_context)
 
-    def create_contexts(self, path_context: str) -> Tuple[str, dict]:
+    def create_contexts(self, path_context: str) -> str:
         path = path_context
-        # TODO: consider keeping track of model path suffixes in model_graph instead
-        # TODO: of full paths
-        model_paths = self.get_models_attribute_dict(attribute="path")
-        for model, prev_path in model_paths.items():
-            model_local_path = prev_path.split(self.path, 1)[1]
-            new_path = path + model_local_path
-            model_paths[model] = new_path
 
-        return path, model_paths
+        return path
 
     def save(self) -> None:
         # todo: remove / revise low_memory logic
         models = self.models
         if self.low_memory:
             self.models = {}
         try:
@@ -140,15 +132,15 @@
             self.models = {}
             save_pkl.save(path=self.path_pkl, object=self)
         if not self.models:
             self.models = models
 
     @classmethod
     def load(cls, path: str, reset_paths: bool = False) -> "SimpleAbstractTrainer":
-        load_path = path + cls.trainer_file_name
+        load_path = os.path.join(path, cls.trainer_file_name)
         if not reset_paths:
             return load_pkl.load(path=load_path)
         else:
             obj = load_pkl.load(path=load_path)
             obj.set_contexts(path)
             obj.reset_paths = reset_paths
             return obj
@@ -169,15 +161,15 @@
         if model_name in self.models.keys():
             return self.models[model_name]
 
         if path is None:
             path = self.get_model_attribute(model=model_name, attribute="path")
         if model_type is None:
             model_type = self.get_model_attribute(model=model_name, attribute="type")
-        return model_type.load(path=path, reset_paths=self.reset_paths)
+        return model_type.load(path=os.path.join(self.path, path), reset_paths=self.reset_paths)
 
     def construct_model_templates(self, hyperparameters: Union[str, Dict[str, Any]], **kwargs):
         raise NotImplementedError
 
     # FIXME: Copy pasted from Tabular
     def get_minimum_model_set(self, model: Union[str, AbstractTimeSeriesModel], include_self: bool = True) -> list:
         """Gets the minimum set of models that the provided model depends on, including itself.
@@ -195,37 +187,37 @@
         model_info_dict = dict()
         for model in models:
             if isinstance(model, str):
                 if model in self.models.keys():
                     model = self.models[model]
             if isinstance(model, str):
                 model_type = self.get_model_attribute(model=model, attribute="type")
-                model_path = self.get_model_attribute(model=model, attribute="path")
+                model_path = os.path.join(self.path, self.get_model_attribute(model=model, attribute="path"))
                 model_info_dict[model] = model_type.load_info(path=model_path)
             else:
                 model_info_dict[model.name] = model.get_info()
         return model_info_dict
 
     @classmethod
     def load_info(cls, path, reset_paths=False, load_model_if_required=True) -> Dict[str, Any]:
-        load_path = path + cls.trainer_info_name
+        load_path = os.path.join(path, cls.trainer_info_name)
         try:
             return load_pkl.load(path=load_path)
         except:  # noqa
             if load_model_if_required:
                 trainer = cls.load(path=path, reset_paths=reset_paths)
                 return trainer.get_info()
             else:
                 raise
 
     def save_info(self, include_model_info: bool = False):
         info = self.get_info(include_model_info=include_model_info)
 
-        save_pkl.save(path=self.path + self.trainer_info_name, object=info)
-        save_json.save(path=self.path + self.trainer_info_json_name, obj=info)
+        save_pkl.save(path=os.path.join(self.path, self.trainer_info_name), object=info)
+        save_json.save(path=os.path.join(self.path, self.trainer_info_json_name), obj=info)
         return info
 
     def get_info(self, include_model_info: bool = False) -> Dict[str, Any]:
         num_models_trained = len(self.get_model_names())
         if self.model_best is not None:
             best_model = self.model_best
         else:
@@ -292,27 +284,27 @@
         self.eval_metric = TimeSeriesEvaluator.check_get_evaluation_metric(eval_metric)
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         self.num_val_windows = num_val_windows
         self.cache_predictions = cache_predictions
         self.hpo_results = {}
 
     def save_train_data(self, data: TimeSeriesDataFrame, verbose: bool = True) -> None:
-        path = self.path_data + "train.pkl"
+        path = os.path.join(self.path_data, "train.pkl")
         save_pkl.save(path=path, object=data, verbose=verbose)
 
     def save_val_data(self, data: TimeSeriesDataFrame, verbose: bool = True) -> None:
-        path = self.path_data + "val.pkl"
+        path = os.path.join(self.path_data, "val.pkl")
         save_pkl.save(path=path, object=data, verbose=verbose)
 
     def load_train_data(self) -> TimeSeriesDataFrame:
-        path = self.path_data + "train.pkl"
+        path = os.path.join(self.path_data, "train.pkl")
         return load_pkl.load(path=path)
 
     def load_val_data(self) -> Optional[TimeSeriesDataFrame]:
-        path = self.path_data + "val.pkl"
+        path = os.path.join(self.path_data, "val.pkl")
         if os.path.exists(path):
             return load_pkl.load(path=path)
         else:
             return None
 
     def load_data(self) -> Tuple[TimeSeriesDataFrame, Optional[TimeSeriesDataFrame]]:
         train_data = self.load_train_data()
@@ -326,15 +318,15 @@
         save_pkl.save(path=self.path_pkl, object=self)
         for model in self.models.values():
             model.save()
 
         self.models = models
 
     def _get_model_oof_predictions(self, model_name: str) -> TimeSeriesDataFrame:
-        model_path = self.get_model_attribute(model=model_name, attribute="path")
+        model_path = os.path.join(self.path, self.get_model_attribute(model=model_name, attribute="path"))
         model_type = self.get_model_attribute(model=model_name, attribute="type")
         return model_type.load_oof_predictions(path=model_path)
 
     def _add_model(
         self,
         model: AbstractTimeSeriesModel,
         base_models: List[str] = None,
@@ -352,15 +344,15 @@
 
         Raises
         ------
         AssertionError
             If ``base_models`` are provided and ``model`` is not a ``AbstractTimeSeriesEnsembleModel``.
         """
         node_attrs = dict(
-            path=model.path,
+            path=os.path.relpath(model.path, self.path).split(os.sep),
             type=type(model),
             fit_time=model.fit_time,
             predict_time=model.predict_time,
             val_score=model.val_score,
         )
         self.model_graph.add_node(model.name, **node_attrs)
 
@@ -440,15 +432,15 @@
             )
         total_tuning_time = time.time() - tuning_start_time
 
         self.hpo_results[model.name] = hpo_models
         model_names_trained = []
         # add each of the trained HPO configurations to the trained models
         for model_hpo_name, model_info in hpo_models.items():
-            model_path = model_info["path"]
+            model_path = os.path.join(self.path, model_info["path"])
             # Only load model configurations that didn't fail
             if Path(model_path).exists():
                 model_hpo = self.load_model(model_hpo_name, path=model_path, model_type=type(model))
                 self._add_model(model_hpo)
                 model_names_trained.append(model_hpo.name)
 
         logger.info(f"\tTrained {len(model_names_trained)} models while tuning {model.name}.")
@@ -733,15 +725,14 @@
         ensemble.val_score = self._score_with_predictions(val_data, predictions)
 
         self._log_scores_and_times(
             val_score=ensemble.val_score,
             fit_time=ensemble.fit_time,
             predict_time=ensemble.predict_time,
         )
-
         self._add_model(model=ensemble, base_models=ensemble.model_names)
         self.save_model(model=ensemble)
         return ensemble.name
 
     def leaderboard(self, data: Optional[TimeSeriesDataFrame] = None, use_cache: bool = True) -> pd.DataFrame:
         logger.debug("Generating leaderboard for all models trained")
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.8.3b20230713/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.8.3b20230712
+Version: 0.8.3b20230713
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.8.3b20230712/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.8.3b20230713/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

