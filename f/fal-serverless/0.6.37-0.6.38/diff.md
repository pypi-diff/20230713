# Comparing `tmp/fal_serverless-0.6.37.tar.gz` & `tmp/fal_serverless-0.6.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.37.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.38.tar", max compression
```

## Comparing `fal_serverless-0.6.37.tar` & `fal_serverless-0.6.38.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      866 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/README.md
--rw-r--r--   0        0        0      151 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/__init__.py
--rw-r--r--   0        0        0       47 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
--rw-r--r--   0        0        0     4833 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
--rw-r--r--   0        0        0     4182 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/delete.py
--rw-r--r--   0        0        0     4176 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/download.py
--rw-r--r--   0        0        0     5184 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/file_exists.py
--rw-r--r--   0        0        0     4558 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/list_directory.py
--rw-r--r--   0        0        0     4247 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/list_root.py
--rw-r--r--   0        0        0     4736 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/upload_from_url.py
--rw-r--r--   0        0        0     5735 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
--rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/__init__.py
--rw-r--r--   0        0        0     3974 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/create_key.py
--rw-r--r--   0        0        0     4102 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/delete_key.py
--rw-r--r--   0        0        0     4278 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/list_keys.py
--rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/logs/__init__.py
--rw-r--r--   0        0        0     4963 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/logs/list_since.py
--rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/__init__.py
--rw-r--r--   0        0        0     6864 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage.py
--rw-r--r--   0        0        0     4851 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage_details.py
--rw-r--r--   0        0        0     2817 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/client.py
--rw-r--r--   0        0        0      470 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/errors.py
--rw-r--r--   0        0        0      784 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/__init__.py
--rw-r--r--   0        0        0     1980 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
--rw-r--r--   0        0        0     2945 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/file_spec.py
--rw-r--r--   0        0        0     1352 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
--rw-r--r--   0        0        0     2131 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
--rw-r--r--   0        0        0     1713 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/log_entry.py
--rw-r--r--   0        0        0     1574 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/new_user_key.py
--rw-r--r--   0        0        0     1357 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/url_file_upload.py
--rw-r--r--   0        0        0     3558 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/usage_per_machine_type.py
--rw-r--r--   0        0        0     1918 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/usage_run_detail.py
--rw-r--r--   0        0        0     1682 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/user_key_info.py
--rw-r--r--   0        0        0     2091 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
--rw-r--r--   0        0        0       25 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/py.typed
--rw-r--r--   0        0        0      993 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/types.py
--rw-r--r--   0        0        0     1353 2023-07-04 23:01:35.312903 fal_serverless-0.6.37/pyproject.toml
--rw-r--r--   0        0        0      405 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    23138 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2593 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5426 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    15747 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0     5342 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/decorators.py
--rw-r--r--   0        0        0      158 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      684 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0     1209 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/rest_client.py
--rw-r--r--   0        0        0    17370 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     4287 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 fal_serverless-0.6.37/setup.py
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 fal_serverless-0.6.37/PKG-INFO
+-rw-r--r--   0        0        0      866 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/README.md
+-rw-r--r--   0        0        0      151 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
+-rw-r--r--   0        0        0     4833 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
+-rw-r--r--   0        0        0     4182 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/delete.py
+-rw-r--r--   0        0        0     4176 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/download.py
+-rw-r--r--   0        0        0     5184 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/file_exists.py
+-rw-r--r--   0        0        0     4558 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/list_directory.py
+-rw-r--r--   0        0        0     4247 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/list_root.py
+-rw-r--r--   0        0        0     4736 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/upload_from_url.py
+-rw-r--r--   0        0        0     5735 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/__init__.py
+-rw-r--r--   0        0        0     3974 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/create_key.py
+-rw-r--r--   0        0        0     4102 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/delete_key.py
+-rw-r--r--   0        0        0     4278 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/list_keys.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/logs/__init__.py
+-rw-r--r--   0        0        0     4963 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/logs/list_since.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/usage/__init__.py
+-rw-r--r--   0        0        0     6864 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage.py
+-rw-r--r--   0        0        0     4851 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage_details.py
+-rw-r--r--   0        0        0     2817 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/client.py
+-rw-r--r--   0        0        0      470 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/errors.py
+-rw-r--r--   0        0        0      784 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/__init__.py
+-rw-r--r--   0        0        0     1980 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
+-rw-r--r--   0        0        0     2945 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/file_spec.py
+-rw-r--r--   0        0        0     1352 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
+-rw-r--r--   0        0        0     2131 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
+-rw-r--r--   0        0        0     1713 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/log_entry.py
+-rw-r--r--   0        0        0     1574 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/new_user_key.py
+-rw-r--r--   0        0        0     1357 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/url_file_upload.py
+-rw-r--r--   0        0        0     3558 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/usage_per_machine_type.py
+-rw-r--r--   0        0        0     1918 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/usage_run_detail.py
+-rw-r--r--   0        0        0     1682 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/user_key_info.py
+-rw-r--r--   0        0        0     2091 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
+-rw-r--r--   0        0        0       25 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/py.typed
+-rw-r--r--   0        0        0      993 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/types.py
+-rw-r--r--   0        0        0     1354 2023-07-13 00:07:27.881625 fal_serverless-0.6.38/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    23138 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2593 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5426 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    16069 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0     5714 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/decorators.py
+-rw-r--r--   0        0        0      172 2023-07-13 00:07:20.077577 fal_serverless-0.6.38/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-07-13 00:07:08.657506 fal_serverless-0.6.38/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      684 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0     1209 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/rest_client.py
+-rw-r--r--   0        0        0    18209 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     4287 2023-07-13 00:07:08.661507 fal_serverless-0.6.38/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 fal_serverless-0.6.38/setup.py
+-rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 fal_serverless-0.6.38/PKG-INFO
```

### Comparing `fal_serverless-0.6.37/README.md` & `fal_serverless-0.6.38/README.md`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/delete.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/delete.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/download.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/download.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/file_exists.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/file_exists.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/list_directory.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/list_directory.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/list_root.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/list_root.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/upload_from_url.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/upload_from_url.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/create_key.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/create_key.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/delete_key.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/delete_key.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/list_keys.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/keys/list_keys.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/logs/list_since.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/logs/list_since.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage_details.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage_details.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/client.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/client.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/__init__.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/file_spec.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/file_spec.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/hash_check.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/hash_check.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/log_entry.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/log_entry.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/new_user_key.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/new_user_key.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/url_file_upload.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/url_file_upload.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/usage_per_machine_type.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/usage_per_machine_type.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/usage_run_detail.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/usage_run_detail.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/user_key_info.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/user_key_info.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/validation_error.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/types.py` & `fal_serverless-0.6.38/openapi-fal-rest/openapi_fal_rest/types.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/pyproject.toml` & `fal_serverless-0.6.38/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.37"
+version = "0.6.38"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 packages = [
     { include = "fal_serverless", from = "src" },
     { include = "openapi_fal_rest", from = "openapi-fal-rest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 isolate = {version = ">=0.12.2, <1.0", extras = ["build"]}
-isolate-proto = "0.0.33"
+isolate-proto = "^0.0.34"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 grpcio = "^1.50.0"
 dill = ">=0.3.6,<0.3.7"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
```

