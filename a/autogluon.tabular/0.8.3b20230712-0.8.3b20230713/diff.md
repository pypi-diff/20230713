# Comparing `tmp/autogluon.tabular-0.8.3b20230712.tar.gz` & `tmp/autogluon.tabular-0.8.3b20230713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.8.3b20230712.tar", last modified: Wed Jul 12 09:04:30 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.8.3b20230713.tar", last modified: Thu Jul 13 09:04:25 2023, max compression
```

## Comparing `autogluon.tabular-0.8.3b20230712.tar` & `autogluon.tabular-0.8.3b20230713.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.768253 autogluon.tabular-0.8.3b20230712/
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-07-12 09:04:30.768253 autogluon.tabular-0.8.3b20230712/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:04:30.768253 autogluon.tabular-0.8.3b20230712/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.748253 autogluon.tabular-0.8.3b20230712/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.748253 autogluon.tabular-0.8.3b20230712/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.752253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.752253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.752253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50070 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.752253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15630 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25573 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.756253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36172 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    22903 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22575 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.760253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    16873 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34250 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.764253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)   264044 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.768253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.768253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.768253 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-12 09:04:00.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:30.752253 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:30.000000 autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50070 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25573 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.638717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36172 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22903 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16873 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32457 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34250 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.642717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264148 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.646717 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-13 09:03:54.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:25.634717 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:04:25.000000 autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.8.3b20230712/PKG-INFO` & `autogluon.tabular-0.8.3b20230713/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
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

### Comparing `autogluon.tabular-0.8.3b20230712/setup.py` & `autogluon.tabular-0.8.3b20230713/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             if "train_dir" not in params:
                 try:
                     # TODO: What if path is in S3?
                     os.makedirs(os.path.dirname(self.path), exist_ok=True)
                 except:
                     pass
                 else:
-                    params["train_dir"] = self.path + "catboost_info"
+                    params["train_dir"] = os.path.join(self.path, "catboost_info")
 
         # TODO: Add more control over these params (specifically early_stopping_rounds)
         verbosity = kwargs.get("verbosity", 2)
         if verbosity <= 1:
             verbose = False
         elif verbosity == 2:
             verbose = False
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,29 +139,29 @@
         __model = self.model
         self.model = None
         path = super().save(path=path, verbose=verbose)
         self.model = __model
         # save fasttext model: fasttext model cannot be pickled; saved it separately
         # TODO: s3 support
         if self._load_model:
-            fasttext_model_file_name = path + self.model_bin_file_name
+            fasttext_model_file_name = os.path.join(path, self.model_bin_file_name)
             self.model.save_model(fasttext_model_file_name)
         self._load_model = None
         return path
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
         model: FastTextModel = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
 
         # load binary fasttext model
         if model._load_model:
             try_import_fasttext()
             import fasttext
 
-            fasttext_model_file_name = model.path + cls.model_bin_file_name
+            fasttext_model_file_name = os.path.join(model.path, cls.model_bin_file_name)
             # TODO: hack to subpress a deprecation warning from fasttext
             # remove it once official fasttext is updated beyond 0.9.2
             # https://github.com/facebookresearch/fastText/issues/1067
             with open(os.devnull, "w") as f, contextlib.redirect_stderr(f):
                 model.model = fasttext.load_model(fasttext_model_file_name)
         model._load_model = None
         return model
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,22 +294,24 @@
             y_og = np.array(y)
             y = None
             if X_val is not None:
                 y_val_og = np.array(y_val)
                 y_val = None
 
         # X, W_train = self.convert_to_weight(X=X)
