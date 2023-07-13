# Comparing `tmp/autogluon.core-0.8.3b20230712.tar.gz` & `tmp/autogluon.core-0.8.3b20230713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.8.3b20230712.tar", last modified: Wed Jul 12 09:04:18 2023, max compression
+gzip compressed data, was "autogluon.core-0.8.3b20230713.tar", last modified: Thu Jul 13 09:04:13 2023, max compression
```

## Comparing `autogluon.core-0.8.3b20230712.tar` & `autogluon.core-0.8.3b20230713.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.420117 autogluon.core-0.8.3b20230712/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-12 09:04:18.420117 autogluon.core-0.8.3b20230712/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:04:18.420117 autogluon.core-0.8.3b20230712/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.404116 autogluon.core-0.8.3b20230712/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.404116 autogluon.core-0.8.3b20230712/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.408116 autogluon.core-0.8.3b20230712/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.408116 autogluon.core-0.8.3b20230712/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.408116 autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.408116 autogluon.core-0.8.3b20230712/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29445 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17849 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    93846 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    39287 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.412116 autogluon.core-0.8.3b20230712/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   176163 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36043 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.416117 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.420117 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49501 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-12 09:04:00.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:04:18.408116 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:04:18.000000 autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29443 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17849 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93732 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59573 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39284 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.390701 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176270 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36043 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.394701 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49501 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-13 09:03:54.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:04:13.386701 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:04:13.000000 autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.8.3b20230712/PKG-INFO` & `autogluon.core-0.8.3b20230713/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
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

### Comparing `autogluon.core-0.8.3b20230712/setup.py` & `autogluon.core-0.8.3b20230713/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/__init__.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/constants.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/dataset.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/executors.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
             validation_performance = details.get("validation_performance", None)
             # when equals to -inf, trial finished with TimeLimitExceeded exception and didn't finish at least 1 epoch
             if validation_performance is None or validation_performance == float("-inf"):
                 continue
             trial_id = details.get("trial_id")
             file_id = trial_id  # unique identifier to files from this trial
             trial_model_name = os.path.join(model_name, file_id)
