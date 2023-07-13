# Comparing `tmp/TEST_TC-1.0.8.tar.gz` & `tmp/TEST_TC-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.0.8.tar", last modified: Thu Jul 13 07:33:43 2023, max compression
+gzip compressed data, was "TEST_TC-1.0.9.tar", last modified: Thu Jul 13 14:47:31 2023, max compression
```

## Comparing `TEST_TC-1.0.8.tar` & `TEST_TC-1.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:43.046536 TEST_TC-1.0.8/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.953462 TEST_TC-1.0.8/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.972519 TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-13 07:33:42.000000 TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1606 2023-07-13 07:33:42.000000 TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-13 07:33:42.000000 TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-13 07:33:42.000000 TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-13 07:33:42.000000 TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.974572 TEST_TC-1.0.8/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-13 07:33:33.000000 TEST_TC-1.0.8/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.985555 TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 11:05:00.000000 TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6569 2023-07-12 15:50:29.000000 TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/experiment_model.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7149 2023-07-12 14:57:21.000000 TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/hierarchical_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15204 2023-07-12 15:50:42.000000 TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.989054 TEST_TC-1.0.8/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4306 2023-07-10 11:09:32.000000 TEST_TC-1.0.8/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.992541 TEST_TC-1.0.8/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 11:10:43.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:42.998643 TEST_TC-1.0.8/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    23316 2023-07-12 14:57:21.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3730 2023-07-12 15:51:06.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:43.000346 TEST_TC-1.0.8/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:43.007578 TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8437 2023-07-12 14:57:21.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-13 07:16:53.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-12 14:57:21.000000 TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:43.020949 TEST_TC-1.0.8/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.8/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2125 2023-07-12 14:57:21.000000 TEST_TC-1.0.8/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 11:14:05.000000 TEST_TC-1.0.8/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7128 2023-07-12 15:51:56.000000 TEST_TC-1.0.8/LIB_tc/test_tc/utility/experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-12 14:57:21.000000 TEST_TC-1.0.8/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 11:15:17.000000 TEST_TC-1.0.8/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-13 07:33:43.045532 TEST_TC-1.0.8/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.8/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-13 07:32:16.000000 TEST_TC-1.0.8/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-13 07:33:43.047533 TEST_TC-1.0.8/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 07:33:43.043671 TEST_TC-1.0.8/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_experiment_job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_experiment_models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-07-12 14:57:22.000000 TEST_TC-1.0.8/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.799144 TEST_TC-1.0.9/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.674639 TEST_TC-1.0.9/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.697104 TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-13 14:47:31.000000 TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1606 2023-07-13 14:47:31.000000 TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-13 14:47:31.000000 TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-13 14:47:31.000000 TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-13 14:47:31.000000 TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.701496 TEST_TC-1.0.9/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-13 14:47:04.000000 TEST_TC-1.0.9/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.713000 TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 11:05:00.000000 TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6569 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/experiment_model.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7149 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/hierarchical_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15204 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.719075 TEST_TC-1.0.9/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4306 2023-07-10 11:09:32.000000 TEST_TC-1.0.9/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.723451 TEST_TC-1.0.9/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 11:10:43.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.730113 TEST_TC-1.0.9/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    23316 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3730 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.732999 TEST_TC-1.0.9/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.745748 TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8552 2023-07-13 14:13:36.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.765533 TEST_TC-1.0.9/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.9/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2229 2023-07-13 14:45:36.000000 TEST_TC-1.0.9/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 11:14:05.000000 TEST_TC-1.0.9/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7128 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/LIB_tc/test_tc/utility/experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 11:15:17.000000 TEST_TC-1.0.9/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-13 14:47:31.798148 TEST_TC-1.0.9/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.9/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-13 07:53:51.000000 TEST_TC-1.0.9/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-13 14:47:31.800272 TEST_TC-1.0.9/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-13 14:47:31.794373 TEST_TC-1.0.9/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_experiment_job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_experiment_models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-07-13 13:13:53.000000 TEST_TC-1.0.9/tests/test_tele_logger.py
```

### Comparing `TEST_TC-1.0.8/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.0.9/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/algorithm.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/experiment_model.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/experiment_model.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/hierarchical_utils.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/hierarchical_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/algorithms/prophet_utils.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/algorithms/prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/datapreparation/datapreparation_utils.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/datapreparation/datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/datapreparation/prep.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/datapreparation/prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     Returns
     -------
     _type_
         _description_
     """
 
+    df.index = [i for i in range(int(df.shape[0]/df.Id_pred.unique().shape[0]))] * df.Id_pred.unique().shape[0]
+
     if gerarchia == "Italia":
         n_level = len(gerarchia.split("/")) - 1
         split = np.array_split(df,df[id_pred].unique().shape[0])
         result = [i for i in split if i[id_pred].unique()[0].count("/") == n_level]
     else:
         n_level = len(gerarchia.split("/")) 
         split = np.array_split(df,df[id_pred].unique().shape[0])
```

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/utility/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from hierarchicalforecast.methods import BottomUp, MinTrace
+from hierarchicalforecast.methods import BottomUp, MinTrace, TopDown, OptimalCombination
 
 code_to_region_name: dict[int, str] = {
                  30: 'Lombardia',190: 'Sicilia',50: 'Veneto',80: 'Emilia-Romagna',120: 'Lazio',200: 'Sardegna',
                  150: 'Campania',10: 'Piemonte',42: 'Trento',70: 'Liguria',130: 'Abruzzo',100: 'Umbria',
                  180: 'Calabria',160: 'Puglia',110: 'Marche',90: 'Toscana',20: "Valle D Aosta",170: 'Basilicata',
                  60: 'Friuli-Venezia-Giulia',41: 'Bolzano',140: 'Molise'}
 
@@ -51,8 +51,8 @@
                     ]
 
 format_ = '.parquet'
 filenames_list = ["test_pred" + format_, "test_real" + format_,
                         "train_pred"+ format_, "train_real"+ format_,
                         "val_pred"+ format_, "val_real"+ format_]
 
-reconcilers = [BottomUp(), MinTrace(method='ols')]
+reconcilers = [BottomUp(), MinTrace(method='ols'), TopDown(method='proportion_averages'), OptimalCombination(method='ols')]
```

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/utility/experiment_utils.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/utility/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.0.9/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/README.md` & `TEST_TC-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/pyproject.toml` & `TEST_TC-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_algorithm.py` & `TEST_TC-1.0.9/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_datahandler.py` & `TEST_TC-1.0.9/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_datapreparation_utils.py` & `TEST_TC-1.0.9/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_evaluations.py` & `TEST_TC-1.0.9/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_exceptions.py` & `TEST_TC-1.0.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_experiment_job.py` & `TEST_TC-1.0.9/tests/test_experiment_job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_experiment_models.py` & `TEST_TC-1.0.9/tests/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_experiment_utils.py` & `TEST_TC-1.0.9/tests/test_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_prep.py` & `TEST_TC-1.0.9/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_prophet_utils.py` & `TEST_TC-1.0.9/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_resources.py` & `TEST_TC-1.0.9/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.8/tests/test_tele_logger.py` & `TEST_TC-1.0.9/tests/test_tele_logger.py`

 * *Files identical despite different names*

