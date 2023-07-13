# Comparing `tmp/torchtnt-nightly-2023.7.8.tar.gz` & `tmp/torchtnt-nightly-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-nightly-2023.7.8.tar", last modified: Sat Jul  8 11:23:34 2023, max compression
+gzip compressed data, was "torchtnt-nightly-2023.7.9.tar", last modified: Sun Jul  9 11:23:36 2023, max compression
```

## Comparing `torchtnt-nightly-2023.7.8.tar` & `torchtnt-nightly-2023.7.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.573476 torchtnt-nightly-2023.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-08 11:23:34.573476 torchtnt-nightly-2023.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 11:23:34.573476 torchtnt-nightly-2023.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.565476 torchtnt-nightly-2023.7.8/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.565476 torchtnt-nightly-2023.7.8/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36790 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.569476 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.569476 torchtnt-nightly-2023.7.8/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.569476 torchtnt-nightly-2023.7.8/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.573476 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/prepare_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-08 11:22:12.000000 torchtnt-nightly-2023.7.8/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:23:34.573476 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-08 11:23:34.000000 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-08 11:23:34.000000 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:23:34.000000 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-08 11:23:34.000000 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 11:23:34.000000 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:23:34.000000 torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.092377 torchtnt-nightly-2023.7.9/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.092377 torchtnt-nightly-2023.7.9/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36790 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/prepare_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.7.8/LICENSE` & `torchtnt-nightly-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/PKG-INFO` & `torchtnt-nightly-2023.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.8
+Version: 2023.7.9
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.8 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.9 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.8/README.md` & `torchtnt-nightly-2023.7.9/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/setup.py` & `torchtnt-nightly-2023.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/auto_unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/state.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/train.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.7.9/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/device.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/env.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/prepare_model.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/prepare_model.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/tqdm.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt/utils/version.py` & `torchtnt-nightly-2023.7.9/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.8
+Version: 2023.7.9
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.8 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.9 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.8/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

