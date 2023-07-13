# Comparing `tmp/splight-lib-3.0.9.tar.gz` & `tmp/splight-lib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.0.9.tar", last modified: Fri Jul  7 20:18:31 2023, max compression
+gzip compressed data, was "splight-lib-3.1.0.tar", last modified: Thu Jul 13 12:23:19 2023, max compression
```

## Comparing `splight-lib-3.0.9.tar` & `splight-lib-3.1.0.tar`

### file list

```diff
@@ -1,99 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.582531 splight-lib-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.000000 splight-lib-3.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 20:18:31.582531 splight-lib-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 20:18:31.000000 splight-lib-3.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:18:31.582531 splight-lib-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 20:18:31.000000 splight-lib-3.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.562531 splight-lib-3.0.9/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.562531 splight-lib-3.0.9/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.562531 splight-lib-3.0.9/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.562531 splight-lib-3.0.9/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.566531 splight-lib-3.0.9/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.570531 splight-lib-3.0.9/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.570531 splight-lib-3.0.9/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.570531 splight-lib-3.0.9/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.570531 splight-lib-3.0.9/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.570531 splight-lib-3.0.9/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.574531 splight-lib-3.0.9/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.582531 splight-lib-3.0.9/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.582531 splight-lib-3.0.9/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.582531 splight-lib-3.0.9/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.582531 splight-lib-3.0.9/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:18:31.562531 splight-lib-3.0.9/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 20:18:31.000000 splight-lib-3.0.9/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 12:23:19.650537 splight-lib-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-13 12:23:18.000000 splight-lib-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:23:19.650537 splight-lib-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 12:23:18.000000 splight-lib-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/grpc/reflector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/log_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/data_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.650537 splight-lib-3.1.0/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 12:23:18.000000 splight-lib-3.1.0/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:23:19.646537 splight-lib-3.1.0/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 12:23:19.000000 splight-lib-3.1.0/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.0.9/PKG-INFO` & `splight-lib-3.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.9
+Version: 3.1.0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.9/setup.py` & `splight-lib-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.0.9",
+    version="3.1.0",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.0.9/splight_lib/abstract/client.py` & `splight-lib-3.1.0/splight_lib/abstract/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,18 @@
         if hasattr(self._client, self._count_func):
             return getattr(self._client, self._count_func)(
                 *self._args, **self._kwargs
             )
 
         return len(self.data)
 
+    def first(self):
+        result = self[:1]
+        return result[0] if result else None
+
     def count(self):
         return len(self)
 
     @property
     def data(self):
         if self._cached_results is empty:
             client_func = getattr(self._client, self._client_func)
```

### Comparing `splight-lib-3.0.9/splight_lib/auth/mac_auth.py` & `splight-lib-3.1.0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/communication/abstract.py` & `splight-lib-3.1.0/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/communication/remote_client.py` & `splight-lib-3.1.0/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/database/abstract.py` & `splight-lib-3.1.0/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/database/builder.py` & `splight-lib-3.1.0/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/database/classmap.py` & `splight-lib-3.1.0/splight_lib/client/database/classmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     "alert": f"{ENGINE_PREFIX}/alert/alerts/",
     "asset": f"{ENGINE_PREFIX}/assets/",
     "attribute": f"{ENGINE_PREFIX}/attributes/",
     "chart": f"{ENGINE_PREFIX}/dashboard/charts/",
     "chartitem": f"{ENGINE_PREFIX}/dashboard/chartitems/",
     "component": f"{ENGINE_PREFIX}/component/components/",
     "componentobject": f"{ENGINE_PREFIX}/component/objects/",
+    "routineobject": f"{ENGINE_PREFIX}/component/routines/",
     "dashboard": f"{ENGINE_PREFIX}/dashboard/dashboards/",
     "file": f"{ENGINE_PREFIX}/files/",
     "filter": f"{ENGINE_PREFIX}/dashboard/filters/",
     "query": f"{ENGINE_PREFIX}/queries/",
     "secret": f"{ENGINE_PREFIX}/secrets/",
     "setpoint": f"{ENGINE_PREFIX}/setpoints/",
     "tab": f"{ENGINE_PREFIX}/dashboard/tabs/",
