# Comparing `tmp/powerbot-backtesting-2.0.8.tar.gz` & `tmp/powerbot-backtesting-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerbot-backtesting-2.0.8.tar", last modified: Fri Dec  9 11:39:30 2022, max compression
+gzip compressed data, was "powerbot-backtesting-2.0.9.tar", last modified: Fri Mar 17 10:16:45 2023, max compression
```

## Comparing `powerbot-backtesting-2.0.8.tar` & `powerbot-backtesting-2.0.9.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.753657 powerbot-backtesting-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/.github/workflows/publish-python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/.github/workflows/python-linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      937 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/powerbot_backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/data_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/powerbot_backtesting/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/exceptions/backtesting_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/powerbot_backtesting/models/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27577 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/models/backtesting_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   150128 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/models/exporter_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/models/history_api_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.753657 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/config/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/helpers/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/tests/helpers/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16324 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11522 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/powerbot_backtesting/utils/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.757657 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-09 11:39:30.000000 powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/backtesting_algo_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/config/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:39:30.761657 powerbot-backtesting-2.0.8/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/helpers/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/helpers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/helpers/generate_hardcoded_input_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/helpers/transform_test_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)    27757 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/test_api_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23826 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/test_get_orderbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20549 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/test_history_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28432 2022-12-09 11:38:58.000000 powerbot-backtesting-2.0.8/tests/test_sql_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.710887 powerbot-backtesting-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.710887 powerbot-backtesting-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/.github/workflows/publish-python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/.github/workflows/python-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.710887 powerbot-backtesting-2.0.9/powerbot_backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/data_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/powerbot_backtesting/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/exceptions/backtesting_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/powerbot_backtesting/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27577 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/models/backtesting_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150862 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/models/exporter_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/models/history_api_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.710887 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/config/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/helpers/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/tests/helpers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16324 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/powerbot_backtesting/utils/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-17 10:16:45.000000 powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-17 10:16:45.718887 powerbot-backtesting-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/backtesting_algo_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/config/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:16:45.714887 powerbot-backtesting-2.0.9/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/helpers/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/helpers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/helpers/generate_hardcoded_input_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/helpers/transform_test_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/test_api_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/test_base_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/test_get_orderbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/test_history_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28432 2023-03-17 10:16:15.000000 powerbot-backtesting-2.0.9/tests/test_sql_exporter.py
```

### Comparing `powerbot-backtesting-2.0.8/.github/workflows/publish-python-test.yml` & `powerbot-backtesting-2.0.9/.github/workflows/publish-python-test.yml`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/.github/workflows/python-linting.yml` & `powerbot-backtesting-2.0.9/.github/workflows/python-linting.yml`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/.github/workflows/python-publish.yml` & `powerbot-backtesting-2.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/README.md` & `powerbot-backtesting-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/data_analysis.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/data_analysis.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/models/backtesting_models.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/models/backtesting_models.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/models/exporter_models.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/models/exporter_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,23 @@
 val_Pool = TypeVar("multiprocessing.pool.Pool")
 
 
 class BaseExporter(BaseModel):
     """
     Base class to all of PowerBot's exporter classes.
     """