-            trial_model_path = model_path_root + trial_model_name + os.path.sep
+            trial_model_path = os.path.join(model_path_root, trial_model_name)
             hpo_models[trial_model_name] = dict(path=trial_model_path)
 
             hpo_models[trial_model_name] = dict(
                 path=trial_model_path,
                 val_score=validation_performance,
                 trial=trial,
                 hyperparameters=details["config"],
@@ -548,15 +548,15 @@
 
         hpo_models = {}  # stores all the model names and file paths to model objects created during this HPO run.
         hpo_model_performances = {}
         for trial in sorted(hpo_results["config_history"].keys()):
             # TODO: ignore models which were killed early by scheduler (eg. in Hyperband). How to ID these?
             file_id = f"T{trial+1}"  # unique identifier to files from this trial
             trial_model_name = os.path.join(model_name, file_id)
-            trial_model_path = model_path_root + trial_model_name + os.path.sep
+            trial_model_path = os.path.join(model_path_root, trial_model_name)
             trial_reward = self.scheduler.searcher.get_reward(hpo_results["config_history"][trial])
             if trial_reward is None or trial_reward == float("-inf"):
                 continue
             hpo_models[trial_model_name] = dict(
                 path=trial_model_path, val_score=trial_reward, trial=trial, hyperparameters=hpo_results["config_history"][trial]
             )
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/learner/abstract_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         """Create and return paths to save model objects, the learner object.
 
         Parameters
         ----------
         path_context: str
             Top-level directory where models and trainer will be saved.
         """
-        model_context = os.path.join(path_context, "models") + os.path.sep
+        model_context = os.path.join(path_context, "models")
         save_path = os.path.join(path_context, self.learner_file_name)
         return path_context, model_context, save_path
 
     def set_contexts(self, path_context: str):
         """Update the path where model, learner, and trainer objects will be saved.
         Also see `create_contexts`."""
         self.path, self.model_context, self.save_path = self.create_contexts(path_context)
@@ -82,15 +82,15 @@
                 trainer = self.trainer
                 self.trainer = None
         save_pkl.save(path=self.save_path, object=self)
         self.trainer = trainer
 
     @classmethod
     def load(cls, path_context, reset_paths=True):
-        load_path = path_context + cls.learner_file_name
+        load_path = os.path.join(path_context, cls.learner_file_name)
         obj = load_pkl.load(path=load_path)
         if reset_paths:
             obj.set_contexts(path_context)
             if obj.trainer_path is not None:
                 obj.trainer_path = obj.model_context
             obj.reset_paths = reset_paths
             # TODO: Still have to change paths of models in trainer + trainer object path variables
@@ -109,36 +109,38 @@
 
     def load_trainer(self) -> AbstractTrainer:
         if self.trainer is not None:
             return self.trainer
         else:
             if self.trainer_path is None:
                 raise AssertionError("Trainer does not exist.")
-            return self.trainer_type.load(path=self.trainer_path, reset_paths=self.reset_paths)  # noqa
+            # trainer_path is used to determine if there's a trained trainer
+            # model_context contains the new trainer_path with updated context
+            return self.trainer_type.load(path=self.model_context, reset_paths=self.reset_paths)  # noqa
 
     # reset_paths=True if the learner files have changed location since fitting.
     # TODO: Potentially set reset_paths=False inside load function if it is the same path to
     # TODO: avoid re-computing paths on all models path_context -> path for v0.1
     @classmethod
     def load_info(cls, path, reset_paths=True, load_model_if_required=True):
-        load_path = path + cls.learner_info_name
+        load_path = os.path.join(path, cls.learner_info_name)
         try:
             return load_pkl.load(path=load_path)
         except Exception as e:
             if load_model_if_required:
                 learner = cls.load(path_context=path, reset_paths=reset_paths)
                 return learner.get_info()
             else:
                 raise e
 
     def save_info(self, include_model_info=False):
         info = self.get_info(include_model_info=include_model_info)
 
-        save_pkl.save(path=self.path + self.learner_info_name, object=info)
-        save_json.save(path=self.path + self.learner_info_json_name, obj=info)
+        save_pkl.save(path=os.path.join(self.path, self.learner_info_name), object=info)
+        save_json.save(path=os.path.join(self.path, self.learner_info_json_name), obj=info)
         return info
 
     def get_info(self, **kwargs):
         learner_info = {
             "path": self.path,
             "random_state": self.random_state,
             "version": self.version,
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/_utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     Parameters
     ----------
     path : str, default = None
         Directory location to store all outputs.
         If None, a new unique time-stamped directory is chosen.
     name : str, default = None
         Name of the subdirectory inside path where model will be saved.
-        The final model directory will be path+name+os.path.sep()
+        The final model directory will be os.path.join(path, name)
         If None, defaults to the model's class name: self.__class__.__name__
     problem_type : str, default = None
         Type of prediction problem, i.e. is this a binary/multiclass classification or regression problem (options: 'binary', 'multiclass', 'regression').
         If None, will attempt to infer the problem type based on training data labels during training.
     eval_metric : :class:`autogluon.core.metrics.Scorer` or str, default = None
         Metric by which predictions will be ultimately evaluated on test data.
         This only impacts `model.score()`, as eval_metric is not used during training.
@@ -108,26 +108,20 @@
             logger.log(20, f"Warning: No name was specified for model, defaulting to class name: {self.name}")
         else:
             self.name = name  # TODO: v0.1 Consider setting to self._name and having self.name be a property so self.name can't be set outside of self.rename()
 
         self.path_root = path
         if self.path_root is None:
             path_suffix = self.name
-            if len(self.name) > 0:
-                if self.name[0] != os.path.sep:
-                    path_suffix = os.path.sep + path_suffix
             # TODO: Would be ideal to not create dir, but still track that it is unique. However, this isn't possible to do without a global list of used dirs or using UUID.
             path_cur = setup_outputdir(path=None, create_dir=True, path_suffix=path_suffix)
             self.path_root = path_cur.rsplit(self.path_suffix, 1)[0]
             logger.log(20, f"Warning: No path was specified for model, defaulting to: {self.path_root}")
 
-        # v0.9 FIXME: This is a hack, change so we aren't vulnerable to self.path_root breaking things
-        self.path_root = PathConverter.to_relative(self.path_root)
-
-        self.path = self.create_contexts(self.path_root + self.path_suffix)  # TODO: Make this path a function for consistency.
+        self.path = self.create_contexts(os.path.join(self.path_root, self.path_suffix))  # TODO: Make this path a function for consistency.
 
         self.num_classes = None
         self.model = None
         self.problem_type = problem_type
 
         # whether to calibrate predictions via conformal methods
         self.conformalize = None
@@ -252,15 +246,15 @@
         hyperparameters_aux = self._user_params_aux
         self._set_default_auxiliary_params()
         if hyperparameters_aux is not None:
             self.params_aux.update(hyperparameters_aux)
 
     @property
     def path_suffix(self):
-        return self.name + os.path.sep
+        return self.name
 
     def is_valid(self) -> bool:
         """
         Returns True if the model is capable of inference on new data (if normal model) or has produced out-of-fold predictions (if bagged model)
         This indicates whether the model can be used as a base model to fit a stack ensemble model.
         """
         return self.is_fit()
@@ -369,15 +363,18 @@
     @staticmethod
     def create_contexts(path_context):
         path = path_context
         return path
 
     def rename(self, name: str):
         """Renames the model and updates self.path to reflect the updated name."""
-        self.path = self.path[: -len(self.name) - 1] + name + os.path.sep
+        if self.name is not None and len(self.name) > 0:
+            self.path = os.path.join(os.path.dirname(self.path), name)
+        else:
+            self.path = os.path.join(self.path, name)
         self.name = name
 
     def preprocess(self, X, preprocess_nonadaptive=True, preprocess_stateful=True, **kwargs):
         """
         Preprocesses the input data into internal form ready for fitting or inference.
         It is not recommended to override this method, as it is closely tied to multi-layer stacking logic. Instead, override `_preprocess`.
         """
@@ -998,15 +995,15 @@
 
         Parameters
         ----------
         path : str, default None
             Path to the saved model, minus the file name.
             This should generally be a directory path ending with a '/' character (or appropriate path separator value depending on OS).
             If None, self.path is used.
-            The final model file is typically saved to path + self.model_file_name.
+            The final model file is typically saved to os.path.join(path, self.model_file_name).
         verbose : bool, default True
             Whether to log the location of the saved file.
 
         Returns
         -------
         path : str
             Path to the saved model, minus the file name.
@@ -1033,28 +1030,28 @@
         Loads the model from disk to memory.
 
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
 
         Returns
         -------
         model : cls
             Loaded model object.
         """
-        file_path = path + cls.model_file_name
+        file_path = os.path.join(path, cls.model_file_name)
         model = load_pkl.load(path=file_path, verbose=verbose)
         if reset_paths:
             model.set_contexts(path)
         if hasattr(model, "_compiler"):
             if model._compiler is not None and not model._compiler.save_in_pkl:
                 model.model = model._compiler.load(path=path)
         return model
@@ -1704,29 +1701,29 @@
             "memory_size": self.get_memory_size(),  # Memory usage of model in bytes
             "compile_time": self.compile_time if hasattr(self, "compile_time") else None,
         }
         return info
 
     @classmethod
     def load_info(cls, path, load_model_if_required=True) -> dict:
-        load_path = path + cls.model_info_name
+        load_path = os.path.join(path, cls.model_info_name)
         try:
             return load_pkl.load(path=load_path)
         except:
             if load_model_if_required:
                 model = cls.load(path=path, reset_paths=True)
                 return model.get_info()
             else:
                 raise
 
     def save_info(self) -> dict:
         info = self.get_info()
 
-        save_pkl.save(path=self.path + self.model_info_name, object=info)
-        json_path = self.path + self.model_info_json_name
+        save_pkl.save(path=os.path.join(self.path, self.model_info_name), object=info)
+        json_path = os.path.join(self.path, self.model_info_json_name)
         save_json.save(path=json_path, obj=info)
         return info
 
     def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
         """
         Get the maximum resources allowed to use for this model.
         This can be useful when model not scale well with resources, i.e. cpu cores.
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/abstract/model_trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         if "hyperparameters" not in init_params["model_base_kwargs"]:
             init_params["model_base_kwargs"]["hyperparameters"] = {}
         init_params["model_base_kwargs"]["hyperparameters"].update(args)
     else:
         if "hyperparameters" not in init_params:
             init_params["hyperparameters"] = {}
         init_params["hyperparameters"].update(args)
-    init_params["name"] = init_params["name"] + os.path.sep + file_prefix
+    init_params["name"] = os.path.join(init_params["name"], file_prefix)
 
     return model_cls(**init_params)
 
 
 def fit_and_save_model(model, fit_args, predict_proba_args, y_val, time_start, time_limit=None):
     time_current = time.time()
     time_elapsed = time_current - time_start
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,15 +370,15 @@
 
     def _fit_single(self, X, y, model_base, use_child_oof, time_limit=None, skip_oof=False, **kwargs):
         if self.is_fit():
             raise AssertionError("Model is already fit.")
         if self._n_repeats != 0:
             raise ValueError(f"n_repeats must equal 0 when fitting a single model with k_fold == 1, value: {self._n_repeats}")
         model_base.name = f"{model_base.name}S1F1"
-        model_base.set_contexts(path_context=self.path + model_base.name + os.path.sep)
+        model_base.set_contexts(path_context=os.path.join(self.path, model_base.name))
         time_start_fit = time.time()
         model_base.fit(X=X, y=y, time_limit=time_limit, **kwargs)
         model_base.fit_time = time.time() - time_start_fit
         model_base.predict_time = None
         if not skip_oof:
             X_len = len(X)
             # Check if pred_proba is going to take too long
@@ -744,15 +744,15 @@
 
     def get_features(self):
         assert self.is_fit(), "The model must be fit before calling the get_features method."
         return self.load_child(self.models[0]).get_features()
 
     def load_child(self, model: Union[AbstractModel, str], verbose=False) -> AbstractModel:
         if isinstance(model, str):
-            child_path = self.create_contexts(self.path + model + os.path.sep)
+            child_path = self.create_contexts(os.path.join(self.path, model))
             return self._child_type.load(path=child_path, verbose=verbose)
         else:
             return model
 
     def add_child(self, model: Union[AbstractModel, str], add_child_times=False):
         """
         Add a new fit child model to `self.models`
@@ -784,15 +784,15 @@
             self._add_child_times_to_bag(model=model)
 
     def save_child(self, model: Union[AbstractModel, str], path=None, verbose=False):
         """Save child model to disk."""
         if path is None:
             path = self.path
         child = self.load_child(model)
-        child.set_contexts(path + child.name + os.path.sep)
+        child.set_contexts(os.path.join(path, child.name))
         child.save(verbose=verbose)
 
     def can_compile(self, compiler_configs=None):
         """Check if child models can compile"""
         if not self.is_fit():
             return False
         return self.load_child(self.models[0]).can_compile(compiler_configs=compiler_configs)
@@ -950,36 +950,36 @@
         if load_oof:
             model._load_oof()
         return model
 
     @classmethod
     def load_oof(cls, path, verbose=True):
         try:
-            oof = load_pkl.load(path=os.path.join(path + "utils", cls._oof_filename), verbose=verbose)
+            oof = load_pkl.load(path=os.path.join(path, "utils", cls._oof_filename), verbose=verbose)
             oof_pred_proba = oof["_oof_pred_proba"]
             oof_pred_model_repeats = oof["_oof_pred_model_repeats"]
         except FileNotFoundError:
             model = cls.load(path=path, reset_paths=True, verbose=verbose)
             model._load_oof()
             oof_pred_proba = model._oof_pred_proba
             oof_pred_model_repeats = model._oof_pred_model_repeats
         return cls._oof_pred_proba_func(oof_pred_proba=oof_pred_proba, oof_pred_model_repeats=oof_pred_model_repeats)
 
     def _load_oof(self):
         if self._oof_pred_proba is not None:
             pass
         else:
-            oof = load_pkl.load(path=os.path.join(self.path + "utils", self._oof_filename))
+            oof = load_pkl.load(path=os.path.join(self.path, "utils", self._oof_filename))
             self._oof_pred_proba = oof["_oof_pred_proba"]
             self._oof_pred_model_repeats = oof["_oof_pred_model_repeats"]
 
     def persist_child_models(self, reset_paths=True):
         for i, model_name in enumerate(self.models):
             if isinstance(model_name, str):
-                child_path = self.create_contexts(self.path + model_name + os.path.sep)
+                child_path = self.create_contexts(os.path.join(self.path, model_name))
                 child_model = self._child_type.load(path=child_path, reset_paths=reset_paths, verbose=True)
                 self.models[i] = child_model
 
     def unpersist_child_models(self):
         self.models = self._get_child_model_names(models=self.models)
 
     def _get_child_model_names(self, models: list) -> list:
@@ -988,30 +988,30 @@
             if isinstance(model, str):
                 model_names.append(model)
             else:
                 model_names.append(model.name)
         return model_names
 
     def load_model_base(self):
-        return load_pkl.load(path=os.path.join(self.path + "utils", "model_template.pkl"))
+        return load_pkl.load(path=os.path.join(self.path, "utils", "model_template.pkl"))
 
     def save_model_base(self, model_base):
-        save_pkl.save(path=os.path.join(self.path + "utils", "model_template.pkl"), object=model_base)
+        save_pkl.save(path=os.path.join(self.path, "utils", "model_template.pkl"), object=model_base)
 
     def save(self, path=None, verbose=True, save_oof=True, save_children=False) -> str:
         if path is None:
             path = self.path
 
         if save_children:
             for child in self.models:
                 self.save_child(model=child, path=path, verbose=False)
 
         if save_oof and self._oof_pred_proba is not None:
             save_pkl.save(
-                path=os.path.join(path + "utils", self._oof_filename),
+                path=os.path.join(path, "utils", self._oof_filename),
                 object={
                     "_oof_pred_proba": self._oof_pred_proba,
                     "_oof_pred_model_repeats": self._oof_pred_model_repeats,
                 },
             )
             self._oof_pred_proba = None
             self._oof_pred_model_repeats = None
@@ -1025,28 +1025,28 @@
 
     # If `remove_fit_stack=True`, variables will be removed that are required to fit more folds and to fit new stacker models which use this model as a base model.
     #  This includes OOF variables.
     def reduce_memory_size(self, remove_fit_stack=False, remove_fit=True, remove_info=False, requires_save=True, reduce_children=False, **kwargs):
         super().reduce_memory_size(remove_fit=remove_fit, remove_info=remove_info, requires_save=requires_save, **kwargs)
         if remove_fit_stack:
             try:
-                os.remove(os.path.join(self.path + "utils", self._oof_filename))
+                os.remove(os.path.join(self.path, "utils", self._oof_filename))
             except FileNotFoundError:
                 pass
             if requires_save:
                 self._oof_pred_proba = None
                 self._oof_pred_model_repeats = None
             try:
-                os.remove(os.path.join(self.path + "utils", "model_template.pkl"))
+                os.remove(os.path.join(self.path, "utils", "model_template.pkl"))
             except FileNotFoundError:
                 pass
             if requires_save:
                 self.model_base = None
             try:
-                os.rmdir(self.path + "utils")
+                os.rmdir(os.path.join(self.path, "utils"))
             except OSError:
                 pass
         if reduce_children:
             for model in self.models:
                 model = self.load_child(model)
                 model.reduce_memory_size(remove_fit=remove_fit, remove_info=remove_info, requires_save=requires_save, **kwargs)
                 if requires_save and self.low_memory:
@@ -1132,15 +1132,15 @@
         # memory is checked downstream on the child model
         pass
 
     def _get_child_info(self):
         child_info_dict = dict()
         for model in self.models:
             if isinstance(model, str):
-                child_path = self.create_contexts(self.path + model + os.path.sep)
+                child_path = self.create_contexts(os.path.join(self.path, model))
                 child_info_dict[model] = self._child_type.load_info(child_path)
             else:
                 child_info_dict[model.name] = model.get_info()
         return child_info_dict
 
     def _construct_empty_oof(self, X, y):
         if self.problem_type == MULTICLASS:
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,15 @@
     def _fit(self, model_base, time_start_fold, time_limit_fold, fold_ctx, kwargs):
         fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = self._get_fold_properties(fold_ctx)
         train_index, val_index = fold
         X_fold, X_val_fold = self.X.iloc[train_index, :], self.X.iloc[val_index, :]
         y_fold, y_val_fold = self.y.iloc[train_index], self.y.iloc[val_index]
         fold_model = copy.deepcopy(model_base)
         fold_model.name = f"{fold_model.name}{model_name_suffix}"
-        fold_model.set_contexts(self.bagged_ensemble_model.path + fold_model.name + os.path.sep)
+        fold_model.set_contexts(os.path.join(self.bagged_ensemble_model.path, fold_model.name))
         kwargs_fold = kwargs.copy()
         is_pseudo = self.X_pseudo is not None and self.y_pseudo is not None
         if self.sample_weight is not None:
             kwargs_fold["sample_weight"] = self.sample_weight[train_index]
             kwargs_fold["sample_weight_val"] = self.sample_weight[val_index]
 
             if is_pseudo:
@@ -375,15 +375,15 @@
     logger.debug(f"executing fold on node {node_id}")
     logger.log(10, "ray worker training")
     time_start_fold = time.time()
     fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = FoldFittingStrategy._get_fold_properties(fold_ctx)
     train_index, val_index = fold
     fold_model = copy.deepcopy(model_base)
     fold_model.name = f"{fold_model.name}{model_name_suffix}"
-    fold_model_local_save_path = bagged_ensemble_model_path + fold_model.name + os.path.sep
+    fold_model_local_save_path = os.path.join(bagged_ensemble_model_path, fold_model.name)
     fold_model.set_contexts(fold_model_local_save_path)
     if type(X) == str and type(y) == str:
         with open(X, "rb") as X_f, open(y, "rb") as y_f:
             X = pickle.load(X_f)
             y = pickle.load(y_f)
     is_pseudo = False
     if X_pseudo is not None and y_pseudo is not None:
@@ -551,15 +551,15 @@
                     fold_ctx=fold_ctx,
                 )
                 model_sync_path = None
                 if self.model_sync_path is not None:
                     model_sync_path: str = self.model_sync_path + fold_model
                     if not model_sync_path.endswith("/"):
                         model_sync_path += "/"
-                self.sync_model_artifact(local_path=os.path.join(self.bagged_ensemble_model.path + fold_model), model_sync_path=model_sync_path)
+                self.sync_model_artifact(local_path=os.path.join(self.bagged_ensemble_model.path, fold_model), model_sync_path=model_sync_path)
             except TimeLimitExceeded:
                 # Terminate all ray tasks because a fold failed
                 self.terminate_all_unfinished_tasks(unfinished)
                 raise TimeLimitExceeded
             # NotEnoughMemoryError is an autogluon custom error,
             # it predict memory usage before hand
             # MemoryError is the actual python memory error if the process failed
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,19 +50,15 @@
             base_models_dict = {}
         if base_model_paths_dict is None:
             base_model_paths_dict = {}
         if base_model_types_dict is None:
             base_model_types_dict = {}
         self.base_model_names = base_model_names
         self.base_models_dict: Dict[str, AbstractModel] = base_models_dict  # String name -> Model objects
-        self.base_model_paths_dict = base_model_paths_dict
-
-        # FIXME: DO NOT DO THIS, FIX ASAP
-        self.base_model_paths_dict = {k: PathConverter.to_relative(v) for k, v in self.base_model_paths_dict.items()}
-
+        self.base_model_paths_dict = {key: os.path.relpath(val, self.path) for key, val in base_model_paths_dict.items()}
         self.base_model_types_dict = base_model_types_dict
 
         # TODO: Consider deleting these variables after initialization
         self._base_model_performances_dict = base_model_performances_dict
         self._base_model_types_inner_dict = base_model_types_inner_dict
 
     def _initialize(self, **kwargs):
@@ -164,26 +160,14 @@
         start_time = time.time()
         # TODO: This could be preprocess_nonadaptive=True in general, just have preprocess_nonadaptive=False for child models
         X = self.preprocess(X=X, preprocess_nonadaptive=False, fit=True, compute_base_preds=compute_base_preds)
         if time_limit is not None:
             time_limit = time_limit - (time.time() - start_time)
         return super()._fit(X=X, y=y, time_limit=time_limit, **kwargs)
 
-    def set_contexts(self, path_context):
-        path_root_orig = self.path_root
-        path_root_orig = PathConverter.to_current(path_root_orig)
-        self.path_root = path_root_orig
-        abs_path_root_orig = os.path.abspath(path_root_orig) + os.path.sep
-        self.base_model_paths_dict = {model: PathConverter.to_current(model_path) for model, model_path in self.base_model_paths_dict.items()}
-        super().set_contexts(path_context=path_context)
-        for model, model_path in self.base_model_paths_dict.items():
-            model_path = os.path.abspath(model_path) + os.path.sep
-            model_local_path = model_path.split(abs_path_root_orig, 1)[1]
-            self.base_model_paths_dict[model] = self.path_root + model_local_path
-
     def set_stack_columns(self, stack_column_prefix_lst):
         if self.problem_type in [MULTICLASS, SOFTCLASS]:
             stack_columns = [stack_column_prefix + "_" + str(cls) for stack_column_prefix in stack_column_prefix_lst for cls in range(self.num_classes)]
             num_pred_cols_per_model = self.num_classes
         elif self.problem_type == QUANTILE:
             stack_columns = [stack_column_prefix + "_" + str(q) for stack_column_prefix in stack_column_prefix_lst for q in self.quantile_levels]
             num_pred_cols_per_model = len(self.quantile_levels)
@@ -212,15 +196,15 @@
         return init_args
 
     def load_base_model(self, model_name):
         if model_name in self.base_models_dict.keys():
             model = self.base_models_dict[model_name]
         else:
             model_type = self.base_model_types_dict[model_name]
-            model_path = self.base_model_paths_dict[model_name]
+            model_path = os.path.join(self.path, self.base_model_paths_dict[model_name])
             model = model_type.load(model_path)
         return model
 
     def get_info(self):
         info = super().get_info()
         stacker_info = dict(
             num_base_models=len(self.base_model_names),
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/problem_type.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/space.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         sample_weight=None,
         weight_evaluation=False,
         save_data=False,
         random_state=0,
         verbosity=2,
     ):
         self.path = path
-        self.path = PathConverter.to_relative(self.path)
         self.problem_type = problem_type
         self.feature_metadata = feature_metadata
         self.save_data = save_data
         self.random_state = (
             random_state  # Integer value added to the stack level to get the random_state for kfold splits or the train/val split if bagging is disabled
         )
         self.verbosity = verbosity
@@ -175,83 +174,83 @@
         self._models_failed_to_train = []  # List of models which failed to train
 
         # self._exceptions_list = []  # TODO: Keep exceptions list for debugging during benchmarking.
 
     # path_root is the directory containing learner.pkl
     @property
     def path_root(self) -> str:
-        return self.path.rsplit(os.path.sep, maxsplit=2)[0] + os.path.sep
+        return os.path.dirname(self.path)
 
     @property
     def path_utils(self) -> str:
-        return self.path_root + "utils" + os.path.sep
+        return os.path.join(self.path_root, "utils")
 
     @property
     def _path_attr(self) -> str:
         """Path to cached model graph attributes"""
-        return f"{self.path_utils}attr{os.path.sep}"
+        return os.path.join(self.path_utils, "attr")
 
     @property
     def path_data(self) -> str:
-        return self.path_utils + "data" + os.path.sep
+        return os.path.join(self.path_utils, "data")
 
     @property
     def has_val(self) -> bool:
         """Whether the trainer uses validation data"""
         return self._num_rows_val is not None
 
     def load_X(self):
         if self._X_saved:
-            path = self.path_data + "X.pkl"
+            path = os.path.join(self.path_data, "X.pkl")
             return load_pkl.load(path=path)
         return None
 
     def load_X_val(self):
         if self._X_val_saved:
-            path = self.path_data + "X_val.pkl"
+            path = os.path.join(self.path_data, "X_val.pkl")
             return load_pkl.load(path=path)
         return None
 
     def load_y(self):
         if self._y_saved:
-            path = self.path_data + "y.pkl"
+            path = os.path.join(self.path_data, "y.pkl")
             return load_pkl.load(path=path)
         return None
 
     def load_y_val(self):
         if self._y_val_saved:
-            path = self.path_data + "y_val.pkl"
+            path = os.path.join(self.path_data, "y_val.pkl")
             return load_pkl.load(path=path)
         return None
 
     def load_data(self):
         X = self.load_X()
         y = self.load_y()
         X_val = self.load_X_val()
         y_val = self.load_y_val()
 
         return X, y, X_val, y_val
 
     def save_X(self, X, verbose=True):
-        path = self.path_data + "X.pkl"
+        path = os.path.join(self.path_data, "X.pkl")
         save_pkl.save(path=path, object=X, verbose=verbose)
         self._X_saved = True
 
     def save_X_val(self, X, verbose=True):
-        path = self.path_data + "X_val.pkl"
+        path = os.path.join(self.path_data, "X_val.pkl")
         save_pkl.save(path=path, object=X, verbose=verbose)
         self._X_val_saved = True
 
     def save_y(self, y, verbose=True):
-        path = self.path_data + "y.pkl"
+        path = os.path.join(self.path_data, "y.pkl")
         save_pkl.save(path=path, object=y, verbose=verbose)
         self._y_saved = True
 
     def save_y_val(self, y, verbose=True):
-        path = self.path_data + "y_val.pkl"
+        path = os.path.join(self.path_data, "y_val.pkl")
         save_pkl.save(path=path, object=y, verbose=verbose)
         self._y_val_saved = True
 
     def get_model_names(
         self, stack_name: Union[List[str], str] = None, level: Union[List[int], int] = None, can_infer: bool = None, models: List[str] = None
     ) -> List[str]:
         if models is None:
@@ -288,31 +287,20 @@
         """Constructs a list of unfit models based on the hyperparameters dict for softclass distillation."""
         raise NotImplementedError
 
     def get_model_level(self, model_name: str) -> int:
         return self.get_model_attribute(model=model_name, attribute="level")
 
     def set_contexts(self, path_context):
-        self.path, model_paths = self.create_contexts(path_context)
-        for model, path in model_paths.items():
-            self.set_model_attribute(model=model, attribute="path", val=path)
+        self.path = self.create_contexts(path_context)
 
-    def create_contexts(self, path_context: str) -> (str, dict):
-        self.path = PathConverter.to_current(self.path)
+    def create_contexts(self, path_context: str) -> str:
         path = path_context
-        model_paths = self.get_models_attribute_dict(attribute="path")
-        model_paths = {model: PathConverter.to_current(model_path) for model, model_path in model_paths.items()}
-        for model, prev_path in model_paths.items():
-            prev_path = os.path.abspath(prev_path) + os.path.sep
-            abs_path = os.path.abspath(self.path) + os.path.sep
-            model_local_path = prev_path.split(abs_path, 1)[1]
-            new_path = path + model_local_path
-            model_paths[model] = new_path
 
-        return path, model_paths
+        return path
 
     def fit(self, X, y, hyperparameters: dict, X_val=None, y_val=None, **kwargs):
         raise NotImplementedError
 
     # TODO: Enable easier re-mapping of trained models -> hyperparameters input (They don't share a key since name can change)
     def train_multi_levels(
         self,
@@ -1119,15 +1107,15 @@
             return model_pred_dict
 
     def get_model_oof(self, model: str) -> np.ndarray:
         """Gets the out of fold prediction probabilities for a bagged ensemble model"""
         model_type = self.get_model_attribute(model=model, attribute="type")
         if issubclass(model_type, BaggedEnsembleModel):
             model_path = self.get_model_attribute(model=model, attribute="path")
-            return model_type.load_oof(path=model_path)
+            return model_type.load_oof(path=os.path.join(self.path, model_path))
         else:
             raise AssertionError(f"Model {model} must be a BaggedEnsembleModel to return oof_pred_proba")
 
     def _update_pred_proba_dict_with_val_cache(self, model_set: set, model_pred_proba_dict):
         """For each model in model_set, check if y_pred_proba_val is cached to disk. If so, load and add it to model_pred_proba_dict"""
         for model in model_set:
             y_pred_proba = self.get_model_attribute(model, attribute="cached_y_pred_proba_val", default=None)
@@ -1412,15 +1400,15 @@
         else:
             self.models[model.name] = model
 
     def save(self):
         models = self.models
         if self.low_memory:
             self.models = {}
-        save_pkl.save(path=self.path + self.trainer_file_name, object=self)
+        save_pkl.save(path=os.path.join(self.path, self.trainer_file_name), object=self)
         if self.low_memory:
             self.models = models
 
     def compile_models(self, model_names="all", with_ancestors=False, compiler_configs=None) -> List[str]:
         """
         Compile a list of models for accelerated prediction.
 
@@ -1564,18 +1552,18 @@
     def load_model(self, model_name: str, path: str = None, model_type=None) -> AbstractModel:
         if isinstance(model_name, AbstractModel):
             return model_name
         if model_name in self.models.keys():
             return self.models[model_name]
         else:
             if path is None:
-                path = self.get_model_attribute(model=model_name, attribute="path")
+                path = self.get_model_attribute(model=model_name, attribute="path")  # get relative location of the model to the trainer
             if model_type is None:
                 model_type = self.get_model_attribute(model=model_name, attribute="type")
-            return model_type.load(path=path, reset_paths=self.reset_paths)
+            return model_type.load(path=os.path.join(self.path, path), reset_paths=self.reset_paths)
 
     def unpersist_models(self, model_names="all") -> list:
         if model_names == "all":
             model_names = list(self.models.keys())
         if not isinstance(model_names, list):
             raise ValueError(f"model_names must be a list of model names. Invalid value: {model_names}")
         unpersisted_models = []
@@ -1619,24 +1607,26 @@
         if save_bag_folds is None:
             can_infer_dict = self.get_models_attribute_dict("can_infer", models=base_model_names)
             if False in can_infer_dict.values():
                 save_bag_folds = False
             else:
                 save_bag_folds = True
 
+        base_model_paths_dict = self.get_models_attribute_dict(attribute="path", models=base_model_names)
+        base_model_paths_dict = {key: os.path.join(self.path, val) for key, val in base_model_paths_dict.items()}
         weighted_ensemble_model, _ = get_models_func(
             hyperparameters={
                 "default": {
                     "ENS_WEIGHTED": [child_hyperparameters],
                 }
             },
             ensemble_type=WeightedEnsembleModel,
             ensemble_kwargs=dict(
                 base_model_names=base_model_names,
-                base_model_paths_dict=self.get_models_attribute_dict(attribute="path", models=base_model_names),
+                base_model_paths_dict=base_model_paths_dict,
                 base_model_types_dict=self.get_models_attribute_dict(attribute="type", models=base_model_names),
                 base_model_types_inner_dict=self.get_models_attribute_dict(attribute="type_inner", models=base_model_names),
                 base_model_performances_dict=self.get_models_attribute_dict(attribute="val_score", models=base_model_names),
                 hyperparameters=hyperparameters,
                 random_state=level + self.random_state,
             ),
             ag_args={"name_bag_suffix": ""},
@@ -1855,15 +1845,15 @@
             fit_time=model.fit_time,
             compile_time=model.compile_time,
             predict_time=model.predict_time,
             predict_1_time=model.predict_1_time,
             predict_child_time=predict_child_time,
             predict_1_child_time=predict_1_child_time,
             val_score=model.val_score,
-            path=model.path,
+            path=os.path.relpath(model.path, self.path).split(os.sep),  # model's relative path to trainer
             type=type(model),  # Outer type, can be BaggedEnsemble, StackEnsemble (Type that is able to load the model)
             type_inner=type_inner,  # Inner type, if Ensemble then it is the type of the inner model (May not be able to load with this type)
             can_infer=model.can_infer(),
             can_fit=model.can_fit(),
             is_valid=model.is_valid(),
             stack_name=stack_name,
             level=level,
@@ -1888,19 +1878,19 @@
         self._log_model_stats(model)
         if self.low_memory:
             del model
         return True
 
     def _path_attr_model(self, model: str):
         """Returns directory where attributes are cached"""
-        return f"{self._path_attr}{model}{os.path.sep}"
+        return os.path.join(self._path_attr, model)
 
     def _path_to_model_attr(self, model: str, attribute: str):
         """Returns pkl file path for a cached model attribute"""
-        return f"{self._path_attr_model(model)}{attribute}.pkl"
+        return os.path.join(self._path_attr_model(model), f"{attribute}.pkl")
 
     def _save_model_y_pred_proba_val(self, model: str, y_pred_proba_val):
         """Cache y_pred_proba_val for later reuse to avoid redundant predict calls"""
         save_pkl.save(path=self._path_to_model_attr(model=model, attribute="y_pred_proba_val"), object=y_pred_proba_val)
 
     def _load_model_y_pred_proba_val(self, model: str):
         """Load cached y_pred_proba_val for a given model"""
@@ -2033,15 +2023,15 @@
                 model_names_trained = []
             else:
                 # Commented out because it takes too much space (>>5 GB if run for an hour on a small-medium sized dataset)
                 # self.hpo_results[model.name] = hpo_results
                 model_names_trained = []
                 self._extra_banned_names.add(model.name)
                 for model_hpo_name, model_info in hpo_models.items():
-                    model_hpo = self.load_model(model_hpo_name, path=model_info["path"], model_type=type(model))
+                    model_hpo = self.load_model(model_hpo_name, path=os.path.relpath(model_info["path"], self.path), model_type=type(model))
                     logger.log(20, f"Fitted model: {model_hpo.name} ...")
                     if self._add_model(model=model_hpo, stack_name=stack_name, level=level):
                         model_names_trained.append(model_hpo.name)
         else:
             model_fit_kwargs.update(dict(X_pseudo=X_pseudo, y_pseudo=y_pseudo))
             if isinstance(model, BaggedEnsembleModel):
                 bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(
@@ -2635,15 +2625,18 @@
         models_attribute_dict = nx.get_node_attributes(self.model_graph, attribute)
         if models is not None:
             model_names = []
             for model in models:
                 if not isinstance(model, str):
                     model = model.name
                 model_names.append(model)
-            models_attribute_dict = {key: val for key, val in models_attribute_dict.items() if key in model_names}
+            if attribute == "path":
+                models_attribute_dict = {key: os.path.join(*val) for key, val in models_attribute_dict.items() if key in model_names}
+            else:
+                models_attribute_dict = {key: val for key, val in models_attribute_dict.items() if key in model_names}
         return models_attribute_dict
 
     def get_model_attribute(self, model, attribute: str, **kwargs):
         """
         Return model attribute value.
         If `default` is specified, return default value if attribute does not exist.
         If `default` is not specified, raise ValueError if attribute does not exist.
@@ -2653,14 +2646,16 @@
         if model not in self.model_graph.nodes:
             raise ValueError(f"Model does not exist: (model={model})")
         if attribute not in self.model_graph.nodes[model]:
             if "default" in kwargs:
                 return kwargs["default"]
             else:
                 raise ValueError(f"Model does not contain attribute: (model={model}, attribute={attribute})")
+        if attribute == "path":
+            return os.path.join(*self.model_graph.nodes[model][attribute])
         return self.model_graph.nodes[model][attribute]
 
     def set_model_attribute(self, model, attribute: str, val):
         if not isinstance(model, str):
             model = model.name
         self.model_graph.nodes[model][attribute] = val
 
@@ -2912,28 +2907,28 @@
         for model in models:
             if isinstance(model, str):
                 if model in self.models.keys():
                     model = self.models[model]
             if isinstance(model, str):
                 model_type = self.get_model_attribute(model=model, attribute="type")
                 model_path = self.get_model_attribute(model=model, attribute="path")
-                model_info_dict[model] = model_type.load_info(path=model_path)
+                model_info_dict[model] = model_type.load_info(path=os.path.join(self.path, model_path))
             else:
                 model_info_dict[model.name] = model.get_info()
         return model_info_dict
 
     def reduce_memory_size(
         self, remove_data=True, remove_fit_stack=False, remove_fit=True, remove_info=False, requires_save=True, reduce_children=False, **kwargs
     ):
         if remove_data and self.is_data_saved:
             data_files = [
-                self.path_data + "X.pkl",
-                self.path_data + "X_val.pkl",
-                self.path_data + "y.pkl",
-                self.path_data + "y_val.pkl",
+                os.path.join(self.path_data, "X.pkl"),
+                os.path.join(self.path_data, "X_val.pkl"),
+                os.path.join(self.path_data, "y.pkl"),
+                os.path.join(self.path_data, "y_val.pkl"),
             ]
             for data_file in data_files:
                 try:
                     os.remove(data_file)
                 except FileNotFoundError:
                     pass
             if requires_save:
@@ -3027,40 +3022,40 @@
         if model in self.models:
             self.models.pop(model)
         path_attr_model = Path(self._path_attr_model(model))
         shutil.rmtree(path=path_attr_model, ignore_errors=True)
 
     @classmethod
     def load(cls, path, reset_paths=False):
-        load_path = path + cls.trainer_file_name
+        load_path = os.path.join(path, cls.trainer_file_name)
         if not reset_paths:
             return load_pkl.load(path=load_path)
         else:
             obj = load_pkl.load(path=load_path)
             obj.set_contexts(path)
             obj.reset_paths = reset_paths
             return obj
 
     @classmethod
     def load_info(cls, path, reset_paths=False, load_model_if_required=True):
-        load_path = path + cls.trainer_info_name
+        load_path = os.path.join(path, cls.trainer_info_name)
         try:
             return load_pkl.load(path=load_path)
         except:
             if load_model_if_required:
                 trainer = cls.load(path=path, reset_paths=reset_paths)
                 return trainer.get_info()
             else:
                 raise
 
     def save_info(self, include_model_info=False):
         info = self.get_info(include_model_info=include_model_info)
 
-        save_pkl.save(path=self.path + self.trainer_info_name, object=info)
-        save_json.save(path=self.path + self.trainer_info_json_name, obj=info)
+        save_pkl.save(path=os.path.join(self.path, self.trainer_info_name), object=info)
+        save_json.save(path=os.path.join(self.path, self.trainer_info_json_name), obj=info)
         return info
 
     def _process_hyperparameters(self, hyperparameters: dict) -> dict:
         return process_hyperparameters(hyperparameters=hyperparameters)
 
     def distill(
         self,
```

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/files.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/plots.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/time.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.8.3b20230713/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
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

### Comparing `autogluon.core-0.8.3b20230712/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.8.3b20230713/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