### Comparing `fal_serverless-0.6.37/src/fal_serverless/api.py` & `fal_serverless-0.6.38/src/fal_serverless/api.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.38/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.38/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.38/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/cli.py` & `fal_serverless-0.6.38/src/fal_serverless/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import grpc
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
 from fal_serverless.logging import get_logger, set_debug_logging
 from fal_serverless.logging.isolate import IsolateLogPrinter
 from fal_serverless.logging.trace import get_tracer
+from fal_serverless.sdk import KeyScope
 from rich.table import Table
 
 DEFAULT_HOST = "api.alpha.fal.ai"
 HOST_ENVVAR = "FAL_HOST"
 
 DEFAULT_PORT = "443"
 PORT_ENVVAR = "FAL_PORT"
@@ -171,36 +172,45 @@
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def key_cli(ctx, host: str, port: str):
     ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
 
 
 @key_cli.command(name="generate")
+@click.option(
+    "--scope",
+    default=None,
+    required=True,
+    type=click.Choice([KeyScope.ADMIN.value, KeyScope.API.value]),
+    help="The privilage scope of the key.",
+)
 @click.pass_obj
-def key_generate(client: sdk.FalServerlessClient):
+def key_generate(client: sdk.FalServerlessClient, scope: KeyScope):
     with client.connect() as connection:
-        result = connection.create_user_key()
+        result = connection.create_user_key(scope)
         print(
-            "Generated key id and key secret.\n"
+            f"Generated key id and key secret, with the scope `{scope}`.\n"
             "This is the only time the secret will be visible.\n"
             "You will need to generate a new key pair if you lose access to this secret."
         )
         print(f"KEY_ID='{result[1]}'\nKEY_SECRET='{result[0]}'")
 
 
 @key_cli.command(name="list")
 @click.pass_obj
 def key_list(client: sdk.FalServerlessClient):
     table = Table(title="Keys")
     table.add_column("Key ID")
     table.add_column("Created At")
+    table.add_column("Scope")
+
     with client.connect() as connection:
         keys = connection.list_user_keys()
         for key in keys:
-            table.add_row(key.key_id, str(key.created_at))
+            table.add_row(key.key_id, str(key.created_at), str(key.scope.value))
 
     console.print(table)
 
 
 @key_cli.command(name="revoke")
 @click.argument("key_id", required=True)
 @click.pass_obj
```

### Comparing `fal_serverless-0.6.37/src/fal_serverless/decorators.py` & `fal_serverless-0.6.38/src/fal_serverless/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,23 +140,29 @@
         checksum_sha256,
         checksum_md5,
         force=force,
         # isolated configs
         requirements=["urllib3"],
     )
     def download():
-        from urllib.request import urlretrieve
+        from shutil import copyfileobj
+        from urllib.request import Request, urlopen
 
         print(f"Downloading {url} to {check_path}")
 
         # Make sure the directory exists
         check_path.parent.mkdir(parents=True, exist_ok=True)
 
         try:
-            urlretrieve(url, check_path)
+            # TODO: how can we randomize the user agent to avoid being blocked?
+            user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.8; rv:21.0) Gecko/20100101 Firefox/21.0"
+
+            req = Request(url, headers={"User-Agent": user_agent})
+            with urlopen(req) as response, check_path.open("wb") as f:
+                copyfileobj(response, f)
         except Exception as e:
             # raise exception in generally-available class
             raise FileNotFoundError(
                 f"Failed to download {url} to {check_path}\n{e}"
             ) from None
 
     return download()
```

### Comparing `fal_serverless-0.6.37/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.38/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.38/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/flags.py` & `fal_serverless-0.6.38/src/fal_serverless/flags.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.38/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.38/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.38/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.38/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.38/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/rest_client.py` & `fal_serverless-0.6.38/src/fal_serverless/rest_client.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/src/fal_serverless/sdk.py` & `fal_serverless-0.6.38/src/fal_serverless/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import enum
 import os
 from contextlib import ExitStack
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from enum import Enum
 from typing import Any, Callable, Generic, Iterator, Literal, TypeVar
 
@@ -222,26 +223,46 @@
     application_id: str
 
 
 @dataclass
 class UserKeyInfo:
     key_id: str
     created_at: datetime
+    scope: KeyScope
 
 
 @dataclass
 class WorkerStatus:
     worker_id: str
     start_time: datetime
     end_time: datetime
     duration: timedelta
     user_id: str
     machine_type: str
 
 
+class KeyScope(enum.Enum):
+    ADMIN = "ADMIN"
+    API = "API"
+
+    @staticmethod
+    def from_proto(
+        proto: isolate_proto.CreateUserKeyRequest.Scope.ValueType | None,
+    ) -> KeyScope:
+        if proto is None:
+            return KeyScope.API
+
+        if proto is isolate_proto.CreateUserKeyRequest.Scope.ADMIN:
+            return KeyScope.ADMIN
+        elif proto is isolate_proto.CreateUserKeyRequest.Scope.API:
+            return KeyScope.API
+        else:
+            raise ValueError(f"Unknown KeyScope: {proto}")
+
+
 @from_grpc.register(isolate_proto.RegisterCronResult)
 def _from_grpc_register_cron_result(
     message: isolate_proto.RegisterCronResult,
 ) -> RegisterCronResult:
     return RegisterCronResult(
         result=RegisterCronResultType(message.result.cron_id),
     )