+    cache_path: Path = Field(description="The parent directory of the cached path", default_factory=type("%s"))
+
+    def __init__(self, **data: Any):
+        super().__init__(**data)
+
+        if len(self.cache_path.__str__()) > 0 and "__pb_cache__" == self.cache_path.parts[-1]:
+            self.cache_path = Path(self.cache_path)
+        else:
+            self.cache_path = Path(self.cache_path).joinpath("__pb_cache__")
 
     def get_contract_ids(self,
                          time_from: datetime = None,
                          time_till: datetime = None,
                          contract_ids: list[str] = None,
                          contract_time: str = "all",
                          products: list[str] = None,
@@ -196,15 +205,15 @@
 
         for tr in time_range:
             # Extract date information
             year_month = tr[0].strftime(DATE_YM)
             day_month = tr[0].strftime(DATE_MD)
 
             # Construct path to index file
-            file_path = Path(f"./__pb_cache__/prod/{self.client.exchange}_{self.client.delivery_area}/{year_month}/{day_month}/raw")  # noqa: W605
+            file_path = self.cache_path.joinpath("prod", f"{self.client.exchange}_{self.client.delivery_area}", year_month, day_month, "raw")
             if not file_path.exists():
                 raise NotInCacheError("The requested data is currently not cached")
             index = next((i for i in file_path.iterdir() if i.is_file() and "contract" in i.name))
 
             if not index:
                 raise NotInCacheError("Cannot find correct index file in local cache")
             index = pd.read_json(gzip.open(index))
@@ -279,16 +288,17 @@
         if use_cached_data:
             # Find __cache__ directory
             for key, value in tqdm(contract_ids.items(), desc="Loading Cached Trades", unit="time periods", leave=False):
                 filepath = _get_file_cachepath(self.client, key, delivery_area)
                 tmp_df = None
 
                 for i in [".json.gz", ".json"]:
-                    if Path(f"./__pb_cache__/{filepath}_trades{i}").exists():
-                        tmp_df = pd.read_json(f"__pb_cache__/{filepath}_trades{i}", dtype=False)
+                    fp_trades = self.cache_path.joinpath(f"{filepath}_trades{i}")
+                    if fp_trades.exists():
+                        tmp_df = pd.read_json(fp_trades, dtype=False)
 
                 if isinstance(tmp_df, pd.DataFrame):
                     tmp_df['api_timestamp'] = pd.to_datetime(tmp_df['api_timestamp'])
                     tmp_df['exec_time'] = pd.to_datetime(tmp_df['exec_time'])
                     tmp_df = tmp_df.astype({"price": "float64", "trade_id": "str", "contract_id": "str"})
                     for i in ["price", "quantity"]:
                         tmp_df[i] = round(tmp_df[i], 2)
@@ -345,15 +355,15 @@
 
         if add_vwap:
             for k, v in trades.items():
                 trades[k] = self.calc_trade_vwap(trade_data={k: v}, contract_time=contract_time,
                                                  delivery_area=delivery_area, index="all")
 
         if caching:
-            _cache_data("trades", trades, delivery_area, api_client=self.client, gzip_files=gzip_files, as_csv=as_csv)
+            _cache_data("trades", trades, delivery_area, api_client=self.client, gzip_files=gzip_files, as_csv=as_csv, cache_path=self.cache_path)
         return trades
 
     def get_contract_history(self,
                              contract_ids: dict[tuple[datetime, datetime], list[str]],
                              delivery_area: str = None,
                              iteration_delay: float = 0,
                              serialize_data: bool = True,
@@ -385,17 +395,17 @@
         if use_cached_data:
             # Find __cache__ directory
             for key, value in contract_ids.items():
                 filepath = _get_file_cachepath(self.client, key, delivery_area)
                 tmp_df = None
 
                 for i in [".json.gz", ".json"]:
-                    if Path(f"./__pb_cache__/{filepath}_ordhist{i}").exists():
-                        tmp_df = pd.read_json(f"./__pb_cache__/{filepath}_ordhist{i}", dtype=False,
-                                              convert_dates=False)
+                    fp_ordhist = self.cache_path.joinpath(f"{filepath}_ordhist{i}")
+                    if fp_ordhist.exists():
+                        tmp_df = pd.read_json(fp_ordhist, dtype=False, convert_dates=False)
 
                 if isinstance(tmp_df, pd.DataFrame):
                     tmp_df['as_of'] = pd.to_datetime(tmp_df['as_of'])
 
                     cols = {"internal_trades": "object", "contract_id": "str", "auction_price": "float64"}
                     cols = {k: v for k, v in cols.items() if k in tmp_df.columns}
                     tmp_df = tmp_df.astype(cols, errors='ignore')
@@ -476,15 +486,15 @@
                 df_history['as_of'] = pd.to_datetime(df_history['as_of'], utc=True)
                 df_history.drop(columns=["auction_price", "internal_trades"], inplace=True, errors="ignore")
 
                 orders[key] = df_history
                 sleep(iteration_delay)
 
         if caching:
-            _cache_data("ordhist", orders, delivery_area, api_client=self.client, gzip_files=gzip_files, as_csv=as_csv)
+            _cache_data("ordhist", orders, delivery_area, api_client=self.client, gzip_files=gzip_files, as_csv=as_csv, cache_path=self.cache_path)
         return orders
 
     @validate_arguments
     def get_ohlc_data(self,
                       trade_data: dict[tuple[datetime, datetime], pandas_DataFrame],
                       timesteps: int,
                       time_unit: str,
@@ -527,20 +537,18 @@
             day_month = key[1].strftime(DATE_MD)
             file_name = (f"{key[0].strftime(DATE_YMD_TIME_HM).replace(':', '-')} - "
                          f"{key[1].strftime(DATE_YMD_TIME_HM).replace(':', '-')}")
             data_ohlc = None
 
             if use_cached_data:
                 for i in [".json.gz", ".json"]:
-                    if Path(f'./__pb_cache__/{environment}/{exchange}_{delivery_area}/{year_month}/{day_month}'
-                            f'/processed/{file_name}_ohlc_{timesteps}{time_unit[0]}{i}').exists():
-                        data_ohlc = pd.read_json(f'./__pb_cache__/{environment}/{exchange}_{delivery_area}/'
-                                                 f'{year_month}/{day_month}/processed/'
-                                                 f'{file_name}_ohlc_{timesteps}{time_unit[0]}{i}',
-                                                 dtype=False)
+                    fp_ohlc = self.cache_path.joinpath(environment, f"{exchange}_{delivery_area}", year_month, day_month, "processed",
+                                                       f"{file_name}_ohlc_{timesteps}{time_unit[0]}{i}")
+                    if fp_ohlc.exists():
+                        data_ohlc = pd.read_json(fp_ohlc, dtype=False)
 
             if isinstance(data_ohlc, pd.DataFrame):
                 data_ohlc.rename(columns={0: 'exec_time'}, inplace=True)
                 all_ohlc_data[key] = data_ohlc
 
             else:
                 data_ohlc = value.set_index('exec_time')
@@ -549,16 +557,16 @@
                 data_ohlc = data_ohlc.dropna(how='all')
 
                 # Append to complete OHLC collection
                 all_ohlc_data[key] = data_ohlc
 
         # Cache Data as JSON
         if caching:
-            _cache_data("ohlc", all_ohlc_data, delivery_area, exchange=exchange, api_client=client,
-                        gzip_files=gzip_files, timesteps=timesteps, time_unit=time_unit[0], as_csv=False)
+            _cache_data(data_type="ohlc", data=all_ohlc_data, delivery_area=delivery_area, exchange=exchange, api_client=client,
+                        gzip_files=gzip_files, timesteps=timesteps, time_unit=time_unit[0], as_csv=False, cache_path=self.cache_path)
 
         return all_ohlc_data
 
     @validate_arguments
     def get_orderbooks(self,
                        contract_hist_data: dict[tuple[datetime, datetime], pandas_DataFrame],
                        delivery_area: str = None,
@@ -625,15 +633,15 @@
         first_contract = contract_times[0][0]
         last_contract = contract_times[-1][1]
         year_month = first_contract.strftime(DATE_YM)
         day_month = first_contract.strftime(DATE_MD)
         first_contract = first_contract.strftime(DATE_YMD_TIME_HM_ALT)
         last_contract = last_contract.strftime(DATE_YMD_TIME_HM_ALT) if len(contract_times) > 1 else None
 
-        new_dir = f"./__pb_cache__/{environment}/{exchange}_{delivery_area}/{year_month}/{day_month}/processed"
+        new_dir = self.cache_path.joinpath(environment, f"{exchange}_{delivery_area}", year_month, day_month, "processed")
 
         if lightweight:
             for key in tqdm(contract_hist_data):
                 df = contract_hist_data[key]
                 df = df.sort_values("revision_no")
                 if "orders" in df.columns:
                     first_valid_entry = df[["best_bid_price", "best_ask_price"]].notna().idxmax().min()
@@ -712,15 +720,15 @@
                 all_order_books_df["contract_id"] = all_order_books_df["contract_id"].astype(int).astype(str)
 
         # Cache Data as pickle
         if caching:
             _cache_data("orderbook", all_order_books_df, delivery_area, exchange=exchange, api_client=client,
                         gzip_files=False, timesteps=timesteps,
                         time_unit=time_unit[0], shortest_interval=shortest_interval, as_json=False,
-                        as_pickle=True)
+                        as_pickle=True, cache_path=self.cache_path)
 
         # Saving Complete Orderbook as JSON
         if as_json:
             new_dir.mkdir(parents=True, exist_ok=True)
 
             filename = f'orderbook_{first_contract} - {last_contract}_{timesteps}{time_unit[0]}.json.gz' \
                 if last_contract else f'orderbook_{first_contract}_{timesteps}{time_unit[0]}.json.gz'
@@ -1294,15 +1302,14 @@
     load the data in question via the HistoryExporter.
     """
     pool: val_Pool = Field(description="Multiprocessing Pool", default_factory=type(None))
     api_key: str = Field(description="A Standard API Key",
                          example="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXX")
     host: str = Field(description="URL of the PowerBot instance to connect to",
                       example="https://backup.powerbot-trading.com/{COMPANY NAME}/{EXCHANGE}/v2/api")
-
     client: val_ApiClient = Field(description="Placeholder value, do not overwrite", default_factory=type(None))
 
     def __init__(self, **data: Any):
         super().__init__(**data)
 
         # Init client
         self.pool = Pool(min(os.cpu_count(), 4), maxtasksperchild=1000)
@@ -1667,14 +1674,15 @@
     delivery_area: str = Field(description="EIC-code of the delivery area data should be loaded for")
     pool: val_Pool = Field(description="Multiprocessing Pool", default_factory=type(None))
     client: val_HistoryApiClient = Field(description="Placeholder value, do not overwrite", default_factory=type(None))
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         self.pool = Pool(min(os.cpu_count(), 4), maxtasksperchild=1000)
+
         # Init client
         self.client = HistoryApiClient(self.exchange, self.delivery_area)
 
     @root_validator
     def check_credentials(cls, values):
         exchange, delivery_area = values.get('exchange'), values.get('delivery_area')
 
@@ -1732,16 +1740,20 @@
         if day_to and not isinstance(day_to, datetime):
             try:
                 day_to = datetime.strptime(day_to, DATE_YMD)
             except ValueError:
                 raise ValueError("day_to needs to be a date or a string in YYYY-MM-DD format")
 
         delivery_areas = delivery_areas if isinstance(delivery_areas, list) else [delivery_areas]
-        cache_path = "./__pb_cache__" if not cache_path else cache_path
-        cache_path = Path(cache_path) if not isinstance(cache_path, Path) else cache_path
+        if cache_path:
+            if not cache_path.exists():
+                raise FileNotFoundError
+        else:
+            cache_path = self.cache_path
+
         headers = {"accept": "application/zip", "X-API-KEY": api_key}
         day_to = day_to if day_to else day_from
         skip_on_error = True if skip_on_error and day_to and day_to - day_from >= timedelta(days=2) else False
 
         zipfiles = []
         extracted_files = {}
         retry = 0
@@ -1751,16 +1763,15 @@
             # While False, days will continue with iteration
             prevent_update = False
 
             for del_area in delivery_areas:
                 host = f"https://history.powerbot-trading.com/history/{self.client.exchange}/{del_area}/{day_from.strftime(DATE_YMD)}"
 
                 # Filepath
-                filepath = cache_path.joinpath(
-                    f"history/{self.client.exchange}_{del_area}/{day_from.strftime(DATE_YM)}")
+                filepath = cache_path.joinpath(f"history/{self.client.exchange}_{del_area}/{day_from.strftime(DATE_YM)}")
 
                 # File
                 filename = f"{day_from.strftime(DATE_MD)}_public_data.zip"
                 zipfiles.append(f"{del_area}_{filename.strip('.zip')}")
 
                 # Skip if file exists
                 if not filepath.joinpath(filename).exists() and not filepath.joinpath(
@@ -1873,15 +1884,15 @@
 
         Args:
             extracted_files (list(str), dict[str, list[str]]): List of files extracted with get_historic_data
             (-> return value of get_historic_data)
             keep_zip_files (bool): True if zip-files should be kept after download
         """
         # Setup
-        prod_path = Path("./__pb_cache__/prod")
+        prod_path = self.cache_path.joinpath("prod")
         prod_files = []
 
         for f_name, unzipped_files in (tqdm(extracted_files.items(),
                                             desc="Transform extracted files",
                                             unit="days",
                                             eave=False) if concurrent else extracted_files.items()):
 
@@ -1945,27 +1956,30 @@
                                 transformed_trade_files[time] = _historic_data_transformation(v, self.client.exchange,
                                                                                               k)
                             else:
                                 transformed_order_files[time] = _historic_data_transformation(v, self.client.exchange,
                                                                                               k)
 
             # Cache the result
-            _cache_data("contracts", {index.delivery_start.iloc[0].date(): index}, delivery_area, self.client.exchange)
-            _cache_data("trades", transformed_trade_files, delivery_area, self.client.exchange)
-            _cache_data("ordhist", transformed_order_files, delivery_area, self.client.exchange)
+            _cache_data(data_type="contracts", data={index.delivery_start.iloc[0].date(): index}, delivery_area=delivery_area,
+                        exchange=self.client.exchange, cache_path=self.cache_path)
+            _cache_data(data_type="trades", data=transformed_trade_files, delivery_area=delivery_area, exchange=self.client.exchange,
+                        cache_path=self.cache_path)
+            _cache_data(data_type="ordhist", data=transformed_order_files, delivery_area=delivery_area, exchange=self.client.exchange,
+                        cache_path=self.cache_path)
 
             # Save paths of all transformed files
             # noqa: W605
             prod_files += [Path(e) for e in
                            prod_path.joinpath(
                                f"{self.client.exchange}_{delivery_area}/{end.strftime('%Y-%m')}/{end.strftime('%m-%d')}/raw").iterdir()  # noqa: W605
                            if e.is_file()]
 
         # Delete history directory if it's empty (no files)
-        history_path = Path("./__pb_cache__/history")
+        history_path = self.cache_path.joinpath("history")
         history_files = [file for root, directory, file in os.walk(history_path)]
 
         if not all(i for i in history_files) and not keep_zip_files:
             shutil.rmtree(history_path)
 
         return prod_files
 
@@ -2232,14 +2246,15 @@
                     "exasolution": "exa+pyodbc",
                     "firebird": "firebird",
                     "ibm_db2": "db2+ibm_db",
                     "monetdb": "monetdb",
                     "snowflake": "snowflake",
                     "teradata_vantage": "teradatasql"}
 
+        engine = None
         if self.port:
             try:
                 engine = create_engine(
                     f'{db_types[self.db_type]}://{self.user}:{self.password}@{self.host}:{self.port}/{self.database}')
             except:  # noqa: E722
                 pass
         try:
@@ -2428,16 +2443,17 @@
             missing_contracts = {}
 
             for key, value in tqdm(contract_ids.items(), desc="Loading Cached Trades", unit="time periods", leave=False):
                 filepath = _get_file_cachepath(None, key, delivery_area[0], exchange)
                 tmp_df = None
 
                 for i in [".json.gz", ".json"]:
-                    if Path(f"__pb_cache__/{filepath}_trades{i}").exists():
-                        tmp_df = pd.read_json(f"__pb_cache__/{filepath}_trades{i}", dtype=False)
+                    fp_trades = self.cache_path.joinpath(f"{filepath}_trades{i}")
+                    if fp_trades.exists():
+                        tmp_df = pd.read_json(fp_trades, dtype=False)
 
                 if isinstance(tmp_df, pd.DataFrame):
                     tmp_df['api_timestamp'] = pd.to_datetime(tmp_df['api_timestamp'])
                     tmp_df['exec_time'] = pd.to_datetime(tmp_df['exec_time'])
                     tmp_df = tmp_df.astype({"price": "float64", "trade_id": "str", "contract_id": "str"})
                     for i in ["price", "quantity"]:
                         tmp_df[i] = round(tmp_df[i], 2)
@@ -2480,16 +2496,16 @@
 
                     output['api_timestamp'] = pd.to_datetime(output['api_timestamp'], utc=True)
                     output['exec_time'] = pd.to_datetime(output['exec_time'], utc=True)
                     trades |= self.__convert_dataframe("trades", output)
 
             # Caching
             if caching:
-                _cache_data("trades", trades, delivery_area[0], api_client=None, gzip_files=gzip_files, as_csv=as_csv,
-                            exchange=exchange)
+                _cache_data(data_type="trades", data=trades, delivery_area=delivery_area[0], api_client=None, gzip_files=gzip_files, as_csv=as_csv,
+                            exchange=exchange, cache_path=self.cache_path)
 
             self.logger.info("Successfully exported trades")
             return trades
 
         self.logger.info("Successfully exported trades")
 
         return result
@@ -2536,17 +2552,17 @@
 
         if use_cached_data and as_dataframe and (contract_ids := kwargs.get("contract_id")):
             for key, value in contract_ids.items():
                 filepath = _get_file_cachepath(None, key, delivery_area[0], exchange)
                 tmp_df = None
 
                 for i in [".json.gz", ".json"]:
-                    if Path(f"./__pb_cache__/{filepath}_ordhist{i}").exists():
-                        tmp_df = pd.read_json(f"./__pb_cache__/{filepath}_ordhist{i}", dtype=False,
-                                              convert_dates=False)
+                    fp_ordhist = self.cache_path.joinpath(f"{filepath}_ordhist{i}")
+                    if fp_ordhist.exists():
+                        tmp_df = pd.read_json(fp_ordhist, dtype=False, convert_dates=False)
 
                 if isinstance(tmp_df, pd.DataFrame):
                     tmp_df['as_of'] = pd.to_datetime(tmp_df['as_of'])
 
                     cols = {"internal_trades": "object", "contract_id": "str", "auction_price": "float64"}
                     cols = {k: v for k, v in cols.items() if k in tmp_df.columns}
                     tmp_df = tmp_df.astype(cols, errors='ignore')
@@ -2614,16 +2630,16 @@
                                  8: 'best_ask_qty', 9: 'vwap', 10: 'high', 11: 'low', 12: 'last_price',
                                  13: 'last_qty', 14: "last_trade_time", 15: 'volume', 16: 'delta',
                                  17: 'bids', 18: 'asks'})
                 orders |= self.__convert_dataframe("orders", output)
 
             # Caching
             if caching:
