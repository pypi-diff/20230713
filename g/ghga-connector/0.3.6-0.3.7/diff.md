# Comparing `tmp/ghga_connector-0.3.6.tar.gz` & `tmp/ghga_connector-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_connector-0.3.6.tar", last modified: Wed Jul 12 13:28:31 2023, max compression
+gzip compressed data, was "ghga_connector-0.3.7.tar", last modified: Thu Jul 13 11:04:21 2023, max compression
```

## Comparing `ghga_connector-0.3.6.tar` & `ghga_connector-0.3.7.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.907958 ghga_connector-0.3.6/ghga_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/ghga_connector/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/ghga_connector/core/api_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/work_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/batch_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/http_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/message_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.907958 ghga_connector-0.3.6/ghga_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/get_package_name.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/license_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/scripts/script_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/script_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/script_utils/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/update_config_docs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/update_readme.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/update_template_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.907958 ghga_connector-0.3.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/endpoints_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/fixtures/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/mock_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/mock_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/test_file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/test_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector/core/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/well_knowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/work_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/batch_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/http_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/message_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-13 11:04:21.000000 ghga_connector-0.3.7/ghga_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/script_utils/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/update_config_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/update_readme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.010511 ghga_connector-0.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/endpoints_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/fixtures/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/mock_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/mock_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/test_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/test_file_operations.py
```

### Comparing `ghga_connector-0.3.6/LICENSE` & `ghga_connector-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/PKG-INFO` & `ghga_connector-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_connector
-Version: 0.3.6
+Version: 0.3.7
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.6
+docker pull ghga/ghga-connector:0.3.7
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.6 .
+docker build -t ghga/ghga-connector:0.3.7 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.6 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.7 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -71,27 +71,21 @@
 ghga_connector --help
 ```
 
 ## Configuration
 ### Parameters
 
 The service requires the following configuration parameters:
-- **`upload_api`** *(string)*: URL to the root of the upload controller API. Default: `https://hd-dev.ghga-dev.de/ucs`.
-
-- **`download_api`** *(string)*: URL to the root of the DRS-compatible API used for download. Default: `https://hd-dev.ghga-dev.de/drs3/ga4gh/drs/v1`.
-
 - **`max_retries`** *(integer)*: Number of times to retry failed API calls. Default: `5`.
 
 - **`max_wait_time`** *(integer)*: Maximal time in seconds to wait before quitting without a download. Default: `3600`.
 
 - **`part_size`** *(integer)*: The part size to use for download. Default: `16777216`.
 
-- **`server_pubkey`** *(string)*: Base64 encoded current GHGA public key for Crypt4GH encryption.
-
-- **`wps_api_url`** *(string)*: URL to the root of the WPS API.
+- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://.
 
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.ghga_connector.yaml`, and place it into one of the following locations:
```

### Comparing `ghga_connector-0.3.6/README.md` & `ghga_connector-0.3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.6
+docker pull ghga/ghga-connector:0.3.7
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.6 .
+docker build -t ghga/ghga-connector:0.3.7 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.6 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.7 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -54,27 +54,21 @@
 ghga_connector --help
 ```
 
 ## Configuration
 ### Parameters
 
 The service requires the following configuration parameters:
-- **`upload_api`** *(string)*: URL to the root of the upload controller API. Default: `https://hd-dev.ghga-dev.de/ucs`.
-
-- **`download_api`** *(string)*: URL to the root of the DRS-compatible API used for download. Default: `https://hd-dev.ghga-dev.de/drs3/ga4gh/drs/v1`.
-
 - **`max_retries`** *(integer)*: Number of times to retry failed API calls. Default: `5`.
 
 - **`max_wait_time`** *(integer)*: Maximal time in seconds to wait before quitting without a download. Default: `3600`.
 
 - **`part_size`** *(integer)*: The part size to use for download. Default: `16777216`.
 
-- **`server_pubkey`** *(string)*: Base64 encoded current GHGA public key for Crypt4GH encryption.
-
-- **`wps_api_url`** *(string)*: URL to the root of the WPS API.
+- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://.
 
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.ghga_connector.yaml`, and place it into one of the following locations:
```