-        dataset_train = construct_dataset(x=X, y=y, location=f"{self.path}datasets{os.path.sep}train", params=data_params, save=save, weight=sample_weight)
+        dataset_train = construct_dataset(
+            x=X, y=y, location=os.path.join("self.path", "datasets", "train"), params=data_params, save=save, weight=sample_weight
+        )
         # dataset_train = construct_dataset_lowest_memory(X=X, y=y, location=self.path + 'datasets/train', params=data_params)
         if X_val is not None:
             # X_val, W_val = self.convert_to_weight(X=X_val)
             dataset_val = construct_dataset(
                 x=X_val,
                 y=y_val,
-                location=f"{self.path}datasets{os.path.sep}val",
+                location=os.path.join(self.path, "datasets", "val"),
                 reference=dataset_train,
                 params=data_params,
                 save=save,
                 weight=sample_weight_val,
             )
             # dataset_val = construct_dataset_lowest_memory(X=X_val, y=y_val, location=self.path + 'datasets/val', reference=dataset_train, params=data_params)
         else:
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,23 @@
             The path for saving the compiled model.
         input_types : list, default=None
             A list of tuples containing shape and element type info, e.g. [((1, 14), np.float32),].
             The list would be used as the input data for the model.
             The compiler would optimize the model to perform best with the given input type.
         """
         AbstractNativeCompiler.save(model, path)
-        return model
 
     @staticmethod
     def save(model, path: str):
         os.makedirs(os.path.dirname(path), exist_ok=True)
-        with open(path + "model_native.pkl", "wb") as fp:
+        with open(os.path.join(path, "model_native.pkl"), "wb") as fp:
             fp.write(pickle.dumps(model))
 
     @staticmethod
     def load(path: str):
-        with open(path + "model_native.pkl", "rb") as fp:
+        pkl = None
+        with open(os.path.join(path, "model_native.pkl"), "rb") as fp:
             pkl = fp.read()
         return pickle.loads(pkl)
 
 
-RFNativeCompiler = AbstractNativeCompiler
+TabularNeuralNetTorchNativeCompiler = AbstractNativeCompiler
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,18 +106,18 @@
         RFOnnxCompiler.save(onnx_model, path)
         return predictor
 
     @staticmethod
     def save(model, path: str) -> str:
         """Save the compiled model into onnx file format."""
         os.makedirs(os.path.dirname(path), exist_ok=True)
-        with open(path + "model.onnx", "wb") as f:
+        with open(os.path.join(path, "model.onnx"), "wb") as f:
             f.write(model.SerializeToString())
-        return path + "model.onnx"
+        return os.path.join(path, "model.onnx")
 
     @staticmethod
     def load(path: str) -> RFOnnxPredictor:
         """Load from the path that contains an onnx file."""
         import onnx
 
-        onnx_bytes = onnx.load(path + "model.onnx")
+        onnx_bytes = onnx.load(os.path.join(path, "model.onnx"))
         return RFOnnxPredictor(model=onnx_bytes)
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,30 +336,30 @@
                 if val_metric >= best_val_metric or e == 0:
                     if loader_val is not None:
                         if not np.isnan(val_metric):
                             best_val_metric = val_metric
 
                     best_val_epoch = e
                     os.makedirs(os.path.dirname(self.path), exist_ok=True)
-                    torch.save(self.model, self.path + self._temp_file_name)
+                    torch.save(self.model, os.path.join(self.path, self._temp_file_name))
 
             # If time limit has exceeded or we haven't improved in some number of epochs, stop early.
             if e - best_val_epoch > epochs_wo_improve:
                 break
             if time_limit:
                 time_elapsed = time.time() - start_time
                 time_left = time_limit - time_elapsed
                 if time_left <= 0:
                     logger.log(20, "\tRan out of time, stopping training early.")
                     break
 
         if loader_val is not None:
             try:
-                self.model = torch.load(self.path + self._temp_file_name)
-                os.remove(self.path + self._temp_file_name)
+                self.model = torch.load(os.path.join(self.path, self._temp_file_name))
+                os.remove(os.path.join(self.path, self._temp_file_name))
             except:
                 pass
             logger.log(15, "Best model found in epoch %d" % best_val_epoch)
 
     def _fit(self, X, y, X_val=None, y_val=None, X_unlabeled=None, time_limit=None, sample_weight=None, reporter=None, **kwargs):
         import torch
 
@@ -485,15 +485,15 @@
 
     def save(self, path: str = None, verbose=True) -> str:
         import torch
 
         if path is None:
             path = self.path
 
-        params_filepath = path + self.params_file_name
+        params_filepath = os.path.join(path, self.params_file_name)
 
         os.makedirs(os.path.dirname(path), exist_ok=True)
 
         temp_model = self.model
         if self.model is not None:
             torch.save(self.model, params_filepath)
 
@@ -504,19 +504,19 @@
 
         return modelobj_filepath
 
     @classmethod
     def load(cls, path: str, reset_paths=False, verbose=True):
         import torch
 
-        obj: TabTransformerModel = load_pkl.load(path=path + cls.model_file_name, verbose=verbose)
+        obj: TabTransformerModel = load_pkl.load(path=os.path.join(path, cls.model_file_name), verbose=verbose)
         if reset_paths:
             obj.set_contexts(path)
 
-        obj.model = torch.load(path + cls.params_file_name)
+        obj.model = torch.load(os.path.join(path, cls.params_file_name))
 
         return obj
 
         """
         List of features to add (Updated by Anthony Galczak 11-19-20):
 
         1) Allow for saving of pretrained model for future use. This will be done in a future PR as the
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,23 +23,23 @@
             The path for saving the compiled model.
         input_types : list, default=None
             A list of tuples containing shape and element type info, e.g. [((1, 14), np.float32),].
             The list would be used as the input data for the model.
             The compiler would optimize the model to perform best with the given input type.
         """
         AbstractNativeCompiler.save(model, path)
+        return model
 
     @staticmethod
     def save(model, path: str):
         os.makedirs(os.path.dirname(path), exist_ok=True)
         with open(os.path.join(path, "model_native.pkl"), "wb") as fp:
             fp.write(pickle.dumps(model))
 
     @staticmethod
     def load(path: str):
-        pkl = None
         with open(os.path.join(path, "model_native.pkl"), "rb") as fp:
             pkl = fp.read()
         return pickle.loads(pkl)
 
 
-TabularNeuralNetTorchNativeCompiler = AbstractNativeCompiler
+RFNativeCompiler = AbstractNativeCompiler
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,15 +593,15 @@
         then `cpu` will be used.
 
         Parameters
         ----------
         path : str
             Path to the saved model, minus the file name.
             This should generally be a directory path ending with a '/' character (or appropriate path separator value depending on OS).
-            The model file is typically located in path + cls.model_file_name.
+            The model file is typically located in os.path.join(path, cls.model_file_name).
         reset_paths : bool, default True
             Whether to reset the self.path value of the loaded model to be equal to path.
             It is highly recommended to keep this value as True unless accessing the original self.path value is important.
             If False, the actual valid path and self.path may differ, leading to strange behaviour and potential exceptions if the model needs to load any other files at a later time.
         verbose : bool, default True
             Whether to log the location of the loaded file.
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import time
 
 import numpy as np
 import pandas as pd
 
 from autogluon.common.features.types import (
     R_CATEGORY,
@@ -179,15 +180,15 @@
         self._load_model = self.model is not None
         __model = self.model
         self.model = None
         path = super().save(path=path, verbose=verbose)
         self.model = __model
         # Export model
         if self._load_model:
-            file_path = path + self.model_internals_file_name
+            file_path = os.path.join(path, self.model_internals_file_name)
             self.model.save(file_path)
         self._load_model = None
         return path
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
         """