@@ -354,26 +375,33 @@
         channel = self._stack.enter_context(
             grpc.secure_channel(self.hostname, channel_creds, options)
         )
         channel = grpc.intercept_channel(channel, TraceContextInterceptor())
         self._stub = isolate_proto.IsolateControllerStub(channel)
         return self._stub
 
-    def create_user_key(self) -> tuple[str, str]:
-        request = isolate_proto.CreateUserKeyRequest()
+    def create_user_key(self, scope: KeyScope) -> tuple[str, str]:
+        scope_proto = (
+            isolate_proto.CreateUserKeyRequest.Scope.ADMIN
+            if scope is KeyScope.ADMIN
+            else isolate_proto.CreateUserKeyRequest.Scope.API
+        )
+
+        request = isolate_proto.CreateUserKeyRequest(scope=scope_proto)
         response = self.stub.CreateUserKey(request)
         return response.key_secret, response.key_id
 
     def list_user_keys(self) -> list[UserKeyInfo]:
         request = isolate_proto.ListUserKeysRequest()
         response: isolate_proto.ListUserKeysResponse = self.stub.ListUserKeys(request)
         return [
             UserKeyInfo(
                 key.key_id,
                 isolate_proto.datetime_from_timestamp(key.created_at),
+                KeyScope.from_proto(key.scope),
             )
             for key in response.user_keys
         ]
 
     def revoke_user_key(self, key_id) -> None:
         request = isolate_proto.RevokeUserKeyRequest(key_id=key_id)
         self.stub.RevokeUserKey(request)
@@ -518,15 +546,14 @@
         )
         response = self.stub.GetActivationLogs(request)
         return [from_grpc(log) for log in response.logs]
 
     def get_logs(
         self, lines: int | None = None, url: str | None = None
     ) -> Iterator[Log]:
-
         filter = isolate_proto.LogsFilter(lines=lines, url=url)
         request = isolate_proto.GetLogsRequest(filter=filter)
         for partial_result in self.stub.GetLogs(request):
             yield from_grpc(partial_result.log_entry)
 
     def list_worker_status(self, user_id: str | None = None) -> list[WorkerStatus]:
         request = isolate_proto.WorkerStatusListRequest(user_id=user_id)
```

### Comparing `fal_serverless-0.6.37/src/fal_serverless/sync.py` & `fal_serverless-0.6.38/src/fal_serverless/sync.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.37/setup.py` & `fal_serverless-0.6.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client==2.12.0',
  'dill>=0.3.6,<0.3.7',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
  'httpx>=0.15.4,<0.25.0',
- 'isolate-proto==0.0.33',
+ 'isolate-proto>=0.0.34,<0.0.35',
  'isolate[build]>=0.12.2,<1.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'packaging>=21.3',
  'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'python-dateutil>=2.8.0,<3.0.0',
@@ -56,15 +56,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.37',
+    'version': '0.6.38',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n\n## Generate OpenAPI client for the REST API\n\nThe recommended way is to use bop. First set the `FAL_REST` variable to the right value and then run:\n\n```sh\nbop openapi\n```\n\nInitial client was generated using\n\n```sh\ncd projects/fal_serverless\n# Notice that you can point to any environment\nopenapi-python-client generate --url https://rest.shark.fal.ai/openapi.json --meta none --config openapi_rest.config.yaml\n```\n\nAnd can be manually updated with\n\n```sh\ncd projects/fal_serverless\n# Notice that you can point to any environment\nopenapi-python-client update --url https://rest.shark.fal.ai/openapi.json --meta none --config openapi_rest.config.yaml\n```\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.37/PKG-INFO` & `fal_serverless-0.6.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.37
+Version: 0.6.38
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (==2.12.0)
 Requires-Dist: dill (>=0.3.6,<0.3.7)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: httpx (>=0.15.4,<0.25.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (==0.0.33)
+Requires-Dist: isolate-proto (>=0.0.34,<0.0.35)
 Requires-Dist: isolate[build] (>=0.12.2,<1.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
```

