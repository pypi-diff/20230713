# Comparing `tmp/rubicon-ml-0.4.5.tar.gz` & `tmp/rubicon-ml-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-ml-0.4.5.tar", last modified: Wed Jul 12 19:53:07 2023, max compression
+gzip compressed data, was "rubicon-ml-0.4.6.tar", last modified: Thu Jul 13 14:54:20 2023, max compression
```

## Comparing `rubicon-ml-0.4.5.tar` & `rubicon-ml-0.4.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.677426 rubicon-ml-0.4.5/rubicon_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-12 19:53:07.677426 rubicon-ml-0.4.5/rubicon_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.665425 rubicon-ml-0.4.5/rubicon_ml/client/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/rubicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.665425 rubicon-ml-0.4.5/rubicon_ml/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/utils/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/utils/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/utils/training_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/utils/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44598 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/repository/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/utils/slugify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/filter_estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.661425 rubicon-ml-0.4.5/rubicon_ml/viz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/common.css
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/dropdown-header.css
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/experiments-table.css
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/frame.css
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/metric-correlation-plot.css
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/metric-lists-comparison.css
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/plots-comparison.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/common/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/common/dropdown_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/dataframe_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/experiments_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/metric_correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/metric_lists_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.665425 rubicon-ml-0.4.5/rubicon_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-12 19:53:07.677426 rubicon-ml-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.105017 rubicon-ml-0.4.6/rubicon_ml/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/rubicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.105017 rubicon-ml-0.4.6/rubicon_ml/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/utils/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/client/utils/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.105017 rubicon-ml-0.4.6/rubicon_ml/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.105017 rubicon-ml-0.4.6/rubicon_ml/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/utils/training_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/domain/utils/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.109017 rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.109017 rubicon-ml-0.4.6/rubicon_ml/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44598 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.109017 rubicon-ml-0.4.6/rubicon_ml/repository/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/repository/utils/slugify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.109017 rubicon-ml-0.4.6/rubicon_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/sklearn/estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/sklearn/filter_estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/sklearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.109017 rubicon-ml-0.4.6/rubicon_ml/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.101017 rubicon-ml-0.4.6/rubicon_ml/viz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/dropdown-header.css
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/experiments-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/frame.css
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/metric-correlation-plot.css
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/metric-lists-comparison.css
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/css/plots-comparison.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/viz/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/viz/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/common/dropdown_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/dataframe_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/experiments_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/metric_correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/viz/metric_lists_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/rubicon_ml/workflow/prefect/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/workflow/prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/rubicon_ml/workflow/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.101017 rubicon-ml-0.4.6/rubicon_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 14:54:20.000000 rubicon-ml-0.4.6/rubicon_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:20.113017 rubicon-ml-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-13 14:54:06.000000 rubicon-ml-0.4.6/versioneer.py
```

### Comparing `rubicon-ml-0.4.5/LICENSE` & `rubicon-ml-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/PKG-INFO` & `rubicon-ml-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.4.5
+Version: 0.4.6
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.4.5/README.md` & `rubicon-ml-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/__init__.py` & `rubicon-ml-0.4.6/rubicon_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/cli.py` & `rubicon-ml-0.4.6/rubicon_ml/cli.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/__init__.py` & `rubicon-ml-0.4.6/rubicon_ml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/artifact.py` & `rubicon-ml-0.4.6/rubicon_ml/client/artifact.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/base.py` & `rubicon-ml-0.4.6/rubicon_ml/client/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/config.py` & `rubicon-ml-0.4.6/rubicon_ml/client/config.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/dataframe.py` & `rubicon-ml-0.4.6/rubicon_ml/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/experiment.py` & `rubicon-ml-0.4.6/rubicon_ml/client/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/feature.py` & `rubicon-ml-0.4.6/rubicon_ml/client/feature.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/metric.py` & `rubicon-ml-0.4.6/rubicon_ml/client/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/mixin.py` & `rubicon-ml-0.4.6/rubicon_ml/client/mixin.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/parameter.py` & `rubicon-ml-0.4.6/rubicon_ml/client/parameter.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/project.py` & `rubicon-ml-0.4.6/rubicon_ml/client/project.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/rubicon.py` & `rubicon-ml-0.4.6/rubicon_ml/client/rubicon.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/utils/exception_handling.py` & `rubicon-ml-0.4.6/rubicon_ml/client/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/client/utils/tags.py` & `rubicon-ml-0.4.6/rubicon_ml/client/utils/tags.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/domain/experiment.py` & `rubicon-ml-0.4.6/rubicon_ml/domain/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/domain/metric.py` & `rubicon-ml-0.4.6/rubicon_ml/domain/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/domain/utils/training_metadata.py` & `rubicon-ml-0.4.6/rubicon_ml/domain/utils/training_metadata.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/base.py` & `rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/experiment.py` & `rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/publish.py` & `rubicon-ml-0.4.6/rubicon_ml/intake_rubicon/publish.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/repository/base.py` & `rubicon-ml-0.4.6/rubicon_ml/repository/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/repository/local.py` & `rubicon-ml-0.4.6/rubicon_ml/repository/local.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/repository/memory.py` & `rubicon-ml-0.4.6/rubicon_ml/repository/memory.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/repository/s3.py` & `rubicon-ml-0.4.6/rubicon_ml/repository/s3.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/repository/utils/json.py` & `rubicon-ml-0.4.6/rubicon_ml/repository/utils/json.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/sklearn/estimator_logger.py` & `rubicon-ml-0.4.6/rubicon_ml/sklearn/estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/sklearn/filter_estimator_logger.py` & `rubicon-ml-0.4.6/rubicon_ml/sklearn/filter_estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/sklearn/pipeline.py` & `rubicon-ml-0.4.6/rubicon_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/assets/images/rubicon-logo-dark.png` & `rubicon-ml-0.4.6/rubicon_ml/viz/assets/images/rubicon-logo-dark.png`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/base.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/common/dropdown_header.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/common/dropdown_header.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/dashboard.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/dataframe_plot.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/dataframe_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/experiments_table.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/experiments_table.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/metric_correlation_plot.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/metric_correlation_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/viz/metric_lists_comparison.py` & `rubicon-ml-0.4.6/rubicon_ml/viz/metric_lists_comparison.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/__init__.py` & `rubicon-ml-0.4.6/rubicon_ml/workflow/prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/tasks.py` & `rubicon-ml-0.4.6/rubicon_ml/workflow/prefect/tasks.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/rubicon_ml.egg-info/PKG-INFO` & `rubicon-ml-0.4.6/rubicon_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.4.5
+Version: 0.4.6
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.4.5/rubicon_ml.egg-info/SOURCES.txt` & `rubicon-ml-0.4.6/rubicon_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/setup.cfg` & `rubicon-ml-0.4.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -24,39 +24,39 @@
 	Programming Language :: Python :: 3
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	click<=8.1.3,>=7.1
-	fsspec<=2023.5.0,>=2021.4.0
+	click<=8.1.4,>=7.1
+	fsspec<=2023.6.0,>=2021.4.0
 	intake[dataframe]<=0.7.0,>=0.5.2
-	numpy<=1.24.3,>=1.22.0
-	pandas<=2.0.2,>=1.0.0
-	pyarrow<=12.0.0,>=0.18.0
+	numpy<=1.25.1,>=1.22.0
+	pandas<=2.0.3,>=1.0.0
+	pyarrow<=12.0.1,>=0.18.0
 	PyYAML<=6.0,>=5.4.0
-	scikit-learn<=1.2.2,>=0.22.0
+	scikit-learn<=1.3.0,>=0.22.0
 
 [options.extras_require]
 prefect = 
 	prefect<=1.2.4,>=0.12.0
 s3 = 
-	s3fs<=2023.5.0,>=0.4
+	s3fs<=2023.6.0,>=0.4
 ui = 
-	dash<=2.10.2,>=2.0.0
+	dash<=2.11.1,>=2.0.0
 	dash-bootstrap-components<=1.4.1,>=1.0.0
 viz = 
-	dash<=2.10.2,>=2.0.0
+	dash<=2.11.1,>=2.0.0
 	dash-bootstrap-components<=1.4.1,>=1.0.0
 all = 
-	dash<=2.10.2,>=2.0.0
+	dash<=2.11.1,>=2.0.0
 	dash-bootstrap-components<=1.4.1,>=1.0.0
 	prefect<=1.2.4,>=0.12.0
-	s3fs<=2023.5.0,>=0.4
+	s3fs<=2023.6.0,>=0.4
 
 [options.entry_points]
 console_scripts = 
 	rubicon_ml = rubicon_ml.cli:cli
 intake.drivers = 
 	rubicon_ml_experiment = rubicon_ml.intake_rubicon.experiment:ExperimentSource
 
@@ -119,12 +119,14 @@
 	intake[dataframe]
 	numpy
 	pandas
 	pyarrow
 	PyYAML
 	s3fs
 	scikit-learn
+command = 
+	pytest -m 'not run_notebooks and not write_files'
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rubicon-ml-0.4.5/tests/fixtures.py` & `rubicon-ml-0.4.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.5/versioneer.py` & `rubicon-ml-0.4.6/versioneer.py`

 * *Files identical despite different names*