@@ -199,15 +200,15 @@
         import vowpalwabbit
 
         # Load Abstract Model. This is without the internal model
         model = super().load(path, reset_paths=reset_paths, verbose=verbose)
         params = model._get_model_params()
         # Load the internal model file
         if model._load_model:
-            file_path = path + cls.model_internals_file_name
+            file_path = os.path.join(path, cls.model_internals_file_name)
 
             model_load_params = f" -i {file_path} --quiet"
             if model.problem_type in PROBLEM_TYPES_CLASSIFICATION:
                 model_load_params += " --probabilities --loss_function=logistic"
             if params["sparse_weights"]:
                 model_load_params += " --sparse_weights"
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import time
 
 from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_xgboost
@@ -202,25 +203,25 @@
         _model = self.model
         self.model = None
         if _model is not None:
             self._xgb_model_type = _model.__class__
         path = super().save(path=path, verbose=verbose)
         if _model is not None:
             # Halves disk usage compared to .json / .pkl
-            _model.save_model(path + "xgb.ubj")
+            _model.save_model(os.path.join(path, "xgb.ubj"))
         self.model = _model
         return path
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
         model = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
         if model._xgb_model_type is not None:
             model.model = model._xgb_model_type()
             # Much faster to load using .ubj than .json (10x+ speedup)
-            model.model.load_model(path + "xgb.ubj")
+            model.model.load_model(os.path.join(path, "xgb.ubj"))
             model._xgb_model_type = None
         return model
 
     def _more_tags(self):
         # `can_refit_full=True` because n_estimators is communicated at end of `_fit`:
         #  self.params_trained['n_estimators'] = bst.best_ntree_limit
         return {"can_refit_full": True}
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/predictor/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3527,36 +3527,36 @@
         self._learner_type = type(self._learner)
         if self._learner.trainer_path is not None:
             self._learner.persist_trainer(low_memory=True)
             self._trainer: AbstractTrainer = self._learner.load_trainer()  # Trainer object
 
     @classmethod
     def _load_version_file(cls, path) -> str:
-        version_file_path = path + cls._predictor_version_file_name
+        version_file_path = os.path.join(path, cls._predictor_version_file_name)
         version = load_str.load(path=version_file_path)
         return version
 
     @classmethod
     def _load_metadata_file(cls, path: str, silent=True):
