# Comparing `tmp/wpp-bavapi-0.5.0.tar.gz` & `tmp/wpp-bavapi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp-bavapi-0.5.0.tar", last modified: Fri Jul  7 17:43:11 2023, max compression
+gzip compressed data, was "wpp-bavapi-0.6.0.tar", last modified: Thu Jul 13 12:47:18 2023, max compression
```

## Comparing `wpp-bavapi-0.5.0.tar` & `wpp-bavapi-0.6.0.tar`

### file list

```diff
@@ -1,92 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.397636 wpp-bavapi-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/BAVAPI Jupyter Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/bavapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/bavapi/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/parsing/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/parsing/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/bavapi/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/reference/_int_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/reference/generate_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/bavapi/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/assets/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/assets/wpp-bav-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/audiences.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/brands.md
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/brandscape-data.md
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/endpoints/studies.md
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/gen_ref_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.401636 wpp-bavapi-0.5.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/getting-started/authentication.md
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/getting-started/reference-classes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/reference/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/usage/advanced.md
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/docs/usage/basic.md
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/integration/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/integration/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/parsing/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/parsing/test_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/tests/reference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/reference/test_generate_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/reference/test_int_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/type_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 17:42:43.000000 wpp-bavapi-0.5.0/type_stubs/nest_asyncio.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:43:11.405636 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 17:43:11.000000 wpp-bavapi-0.5.0/wpp_bavapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.197203 wpp-bavapi-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 12:47:18.197203 wpp-bavapi-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/bavapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/bavapi/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/parsing/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/parsing/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/bavapi/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/reference/_int_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/reference/generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/bavapi/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:47:18.197203 wpp-bavapi-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 12:46:49.000000 wpp-bavapi-0.6.0/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:47:18.193203 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 12:47:18.000000 wpp-bavapi-0.6.0/wpp_bavapi.egg-info/top_level.txt
```

### Comparing `wpp-bavapi-0.5.0/LICENSE` & `wpp-bavapi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/PKG-INFO` & `wpp-bavapi-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://github.com/wppbav/bavapi-sdk-python
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wpp-bavapi-0.5.0/README.md` & `wpp-bavapi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/bavapi/__init__.py` & `wpp-bavapi-0.6.0/bavapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 -------------
 
 >>> import bavapi
 >>> async with bavapi.Client("API_TOKEN") as client:
 ...     result = await client.brands(name="Facebook")
 """
 
-from importlib.metadata import version, PackageNotFoundError
+from importlib.metadata import PackageNotFoundError, version
 
 from bavapi import filters
 from bavapi.client import Client
 from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
 from bavapi.query import Query
 from bavapi.sync import audiences, brands, brandscape_data, raw_query, studies
 
 __all__ = (
-    "raw_query",
     "audiences",
     "brands",
     "brandscape_data",
+    "raw_query",
     "studies",
     "Client",
+    "Query",
+    "filters",
     "APIError",
     "DataNotFoundError",
     "RateLimitExceededError",
-    "Query",
-    "filters",
 )
 
 try:
     __version__ = version(__package__ or __name__)
 except PackageNotFoundError:  # pragma: no cover
-    pass
+    __version__ = "not_found"
```

### Comparing `wpp-bavapi-0.5.0/bavapi/client.py` & `wpp-bavapi-0.6.0/bavapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 from typing import (
     TYPE_CHECKING,
     Final,
     List,
     Literal,
     Optional,
+    Type,
     TypeVar,
     Union,
     overload,
 )
 
 from bavapi import filters as _filters
 from bavapi.http import HTTPClient
 from bavapi.parsing.responses import parse_response
 from bavapi.query import Query
 from bavapi.typing import BaseListOrValues, JSONDict, OptionalListOr
 
 if TYPE_CHECKING:
+    from types import TracebackType
+
     from pandas import DataFrame
 
 __all__ = ("Client",)
 
 BASE_URL: Final[str] = "https://fount.wppbav.com/api/v2/"
 
 F = TypeVar("F", bound=_filters.FountFilters)
@@ -145,16 +148,21 @@
     def per_page(self, value: int) -> None:
         self._client.per_page = value
 
     async def __aenter__(self) -> "Client":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *args, **kwargs):
-        await self._client.__aexit__(*args, **kwargs)
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: "Optional[TracebackType]" = None,
+    ) -> None:
+        await self._client.__aexit__(exc_type, exc_value, traceback)
 
     async def aclose(self) -> None:
         """Close existing HTTP connections."""
         return await self._client.aclose()
 
     async def raw_query(self, endpoint: str, params: Query[F]) -> List[JSONDict]:
         """Perform a raw GET query to the Fount API, returning the response JSON data
