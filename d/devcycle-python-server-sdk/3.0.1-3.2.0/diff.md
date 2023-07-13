# Comparing `tmp/devcycle-python-server-sdk-3.0.1.tar.gz` & `tmp/devcycle-python-server-sdk-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-3.0.1.tar", last modified: Thu Jul  6 20:05:24 2023, max compression
+gzip compressed data, was "dist/devcycle-python-server-sdk-3.2.0.tar", last modified: Thu Jul 13 21:25:27 2023, max compression
```

## Comparing `devcycle-python-server-sdk-3.0.1.tar` & `devcycle-python-server-sdk-3.2.0.tar`

### file list

```diff
@@ -1,77 +1,73 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.765314 devcycle-python-server-sdk-3.0.1/
--rw-r--r--   0 chris      (501) staff       (20)     1071 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-3.0.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-07-06 20:05:24.765415 devcycle-python-server-sdk-3.0.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     3139 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.756899 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/
--rw-r--r--   0 chris      (501) staff       (20)        5 2023-07-06 20:04:49.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/VERSION.txt
--rw-r--r--   0 chris      (501) staff       (20)      265 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.758019 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      303 2023-06-26 21:35:27.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/backoff.py
--rw-r--r--   0 chris      (501) staff       (20)     5074 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 chris      (501) staff       (20)     4226 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/config_client.py
--rw-r--r--   0 chris      (501) staff       (20)     3319 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/event_client.py
--rw-r--r--   0 chris      (501) staff       (20)    16322 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 chris      (501) staff       (20)   200891 2023-06-27 20:58:00.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/bucketing-lib.release.wasm
--rw-r--r--   0 chris      (501) staff       (20)     6675 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/cloud_client.py
--rw-r--r--   0 chris      (501) staff       (20)     1053 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/exceptions.py
--rw-r--r--   0 chris      (501) staff       (20)     8605 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/local_client.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.758533 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/managers/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     3122 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 chris      (501) staff       (20)     7909 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.760443 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     3814 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/bucketed_config.py
--rw-r--r--   0 chris      (501) staff       (20)      442 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 chris      (501) staff       (20)     3713 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/event.py
--rw-r--r--   0 chris      (501) staff       (20)      852 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 chris      (501) staff       (20)      783 2023-06-29 23:05:15.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/platform_data.py
--rw-r--r--   0 chris      (501) staff       (20)     2616 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/user.py
--rw-r--r--   0 chris      (501) staff       (20)     1711 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 chris      (501) staff       (20)     4525 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/options.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.760891 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/protobuf/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-20 21:51:55.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/protobuf/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     4684 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/protobuf/utils.py
--rw-r--r--   0 chris      (501) staff       (20)     4244 2023-06-28 18:13:43.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-20 20:00:51.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/py.typed
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.761382 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/util/
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      253 2023-06-23 22:50:02.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.762061 devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-07-06 20:05:24.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2083 2023-07-06 20:05:24.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-07-06 20:05:24.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       85 2023-07-06 20:05:24.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       33 2023-07-06 20:05:24.000000 devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.762426 devcycle-python-server-sdk-3.0.1/example/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-3.0.1/example/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2463 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/example/cloud_client_example.py
--rw-r--r--   0 chris      (501) staff       (20)     2676 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/example/local_bucketing_client_example.py
--rw-r--r--   0 chris      (501) staff       (20)       87 2023-07-05 21:12:29.000000 devcycle-python-server-sdk-3.0.1/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)       79 2023-07-06 20:05:24.765655 devcycle-python-server-sdk-3.0.1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      943 2023-07-06 20:04:49.000000 devcycle-python-server-sdk-3.0.1/setup.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.762813 devcycle-python-server-sdk-3.0.1/test/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-3.0.1/test/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.763666 devcycle-python-server-sdk-3.0.1/test/api/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.1/test/api/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     7565 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/test/api/test_bucketing_client.py
--rw-r--r--   0 chris      (501) staff       (20)     4275 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/test/api/test_config_client.py
--rw-r--r--   0 chris      (501) staff       (20)     3211 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/test/api/test_event_client.py
--rw-r--r--   0 chris      (501) staff       (20)    15156 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/test/api/test_local_bucketing.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.763909 devcycle-python-server-sdk-3.0.1/test/fixture/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-21 22:58:59.000000 devcycle-python-server-sdk-3.0.1/test/fixture/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1372 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.1/test/fixture/data.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.764418 devcycle-python-server-sdk-3.0.1/test/managers/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.1/test/managers/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     5366 2023-07-04 17:13:35.000000 devcycle-python-server-sdk-3.0.1/test/managers/test_config_manager.py
--rw-r--r--   0 chris      (501) staff       (20)    11053 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/test/managers/test_event_queue_manager.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.764628 devcycle-python-server-sdk-3.0.1/test/models/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.1/test/models/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      858 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.1/test/models/test_bucketed_config.py
--rw-r--r--   0 chris      (501) staff       (20)    11442 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/test/test_cloud_client.py
--rw-r--r--   0 chris      (501) staff       (20)    12671 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.1/test/test_local_client.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 20:05:24.765044 devcycle-python-server-sdk-3.0.1/test/util/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.1/test/util/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     6671 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.1/test/util/test_utils.py
--rw-r--r--   0 chris      (501) staff       (20)      368 2023-07-06 20:04:49.000000 devcycle-python-server-sdk-3.0.1/test/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 21:25:26.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:25:26.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 21:25:26.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 21:25:26.000000 devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/example/cloud_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/example/local_bucketing_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/api/test_bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/api/test_config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/api/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/api/test_local_bucketing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/fixture/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/test/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/managers/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/models/test_bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/test_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/test_local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:27.000000 devcycle-python-server-sdk-3.2.0/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/util/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 21:25:12.000000 devcycle-python-server-sdk-3.2.0/test/util/test_version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `devcycle-python-server-sdk-3.0.1/README.md` & `devcycle-python-server-sdk-3.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ```
 ruff check . --fix
 ```
 
 Formatting checks on PRs are done using [black](https://github.com/psf/black). To run the formatter locally, run this command from the top level of the repo:
 
 ```