```

### Comparing `splight-lib-3.0.9/splight_lib/client/database/local_client.py` & `splight-lib-3.1.0/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/database/remote_client.py` & `splight-lib-3.1.0/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/datalake/abstract.py` & `splight-lib-3.1.0/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/datalake/builder.py` & `splight-lib-3.1.0/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/datalake/local_client.py` & `splight-lib-3.1.0/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.1.0/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/exceptions.py` & `splight-lib-3.1.0/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/file_handler.py` & `splight-lib-3.1.0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/filter.py` & `splight-lib-3.1.0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/hub/abstract.py` & `splight-lib-3.1.0/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/client/hub/client.py` & `splight-lib-3.1.0/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/communication/event_handler.py` & `splight-lib-3.1.0/splight_lib/communication/event_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.models.base import SplightDatabaseBaseModel
 from splight_lib.models.component import (
     DB_MODEL_TYPE_MAPPING,
     Command,
     ComponentObject,
     ComponentObjectInstance,
+    RoutineObject,
+    RoutineObjectInstance,
     get_field_value,
 )
 from splight_lib.models.event import (
     CommunicationEvent,
     ComponentCommand,
     ComponentCommandStatus,
     ComponentCommandTriggerEvent,
@@ -31,14 +33,18 @@
     pass
 
 
 class InvalidSetPointResponse(Exception):
     pass
 
 
+class InvalidBidingObject(Exception):
+    pass
+
+
 def database_object_event_handler(
     binding_function: Callable,
     binding_object_type: Type[SplightDatabaseBaseModel],
     event_str: str,
 ):
     """General handler for database events used for Component Bindings.
 
@@ -49,28 +55,40 @@
     binding_object_type: Type[SplightDatabaseBaseModel]
         The class for the object associated with the binding event.
     event_str:
         The raw event string from pusher client.
     """
     try:
         logger.info(
-            "Binding for native object of type %s triggered.",
-            binding_object_type,
+            f"Binding for object of type {binding_object_type} triggered.",
             tags=LogTags.BINDING,
         )
         event = CommunicationEvent.parse_raw(event_str)
         if binding_object_type in DB_MODEL_TYPE_MAPPING.values():
             # Case in which is not a ComponentObject
             handler_arg = binding_object_type.parse_obj(event.data)
-        else:
+        elif issubclass(binding_object_type, ComponentObjectInstance):
             # Case for data represents a ComponentObject
             component_obj = ComponentObject.parse_obj(event.data)
-            handler_arg = ComponentObjectInstance.from_component_object(
+            model_class = ComponentObjectInstance.from_object(
                 component_obj
             )
+            handler_arg = model_class.parse_object(component_obj)
+        elif issubclass(binding_object_type, RoutineObjectInstance):
+            # Case for data represents a RoutineObject
+            routine_obj = RoutineObject.parse_obj(event.data)
+            model_class = RoutineObjectInstance.from_object(
+                component_obj
+            )
+            handler_arg = model_class.parse_object(routine_obj)
+        else:
+            raise InvalidBidingObject(
+                f"Invalid binding object type: {binding_object_type}"
+            )
+
         binding_function(handler_arg)
     except Exception as exc:
         logger.error(
             "Error while handling native object trigger: %s",
             exc,
             exc_info=True,
             tags=LogTags.BINDING,
```

### Comparing `splight-lib-3.0.9/splight_lib/component/abstract.py` & `splight-lib-3.1.0/splight_lib/component/abstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import os
 import sys
 from functools import partial
 from tempfile import NamedTemporaryFile
-from threading import Thread
 from time import sleep
 from typing import Dict, List, Optional, Type
 
 from furl import furl
 from pydantic import BaseModel, create_model
 from retry import retry
 from splight_lib.auth import SplightAuthToken
 
 # TODO: Use builder pattern
+from splight_lib.execution import Thread
 from splight_lib.client.communication import RemoteCommunicationClient
 from splight_lib.communication.event_handler import (
     command_event_handler,
     database_object_event_handler,
     setpoint_event_handler,
 )
 from splight_lib.component.exceptions import (
     DuplicatedComponentException,
     InvalidBidingObject,
     MissingBindingCallback,
+    MissingRoutineCallback,
     MissingCommandCallback,
     MissingSetPointCallback,
 )
 from splight_lib.component.spec import Spec
 from splight_lib.execution import ExecutionClient
 from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.models.component import (
     DB_MODEL_TYPE_MAPPING,
     Binding,
     Command,
     ComponentObjectInstance,
+    Routine,
+    RoutineObject,
+    RoutineObjectInstance,
 )
 from splight_lib.models.event import EventNames
 from splight_lib.models.setpoint import SetPoint
 from splight_lib.restclient import (
     ConnectError,
     HTTPError,
     SplightRestClient,
@@ -106,66 +110,84 @@
             access_id=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
             instance_id=component_id,
         )
         self._execution_engine = ExecutionClient()
         health_check = HealthCheckProcessor(self._execution_engine)
         self._health_check_thread = Thread(
-            target=health_check.start, args=(), daemon=True
+            target=health_check.start, args=()
         )
         self._execution_engine.start(self._health_check_thread)
 
         self._spec = self._load_spec()
         self._input = self._spec.component_input(component_id)
         self._output = self._spec.get_output_models(component_id)
 
         component_objects = {
             ct.name: ComponentObjectInstance.from_custom_type(
                 ct, component_id=component_id
             )
             for ct in self._spec.custom_types
         }
+        routines_objects = {
+            routine.name: RoutineObjectInstance.from_routine(
+                routine, component_id=self._component_id
+            )
+            for routine in self._spec.routines
+        }
 
         bindings = [
             binding
             for binding in self._spec.bindings
             if binding.object_type != "SetPoint"
         ]
         setpoints = [
             binding
             for binding in self._spec.bindings
             if binding.object_type == "SetPoint"
         ]
         self._load_bindings(bindings, component_objects)
         self._load_setpoints(setpoints)
+        self._load_routines(self._spec.routines, routines_objects)
         self._load_commands(self._spec.commands)
         self._custom_types = self._get_custom_type_model(component_objects)
+        self._routines = self._get_routine_model(routines_objects)
 
     @property
     def input(self) -> BaseModel:
         return self._input
 
     @property
     def output(self) -> BaseModel:
         return self._output
 
     @property
+    def routines(self) -> Type:
+        return self._routines
+
+    @property
     def custom_types(self) -> BaseModel:
         return self._custom_types
 
     @property
     def execution_engine(self) -> ExecutionClient:
         return self._execution_engine
 
     def _get_custom_type_model(
         self, component_object: Dict[str, Type[ComponentObjectInstance]]
-    ):
+    ) -> BaseModel:
         custom_type_model = create_model("CustomTypes", **component_object)
         return custom_type_model()
 
+    def _get_routine_model(
+        self, routine_object: Dict[str, Type[RoutineObjectInstance]]
+    ) -> BaseModel:
+        custom_type_model = create_model("CustomTypes", **routine_object)
+        return custom_type_model()
+
     def _load_spec(self) -> Spec:
         """Loads the spec.json files located at the same level that the
         main file.
         """
         base_path = os.getcwd()
         spec = Spec.from_file(os.path.join(base_path, "spec.json"))
         return spec
@@ -178,31 +200,64 @@
         """Loads and assigns callbacks for the bindings."""
         for binding in bindings:
             type_ = binding.object_type
             model_class = DB_MODEL_TYPE_MAPPING.get(
                 type_, component_objects.get(type_)
             )
             if not model_class:
-                raise InvalidBidingObject(model_class.__class__.__name__)
+                raise InvalidBidingObject(model_class.__name__)
             event_name = model_class.get_event_name(
-                model_class.__class__.__name__, binding.object_action
+                model_class.__name__, binding.object_action
             )
             callback_func = getattr(self, binding.name, None)
             if not callback_func:
                 raise MissingBindingCallback(binding.name)
 
             self._comm_client.bind(
                 event_name,
                 partial(
                     database_object_event_handler,
                     callback_func,
                     model_class,
                 ),
             )
 
+    def _load_routines(
+        self,
+        routines: List[Routine],
+        routines_objects: Dict[str, Type[RoutineObjectInstance]],
+    ) -> None:
+        """Loads and assigns callbacks to the routines."""
+
+        actions = ["create", "update", "delete"]
+        for routine in routines:
+            model_calss = routines_objects.get(routine.name)
+
+            for action in actions:
+
+                event_name = RoutineObject.get_event_name(
+                    model_calss .__name__, action
+                )
+
+                callback_func = getattr(
+                    self,
+                    getattr(routine, f"{action}_handler"),
+                    None
+                )
+                if not callback_func:
+                    raise MissingRoutineCallback(routine.name, action)
+                self._comm_client.bind(
+                    event_name,
+                    partial(
+                        database_object_event_handler,
+                        callback_func,
+                        model_calss
+                    ),
+                )
+
     def _load_setpoints(self, setpoints: List[SetPoint]):
         """Loads and assigns callbacks to the setpoing."""
         for setpoint in setpoints:
             event_name = SetPoint.get_event_name(
                 SetPoint.__name__, setpoint.object_action
             )
             callback_func = getattr(self, setpoint.name, None)
```

### Comparing `splight-lib-3.0.9/splight_lib/component/exceptions.py` & `splight-lib-3.1.0/splight_lib/component/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
 class MissingBindingCallback(Exception):
     def __init__(self, binding_name: str):
         msg = f"Missing method {binding_name} associated with a Binding"
         super().__init__(msg)
 
 
+class MissingRoutineCallback(Exception):
+    def __init__(self, routine_name: str, action: str):
+        msg = f"Missing method associated with a Routine: {routine_name} {action}_handler event"
+        super().__init__(msg)
+
+
 class InvalidBidingObject(Exception):
     def __init__(self, model_name: str):
         msg = f"Model {model_name} is not a valid model for a binding"
         super().__init__(msg)
 
 
 class MissingSetPointCallback(Exception):
```

### Comparing `splight-lib-3.0.9/splight_lib/component/spec.py` & `splight-lib-3.1.0/splight_lib/component/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     ComponentObjectInstance,
     ComponentType,
     CustomType,
     Endpoint,
     InputParameter,
     Output,
     PrivacyPolicy,
+    Routine,
     get_field_value,
 )
 from splight_lib.utils.custom_model import create_custom_model
 
 VALID_PARAMETER_VALUES = {
     "int": int,
     "bool": bool,
@@ -81,14 +82,15 @@
     privacy_policy: PrivacyPolicy = PrivacyPolicy.PUBLIC
     tags: Set[str] = set()
     component_type: ComponentType = ComponentType.CONNECTOR
     custom_types: List[CustomType] = []
     input: List[InputParameter] = []
     output: List[Output] = []
     bindings: List[Binding] = []
+    routines: List[Routine] = []
     commands: List[Command] = []
     endpoints: List[Endpoint] = []
 
     @validator("custom_types")
     def validate_custom_types(
         cls, custom_types: List[CustomType]
     ) -> List[CustomType]:
```

### Comparing `splight-lib-3.0.9/splight_lib/encryption.py` & `splight-lib-3.1.0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/execution.py` & `splight-lib-3.1.0/splight_lib/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,17 @@
         return
 
     def _start_task(self, job: Task) -> None:
         logger.debug("Starting Task", tags=LogTags.RUNTIME)
         if not getattr(self, "_scheduler", None):
             # Instantiate and start Scheduler thread
             self._scheduler = Scheduler()
-            self._start_thread(Thread(target=self._scheduler.start))
+            self._start_thread(
+                Thread(target=self._scheduler.start, daemon=False)
+            )
 
         return self._scheduler.schedule(job)
 
     def _stop_task(self, job: Task) -> None:
         logger.debug("Stopping Task", tags=LogTags.RUNTIME)
         return self._scheduler.unschedule(job)
```

### Comparing `splight-lib-3.0.9/splight_lib/logging/_internal.py` & `splight-lib-3.1.0/splight_lib/logging/component.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 import os
-from enum import auto
 from logging import INFO, Formatter, Handler
 from typing import Optional
 
 from concurrent_log_handler import ConcurrentRotatingFileHandler
-from splight_lib.logging.constants import LOGGING_DEV
 from splight_lib.logging.logging import (
-    ElasticDocumentFormatter,
     SplightFormatter,
     SplightLogger,
-    elastic_document_handler,
     standard_output_handler,
 )
-from strenum import UppercaseStrEnum
 
 
-# TODO: add more tags
-class LogTags(UppercaseStrEnum):
-    RUNTIME = auto()
-    BINDING = auto()
-    COMMUNICATION = auto()
-    INDEX = auto()
-    SECRET = auto()
-    HOOK = auto()
-    SETPOINT = auto()
-    COMMAND = auto()
-    PARAMETER = auto()
-    COMPONENT = auto()
-    DATABASE = auto()
-    DATALAKE = auto()
-    CACHE = auto()
-
-
-# don't used now
-def splight_dev_file_handler(
+def component_file_handler(
     formatter: Optional[Formatter] = SplightFormatter(),
     log_level: Optional[str] = INFO,
 ) -> Handler:
-    filename = os.getenv("SPLIGHT_DEVELOPER_LOG_FILE", "/tmp/splight-dev.log")
-    max_bytes = int(os.getenv("SPLIGHT_DEVELOPER_MAX_BYTES", 5e6))  # 5MB
-    backup_count = int(os.getenv("SPLIGHT_DEVELOPER_BACKUP_COUNT", 100))
+    filename = os.getenv("SPLIGHT_COMPONENT_LOG_FILE", "/tmp/components.log")
+    max_bytes = int(os.getenv("SPLIGHT_COMPONENT_MAX_BYTES", 5e6))  # 5MB
+    backup_count = int(os.getenv("SPLIGHT_COMPONENT_BACKUP_COUNT", 100))
 
     handler = ConcurrentRotatingFileHandler(
         filename=filename, maxBytes=max_bytes, backupCount=backup_count
     )
     handler.setFormatter(formatter)
     handler.setLevel(log_level)
     return handler
 
 
-def get_splight_logger(name: Optional[str] = None):
-    """Stdout logger."""
+def get_component_logger(name: Optional[str] = None):
+    """Stdout and file logger."""
     if name is None:
-        name = "splight-dev"
+        name = "component"
     logger = SplightLogger(name=name)
     logger.propagate = False
     stdout_handler = standard_output_handler(log_level=logger.level)
     logger.addHandler(stdout_handler)
-    es_handler = elastic_document_handler(
-        formatter=ElasticDocumentFormatter(type=LOGGING_DEV),
-        log_level=logger.level,
-    )
-    logger.addHandler(es_handler)
+    file_handler = component_file_handler(log_level=logger.level)
+    logger.addHandler(file_handler)
+
     # Add logger.level to root logger
     logger.setLevel(logger.level)
     return logger
+
+
+def getLogger(name: Optional[str] = None):
+    return get_component_logger(name)
```

### Comparing `splight-lib-3.0.9/splight_lib/logging/logging.py` & `splight-lib-3.1.0/splight_lib/logging/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-import json
+import time
 import os
 import sys
-import time
 from logging import (
     CRITICAL,
     DEBUG,
     ERROR,
     INFO,
-    NOTSET,
     WARNING,
     Formatter,
     Handler,
     Logger,
     StreamHandler,
 )
 from logging import root as rootLogger
-from typing import Dict, Literal, Optional
-
-from concurrent_log_handler import ConcurrentRotatingFileHandler
-from pydantic import BaseSettings
-from splight_lib.logging.constants import LOGGING_DEV, LogType
+from typing import Dict, Optional
 
 TAGS_KEY = "tags"
 
 
 class SplightFormatter(Formatter):
     DEFAULT_FMT: str = (
         "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
@@ -32,34 +26,19 @@
     def format(self, record):
         fmt = self.DEFAULT_FMT
         try:
             if record.tags is not None:
                 fmt = " | ".join([fmt, "%(tags)s"])
         except AttributeError:
             pass  # tags aren't present
-        formatter = Formatter(fmt=fmt)
+        formatter = Formatter(fmt=fmt, datefmt="%Y-%m-%dT%H:%M:%SZ")
         formatter.converter = time.gmtime
         return formatter.format(record)
 
 
-class ElasticDocumentFormatter(Formatter):
-    def __init__(self, fmt: str = None, type: LogType = LOGGING_DEV) -> None:
-        super().__init__(fmt=fmt)
-        self.type = type
-
-    @property
-    def _extra_fields(self) -> Dict:
-        return {
-            "type": self.type,
-        }
-
-    def format(self, record):
-        return json.dumps({**record.__dict__, **self._extra_fields})
-
-
 class SplightLogger(Logger):
     def __init__(self, name: str = None) -> None:
         # this is to avoid adding handlers to root logger
         # and interfering with third party app logs
         self.name = name if name is not None else "splight"
         level = int(os.getenv("LOG_LEVEL", INFO))
         super().__init__(name, level)
@@ -161,34 +140,7 @@
     formatter: Optional[Formatter] = SplightFormatter(),
     log_level: Optional[str] = INFO,
 ) -> Handler:
     handler = StreamHandler(sys.stdout)
     handler.setFormatter(formatter)
     handler.setLevel(log_level)
     return handler
-
-
-class ElasticDocumentHandlerSettings(BaseSettings):
-    splight_elastic_logs_filename: str = "/tmp/splight_elastic_logs.log"
-    splight_elastic_logs_max_bytes: int = 5e6
-    splight_elastic_logs_backup_count: int = 5
-
-    @property
-    def file_handler_settings(self) -> Dict:
-        return {
-            "filename": self.splight_elastic_logs_filename,
-            "maxBytes": self.splight_elastic_logs_max_bytes,
-            "backupCount": self.splight_elastic_logs_backup_count,
-            "encoding": "utf-8",
-        }
-
-
-def elastic_document_handler(
-    formatter: Optional[Formatter] = SplightFormatter(),
-    log_level: Optional[str] = INFO,
-) -> Handler:
-    settings = ElasticDocumentHandlerSettings()
-    handler = ConcurrentRotatingFileHandler(**settings.file_handler_settings)
-
-    handler.setFormatter(formatter)
-    handler.setLevel(log_level)
-    return handler
```

### Comparing `splight-lib-3.0.9/splight_lib/models/__init__.py` & `splight-lib-3.1.0/splight_lib/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from splight_lib.models.alert import Alert, AlertCondition
 from splight_lib.models.asset import Asset
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.component import (
     Component,
     ComponentObject,
+    RoutineObject,
     ComponentObjectInstance,
+    RoutineObjectInstance,
 )
 from splight_lib.models.dashboard import Dashboard, Tab, Chart, ChartItem, Filter, AdvancedFilter
 from splight_lib.models.file import File
 from splight_lib.models.hub import HubComponent, HubComponentVersion
 from splight_lib.models.native import Boolean, Number, String
 from splight_lib.models.query import Query
 from splight_lib.models.secret import Secret
```

### Comparing `splight-lib-3.0.9/splight_lib/models/alert.py` & `splight-lib-3.1.0/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/asset.py` & `splight-lib-3.1.0/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/base.py` & `splight-lib-3.1.0/splight_lib/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,18 +78,14 @@
     instance_type: Optional[str] = None
     _collection_name: ClassVar[str] = "DatalakeModel"
     _dl_client: AbstractDatalakeClient = PrivateAttr()
 
     class Config:
         json_dumps = datalake_model_serializer
 
-    def __init__(self, **data):
-        super().__init__(**data)
-        self._dl_client = self.__get_datalake_client()
-
     @classmethod
     def get(cls, **params: Dict) -> List["SplightDatalakeBaseModel"]:
         dl_client = cls.__get_datalake_client()
         instances = dl_client.get(
             resource_name=cls.__name__,
             collection=cls._collection_name,
             **params,
@@ -104,15 +100,16 @@
             resource_name=cls.__name__,
             collection=cls._collection_name,
             **params,
         )
         return df
 
     def save(self):
-        self._dl_client.save(
+        dl_client = self.__get_datalake_client()
+        dl_client.save(
             collection=self._collection_name,
             instances=json.loads(self.json()),
         )
 
     @classmethod
     def save_dataframe(cls, dataframe: pd.DataFrame):
         dl_client = cls.__get_datalake_client()
```

### Comparing `splight-lib-3.0.9/splight_lib/models/communication.py` & `splight-lib-3.1.0/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/dashboard.py` & `splight-lib-3.1.0/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/event.py` & `splight-lib-3.1.0/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/file.py` & `splight-lib-3.1.0/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/hub.py` & `splight-lib-3.1.0/splight_lib/models/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 
 import py7zr
 from pydantic import BaseModel, PrivateAttr, validator
 from splight_lib.client.hub.abstract import AbstractHubClient
 from splight_lib.client.hub.client import SplightHubClient
 from splight_lib.models.component import (
     Binding,
+    CustomType,
     Command,
     ComponentType,
     Endpoint,
     InputParameter,
     Output,
+    CustomType,
+    Routine
 )
 from splight_lib.settings import settings
 from splight_lib.utils.hub import (
     COMPRESSION_TYPE,
     README_FILE_1,
     README_FILE_2,
     get_ignore_pathspec,
@@ -51,16 +54,19 @@
     verification: Optional[str]
     created_at: Optional[str]
     last_modified: Optional[str]
     tags: List[str] = []
     min_component_capacity: Optional[str]
     usage_count: int = 0
 
+    custom_types: List[CustomType] = []
     input: List[InputParameter] = []
     output: List[Output] = []
+    routines: List[Routine] = []
+    custom_types: List[CustomType] = []
     commands: List[Command] = []
     endpoints: List[Endpoint] = []
     bindings: List[Binding] = []
 
     _hub_client: AbstractHubClient = PrivateAttr()
 
     def __init__(self, *args, **kwargs):
@@ -164,34 +170,31 @@
         with py7zr.SevenZipFile(file_name, "w") as archive:
             all_files = glob(f"{path}/**", recursive=True)
             for filepath in all_files:
                 if ignore_pathspec and ignore_pathspec.match_file(filepath):
                     continue
                 if os.path.isdir(filepath):
                     continue
-                filename = os.path.basename(filepath)
-                new_filepath = os.path.join(versioned_path, filename)
+                rel_filename = os.path.relpath(filepath, path)
+                new_filepath = os.path.join(versioned_path, rel_filename)
                 archive.write(filepath, new_filepath)
 
-        data = {
-            "name": name,
-            "version": version,
-            "splight_cli_version": spec["splight_cli_version"],
-            "privacy_policy": spec.get("privacy_policy", "private"),
-            "tags": spec.get("tags", []),
-            "custom_types": json.dumps(spec.get("custom_types", [])),
-            "input": json.dumps(spec.get("input", [])),
-            "output": json.dumps(spec.get("output", [])),
-            "component_type": spec.get(
-                "component_type", ComponentType.CONNECTOR.value
-            ),
-            "commands": json.dumps(spec.get("commands", [])),
-            "bindings": json.dumps(spec.get("bindings", [])),
-            "endpoints": json.dumps(spec.get("endpoints", [])),
-        }
+        spec["name"] = name
+        spec["version"] = version
+        spec.setdefault(
+            "component_type", ComponentType.CONNECTOR.value
+        )
+        data_cls = cls.parse_obj(spec)
+
+        data = data_cls.dict(exclude_none=True)
+
+        to_json = ["tags", "routines", "custom_types", "input", "output", "commands", "bindings", "endpoints"]
+        for key in to_json:
+            data[key] = json.dumps(data[key])
+
         files = {
             "file": open(file_name, "rb"),
             "readme": open(readme_path, "rb"),
         }
         try:
             component = hub_client.upload(data=data, files=files)
         except Exception as exc:
```

### Comparing `splight-lib-3.0.9/splight_lib/models/query.py` & `splight-lib-3.1.0/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/models/setpoint.py` & `splight-lib-3.1.0/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/restclient/client.py` & `splight-lib-3.1.0/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/restclient/exceptions.py` & `splight-lib-3.1.0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/restclient/types.py` & `splight-lib-3.1.0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/settings.py` & `splight-lib-3.1.0/splight_lib/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     return config
 
 
 class SplightSettings(BaseSettings, Singleton):
     SPLIGHT_ACCESS_ID: str = ""
     SPLIGHT_SECRET_KEY: str = ""
     SPLIGHT_PLATFORM_API_HOST: str = "https://api.splight-ai.com"
+    SPLIGHT_GRPC_HOST: str = "grpc.splight-ai.com:443"
 
     # Parameters for local environment
     LOCAL_ENVIRONMENT: bool = False
     CURRENT_DIR: Optional[str]
 
     @root_validator(allow_reuse=True)
     def validate_local_environment(cls, values: Dict):
```

### Comparing `splight-lib-3.0.9/splight_lib/testing/__init__.py` & `splight-lib-3.1.0/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/utils/custom_model.py` & `splight-lib-3.1.0/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/utils/hub.py` & `splight-lib-3.1.0/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib/webhook.py` & `splight-lib-3.1.0/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.9/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.1.0/splight_lib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.9
+Version: 3.1.0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.9/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.1.0/splight_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,36 +36,41 @@
 splight_lib/client/database/local_client.py
 splight_lib/client/database/remote_client.py
 splight_lib/client/datalake/__init__.py
 splight_lib/client/datalake/abstract.py
 splight_lib/client/datalake/builder.py
 splight_lib/client/datalake/local_client.py
 splight_lib/client/datalake/remote_client.py
+splight_lib/client/grpc/__init__.py
+splight_lib/client/grpc/client.py
+splight_lib/client/grpc/reflector.py
 splight_lib/client/hub/__init__.py
 splight_lib/client/hub/abstract.py
 splight_lib/client/hub/client.py
 splight_lib/communication/__init__.py
 splight_lib/communication/event_handler.py
 splight_lib/component/__init__.py
 splight_lib/component/abstract.py
 splight_lib/component/exceptions.py
+splight_lib/component/log_streamer.py
 splight_lib/component/spec.py
 splight_lib/logging/__init__.py
 splight_lib/logging/_internal.py
 splight_lib/logging/component.py
 splight_lib/logging/constants.py
 splight_lib/logging/logging.py
 splight_lib/models/__init__.py
 splight_lib/models/alert.py
 splight_lib/models/asset.py
 splight_lib/models/attribute.py
 splight_lib/models/base.py
 splight_lib/models/communication.py
 splight_lib/models/component.py
 splight_lib/models/dashboard.py
+splight_lib/models/data_address.py
 splight_lib/models/event.py
 splight_lib/models/exceptions.py
 splight_lib/models/file.py
 splight_lib/models/hub.py
 splight_lib/models/native.py
 splight_lib/models/query.py
 splight_lib/models/secret.py
```