```

### Comparing `wpp-bavapi-0.5.0/bavapi/filters.py` & `wpp-bavapi-0.6.0/bavapi/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Filter objects for Fount API queries based on `pydantic`."""
 
 # pylint: disable=no-name-in-module, too-few-public-methods
 
 from typing import Dict, Literal, Mapping, Optional, Type, TypeVar, Union
 
-from pydantic import BaseModel, root_validator, validator
+from pydantic import BaseModel, field_validator, model_validator
 
 from bavapi.parsing.params import parse_date
 from bavapi.typing import (
     DTValues,
     InputParamsMapping,
     InputSequenceOrValues,
     OptionalListOr,
@@ -37,20 +37,20 @@
     updated_since : str, date or datetime, optional
         Request items that have been updated since the specified date, by default None
     **kwargs : str, int or float, or list of str, int or floats, optional
         Any additional filters to apply to the request, including for columns within
         the response data.
     """
 
-    updated_since: DTValues = None
+    # Allow arbitrary filters for compatibility with raw_query
+    model_config = {"extra": "allow"}
 
-    class Config:  #pylint: disable=missing-class-docstring
-        extra = "allow"
+    updated_since: DTValues = None
 
-    @validator("updated_since", pre=True)
+    @field_validator("updated_since", mode="before")
     @classmethod
     def _parse_date(cls, value: DTValues) -> Optional[str]:
         if value is None:
             return value
         return parse_date(value)
 
     @classmethod
@@ -83,15 +83,15 @@
             return cls(**addl_filters)  # type: ignore[arg-type]
 
         new_filters = addl_filters.copy()
 
         if isinstance(filters, Mapping):
             new_filters.update(filters)
         else:
-            new_filters.update(filters.dict(exclude_defaults=True))
+            new_filters.update(filters.model_dump(exclude_defaults=True))
 
         return cls(**new_filters)  # type: ignore[arg-type]
 
 
 class AudiencesFilters(FountFilters):
     """Filters for the `brands` endpoint.
 
@@ -230,15 +230,15 @@
     metric_keys: OptionalListOr[str] = None
     studies: OptionalListOr[int] = None
     countries: OptionalListOr[int] = None
     years: OptionalListOr[int] = None
     brands: OptionalListOr[int] = None
     categories: OptionalListOr[int] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
     def _check_params(cls, values: Dict[str, object]) -> Dict[str, object]:
         if not (
             "brands" in values
             or "brand_name" in values
             or "studies" in values
             or (
@@ -308,13 +308,13 @@
     inactive: Literal[0, 1] = 0
     bav_study: Literal[0, 1] = 0
     data_updated_since: DTValues = None
     years: OptionalListOr[int] = None
     countries: OptionalListOr[int] = None
     regions: OptionalListOr[int] = None
 
-    @validator("data_updated_since", pre=True)
+    @field_validator("data_updated_since", mode="before")
     @classmethod
     def _parse_date(cls, value: DTValues) -> Optional[str]:
         if value is None:
             return value
         return parse_date(value)
```

### Comparing `wpp-bavapi-0.5.0/bavapi/http.py` & `wpp-bavapi-0.6.0/bavapi/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 
 # pylint: disable=too-many-arguments, too-few-public-methods
 
 import asyncio
 import math
 from json import JSONDecodeError
 from typing import (
+    TYPE_CHECKING,
     Dict,
     Iterator,
     List,
     Optional,
     Protocol,
+    Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import httpx
 from tqdm.asyncio import tqdm
 
 from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
 from bavapi.typing import BaseParamsMapping, JSONData, JSONDict
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
 __all__ = ("HTTPClient",)
 
 
 class Query(Protocol):
     """Protocol for Query objects."""
 
     item_id: Optional[int]
@@ -104,16 +109,21 @@
                 base_url=base_url,
             )
 
     async def __aenter__(self: C) -> C:
         await self.client.__aenter__()
         return self
 
-    async def __aexit__(self, *args, **kwargs) -> None:
-        await self.client.__aexit__(*args, **kwargs)
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: "Optional[TracebackType]" = None,
+    ) -> None:
+        await self.client.__aexit__(exc_type, exc_value, traceback)
 
     async def aclose(self) -> None:
         """Asynchronously close all client connections."""
         return await self.client.aclose()
 
     async def get(self, endpoint: str, params: Query) -> httpx.Response:
         """Perform GET request on the given endpoint.