-black --target-version py37 --extend-exclude '_pb2\.pyi?$' .
+black .
 ```
 
 ### Unit Tests
 
 To run the unit tests, run:
 ```bash
 pytest
```

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/config_client.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/event_client.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/api/local_bucketing.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/api/local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/cloud_client.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/local_client.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/managers/config_manager.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/managers/config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/managers/event_queue_manager.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/managers/event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/bucketed_config.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/platform_data.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/platform_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/options.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/options.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/protobuf/utils.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/protobuf/utils.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py` & `devcycle-python-server-sdk-3.2.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.2.0/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-devcycle_python_sdk/VERSION.txt
 devcycle_python_sdk/__init__.py
-devcycle_python_sdk/bucketing-lib.release.wasm
 devcycle_python_sdk/cloud_client.py
 devcycle_python_sdk/exceptions.py
 devcycle_python_sdk/local_client.py
 devcycle_python_sdk/options.py
-devcycle_python_sdk/py.typed
 devcycle_python_sdk/api/__init__.py
 devcycle_python_sdk/api/backoff.py
 devcycle_python_sdk/api/bucketing_client.py
 devcycle_python_sdk/api/config_client.py
 devcycle_python_sdk/api/event_client.py
 devcycle_python_sdk/api/local_bucketing.py
 devcycle_python_sdk/managers/__init__.py
```

### Comparing `devcycle-python-server-sdk-3.0.1/example/cloud_client_example.py` & `devcycle-python-server-sdk-3.2.0/example/cloud_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/example/local_bucketing_client_example.py` & `devcycle-python-server-sdk-3.2.0/example/local_bucketing_client_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,22 @@
 
     # create an instance of the DevCycle Client object
     server_sdk_key = os.environ["DEVCYCLE_SERVER_SDK_KEY"]
     options = DevCycleLocalOptions()
     client = DevCycleLocalClient(server_sdk_key, options)
 
     # Wait for DevCycle to initialize and load the configuration
-    while not client.is_initialized():
+    for i in range(10):
+        if client.is_initialized():
+            break
         logger.info("Waiting for DevCycle to initialize...")
-        time.sleep(1)
+        time.sleep(0.5)
+    else:
+        logger.error("DevCycle failed to initialize")
+        exit(1)
 
     user = DevCycleUser(user_id="test-1234", email="test-user@domain.com", country="US")
 
     # Use variable_value to access the value of a variable directly
     if client.variable_value(user, VARIABLE_KEY, False):
         logger.info(f"Variable {VARIABLE_KEY} is enabled")
     else:
```

### Comparing `devcycle-python-server-sdk-3.0.1/setup.py` & `devcycle-python-server-sdk-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.2.0/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/api/test_config_client.py` & `devcycle-python-server-sdk-3.2.0/test/api/test_config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/api/test_event_client.py` & `devcycle-python-server-sdk-3.2.0/test/api/test_event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/api/test_local_bucketing.py` & `devcycle-python-server-sdk-3.2.0/test/api/test_local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/fixture/data.py` & `devcycle-python-server-sdk-3.2.0/test/fixture/data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/managers/test_config_manager.py` & `devcycle-python-server-sdk-3.2.0/test/managers/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/managers/test_event_queue_manager.py` & `devcycle-python-server-sdk-3.2.0/test/managers/test_event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/models/test_bucketed_config.py` & `devcycle-python-server-sdk-3.2.0/test/models/test_bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/test_cloud_client.py` & `devcycle-python-server-sdk-3.2.0/test/test_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/test_local_client.py` & `devcycle-python-server-sdk-3.2.0/test/test_local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.0.1/test/util/test_utils.py` & `devcycle-python-server-sdk-3.2.0/test/util/test_utils.py`

 * *Files identical despite different names*