### Comparing `ghga_connector-0.3.6/ghga_connector/__init__.py` & `ghga_connector-0.3.7/ghga_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CLI - Client to perform up- and download operations to and from a local ghga instance
 """
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

### Comparing `ghga_connector-0.3.6/ghga_connector/__main__.py` & `ghga_connector-0.3.7/ghga_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/cli.py` & `ghga_connector-0.3.7/ghga_connector/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """ CLI-specific wrappers around core functions."""
 
 import os
+import sys
 from distutils.util import strtobool
 from pathlib import Path
 
 import crypt4gh.keys
 import typer
 from ghga_service_commons.utils import crypt
 
@@ -51,108 +52,129 @@
     def failure(self, message: str):
         """
         Write message to stderr representing information about a failed operation
         """
         typer.secho(message, fg=core.MessageColors.FAILURE, err=True)
 
 
-cli = typer.Typer()
+cli = typer.Typer(no_args_is_help=True)
 
 
 def upload(  # noqa C901
     *,
-    file_id: str = typer.Option(..., help="The id if the file to upload"),
+    file_id: str = typer.Option(..., help="The id of the file to upload"),
     file_path: Path = typer.Option(..., help="The path to the file to upload"),
     submitter_pubkey_path: Path = typer.Argument(
         "./key.pub",
         help="The path to a public key from the key pair that was announced in the "
         + "metadata. Defaults to key.pub in the current folder.",
     ),
     submitter_private_key_path: Path = typer.Argument(
         "./key.sec",
         help="The path to a private key from the key pair that will be used to encrypt the "
-        + "crypt4gh envelope. Defaults to key in the current folder.",
+        + "crypt4gh envelope. Defaults to key.sec in the current folder.",
+    ),
+    debug: bool = typer.Option(
+        False, help="Set this option in order to view traceback for errors."
     ),
 ):
     """
     Command to upload a file
     """
+    if not debug:
+        sys.excepthook = lambda x, y, z: None
+
     core.HttpxClientState.configure(CONFIG.max_retries)
 
+    wkvs_caller = core.WKVSCaller(CONFIG.wkvs_api_url)
+    server_pubkey = wkvs_caller.get_server_pubkey()
+    ucs_api_url = wkvs_caller.get_ucs_api_url()
+
     core.upload(
-        api_url=CONFIG.upload_api,
+        api_url=ucs_api_url,
         file_id=file_id,
         file_path=file_path,
         message_display=CLIMessageDisplay(),
-        server_pubkey=CONFIG.server_pubkey,
+        server_pubkey=server_pubkey,
         submitter_pubkey_path=submitter_pubkey_path,
         submitter_private_key_path=submitter_private_key_path,
     )
 
 
 if strtobool(os.getenv("UPLOAD_ENABLED") or "false"):
     cli.command()(upload)
 
 
 @cli.command()
-def download(  # pylint: disable=too-many-arguments
+def download(  # pylint: disable=too-many-arguments,too-many-locals
     *,
     output_dir: Path = typer.Option(
         ..., help="The directory to put the downloaded files into."
     ),
     submitter_pubkey_path: Path = typer.Argument(
         "./key.pub",
         help="The path to a public key from the key pair that was announced in the "
         + "metadata. Defaults to key.pub in the current folder.",
     ),
     submitter_private_key_path: Path = typer.Argument(
         "./key.sec",
-        help="The path to a private key from the key pair that will be used to decrypt the"
-        + "work package access and work order tokens. Defaults to key in the current folder.",
+        help="The path to a private key from the key pair that will be used to decrypt "
+        + "the work package access token and work order token. Defaults to key.sec in "
+        + "the current folder.",
+    ),
+    debug: bool = typer.Option(
+        False, help="Set this option in order to view traceback for errors."
     ),
 ):
     """
     Command to download files
     """
+    if not debug:
+        sys.excepthook = lambda x, y, z: None
+
     core.HttpxClientState.configure(CONFIG.max_retries)
     message_display = CLIMessageDisplay()
 
     if not submitter_pubkey_path.is_file():
-        message_display.failure(f"The file {submitter_pubkey_path} does not exist.")
+        message_display.failure(f"The file '{submitter_pubkey_path}' does not exist.")
         raise core.exceptions.PubKeyFileDoesNotExistError(
             pubkey_path=submitter_pubkey_path
         )
 
     if not output_dir.is_dir():
-        message_display.failure(f"The directory {output_dir} does not exist.")
+        message_display.failure(f"The directory '{output_dir}' does not exist.")
         raise core.exceptions.DirectoryDoesNotExistError(output_dir=output_dir)
 
     submitter_public_key = crypt4gh.keys.get_public_key(filepath=submitter_pubkey_path)
     submitter_private_key = crypt4gh.keys.get_private_key(
         filepath=submitter_private_key_path, callback=None
     )
 
     # get work package access token and id from user input, will be used in later PR
     work_package_id, work_package_token = core.main.get_wps_token(
         max_tries=3, message_display=message_display
     )
     decrypted_token = crypt.decrypt(data=work_package_token, key=submitter_private_key)
 
+    wkvs_caller = core.WKVSCaller(CONFIG.wkvs_api_url)
+    wps_api_url = wkvs_caller.get_wps_api_url()
+    dcs_api_url = wkvs_caller.get_dcs_api_url()
+
     work_package_accessor = core.WorkPackageAccessor(
         access_token=decrypted_token,
-        api_url=CONFIG.wps_api_url,
-        dcs_api_url=CONFIG.download_api,
+        api_url=wps_api_url,
+        dcs_api_url=dcs_api_url,
         package_id=work_package_id,
         submitter_private_key=submitter_private_key,
     )
     file_ids_with_extension = work_package_accessor.get_package_files()
 
     io_handler = core.CliIoHandler()
     staging_parameters = core.StagingParameters(
-        api_url=CONFIG.download_api,
+        api_url=dcs_api_url,
         file_ids_with_extension=file_ids_with_extension,
         max_wait_time=CONFIG.max_wait_time,
     )
 
     file_stager = core.FileStager(
         message_display=message_display,
         io_handler=io_handler,
@@ -160,60 +182,66 @@
         work_package_accessor=work_package_accessor,
     )
     file_stager.check_and_stage(output_dir=output_dir)
 
     while file_stager.file_ids_remain():
         for file_id in file_stager.get_staged():
             core.download(
-                api_url=CONFIG.download_api,
+                api_url=dcs_api_url,
                 file_id=file_id,
                 file_extension=file_ids_with_extension[file_id],
                 output_dir=output_dir,
                 max_wait_time=CONFIG.max_wait_time,
                 part_size=CONFIG.part_size,
                 message_display=message_display,
                 submitter_public_key=submitter_public_key,
                 work_package_accessor=work_package_accessor,
             )
         file_stager.update_staged_files()
 
 
 @cli.command()
-def decrypt(  # noqa: C901
+def decrypt(  # noqa: C901 # pylint: disable=too-many-branches
     *,
     input_dir: Path = typer.Option(
         ...,
         help="Path to the directory containing files that should be decrypted using a "
         + "common decryption key.",
     ),
     output_dir: Path = typer.Option(
         None,
-        help="Optional path to a directory the decrypted file should be written to. "
+        help="Optional path to a directory that the decrypted file should be written to. "
         + "Defaults to current working directory.",
     ),
     decryption_private_key_path: Path = typer.Option(
         ...,
         help="Path to the private key that should be used to decrypt the file.",
     ),
+    debug: bool = typer.Option(
+        False, help="Set this option in order to view traceback for errors."
+    ),
 ):
     """Command to decrypt a downloaded file"""
 
+    if not debug:
+        sys.excepthook = lambda x, y, z: None
+
     message_display = CLIMessageDisplay()
 
     if not input_dir.is_dir():
         message_display.failure(
-            f"Input directory {input_dir} does not exist or is not a directory."
+            f"Input directory '{input_dir}' does not exist or is not a directory."
         )
 
     if not output_dir:
         output_dir = Path(os.getcwd())
 
     if output_dir.exists() and not output_dir.is_dir():
         message_display.failure(
-            f"Output directory location {input_dir} exists, but is not a directory."
+            f"Output directory location '{input_dir}' exists, but is not a directory."
         )
 
     if not output_dir.exists():
         output_dir.mkdir(parents=True)
 
     errors = {}
     skipped_files = []
@@ -224,15 +252,15 @@
 
         # strip the .c4gh extension for the output file
         output_file = output_dir / input_file.with_suffix("")
 
         if output_file.exists():
             errors[
                 str(input_file)
-            ] = f"File already exists at {output_file}, will not overwrite."
+            ] = f"File already exists at '{output_file}', will not overwrite."
             continue
 
         try:
             core.decrypt_file(
                 input_file=input_file,
                 output_file=output_file,
                 decryption_private_key_path=decryption_private_key_path,
@@ -240,20 +268,20 @@
         except ValueError as error:
             errors[
                 str(input_file)
             ] = f"Could not decrypt the provided file with the given key.\nError: {str(error)}"
             continue
 
         message_display.success(
-            f"Successfully decrypted file {input_file} to location {output_dir}."
+            f"Successfully decrypted file '{input_file}' to location '{output_dir}'."
         )
 
     if skipped_files:
         message_display.display(
-            "The following files were skipped as they are not .c4gh files"
+            "The following files were skipped as they are not .c4gh files:"
         )
         for file in skipped_files:
             message_display.display(f"- {file}")
 
     if errors:
         message_display.failure("The following files could not be decrypted:")
         for input_path, cause in errors.items():
```

### Comparing `ghga_connector-0.3.6/ghga_connector/config.py` & `ghga_connector-0.3.7/ghga_connector/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,30 +22,20 @@
 from ghga_connector.core.constants import DEFAULT_PART_SIZE, MAX_RETRIES, MAX_WAIT_TIME
 
 
 @config_from_yaml(prefix="ghga_connector")
 class Config(BaseSettings):
     "Global Config Parameters"
 
-    upload_api: str = Field(
-        "https://hd-dev.ghga-dev.de/ucs",
-        description="URL to the root of the upload controller API.",
-    )
-    download_api: str = Field(
-        "https://hd-dev.ghga-dev.de/drs3/ga4gh/drs/v1",
-        description="URL to the root of the DRS-compatible API used for download.",
-    )
     max_retries: int = Field(
         MAX_RETRIES, description="Number of times to retry failed API calls."
     )
     max_wait_time: int = Field(
         MAX_WAIT_TIME,
         description="Maximal time in seconds to wait before quitting without a download.",
     )
     part_size: int = Field(
         DEFAULT_PART_SIZE, description="The part size to use for download."
     )
-    server_pubkey: str = Field(
-        ...,
-        description="Base64 encoded current GHGA public key for Crypt4GH encryption.",
+    wkvs_api_url: str = Field(
+        ..., description="URL to the root of the WKVS API. Should start with https://"
     )
-    wps_api_url: str = Field(..., description="URL to the root of the WPS API.")
```

### Comparing `ghga_connector-0.3.6/ghga_connector/core/__init__.py` & `ghga_connector-0.3.7/ghga_connector/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """
 This sub-package contains the main business functionality of this service.
 It should not contain any service API-related code.
 """
 
 from . import exceptions  # noqa: F401
-from .api_calls import WorkPackageAccessor  # noqa: F401
+from .api_calls import WKVSCaller, WorkPackageAccessor  # noqa: F401
 from .batch_processing import CliIoHandler, FileStager, StagingParameters  # noqa: F401
 from .client import HttpxClientState, httpx_client  # noqa: F401
 from .constants import (  # noqa: F401
     DEFAULT_PART_SIZE,
     MAX_PART_NUMBER,
     MAX_RETRIES,
     MAX_WAIT_TIME,
```

### Comparing `ghga_connector-0.3.6/ghga_connector/core/api_calls/__init__.py` & `ghga_connector-0.3.7/ghga_connector/core/api_calls/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,8 +30,9 @@
     get_part_upload_urls,
     get_upload_info,
     initiate_multipart_upload,
     patch_multipart_upload,
     start_multipart_upload,
 )
 from .utils import check_url  # noqa: F401
+from .well_knowns import WKVSCaller  # noqa: F401
 from .work_package import WorkPackageAccessor  # noqa: F401
```

### Comparing `ghga_connector-0.3.6/ghga_connector/core/api_calls/download.py` & `ghga_connector-0.3.7/ghga_connector/core/api_calls/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,19 +141,19 @@
         try:
             response_body = get_download_url(
                 file_id=file_id,
                 work_package_accessor=work_package_accessor,
             )
         except exceptions.BadResponseCodeError as error:
             message_display.failure(
-                "The request was invalid and returnd a wrong HTTP status code."
+                "The request was invalid and returned a bad HTTP status code."
             )
             raise error
         except exceptions.RequestFailedError as error:
-            message_display.failure("The request has failed.")
+            message_display.failure("The request failed.")
             raise error
 
         if response_body[0] is not None:
             download_url: str = response_body[0]
             file_size: int = response_body[1]
             return (download_url, file_size)
```

### Comparing `ghga_connector-0.3.6/ghga_connector/core/api_calls/upload.py` & `ghga_connector-0.3.7/ghga_connector/core/api_calls/upload.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/api_calls/utils.py` & `ghga_connector-0.3.7/ghga_connector/core/api_calls/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/api_calls/work_package.py` & `ghga_connector-0.3.7/ghga_connector/core/api_calls/work_package.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/batch_processing.py` & `ghga_connector-0.3.7/ghga_connector/core/batch_processing.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/client.py` & `ghga_connector-0.3.7/ghga_connector/core/client.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/constants.py` & `ghga_connector-0.3.7/ghga_connector/core/constants.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/exceptions.py` & `ghga_connector-0.3.7/ghga_connector/core/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         super().__init__(message)
 
 
 class FileAlreadyExistsError(RuntimeError):
     """Thrown, when the specified file already exists."""
 
     def __init__(self, *, output_file: str):
-        message = f"The file {output_file} does already exist."
+        message = f"The file {output_file} already exists."
         super().__init__(message)
 
 
 class FileAlreadyEncryptedError(RuntimeError):
     """Thrown, when the specified file is already encrypted."""
 
     def __init__(self, *, file_path: Path):
@@ -74,15 +74,17 @@
 class PubkeyMismatchError(RuntimeError):
     """
     Thrown when the user public key announced in the submission metadata retrieved from
     the work package service does not match the user public key provided to the connector
     """
 
     def __init__(self):
-        message = "Provided user public key does not match announced user public key."
+        message = (
+            "Provided user public key does not match the announced user public key."
+        )
         super().__init__(message)
 
 
 class PrivateKeyFileDoesNotExistError(RuntimeError):
     """Thrown, when the specified private key file does exist."""
 
     def __init__(self, *, private_key_path: Path):
@@ -126,15 +128,15 @@
 
 
 class FileNotRegisteredError(RuntimeError):
     """Thrown, when a request for a file returns a 404 error."""
 
     def __init__(self, *, file_id: str):
         message = (
-            f"The request for the file {file_id} failed, "
+            f"The request for the file '{file_id}' failed, "
             "because this file id does not exist."
         )
         super().__init__(message)
 
 
 class UploadNotRegisteredError(RuntimeError):
     """Thrown, when a request for a multipart upload returns a 404 error."""
@@ -157,17 +159,17 @@
 
 
 class NoUploadPossibleError(RuntimeError):
     """Thrown, when a multipart upload currently can't be started (response code 400)"""
 
     def __init__(self, *, file_id: str):
         message = (
-            "It is not possible to start a multipart upload for file with id"
-            + f" '{file_id}', because this download is already pending or has been"
-            + " accepted."
+            "It is not possible to start a multipart upload for file with id "
+            + f"'{file_id}', because this download is already pending or has been "
+            + "accepted."
         )
         super().__init__(message)
 
 
 class DownloadFinalizationError(RuntimeError):
     """
     Thrown when a downloaded file cannot be moved to its final location, as another file
@@ -187,29 +189,29 @@
     Thrown when a user does not have the credentials to get or change
     details of an ongoing upload with a specific upload id
     (response code 403)
     """
 
     def __init__(self, *, upload_id: str):
         message = (
-            "This user is not registered as data submitter "
+            "This user is not registered as the data submitter "
             f"for the file corresponding to the upload_id '{upload_id}'."
         )
         super().__init__(message)
 
 
 class UserHasNoFileAccessError(RuntimeError):
     """
     Thrown when a user does not have the credentials for
     a specific file id (response code 403)
     """
 
     def __init__(self, *, file_id: str):
         message = (
-            "This user is not registered as data submitter "
+            "This user is not registered as the data submitter "
             f"for the file with the id '{file_id}'."
         )
         super().__init__(message)
 
 
 class CantChangeUploadStatusError(RuntimeError):
     """
@@ -231,15 +233,15 @@
         super().__init__(message)
 
 
 class ConnectionFailedError(RuntimeError):
     """Thrown, when a ConnectError or ConnectTimeout error is raised by httpx"""
 
     def __init__(self, *, url: str, reason: str):
-        message = f"Request to '{url}' failed to connect. Reason: {reason}"
+        message = f"Request to {url} failed to connect. Reason: {reason}"
         super().__init__(message)
 
 
 class MaxPartNoExceededError(RuntimeError):
     """
     Thrown requesting a part number larger than the maximally possible number of parts.
 