```

### Comparing `wpp-bavapi-0.5.0/bavapi/jupyter.py` & `wpp-bavapi-0.6.0/bavapi/jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/bavapi/parsing/params.py` & `wpp-bavapi-0.6.0/bavapi/parsing/params.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/bavapi/parsing/responses.py` & `wpp-bavapi-0.6.0/bavapi/parsing/responses.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/bavapi/query.py` & `wpp-bavapi-0.6.0/bavapi/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from bavapi import filters as _filters
 from bavapi.parsing.params import list_to_str, to_fount_params
 from bavapi.typing import (
     BaseMutableParamsMapping,
     BaseParamsDict,
     BaseParamsDictValues,
+    BaseParamsMapping,
     OptionalListOr,
 )
 
 __all__ = ("Query",)
 
 F = TypeVar("F", bound=_filters.FountFilters)
 
@@ -72,26 +73,28 @@
         Returns
         -------
         dict[str, Any]
             Fount-compatible dictionary of the query.
         """
         exclude: Final[Set[str]] = {"filters", "fields", "max_pages"}
 
-        filters: BaseParamsDict = {}
+        filters: BaseParamsMapping = {}
         fields: BaseMutableParamsMapping = {}
 
         if isinstance(self.filters, _filters.FountFilters):
-            filters = self.filters.dict(by_alias=True, exclude_defaults=True)
+            filters = self.filters.model_dump(by_alias=True, exclude_defaults=True)
+        elif self.filters is not None:
+            filters = cast(BaseParamsDict, self.filters)
         filters = to_fount_params(filters, "filter")
         fields = to_fount_params(
             {endpoint: self.fields} if self.fields else fields, "fields"
         )
 
         params = {
-            **self.dict(exclude=exclude, by_alias=True, exclude_defaults=True),
+            **self.model_dump(exclude=exclude, by_alias=True, exclude_defaults=True),
             **filters,
             **fields,
         }
 
         return cast(BaseParamsDictValues, list_to_str(params))
 
     def with_page(self, page: int, per_page: int) -> "Query[F]":
@@ -110,20 +113,20 @@
         -------
         Query
             New `Query` instance with page parameters.
         """
         if self.page and self.per_page:
             return self
 
-        return self.__class__.construct(
-            self.__fields_set__.union({"page", "per_page"}),
+        return self.__class__.model_construct(
+            self.model_fields_set.union({"page", "per_page"}),
             page=self.page or page,
             per_page=self.per_page or per_page,
             filters=self.filters,  # avoid turning filters into dictionary
-            **self.dict(
+            **self.model_dump(
                 by_alias=True,
                 exclude={"page", "per_page", "filters"},
                 exclude_defaults=True,
             ),
         )
 
     def paginated(self, per_page: int, n_pages: int) -> Iterator["Query[F]"]:
```

### Comparing `wpp-bavapi-0.5.0/bavapi/reference/generate_reference.py` & `wpp-bavapi-0.6.0/bavapi/reference/generate_reference.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/bavapi/sync.py` & `wpp-bavapi-0.6.0/bavapi/sync.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/bavapi/typing.py` & `wpp-bavapi-0.6.0/bavapi/typing.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/pyproject.toml` & `wpp-bavapi-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wpp-bavapi"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
     { name = "Ignacio Maiz Vilches", email = "ignacio.maiz@bavgroup.com" },
 ]
 description = "Python consumer for the WPPBAV Fount API."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -37,15 +37,15 @@
     'Topic :: Database :: Database Engines/Servers',
     'Topic :: Scientific/Engineering :: Information Analysis',
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 dependencies = [
     "httpx >= 0.20",
     "pandas >= 0.16.2",
-    "pydantic >= 1.10, < 2",
+    "pydantic >= 2",
     "tqdm >= 4.62",
     "nest-asyncio >= 1.5.6",
     "typing-extensions >= 3.10; python_version < '3.10'",
 ]
 
 [project.urls]
 homepage = "https://github.com/wppbav/bavapi-sdk-python"
@@ -62,17 +62,14 @@
 ]
 test = ["coverage", "pytest", "pytest-asyncio", "python-dotenv"]
 lint = ["pylint", "mypy", "pandas-stubs"]
 
 [project.scripts]
 bavapi-gen-refs = "bavapi.reference.generate_reference:main"
 
