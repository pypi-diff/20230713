# Comparing `tmp/ievv-auth-2.0.2.tar.gz` & `tmp/ievv_auth-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ievv-auth-2.0.2.tar", last modified: Tue Apr  5 11:12:55 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ievv-auth-2.0.2.tar` & `ievv_auth-3.0.0.tar`

### file list

```diff
@@ -1,88 +1,60 @@
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.537246 ievv-auth-2.0.2/
--rw-r--r--   0 jimnordal   (501) staff       (20)     1485 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/LICENSE
--rw-r--r--   0 jimnordal   (501) staff       (20)      123 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/MANIFEST.in
--rw-r--r--   0 jimnordal   (501) staff       (20)      572 2022-04-05 11:12:55.536405 ievv-auth-2.0.2/PKG-INFO
--rw-r--r--   0 jimnordal   (501) staff       (20)      893 2022-04-05 11:11:59.000000 ievv-auth-2.0.2/README.md
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.504080 ievv-auth-2.0.2/ievv_auth/
--rw-r--r--   0 jimnordal   (501) staff       (20)      139 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/__init__.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.509766 ievv-auth-2.0.2/ievv_auth/ievv_api_key/
--rw-r--r--   0 jimnordal   (501) staff       (20)     1158 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/README.md
--rw-r--r--   0 jimnordal   (501) staff       (20)       68 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     2408 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/admin.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      107 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/apps.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.510264 ievv-auth-2.0.2/ievv_auth/ievv_api_key/management/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/management/__init__.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.510563 ievv-auth-2.0.2/ievv_auth/ievv_api_key/management/commands/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/management/commands/__init__.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.511994 ievv-auth-2.0.2/ievv_auth/ievv_api_key/migrations/
--rw-r--r--   0 jimnordal   (501) staff       (20)     2282 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/migrations/0001_initial.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      595 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/migrations/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     8070 2022-04-05 11:07:56.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/models.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.512502 ievv-auth-2.0.2/ievv_auth/ievv_api_key/tests/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/tests/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     3610 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/tests/test_models.py
--rw-r--r--   0 jimnordal   (501) staff       (20)       63 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_api_key/views.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.517206 ievv-auth-2.0.2/ievv_auth/ievv_jwt/
--rw-r--r--   0 jimnordal   (501) staff       (20)     2407 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/README.md
--rw-r--r--   0 jimnordal   (501) staff       (20)       61 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)       63 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/admin.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.518634 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     2666 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/authentication.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.519375 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/serializers/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/serializers/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     1311 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.521207 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/views/
--rw-r--r--   0 jimnordal   (501) staff       (20)       64 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/views/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      259 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/views/api_key_views.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      739 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/views/base_view.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      381 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/apps.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.523370 ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      478 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/api_key_backend.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      747 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/backend_registry.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     3283 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/base_backend.py
--rw-r--r--   0 jimnordal   (501) staff       (20)       43 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/exceptions.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.524134 ievv-auth-2.0.2/ievv_auth/ievv_jwt/migrations/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/migrations/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)       57 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/models.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      766 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/settings.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.524618 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/__init__.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.526412 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_api/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_api/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     2979 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     3199 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.528897 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     6585 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     1812 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     3025 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     2235 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_utils.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.531023 ievv-auth-2.0.2/ievv_auth/ievv_jwt/utils/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/utils/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     1012 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/utils/deep_merge.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      897 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/utils/load_settings.py
--rw-r--r--   0 jimnordal   (501) staff       (20)       63 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/ievv_jwt/views.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.531781 ievv-auth-2.0.2/ievv_auth/project/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/__init__.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.532801 ievv-auth-2.0.2/ievv_auth/project/default/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/default/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     3150 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/default/settings.py
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.535242 ievv-auth-2.0.2/ievv_auth/project/develop/
--rw-r--r--   0 jimnordal   (501) staff       (20)        0 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/develop/__init__.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      227 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/develop/common_settings.py
--rw-r--r--   0 jimnordal   (501) staff       (20)       56 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/develop/develop_settings.py
--rw-r--r--   0 jimnordal   (501) staff       (20)      382 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/develop/test_settings.py
--rw-r--r--   0 jimnordal   (501) staff       (20)     1250 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/ievv_auth/project/settingsproxy.py
--rw-r--r--   0 jimnordal   (501) staff       (20)        8 2022-04-05 11:11:22.000000 ievv-auth-2.0.2/ievv_auth/version.json
-drwxr-xr-x   0 jimnordal   (501) staff       (20)        0 2022-04-05 11:12:55.506025 ievv-auth-2.0.2/ievv_auth.egg-info/
--rw-r--r--   0 jimnordal   (501) staff       (20)      572 2022-04-05 11:12:55.000000 ievv-auth-2.0.2/ievv_auth.egg-info/PKG-INFO
--rw-r--r--   0 jimnordal   (501) staff       (20)     2484 2022-04-05 11:12:55.000000 ievv-auth-2.0.2/ievv_auth.egg-info/SOURCES.txt
--rw-r--r--   0 jimnordal   (501) staff       (20)        1 2022-04-05 11:12:55.000000 ievv-auth-2.0.2/ievv_auth.egg-info/dependency_links.txt
--rw-r--r--   0 jimnordal   (501) staff       (20)        1 2022-04-05 11:12:55.000000 ievv-auth-2.0.2/ievv_auth.egg-info/not-zip-safe
--rw-r--r--   0 jimnordal   (501) staff       (20)       66 2022-04-05 11:12:55.000000 ievv-auth-2.0.2/ievv_auth.egg-info/requires.txt
--rw-r--r--   0 jimnordal   (501) staff       (20)       10 2022-04-05 11:12:55.000000 ievv-auth-2.0.2/ievv_auth.egg-info/top_level.txt
--rw-r--r--   0 jimnordal   (501) staff       (20)       38 2022-04-05 11:12:55.537376 ievv-auth-2.0.2/setup.cfg
--rw-r--r--   0 jimnordal   (501) staff       (20)     1004 2022-04-05 10:40:01.000000 ievv-auth-2.0.2/setup.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/__init__.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/version.json
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/README.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/admin.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/apps.py
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/models.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/management/commands/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/tests/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/tests/test_models.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/admin.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/apps.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/exceptions.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/models.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/__init__.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/authentication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/serializers/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/api_key_views.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/base_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/api_key_backend.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/backend_registry.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/base_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/__init__.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/deep_merge.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/load_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/settingsproxy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/default/__init__.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/default/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/common_settings.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/develop_settings.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/test_settings.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/README.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/PKG-INFO
```

