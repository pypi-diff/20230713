# Comparing `tmp/splight-lib-3.1.0.tar.gz` & `tmp/splight-lib-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.1.0.tar", last modified: Thu Jul 13 12:23:19 2023, max compression
+gzip compressed data, was "splight-lib-3.1.1.tar", last modified: Thu Jul 13 16:57:29 2023, max compression
```

## Comparing `splight-lib-3.1.0.tar` & `splight-lib-3.1.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 12:23:19.650537 splight-lib-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-13 12:23:18.000000 splight-lib-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:23:19.650537 splight-lib-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 12:23:18.000000 splight-lib-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/grpc/reflector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/log_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/data_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:29.002098 splight-lib-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 16:57:29.002098 splight-lib-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-13 16:57:28.000000 splight-lib-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:57:29.002098 splight-lib-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 16:57:28.000000 splight-lib-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.990098 splight-lib-3.1.1/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.990098 splight-lib-3.1.1/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.990098 splight-lib-3.1.1/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.990098 splight-lib-3.1.1/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.990098 splight-lib-3.1.1/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.994098 splight-lib-3.1.1/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.994098 splight-lib-3.1.1/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.994098 splight-lib-3.1.1/splight_lib/client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/grpc/reflector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.994098 splight-lib-3.1.1/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.994098 splight-lib-3.1.1/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.994098 splight-lib-3.1.1/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/component/log_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.998098 splight-lib-3.1.1/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.998098 splight-lib-3.1.1/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/data_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.998098 splight-lib-3.1.1/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.998098 splight-lib-3.1.1/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:29.002098 splight-lib-3.1.1/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:57:28.990098 splight-lib-3.1.1/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 16:57:28.000000 splight-lib-3.1.1/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.1.0/PKG-INFO` & `splight-lib-3.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.0/setup.py` & `splight-lib-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.1.0",
+    version="3.1.1",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.1.0/splight_lib/abstract/client.py` & `splight-lib-3.1.1/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/auth/mac_auth.py` & `splight-lib-3.1.1/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/communication/abstract.py` & `splight-lib-3.1.1/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/communication/remote_client.py` & `splight-lib-3.1.1/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/database/abstract.py` & `splight-lib-3.1.1/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/database/builder.py` & `splight-lib-3.1.1/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/database/classmap.py` & `splight-lib-3.1.1/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/database/local_client.py` & `splight-lib-3.1.1/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/database/remote_client.py` & `splight-lib-3.1.1/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/datalake/abstract.py` & `splight-lib-3.1.1/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/datalake/builder.py` & `splight-lib-3.1.1/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/datalake/local_client.py` & `splight-lib-3.1.1/splight_lib/client/datalake/local_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 "group_id": group_id,
                 "group_fields": group_fields,
                 "tzinfo": tzinfo,
             }
         )
 
         documents = self._raw_get(**filters)
-        df = pd.DataFrarame([x.dict() for x in documents])
+        df = pd.DataFrame(documents)
 
         if not df.empty:
             df["timestamp"] = pd.to_datetime(df["timestamp"])
             df.set_index("timestamp", inplace=True, verify_integrity=False)
 
         return df
```

### Comparing `splight-lib-3.1.0/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.1.1/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/exceptions.py` & `splight-lib-3.1.1/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/file_handler.py` & `splight-lib-3.1.1/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/filter.py` & `splight-lib-3.1.1/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/grpc/client.py` & `splight-lib-3.1.1/splight_lib/client/grpc/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/grpc/reflector.py` & `splight-lib-3.1.1/splight_lib/client/grpc/reflector.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/hub/abstract.py` & `splight-lib-3.1.1/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/client/hub/client.py` & `splight-lib-3.1.1/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/communication/event_handler.py` & `splight-lib-3.1.1/splight_lib/communication/event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,24 +65,20 @@
         event = CommunicationEvent.parse_raw(event_str)
         if binding_object_type in DB_MODEL_TYPE_MAPPING.values():
             # Case in which is not a ComponentObject
             handler_arg = binding_object_type.parse_obj(event.data)
         elif issubclass(binding_object_type, ComponentObjectInstance):
             # Case for data represents a ComponentObject
             component_obj = ComponentObject.parse_obj(event.data)
-            model_class = ComponentObjectInstance.from_object(
-                component_obj
-            )
+            model_class = ComponentObjectInstance.from_object(component_obj)
             handler_arg = model_class.parse_object(component_obj)
         elif issubclass(binding_object_type, RoutineObjectInstance):
             # Case for data represents a RoutineObject
             routine_obj = RoutineObject.parse_obj(event.data)
-            model_class = RoutineObjectInstance.from_object(
-                component_obj
-            )
+            model_class = RoutineObjectInstance.from_object(routine_obj)
             handler_arg = model_class.parse_object(routine_obj)
         else:
             raise InvalidBidingObject(
                 f"Invalid binding object type: {binding_object_type}"
             )
 
         binding_function(handler_arg)
```

### Comparing `splight-lib-3.1.0/splight_lib/component/abstract.py` & `splight-lib-3.1.1/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/component/exceptions.py` & `splight-lib-3.1.1/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/component/log_streamer.py` & `splight-lib-3.1.1/splight_lib/component/log_streamer.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/component/spec.py` & `splight-lib-3.1.1/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/encryption.py` & `splight-lib-3.1.1/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/execution.py` & `splight-lib-3.1.1/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/logging/_internal.py` & `splight-lib-3.1.1/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/logging/component.py` & `splight-lib-3.1.1/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/logging/logging.py` & `splight-lib-3.1.1/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/__init__.py` & `splight-lib-3.1.1/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/alert.py` & `splight-lib-3.1.1/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/asset.py` & `splight-lib-3.1.1/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/base.py` & `splight-lib-3.1.1/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/communication.py` & `splight-lib-3.1.1/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/component.py` & `splight-lib-3.1.1/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/dashboard.py` & `splight-lib-3.1.1/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/data_address.py` & `splight-lib-3.1.1/splight_lib/models/data_address.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/event.py` & `splight-lib-3.1.1/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/file.py` & `splight-lib-3.1.1/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/hub.py` & `splight-lib-3.1.1/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/native.py` & `splight-lib-3.1.1/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/query.py` & `splight-lib-3.1.1/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/models/setpoint.py` & `splight-lib-3.1.1/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/restclient/client.py` & `splight-lib-3.1.1/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/restclient/exceptions.py` & `splight-lib-3.1.1/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/restclient/types.py` & `splight-lib-3.1.1/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/settings.py` & `splight-lib-3.1.1/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/testing/__init__.py` & `splight-lib-3.1.1/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/utils/custom_model.py` & `splight-lib-3.1.1/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/utils/hub.py` & `splight-lib-3.1.1/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib/webhook.py` & `splight-lib-3.1.1/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.1.1/splight_lib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.0/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.1.1/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0/splight_lib.egg-info/requires.txt` & `splight-lib-3.1.1/splight_lib.egg-info/requires.txt`

 * *Files identical despite different names*