-[tool.setuptools]
-include-package-data = true
-
 [tool.setuptools.packages.find]
 include = ["bavapi*"]
 
 [tool.coverage.paths]
 source = ["bavapi", "/home/runner/work/*/bavapi", "D:/a/*/*/bavapi"]
 tests = ["tests", "*/tests"]
```

### Comparing `wpp-bavapi-0.5.0/tests/test_client.py` & `wpp-bavapi-0.6.0/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring
 # pylint: disable=protected-access, redefined-outer-name
 
-from typing import List, Optional, Set, TypeVar, Union
+from typing import Set
 from unittest import mock
 
 import pytest
 
 from bavapi.client import Client, _default_brandscape_include
 from bavapi.http import HTTPClient
 from bavapi.query import Query
+from bavapi.typing import OptionalListOr
 
 from .helpers import wraps
 
-T = TypeVar("T")
-
 # CLASS INIT TESTS
 
 
 def test_init():
     fount = Client("test_token")
     assert isinstance(fount._client, HTTPClient)
 
@@ -30,14 +29,39 @@
 def test_init_no_token():
     with pytest.raises(ValueError) as excinfo:
         Client()
 
     assert excinfo.value.args[0] == "You must provide `auth_token` or `client`."
 
 
+# PRIVATE TESTS
+
+
+@pytest.mark.parametrize(
+    ("value", "expected"),
+    (
+        ("test", {"brand", "study", "category", "audience", "test"}),
+        (None, {"brand", "study", "category", "audience"}),
+        (["test"], {"brand", "study", "category", "audience", "test"}),
+    ),
+)
+def test_brandscape_query_default_include(
+    value: OptionalListOr[str], expected: Set[str]
+):
+    assert set(_default_brandscape_include(value)) == expected  # type: ignore
+
+
+def test_brandscape_query_default_include_partial():
+    assert _default_brandscape_include("brand") == "brand"
+
+
+def test_brandscape_query_no_default_include():
+    assert _default_brandscape_include("no_default") is None
+
+
 # PUBLIC TESTS
 
 
 def test_per_page():
     _fount = Client("token")
     assert _fount.per_page == 100
     _fount.per_page = 1000
@@ -109,29 +133,7 @@
 async def test_studies(fount: Client):
     with mock.patch.object(
         fount._client, "query", wraps=wraps([{"1": 1, "2": 2}])
     ) as mock_base_query:
         assert (await fount.studies(study_id=1)).shape == (1, 2)
 
     mock_base_query.assert_awaited_once_with("studies", Query(id=1))
-
-
-@pytest.mark.parametrize(
-    ("value", "expected"),
-    (
-        ("test", {"brand", "study", "category", "audience", "test"}),
-        (None, {"brand", "study", "category", "audience"}),
-        (["test"], {"brand", "study", "category", "audience", "test"}),
-    ),
-)
-def test_brandscape_query_default_include(
-    value: Optional[Union[str, List[str]]], expected: Set[str]
-):
-    assert set(_default_brandscape_include(value)) == expected  # type: ignore
-
-
-def test_brandscape_query_default_include_partial():
-    assert _default_brandscape_include("brand") == "brand"
-
-
-def test_brandscape_query_no_default_include():
-    assert _default_brandscape_include("no_default") is None
```

### Comparing `wpp-bavapi-0.5.0/tests/test_filters.py` & `wpp-bavapi-0.6.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-0.5.0/tests/test_http.py` & `wpp-bavapi-0.6.0/tests/test_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring
 # pylint: disable=protected-access, redefined-outer-name
 
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing import Dict, Optional
 from unittest import mock
 
 import httpx
 import pytest
 
 from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
 from bavapi.http import HTTPClient
 from bavapi.query import Query
+from bavapi.typing import JSONData, JSONDict
 
 from .helpers import wraps
 
-T = TypeVar("T")
-
 # HELPERS
 
 
 @dataclass
 class QueryResult:
     """Model for WPPBAV Fount query results"""
 
-    data: Union[Dict[str, Any], List[Dict[str, Any]]]
+    data: JSONData
     links: Dict[str, str]
-    meta: Dict[str, Any]
+    meta: JSONDict
 