-        metadata_file_path = path + cls._predictor_metadata_file_name
+        metadata_file_path = os.path.join(path, cls._predictor_metadata_file_name)
         return load_json.load(path=metadata_file_path, verbose=not silent)
 
     def _save_version_file(self, silent=False):
         from ..version import __version__
 
         version_file_contents = f"{__version__}"
-        version_file_path = self.path + self._predictor_version_file_name
+        version_file_path = os.path.join(self.path, self._predictor_version_file_name)
         save_str.save(path=version_file_path, data=version_file_contents, verbose=not silent)
 
     def _save_metadata_file(self, silent=False):
         """
         Save metadata json file to disk containing information such as
         python version, autogluon version, installed packages, operating system, etc.
         """
-        metadata_file_path = self.path + self._predictor_metadata_file_name
+        metadata_file_path = os.path.join(self.path, self._predictor_metadata_file_name)
 
         metadata = get_autogluon_metadata()
 
         save_json.save(path=metadata_file_path, obj=metadata)
         if not silent:
             logger.log(15, f"Saving {metadata_file_path}")
 
@@ -3573,15 +3573,15 @@
         """
         path = self.path
         tmp_learner = self._learner
         tmp_trainer = self._trainer
         self._learner.save()
         self._learner = None
         self._trainer = None
-        save_pkl.save(path=path + self.predictor_file_name, object=self)
+        save_pkl.save(path=os.path.join(path, self.predictor_file_name), object=self)
         self._learner = tmp_learner
         self._trainer = tmp_trainer
         self._save_version_file(silent=silent)
         try:
             self._save_metadata_file(silent=silent)
         except Exception as e:
             logger.log(30, f"Failed to save metadata file due to exception {e}, skipping...")
@@ -3589,15 +3589,15 @@
             logger.log(20, f'TabularPredictor saved. To load, use: predictor = TabularPredictor.load("{self.path}")')
 
     @classmethod
     def _load(cls, path: str):
         """
         Inner load method, called in `load`.
         """
-        predictor: TabularPredictor = load_pkl.load(path=path + cls.predictor_file_name)
+        predictor: TabularPredictor = load_pkl.load(path=os.path.join(path, cls.predictor_file_name))
         learner = predictor._learner_type.load(path)
         predictor._set_post_fit_vars(learner=learner)
         return predictor
 
     @classmethod
     def load(cls, path: str, verbosity: int = None, require_version_match: bool = True, require_py_version_match: bool = True, check_packages: bool = False):
         """
@@ -3637,15 +3637,15 @@
             version_current = None
 
         path = setup_outputdir(path, warn_if_exist=False)  # replace ~ with absolute path if it exists
         try:
             version_saved = cls._load_version_file(path=path)
         except:
             logger.warning(
-                f'WARNING: Could not find version file at "{path + cls._predictor_version_file_name}".\n'
+                f'WARNING: Could not find version file at "{os.path.join(path, cls._predictor_version_file_name)}".\n'
                 f"This means that the predictor was fit in a version `<=0.3.1`."
             )
             version_saved = None
 
         if version_saved is None:
             predictor = cls._load(path=path)
             try:
@@ -3664,15 +3664,15 @@
             logger=logger,
         )
 
         try:
             metadata_init = cls._load_metadata_file(path=path)
         except:
             logger.warning(
-                f'WARNING: Could not find metadata file at "{path + cls._predictor_metadata_file_name}".\n'
+                f'WARNING: Could not find metadata file at "{os.path.join(path, cls._predictor_metadata_file_name)}".\n'
                 f"This could mean that the predictor was fit in a version `<=0.5.2`."
             )
             metadata_init = None
 
         metadata_load = get_autogluon_metadata()
 
         if metadata_init is not None:
```

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.8.3b20230713/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
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

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.3b20230712/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.8.3b20230713/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<4,>=3.0
-autogluon.core==0.8.3b20230712
-autogluon.features==0.8.3b20230712
+autogluon.core==0.8.3b20230713
+autogluon.features==0.8.3b20230713
 
 [all]
+xgboost<1.8,>=1.6
+autogluon.core[all]==0.8.3b20230713
+torch<1.14,>=1.9
 catboost<1.3,>=1.1
 fastai<2.8,>=2.3.1
-autogluon.core[all]==0.8.3b20230712
-torch<1.14,>=1.9
 lightgbm<3.4,>=3.3
-xgboost<1.8,>=1.6
 
 [all:sys_platform == "darwin"]
 catboost<1.2,>=1.1
 
 [catboost]
 catboost<1.3,>=1.1
 
@@ -30,15 +30,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.8.3b20230712
+autogluon.core[all]==0.8.3b20230713
 
 [skex]
 scikit-learn-intelex<2023.2,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
```