### Comparing `ievv-auth-2.0.2/LICENSE` & `ievv_auth-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_api_key/README.md` & `ievv_auth-3.0.0/ievv_auth/ievv_api_key/README.md`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_api_key/admin.py` & `ievv_auth-3.0.0/ievv_auth/ievv_api_key/admin.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_api_key/migrations/0001_initial.py` & `ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py` & `ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_api_key/models.py` & `ievv_auth-3.0.0/ievv_auth/ievv_api_key/models.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_api_key/tests/test_models.py` & `ievv_auth-3.0.0/ievv_auth/ievv_api_key/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/README.md` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/README.md`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/authentication.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/authentication.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/api/views/base_view.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/base_view.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/backend_registry.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/backend_registry.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/backends/base_backend.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/base_backend.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/settings.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/tests/test_utils.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/utils/deep_merge.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/deep_merge.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/ievv_jwt/utils/load_settings.py` & `ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `ievv-auth-2.0.2/ievv_auth/project/default/settings.py` & `ievv_auth-3.0.0/ievv_auth/project/default/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 SECRET_KEY = 'gxha11rjtb_7l6^(mzx-q%=+5qeldh&p$jig0x!*&q&5lq$1j6'
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
+DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
 # Application definition
 
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
@@ -64,15 +65,15 @@
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
             ],
         },
     },
 ]
 
-WSGI_APPLICATION = 'ievv_auth.wsgi.application'
+# WSGI_APPLICATION = 'ievv_auth.wsgi.application'
 
 
 # Database
 # https://docs.djangoproject.com/en/1.11/ref/settings/#databases
 #
 # DATABASES = {
 #     'default': {
```

### Comparing `ievv-auth-2.0.2/ievv_auth/project/settingsproxy.py` & `ievv_auth-3.0.0/ievv_auth/project/settingsproxy.py`

 * *Files identical despite different names*