-    def dict(self) -> Dict[str, Any]:
+    def dict(self) -> JSONDict:
         return asdict(self)
 
 
 def response(
     status_code: int = 200,
     message: str = "ok",
     *,
-    json: Optional[Any] = None,
+    json: Optional[JSONData] = None,
     request_url: str = "http://test_url/request",
     headers: Optional[httpx.Headers] = None,
 ) -> httpx.Response:
     return httpx.Response(
         status_code=status_code,
         json=json if json is not None else {"message": message},
         request=httpx.Request("GET", url=request_url),
         headers=headers
         or httpx.Headers({"x-ratelimit-remaining": "500", "x-ratelimit-limit": "500"}),
     )
 
 
 def sample_data(
-    data: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+    data: Optional[JSONData] = None,
     per_page: int = 25,
     on_page: int = 25,
     total: int = 2000,
-) -> Dict[str, Any]:
+) -> JSONDict:
     return QueryResult(
         data=data if data is not None else {},
         links={},
         meta={
             "per_page": per_page,
             "to": on_page,
             "total": total,
@@ -96,19 +95,17 @@
     async with client as client:
         assert isinstance(client, HTTPClient)
 
     assert client.client.is_closed
 
 
 @pytest.mark.anyio
-async def test_aclose(client: HTTPClient):
-    with mock.patch(
-        "bavapi.http.httpx.AsyncClient.aclose", wraps=wraps()
-    ) as mock_aclose:
-        await client.aclose()
+@mock.patch("bavapi.http.httpx.AsyncClient.aclose", wraps=wraps())
+async def test_aclose(mock_aclose: mock.AsyncMock, client: HTTPClient):
+    await client.aclose()
 
     mock_aclose.assert_called_once()
 
 
 @pytest.mark.anyio
 @mock.patch("bavapi.http.httpx.AsyncClient.get", wraps=wraps(response()))
 async def test_get(mock_get: mock.AsyncMock, client: HTTPClient):
```

### Comparing `wpp-bavapi-0.5.0/tests/test_jupyter.py` & `wpp-bavapi-0.6.0/tests/test_jupyter.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,43 +7,51 @@
 from typing import Callable, Optional
 from unittest import mock
 
 import pytest
 
 from bavapi import jupyter
 
+SetIpythonFunc = Callable[[Optional[bool]], None]
+
 
 class IPython(ModuleType):
     """Mock IPython module attributes and functions"""
 
     def __init__(self, kernel: Optional[bool] = None) -> None:
         self.kernel = kernel
         self.get_ipython = self._get_ipython
         super().__init__(self.__class__.__name__)
 
     def _get_ipython(self) -> "IPython":
         return self
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture(scope="function")
 def set_ipython():
     def _set_ipython(kernel: Optional[bool] = None) -> None:
         sys.modules["IPython"] = IPython(kernel)
 
     yield _set_ipython
 
     del sys.modules["IPython"]
 
 
-def test_running_in_jupyter(set_ipython: Callable):
+def test_running_in_jupyter(set_ipython: SetIpythonFunc):
     set_ipython(True)
 
     assert jupyter.running_in_jupyter()
 
 
+def test_not_running_in_jupyter(set_ipython: SetIpythonFunc):
+    set_ipython(None)
+
+    assert not jupyter.running_in_jupyter()
+
+
 @mock.patch("bavapi.jupyter.nest_asyncio.apply")
 def test_enabled_nested(mock_apply: mock.Mock):
     loop = asyncio.new_event_loop()
 
     jupyter.patch_loop(loop)
 
     mock_apply.assert_called_once_with(loop)
```

### Comparing `wpp-bavapi-0.5.0/tests/test_sync.py` & `wpp-bavapi-0.6.0/tests/test_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # pylint: disable=missing-module-docstring, missing-function-docstring
 # pylint: disable=protected-access
 
 import asyncio
-from typing import Any, Dict, TypeVar
+from typing import Any, Dict
 from unittest import mock
 
 import pytest
 
 from bavapi import sync
 from bavapi.query import Query
 
 from .helpers import wraps
 
-T = TypeVar("T")
-
 
 @mock.patch("bavapi.sync.asyncio.new_event_loop", return_value=asyncio.new_event_loop())
 def test_coro_new_loop(mock_new_loop: mock.AsyncMock):
     @sync._coro
     async def mock_func():
         pass
```

### Comparing `wpp-bavapi-0.5.0/wpp_bavapi.egg-info/PKG-INFO` & `wpp-bavapi-0.6.0/wpp_bavapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://github.com/wppbav/bavapi-sdk-python
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