@@ -260,15 +262,17 @@
         raise ConnectionFailedError(url=url, reason=connection_failure)
 
 
 class EnvelopeNotFoundError(RuntimeError):
     """Thrown, when the envelope requested for a file could not be retrieved"""
 
     def __init__(self, *, file_id: str):
-        message = f"The request for an envelope for the file with ID {file_id} failed."
+        message = (
+            f"The request for an envelope for the file with ID '{file_id}' failed."
+        )
         super().__init__(message)
 
 
 class ExternalApiError(RuntimeError):
     """Thrown, when the services request to an external API failed"""
 
     def __init__(self):
@@ -303,21 +307,34 @@
     Thrown when communication with the Work Package Service returns an unexpected response.
     This should be used instead of BadResponseError when handling WPS results to differntiate
     """
 
     def __init__(self, *, url: str, response_code: int):
         self.response_code = response_code
         message = (
-            f"The request to the WPS at {url} failed with an unexpected response code"
-            + f" of {response_code}."
+            f"The request to the WPS at {url} failed with an unexpected response code "
+            + f"of {response_code}."
         )
         super().__init__(message)
 
 
 class UnauthorizedAPICallError(RuntimeError):
     """
     Thrown when a 403 is returned from a call requiring a work order token for authorization
     """
 
     def __init__(self, *, url: str, cause: str):
         message = f"Could not authorize call to {url}: {cause}"
         super().__init__(message)
+
+
+class WellKnownValueNotFound(RuntimeError):
+    """
+    Thrown when a 404 is returned from a call to the well-known-value-service for a
+    specific value name.
+    """
+
+    def __init__(self, *, value_name):
+        message = (
+            f"Unable to retrieve value of '{value_name}' from well-known-value-service"
+        )
+        super().__init__(message)
```

### Comparing `ghga_connector-0.3.6/ghga_connector/core/file_operations.py` & `ghga_connector-0.3.7/ghga_connector/core/file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/http_translation.py` & `ghga_connector-0.3.7/ghga_connector/core/http_translation.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector/core/main.py` & `ghga_connector-0.3.7/ghga_connector/core/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             f"The file {file_path} is already Crypt4GH encrypted."
             + "\nThis is currently not supported."
             + " Please provide your data without Crypt4GH encryption."
         )
         raise exceptions.FileAlreadyEncryptedError(file_path=file_path)
 
     if not check_url(api_url):
-        message_display.failure(f"The url {api_url} is currently not reachable.")
+        message_display.failure(f"The url {api_url} is not currently reachable.")
         raise exceptions.ApiNotReachableError(api_url=api_url)
 
     try:
         upload_id, part_size = start_multipart_upload(
             api_url=api_url, file_id=file_id, pubkey_path=submitter_pubkey_path
         )
     except exceptions.NoUploadPossibleError as error:
@@ -103,19 +103,19 @@
         raise error
     except exceptions.UserHasNoUploadAccessError as error:
         message_display.failure(
             f"The user is not registered as a Data Submitter for the file with id '{file_id}'."
         )
         raise error
     except exceptions.FileNotRegisteredError as error:
-        message_display.failure(f"The file with the id {file_id} is not registered.")
+        message_display.failure(f"The file with the id '{file_id}' is not registered.")
         raise error
     except exceptions.BadResponseCodeError as error:
         message_display.failure(
-            "The request was invalid and returnd a wrong HTTP status code."
+            "The request was invalid and returned a bad HTTP status code."
         )
         raise error
     except exceptions.CantChangeUploadStatusError as error:
         message_display.failure(f"The file with id '{file_id}' was already uploaded.")
         raise error
     except exceptions.RequestFailedError as error:
         message_display.failure("The request to start a multipart upload has failed.")
@@ -132,35 +132,33 @@
         upload_file_parts(
             api_url=api_url,
             upload_id=upload_id,
             part_size=part_size,
             file_path=Path(encrypted_file_path),
         )
     except exceptions.ConnectionFailedError as error:
-        message_display.failure(
-            "The upload has failed too many times. The upload was aborted."
-        )
+        message_display.failure("The upload failed too many times and was aborted.")
         raise error
     finally:
         # remove temporary encrypted file
         os.remove(encrypted_file_path)
 
     try:
         patch_multipart_upload(
             api_url=api_url,
             upload_id=upload_id,
             upload_status=UploadStatus.UPLOADED,
         )
     except exceptions.BadResponseCodeError as error:
         message_display.failure(
-            f"The request to confirm the upload with id {upload_id} was invalid."
+            f"The request to confirm the upload with id '{upload_id}' was invalid."
         )
         raise error
     except exceptions.RequestFailedError as error:
-        message_display.failure(f"Confirming the upload with id {upload_id} failed.")
+        message_display.failure(f"Confirming the upload with id '{upload_id}' failed.")
         raise error
     message_display.success(f"File with id '{file_id}' has been successfully uploaded.")
 
 
 def upload_file_parts(
     *,
     api_url: str,
@@ -193,15 +191,15 @@
     file_extension: str = "",
 ) -> None:
     """
     Core command to download a file. Can be called by CLI, GUI, etc.
     """
 
     if not check_url(api_url):
-        message_display.failure(f"The url {api_url} is currently not reachable.")
+        message_display.failure(f"The url {api_url} is not currently reachable.")
         raise exceptions.ApiNotReachableError(api_url=api_url)
 
     # construct file name with suffix, if given
     file_name = f"{file_id}"
     if file_extension:
         file_name = f"{file_id}{file_extension}"
 
@@ -233,15 +231,15 @@
         )
     except (
         exceptions.FileNotRegisteredError,
         exceptions.EnvelopeNotFoundError,
         exceptions.ExternalApiError,
     ) as error:
         message_display.failure(
-            f"The request to get an envelope for file {file_id} failed."
+            f"The request to get an envelope for file '{file_id}' failed."
         )
         raise error
 
     # perform the download
     try:
         download_parts(
             envelope=envelope,
@@ -253,16 +251,16 @@
         )
     except exceptions.ConnectionFailedError as error:
         # Remove file, if the download failed.
         output_file_ongoing.unlink()
         raise error
     except exceptions.NoS3AccessMethodError as error:
         message_display.failure(
-            f"The request to return information for file {file_id}"
-            + " did not return an S3 access method."
+            f"The request to return information for file '{file_id}' "
+            + "did not return an S3 access method."
         )
         output_file_ongoing.unlink()
         raise error
 
     # rename fully downloaded file
     if output_file.exists():
         raise exceptions.DownloadFinalizationError(file_path=output_file)
@@ -336,15 +334,16 @@
     for _ in range(max_tries):
         work_package_string = input(
             "Paste the complete work package string you got from the UI: "
         )
         work_package_parts = work_package_string.split(":")
         if len(work_package_parts) != 2:
             message_display.display(
-                "Invalid input. Please enter the work package string you got from the UI unaltered."
+                "Invalid input. Please enter the work package string you got from the "
+                + "UI unaltered."
             )
             continue
         return work_package_parts
     message_display.failure(
         f"Tried {max_tries} times to parse the work package string and failed."
     )
     raise exceptions.InvalidWorkPackageToken(tries=max_tries)
```

### Comparing `ghga_connector-0.3.6/ghga_connector/core/message_display.py` & `ghga_connector-0.3.7/ghga_connector/core/message_display.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/ghga_connector.egg-info/PKG-INFO` & `ghga_connector-0.3.7/ghga_connector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-connector
-Version: 0.3.6
+Version: 0.3.7
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.6
+docker pull ghga/ghga-connector:0.3.7
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.6 .
+docker build -t ghga/ghga-connector:0.3.7 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.6 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.7 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -71,27 +71,21 @@
 ghga_connector --help
 ```
 
 ## Configuration
 ### Parameters
 
 The service requires the following configuration parameters:
-- **`upload_api`** *(string)*: URL to the root of the upload controller API. Default: `https://hd-dev.ghga-dev.de/ucs`.
-
-- **`download_api`** *(string)*: URL to the root of the DRS-compatible API used for download. Default: `https://hd-dev.ghga-dev.de/drs3/ga4gh/drs/v1`.
-
 - **`max_retries`** *(integer)*: Number of times to retry failed API calls. Default: `5`.
 
 - **`max_wait_time`** *(integer)*: Maximal time in seconds to wait before quitting without a download. Default: `3600`.
 
 - **`part_size`** *(integer)*: The part size to use for download. Default: `16777216`.
 
-- **`server_pubkey`** *(string)*: Base64 encoded current GHGA public key for Crypt4GH encryption.
-
-- **`wps_api_url`** *(string)*: URL to the root of the WPS API.
+- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://.
 
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.ghga_connector.yaml`, and place it into one of the following locations:
```

### Comparing `ghga_connector-0.3.6/ghga_connector.egg-info/SOURCES.txt` & `ghga_connector-0.3.7/ghga_connector.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ghga_connector/core/http_translation.py
 ghga_connector/core/main.py
 ghga_connector/core/message_display.py
 ghga_connector/core/api_calls/__init__.py
 ghga_connector/core/api_calls/download.py
 ghga_connector/core/api_calls/upload.py
 ghga_connector/core/api_calls/utils.py
+ghga_connector/core/api_calls/well_knowns.py
 ghga_connector/core/api_calls/work_package.py
 scripts/__init__.py
 scripts/get_package_name.py
 scripts/license_checker.py
 scripts/update_config_docs.py
 scripts/update_readme.py
 scripts/update_template_files.py
```

### Comparing `ghga_connector-0.3.6/scripts/__init__.py` & `ghga_connector-0.3.7/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/get_package_name.py` & `ghga_connector-0.3.7/scripts/get_package_name.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/license_checker.py` & `ghga_connector-0.3.7/scripts/license_checker.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/script_utils/__init__.py` & `ghga_connector-0.3.7/scripts/script_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/script_utils/cli.py` & `ghga_connector-0.3.7/scripts/script_utils/cli.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/update_config_docs.py` & `ghga_connector-0.3.7/scripts/update_config_docs.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/update_readme.py` & `ghga_connector-0.3.7/scripts/update_readme.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/scripts/update_template_files.py` & `ghga_connector-0.3.7/scripts/update_template_files.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/setup.cfg` & `ghga_connector-0.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/setup.py` & `ghga_connector-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/fixtures/__init__.py` & `ghga_connector-0.3.7/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/fixtures/config.py` & `ghga_connector-0.3.7/tests/fixtures/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,21 +16,18 @@
 
 """Config utilies."""
 
 from ghga_connector import core
 from ghga_connector.config import Config
 
 DEFAULT_TEST_CONFIG = Config(
-    upload_api="http:/example.org/upload",
-    download_api="http:/example.org/download",
     max_retries=0,
     max_wait_time=2,
     part_size=core.DEFAULT_PART_SIZE,
-    server_pubkey="qx5g31H7rdsq7sgkew9ElkLIXvBje4RxDVcAHcJD8XY=",
-    wps_api_url="http://127.0.0.1",
+    wkvs_api_url="https://127.0.0.1",
 )
 
 
 def get_test_config(**kwargs):
     """Get test config params with the defaults being overwritting by the parameter
     passed as kwargs.
     """
```

### Comparing `ghga_connector-0.3.6/tests/fixtures/endpoints_handler.py` & `ghga_connector-0.3.7/tests/fixtures/endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/fixtures/mock_api/__init__.py` & `ghga_connector-0.3.7/tests/fixtures/mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/fixtures/mock_api/app.py` & `ghga_connector-0.3.7/tests/fixtures/mock_api/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -441,14 +441,38 @@
 
     # has to be at least 48 chars long
     return httpx.Response(
         status_code=201, content=base64.b64encode(b"1234567890" * 5).decode()
     )
 
 
+@EndpointsHandler.get("/values/{value_name}")
+def mock_wkvs(value_name: str):
+    """Mock the WKVS /values/value_name endpoint"""
+    values: dict[str, str] = {
+        "crypt4gh_public_key": "qx5g31H7rdsq7sgkew9ElkLIXvBje4RxDVcAHcJD8XY=",
+        "wps_api_url": "http://127.0.0.1/wps",
+        "dcs_api_url": "http://127.0.0.1/download",
+        "ucs_api_url": "http://127.0.0.1/upload",
+    }
+
+    if value_name in values:
+        return httpx.Response(
+            status_code=200,
+            json={value_name: values[value_name]},
+        )
+    else:
+        raise HttpyException(
+            status_code=404,
+            exception_id="valueNotConfigured",
+            description=f"The value {value_name} is not configured.",
+            data={"value_name": value_name},
+        )
+
+
 def handle_request(request: httpx.Request):
     """
     This is used as the callback function for the httpx_mock fixture in test_cli.py.
     """
     url = str(request.url)
     logger.info("Received request for url: %s", url)
     try:
```

### Comparing `ghga_connector-0.3.6/tests/fixtures/s3.py` & `ghga_connector-0.3.7/tests/fixtures/s3.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/fixtures/state.py` & `ghga_connector-0.3.7/tests/fixtures/state.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/fixtures/utils.py` & `ghga_connector-0.3.7/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/integration/__init__.py` & `ghga_connector-0.3.7/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/integration/fixtures/__init__.py` & `ghga_connector-0.3.7/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/integration/fixtures/utils.py` & `ghga_connector-0.3.7/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/integration/test_cli.py` & `ghga_connector-0.3.7/tests/integration/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from ghga_connector.core.file_operations import Crypt4GHEncryptor
 from tests.fixtures import state
 from tests.fixtures.config import get_test_config
 from tests.fixtures.mock_api.app import handle_request
 from tests.fixtures.s3 import S3Fixture, get_big_s3_object, s3_fixture  # noqa: F401
 from tests.fixtures.utils import PRIVATE_KEY_FILE, PUBLIC_KEY_FILE, mock_wps_token
 
-URL_PATTERN = re.compile(r"^http://127\.0\.0\.1.*")
+URL_PATTERN = re.compile(r"^https?://127\.0\.0\.1.*")
 
 ENVIRON_DEFAULTS = {
     "DEFAULT_PART_SIZE": str(16 * 1024 * 1024),
     "S3_DOWNLOAD_URL": "test://download.url",
     "S3_UPLOAD_URL_1": "test://upload.url",
     "S3_UPLOAD_URL_2": "test://upload.url",
     "S3_DOWNLOAD_FIELD_SIZE": str(146),
@@ -219,17 +219,22 @@
 
     monkeypatch.setenv("S3_DOWNLOAD_URL", download_url)
     monkeypatch.setenv("S3_DOWNLOAD_FIELD_SIZE", str(os.path.getsize(file.file_path)))
     monkeypatch.setenv("FAKE_ENVELOPE", fake_envelope)
 
     api_url = "http://bad_url" if bad_url else "http://127.0.0.1"
 
+    for wkvs_method in ["get_wps_api_url", "get_dcs_api_url"]:
+        monkeypatch.setattr(
+            f"ghga_connector.core.api_calls.well_knowns.WKVSCaller.{wkvs_method}",
+            lambda x: api_url,
+        )
     with patch(
         "ghga_connector.cli.CONFIG",
-        get_test_config(download_api=api_url, wps_api_url=api_url),
+        get_test_config(),
     ):
         # needed to mock user input
         with patch(
             "ghga_connector.core.batch_processing.CliInputHandler.get_input",
             return_value="yes" if proceed_on_missing else "no",
         ):
             if file_name == "file_not_downloadable":
@@ -337,16 +342,20 @@
         part_number=1,
     )
     unintercepted_hosts.append(httpx.URL(upload_url).host)
 
     monkeypatch.setenv("S3_UPLOAD_URL_1", upload_url)
 
     api_url = "http://bad_url" if bad_url else "http://127.0.0.1"
+    monkeypatch.setattr(
+        "ghga_connector.core.api_calls.well_knowns.WKVSCaller.get_ucs_api_url",
+        lambda x: api_url,
+    )
 
-    with patch("ghga_connector.cli.CONFIG", get_test_config(upload_api=api_url)):
+    with patch("ghga_connector.cli.CONFIG", get_test_config()):
         with pytest.raises(  # type: ignore
             expected_exception
         ) if expected_exception else nullcontext():
             if file_name == "encrypted_file":
                 upload(
                     file_id=uploadable_file.file_id,
                     file_path=Path(encrypted_path).resolve(),
@@ -430,18 +439,22 @@
 
     monkeypatch.setenv("S3_UPLOAD_URL_1", upload_url_1)
     monkeypatch.setenv("S3_UPLOAD_URL_2", upload_url_2)
 
     api_url = "http://127.0.0.1"
 
     # create big temp file
+    monkeypatch.setattr(
+        "ghga_connector.core.api_calls.well_knowns.WKVSCaller.get_ucs_api_url",
+        lambda x: api_url,
+    )
     with big_temp_file(file_size) as file:
         with patch(
             "ghga_connector.cli.CONFIG",
-            get_test_config(upload_api=api_url),
+            get_test_config(),
         ):
             upload(
                 file_id=file_id,
                 file_path=Path(file.name),
                 submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
                 submitter_private_key_path=Path(PRIVATE_KEY_FILE),
             )
```

### Comparing `ghga_connector-0.3.6/tests/integration/test_file_operations.py` & `ghga_connector-0.3.7/tests/integration/test_file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/unit/__init__.py` & `ghga_connector-0.3.7/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/unit/fixtures/__init__.py` & `ghga_connector-0.3.7/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/unit/fixtures/utils.py` & `ghga_connector-0.3.7/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/unit/test_api_calls.py` & `ghga_connector-0.3.7/tests/unit/test_api_calls.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 from contextlib import nullcontext
 from typing import Optional
 from unittest.mock import Mock
 
 import pytest
 from pytest_httpx import HTTPXMock
 
+from ghga_connector.core import WKVSCaller
 from ghga_connector.core.api_calls import (
     UploadStatus,
     WorkPackageAccessor,
     get_part_upload_urls,
     patch_multipart_upload,
 )
 from ghga_connector.core.exceptions import (
     CantChangeUploadStatusError,
     ConnectionFailedError,
     InvalidWPSResponseError,
     MaxPartNoExceededError,
     NoWorkPackageAccessError,
     UploadNotRegisteredError,
+    WellKnownValueNotFound,
 )
 from tests.fixtures.utils import mock_wps_token
 
 
 @pytest.mark.parametrize(
     "bad_url,upload_id,upload_status,expected_exception",
     [
@@ -185,7 +187,34 @@
             access_token=wp_token,
             api_url="http://127.0.0.1",
             dcs_api_url="",
             package_id=wp_id,
             submitter_private_key="",
         )
         response = work_package_accessor.get_package_files()
+
+
+@pytest.mark.asyncio
+async def test_wkvs_calls(httpx_mock: HTTPXMock):
+    """Test handling of responses for WKVS api calls"""
+
+    wkvs_url = "https://127.0.0.1"
+    wkvs_caller = WKVSCaller(wkvs_url)
+
+    with pytest.raises(WellKnownValueNotFound):
+        httpx_mock.add_response(status_code=404)
+        wkvs_caller.get_server_pubkey()
+
+    with pytest.raises(KeyError):
+        httpx_mock.add_response(status_code=200, json={})
+        wkvs_caller.get_server_pubkey()
+
+    # test each call to CYA
+    for func, value_name in [
+        (wkvs_caller.get_dcs_api_url, "dcs_api_url"),
+        (wkvs_caller.get_server_pubkey, "crypt4gh_public_key"),
+        (wkvs_caller.get_ucs_api_url, "ucs_api_url"),
+        (wkvs_caller.get_wps_api_url, "wps_api_url"),
+    ]:
+        httpx_mock.add_response(json={value_name: "dummy-value"})
+        value = func()
+        assert value == "dummy-value"
```

### Comparing `ghga_connector-0.3.6/tests/unit/test_core.py` & `ghga_connector-0.3.7/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.6/tests/unit/test_file_operations.py` & `ghga_connector-0.3.7/tests/unit/test_file_operations.py`

 * *Files identical despite different names*