-                _cache_data("ordhist", orders, delivery_area[0], api_client=None, gzip_files=gzip_files, as_csv=as_csv,
-                            exchange=exchange)
+                _cache_data(data_type="ordhist", data=orders, delivery_area=delivery_area[0], api_client=None, gzip_files=gzip_files, as_csv=as_csv,
+                            exchange=exchange, cache_path=self.cache_path)
 
             self.logger.info("Successfully exported contract history")
             return orders
 
         self.logger.info("Successfully exported contract history")
 
         return result
```

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/tests/config/config.yml` & `powerbot-backtesting-2.0.9/powerbot_backtesting/tests/config/config.yml`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/tests/helpers/conftest.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/tests/helpers/conftest.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/__init__.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/constants.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 TIME_HM = "%H:%M"
 TIME_HM_ALT = "%H-%M"
 
 # Exchanges & Delivery Area Codes
 SYSTEMS = {"M7": ("epex", "hupx", "tge", "southpool"), "NordPool": ("nordpool", "ibex", "cropex")}
 EXCHANGES = ("epex", "nordpool", "hupx", "southpool", "tge", "ibex", "cropex")
 EIC_CODES = {
-    "epex": ('10YAT-APG------L', '10YBE----------2', '10YDK-1-------AA', '10YDK-2--------M', '10YFI-1--------U',
+    "epex": ('10YAT-APG------L', '10YBE----------2', '10YDK-1--------W', '10YDK-2--------M', '10YFI-1--------U',
              '10YFR-RTE------C', '10YDE-VE-------2', '10YDE-RWENET---I', '10YDE-EON------1', '10YDE-ENBW-----N',
              '10YLU-CEGEDEL-NQ', '10YNL----------L', '10YNO-1--------2', '10YNO-2--------T', '10YNO-3--------J',
              '10YNO-4--------9', '10Y1001A1001A48H', '10Y1001A1001A44P', '10Y1001A1001A46L', '10Y1001A1001A45N',
              '10YCH-SWISSGRIDZ', '10YGB----------A'),
     "nordpool": ('10YDK-1--------W', '10YDK-2--------M', '10YFI-1--------U', '10YDOM-1001A084H', '10Y1001A1001A39I',
                  '10YLV-1001A00074', '10YLT-1001A0008Q', '10YNO-1--------2', '10YNO-2--------T', '10YNO-3--------J',
                  '10YNO-4--------9', '10Y1001A1001A48H', '10Y1001A1001A44P', '10Y1001A1001A45N', '10Y1001A1001A46L',
```

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_backtesting.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_backtesting.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_general.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_general.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,16 @@
                 api_client: Union[ApiClient, HistoryApiClient] = None,
                 timesteps: int = 0,
                 time_unit: str = None,
                 shortest_interval: bool = False,
                 gzip_files: bool = True,
                 as_json: bool = True,
                 as_csv: bool = False,
-                as_pickle: bool = False):
+                as_pickle: bool = False,
+                cache_path: Path = None):
     """
     Function to be called by data request functions to cache loaded data in a reusable format. Automatically generates
     a folder to cache loaded files, if it cannot find an existing one.
 
     Args:
         data_type (str): One of the following: trades, ordhist, ohlc, orderbook
         data (dict): Dictionary of DataFrames
@@ -96,14 +97,15 @@
         api_client: PowerBot ApiClient
         timesteps (int): only necessary if data_type is ohlc or orderbooks
         time_unit (str): only necessary if data_type is ohlc or orderbooks
         gzip_files (bool): True if cached files should be gzipped
         as_json (bool): True per default, except for orderbooks (optional feature)
         as_csv (bool): if True, will save files as CSV, additionally to JSON
         as_pickle (bool): False per default, except for orderbooks
+        cache_path (Path): Optional path for caching files
     """
     # Setup
     host = api_client.configuration.host if isinstance(api_client, ApiClient) else None
     environment = "staging" if host and host.split("/")[2].split(".")[0] == "staging" else "prod"
     exchange = host.split("/")[4] if host else api_client.exchange if isinstance(api_client,
                                                                                  HistoryApiClient) else exchange
     folder = "raw" if data_type in ["trades", "ordhist", "contracts"] else "processed"
@@ -135,29 +137,29 @@
             day_month = key.strftime("%m-%d")
 
         time_intervals = f"{timesteps}{time_unit}" if not shortest_interval else "shortest"
 
         file_name = f"{file_name}_{data_type}" if folder == "raw" else f"{file_name}_{data_type}_{time_intervals}"
 
         # Check if __cache__ already exists
-        cache_path = Path(f"./__pb_cache__/{environment}/{exchange}_{delivery_area}/{year_month}/{day_month}/{folder}")
+        new_dir = cache_path.joinpath(Path("__pb_cache__", environment, f"{exchange}_{delivery_area}", year_month, day_month, folder))
 
         # Assure That Directory Exists
-        cache_path.mkdir(parents=True, exist_ok=True)
+        new_dir.mkdir(parents=True, exist_ok=True)
 
         # Cache File If It Doesn't Exist Yet
-        if as_json and not cache_path.joinpath(f"{file_name}.json{file_ending}").exists():
-            value.to_json(cache_path.joinpath(f"{file_name}.json{file_ending}"), date_format="iso", date_unit="us",
+        if as_json and not new_dir.joinpath(f"{file_name}.json{file_ending}").exists():
+            value.to_json(new_dir.joinpath(f"{file_name}.json{file_ending}"), date_format="iso", date_unit="us",
                           compression=compression)
 
-        if as_csv and not cache_path.joinpath(f"{file_name}.csv").exists():
-            value.to_csv(cache_path.joinpath(f"{file_name}.csv{file_ending}"), sep=";", compression=compression)
+        if as_csv and not new_dir.joinpath(f"{file_name}.csv").exists():
+            value.to_csv(new_dir.joinpath(f"{file_name}.csv{file_ending}"), sep=";", compression=compression)
 
-        if as_pickle and not cache_path.joinpath(f"{file_name}.p").exists():
-            value.to_pickle(cache_path.joinpath(f"{file_name}.p"))
+        if as_pickle and not new_dir.joinpath(f"{file_name}.p").exists():
+            value.to_pickle(new_dir.joinpath(f"{file_name}.p"))
 
 
 def _get_file_cachepath(api_client: Union[ApiClient, HistoryApiClient], contract_key: str, delivery_area: str, exchange: str = None) -> str:
     """
     Helper function that constructs most of the path of a cached file.
 
     Args:
```

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_history.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_history.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/helpers_processing.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/helpers_processing.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting/utils/utilities.py` & `powerbot-backtesting-2.0.9/powerbot_backtesting/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/powerbot_backtesting.egg-info/SOURCES.txt` & `powerbot-backtesting-2.0.9/powerbot_backtesting.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 powerbot_backtesting/utils/helpers_backtesting.py
 powerbot_backtesting/utils/helpers_general.py
 powerbot_backtesting/utils/helpers_history.py
 powerbot_backtesting/utils/helpers_processing.py
 powerbot_backtesting/utils/utilities.py
 tests/backtesting_algo_.py
 tests/test_api_exporter.py
+tests/test_base_exporter.py
 tests/test_get_orderbooks.py
 tests/test_history_exporter.py
 tests/test_sql_exporter.py
 tests/config/__init__.py
 tests/config/config.yml
 tests/helpers/__init__.py
 tests/helpers/cleanup.py
```

### Comparing `powerbot-backtesting-2.0.8/tests/backtesting_algo_.py` & `powerbot-backtesting-2.0.9/tests/backtesting_algo_.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from datetime import datetime
 from pathlib import Path
-from powerbot_backtesting import HistoryExporter, BacktestingAlgo, ApiExporter
+from powerbot_backtesting import HistoryExporter, BacktestingAlgo
 from powerbot_backtesting.utils import generate_input_file
 
 EXCHANGE = "epex"
 DELIVERY_AREA = "10YAT-APG------L"
-TIME_FROM = datetime.strptime("2022-04-10 00:00:00", "%Y-%m-%d %H:%M:%S")
-TIME_TILL = datetime.strptime("2022-04-10 00:45:00", "%Y-%m-%d %H:%M:%S")
+TIME_FROM = datetime.strptime("2022-06-01 13:30:00", "%Y-%m-%d %H:%M:%S")
+TIME_TILL = datetime.strptime("2022-06-01 13:45:00", "%Y-%m-%d %H:%M:%S")
+DAY_FROM = datetime.strptime("2022-06-01", "%Y-%m-%d")
+DAY_TILL = datetime.strptime("2022-06-02", "%Y-%m-%d")
 CONTRACT_TIME = "quarter-hourly"
 TIMESTEPS = 15
 TIME_UNIT = "minutes"
+CACHE_PATH = Path("data")
 
+HIST_API_KEY = "MY_HISTORY_API_KEY"
 API_KEY = "MY_API_KEY"
 HOST = "MY_API_HOST"
 
 
 class MyAlgo(BacktestingAlgo):
     def algorithm(self, timestamp, orderbook, key):
         # Buy
@@ -49,39 +53,44 @@
 
         else:
             return False
 
 
 if __name__ == '__main__':
     # Initialize HistoryExporter
-    exporter = HistoryExporter(exchange=EXCHANGE, delivery_area=DELIVERY_AREA)
+    exporter = HistoryExporter(exchange=EXCHANGE, delivery_area=DELIVERY_AREA, cache_path=CACHE_PATH)
 
-    exporter = ApiExporter(api_key=API_KEY, host=HOST)
+    # Get historic data
+    historic_data = exporter.get_historic_data(api_key=HIST_API_KEY,
+                                               day_from=DAY_FROM,
+                                               day_to=DAY_TILL,
+                                               extract_files=True,
+                                               process_data=True)
 
     # Get Contract IDs for specific Timeframe
     contract_ids = exporter.get_contract_ids(
         time_from=TIME_FROM,
         time_till=TIME_TILL,
         contract_time="quarter-hourly"
     )
 
-    trade_data = exporter.get_public_trades(contract_ids=contract_ids, contract_time=CONTRACT_TIME, delivery_area=DELIVERY_AREA, use_cached_data=True)
+    trade_data = exporter.get_public_trades(contract_ids=contract_ids, contract_time=CONTRACT_TIME, as_csv=True)
 
-    order_data = exporter.get_contract_history(contract_ids=contract_ids, delivery_area=DELIVERY_AREA, use_cached_data=True)
+    order_data = exporter.get_contract_history(contract_ids=contract_ids, delivery_area=DELIVERY_AREA)
 
     orderbooks = exporter.get_orderbooks(
         contract_hist_data=order_data,
         timesteps=TIMESTEPS,
         time_unit=TIME_UNIT,
         delivery_area=DELIVERY_AREA,
         use_cached_data=True)
 
     ohlc_data = exporter.get_ohlc_data(trade_data, timesteps=15, time_unit="minutes", delivery_area=DELIVERY_AREA, use_cached_data=True)
 
-    if not Path("./__pb_cache__/analysis_input").exists():
+    if not CACHE_PATH.joinpath(Path("__pb_cache__", "analysis_input")).exists():
         # Generate input csv; only need to do once
         generate_input_file(orderbooks)
 
     else:
         # Instantiate the algo and pass the filled out input file
         algo = MyAlgo(orderbooks, "backtesting_input_1.csv", trades=trade_data)
```

### Comparing `powerbot-backtesting-2.0.8/tests/config/config.yml` & `powerbot-backtesting-2.0.9/tests/config/config.yml`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/tests/helpers/conftest.py` & `powerbot-backtesting-2.0.9/tests/helpers/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from random import randint, choice, uniform
 
 import pytest
 
 from powerbot_backtesting import ApiExporter, SqlExporter
 from powerbot_backtesting.utils import init_client
 from powerbot_backtesting.utils.constants import PRODUCTS
-from tests.config import config
-from tests.helpers import do_cleanup
+from config import config
+from helpers import do_cleanup
 
 
 @pytest.fixture
 def random_params_api():
     time_from = datetime.today().replace(hour=randint(0, 23), minute=0, second=0, microsecond=0) - timedelta(days=1)
     time_till = time_from + timedelta(hours=1)
     contract_time = choice(["hourly", "quarter-hourly"])
```

### Comparing `powerbot-backtesting-2.0.8/tests/helpers/generate_hardcoded_input_orderbook.py` & `powerbot-backtesting-2.0.9/tests/helpers/generate_hardcoded_input_orderbook.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/tests/helpers/transform_test_orderbook.py` & `powerbot-backtesting-2.0.9/tests/helpers/transform_test_orderbook.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/tests/test_api_exporter.py` & `powerbot-backtesting-2.0.9/tests/test_api_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from datetime import timedelta, timezone
 from random import choice
 import numpy as np
 import pandas as pd
 import pytest
 from dateutil.tz import tzutc
 from powerbot_client import ApiClient
-
-from tests.helpers import random_params_api  # noqa
+from helpers import random_params_api  # noqa
 
 
 @pytest.mark.parametrize("rndm_params",
                          [pytest.lazy_fixture("random_params_api")])
 def test_api_exporter_init(rndm_params):
     exporter = rndm_params["api_exporter"]
```

### Comparing `powerbot-backtesting-2.0.8/tests/test_get_orderbooks.py` & `powerbot-backtesting-2.0.9/tests/test_get_orderbooks.py`

 * *Files identical despite different names*

### Comparing `powerbot-backtesting-2.0.8/tests/test_history_exporter.py` & `powerbot-backtesting-2.0.9/tests/test_history_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import gzip
-from datetime import datetime, timezone, timedelta
-from pathlib import Path
-
 import numpy as np
 import pandas as pd
 import pytest
 
+from datetime import datetime, timezone, timedelta
+from pathlib import Path
 from powerbot_backtesting import HistoryExporter, ApiExporter
 from powerbot_backtesting.models import HistoryApiClient
-from tests.helpers import random_params_history_cleanup, random_params_history_no_cleanup  # noqa
-from tests.config import config
+from helpers import random_params_history_cleanup, random_params_history_no_cleanup  # noqa
+from config import config
 
 
 @pytest.mark.parametrize("rndm_params",
                          [pytest.lazy_fixture("random_params_history_no_cleanup")])
 def test_history_exporter_init(rndm_params):
     exporter = HistoryExporter(exchange="epex", delivery_area="10YDE-RWENET---I")
```

### Comparing `powerbot-backtesting-2.0.8/tests/test_sql_exporter.py` & `powerbot-backtesting-2.0.9/tests/test_sql_exporter.py`

 * *Files identical despite different names*

