# Comparing `tmp/ezapi-sysaid-0.1.0.tar.gz` & `tmp/ezapi-sysaid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezapi-sysaid-0.1.0.tar", last modified: Tue May  9 07:02:10 2023, max compression
+gzip compressed data, was "ezapi-sysaid-0.1.1.tar", last modified: Thu Jul 13 04:24:53 2023, max compression
```

## Comparing `ezapi-sysaid-0.1.0.tar` & `ezapi-sysaid-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.215993 ezapi-sysaid-0.1.0/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.207449 ezapi-sysaid-0.1.0/.github/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.209559 ezapi-sysaid-0.1.0/.github/workflows/
--rw-r--r--   0 zehengl    (501) staff       (20)      781 2023-05-09 06:56:42.000000 ezapi-sysaid-0.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 zehengl    (501) staff       (20)       53 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/.gitignore
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.210002 ezapi-sysaid-0.1.0/.vscode/
--rw-r--r--   0 zehengl    (501) staff       (20)      469 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/.vscode/extensions.json
--rw-r--r--   0 zehengl    (501) staff       (20)      667 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/.vscode/settings.json
--rw-r--r--   0 zehengl    (501) staff       (20)     1301 2023-05-09 07:02:10.215808 ezapi-sysaid-0.1.0/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)      893 2023-05-09 06:58:21.000000 ezapi-sysaid-0.1.0/README.md
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.210155 ezapi-sysaid-0.1.0/docs/
--rw-r--r--   0 zehengl    (501) staff       (20)      386 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/docs/index.md
--rw-r--r--   0 zehengl    (501) staff       (20)     1362 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/mkdocs.yml
--rw-r--r--   0 zehengl    (501) staff       (20)      296 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/pcufile.toml
--rw-r--r--   0 zehengl    (501) staff       (20)      849 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/pyproject.toml
--rw-r--r--   0 zehengl    (501) staff       (20)      152 2023-05-07 03:45:49.000000 ezapi-sysaid-0.1.0/requirements-dev.txt
--rw-r--r--   0 zehengl    (501) staff       (20)      115 2023-05-08 20:26:01.000000 ezapi-sysaid-0.1.0/requirements-docs.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       48 2023-05-08 20:26:01.000000 ezapi-sysaid-0.1.0/requirements-test.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-05-07 03:45:49.000000 ezapi-sysaid-0.1.0/requirements.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-05-09 07:02:10.216036 ezapi-sysaid-0.1.0/setup.cfg
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.207770 ezapi-sysaid-0.1.0/src/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.210880 ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/
--rw-r--r--   0 zehengl    (501) staff       (20)     1301 2023-05-09 07:02:10.000000 ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)     1110 2023-05-09 07:02:10.000000 ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/SOURCES.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-05-09 07:02:10.000000 ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/dependency_links.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-05-09 07:02:10.000000 ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/requires.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        7 2023-05-09 07:02:10.000000 ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/top_level.txt
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.213867 ezapi-sysaid-0.1.0/src/sysaid/
--rw-r--r--   0 zehengl    (501) staff       (20)      918 2023-05-09 06:54:35.000000 ezapi-sysaid-0.1.0/src/sysaid/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)      243 2023-04-27 03:28:30.000000 ezapi-sysaid-0.1.0/src/sysaid/action_items.py
--rw-r--r--   0 zehengl    (501) staff       (20)      239 2023-05-09 06:34:51.000000 ezapi-sysaid-0.1.0/src/sysaid/add_ons.py
--rw-r--r--   0 zehengl    (501) staff       (20)      534 2023-05-09 06:39:09.000000 ezapi-sysaid-0.1.0/src/sysaid/assets.py
--rw-r--r--   0 zehengl    (501) staff       (20)       25 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/src/sysaid/cis.py
--rw-r--r--   0 zehengl    (501) staff       (20)      337 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/src/sysaid/core.py
--rw-r--r--   0 zehengl    (501) staff       (20)      958 2023-05-09 06:17:51.000000 ezapi-sysaid-0.1.0/src/sysaid/filters.py
--rw-r--r--   0 zehengl    (501) staff       (20)      371 2023-05-09 06:36:28.000000 ezapi-sysaid-0.1.0/src/sysaid/lists.py
--rw-r--r--   0 zehengl    (501) staff       (20)      338 2023-04-27 02:23:25.000000 ezapi-sysaid-0.1.0/src/sysaid/login.py
--rw-r--r--   0 zehengl    (501) staff       (20)       42 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/src/sysaid/non_resource_scenarios.py
--rw-r--r--   0 zehengl    (501) staff       (20)      412 2023-05-09 06:25:54.000000 ezapi-sysaid-0.1.0/src/sysaid/password_services.py
--rw-r--r--   0 zehengl    (501) staff       (20)       36 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/src/sysaid/resource_bundle.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1331 2023-05-09 06:20:37.000000 ezapi-sysaid-0.1.0/src/sysaid/service_requests.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1397 2023-05-09 06:17:17.000000 ezapi-sysaid-0.1.0/src/sysaid/users.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-05-09 07:02:10.215617 ezapi-sysaid-0.1.0/tests/
--rw-r--r--   0 zehengl    (501) staff       (20)      369 2023-05-09 06:55:28.000000 ezapi-sysaid-0.1.0/tests/conftest.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_action_items.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_add_ons.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_assets.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_cis.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_filters.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_lists.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_login.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_non_resource_scenarios.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_password_services.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_resource_bundle.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_service_requests.py
--rw-r--r--   0 zehengl    (501) staff       (20)      112 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_sysaid.py
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.0/tests/test_users.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.382233 ezapi-sysaid-0.1.1/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.371461 ezapi-sysaid-0.1.1/.github/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.374515 ezapi-sysaid-0.1.1/.github/workflows/
+-rw-r--r--   0 zehengl    (501) staff       (20)      308 2023-05-09 07:05:34.000000 ezapi-sysaid-0.1.1/.github/workflows/gh-deploy.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      243 2023-05-09 07:05:34.000000 ezapi-sysaid-0.1.1/.github/workflows/pcu.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      781 2023-05-09 06:56:42.000000 ezapi-sysaid-0.1.1/.github/workflows/pytest.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)       53 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/.gitignore
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.375124 ezapi-sysaid-0.1.1/.vscode/
+-rw-r--r--   0 zehengl    (501) staff       (20)      469 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/.vscode/extensions.json
+-rw-r--r--   0 zehengl    (501) staff       (20)      667 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/.vscode/settings.json
+-rw-r--r--   0 zehengl    (501) staff       (20)     1816 2023-07-13 04:24:53.382061 ezapi-sysaid-0.1.1/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     1280 2023-05-15 04:05:57.000000 ezapi-sysaid-0.1.1/README.md
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.375380 ezapi-sysaid-0.1.1/docs/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.375854 ezapi-sysaid-0.1.1/docs/endpoints/
+-rw-r--r--   0 zehengl    (501) staff       (20)       37 2023-05-15 04:05:57.000000 ezapi-sysaid-0.1.1/docs/endpoints/index.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      519 2023-05-15 04:05:57.000000 ezapi-sysaid-0.1.1/docs/endpoints/users.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      452 2023-05-15 04:05:57.000000 ezapi-sysaid-0.1.1/docs/index.md
+-rw-r--r--   0 zehengl    (501) staff       (20)     1452 2023-05-15 04:05:57.000000 ezapi-sysaid-0.1.1/mkdocs.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      296 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/pcufile.toml
+-rw-r--r--   0 zehengl    (501) staff       (20)      960 2023-05-09 07:05:36.000000 ezapi-sysaid-0.1.1/pyproject.toml
+-rw-r--r--   0 zehengl    (501) staff       (20)      152 2023-07-13 04:24:26.000000 ezapi-sysaid-0.1.1/requirements-dev.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)      143 2023-07-13 04:24:05.000000 ezapi-sysaid-0.1.1/requirements-docs.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       48 2023-07-13 04:24:26.000000 ezapi-sysaid-0.1.1/requirements-test.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-06-30 16:45:52.000000 ezapi-sysaid-0.1.1/requirements.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-07-13 04:24:53.382278 ezapi-sysaid-0.1.1/setup.cfg
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.372056 ezapi-sysaid-0.1.1/src/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.376785 ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1816 2023-07-13 04:24:53.000000 ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     1216 2023-07-13 04:24:53.000000 ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/SOURCES.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-07-13 04:24:53.000000 ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/dependency_links.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-07-13 04:24:53.000000 ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/requires.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        7 2023-07-13 04:24:53.000000 ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/top_level.txt
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.379882 ezapi-sysaid-0.1.1/src/sysaid/
+-rw-r--r--   0 zehengl    (501) staff       (20)      918 2023-05-09 06:54:35.000000 ezapi-sysaid-0.1.1/src/sysaid/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      243 2023-04-27 03:28:30.000000 ezapi-sysaid-0.1.1/src/sysaid/action_items.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      239 2023-05-09 06:34:51.000000 ezapi-sysaid-0.1.1/src/sysaid/add_ons.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      534 2023-05-09 06:39:09.000000 ezapi-sysaid-0.1.1/src/sysaid/assets.py
+-rw-r--r--   0 zehengl    (501) staff       (20)       25 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/src/sysaid/cis.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      337 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/src/sysaid/core.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      958 2023-05-09 06:17:51.000000 ezapi-sysaid-0.1.1/src/sysaid/filters.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      371 2023-05-09 06:36:28.000000 ezapi-sysaid-0.1.1/src/sysaid/lists.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      338 2023-04-27 02:23:25.000000 ezapi-sysaid-0.1.1/src/sysaid/login.py
+-rw-r--r--   0 zehengl    (501) staff       (20)       42 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/src/sysaid/non_resource_scenarios.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      412 2023-05-09 06:25:54.000000 ezapi-sysaid-0.1.1/src/sysaid/password_services.py
+-rw-r--r--   0 zehengl    (501) staff       (20)       36 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/src/sysaid/resource_bundle.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1331 2023-05-09 06:20:37.000000 ezapi-sysaid-0.1.1/src/sysaid/service_requests.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1397 2023-05-09 06:17:17.000000 ezapi-sysaid-0.1.1/src/sysaid/users.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:24:53.381867 ezapi-sysaid-0.1.1/tests/
+-rw-r--r--   0 zehengl    (501) staff       (20)      369 2023-05-09 06:55:28.000000 ezapi-sysaid-0.1.1/tests/conftest.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_action_items.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_add_ons.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_assets.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_cis.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_filters.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_lists.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_login.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_non_resource_scenarios.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_password_services.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_resource_bundle.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_service_requests.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      112 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_sysaid.py
+-rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-04-27 02:15:32.000000 ezapi-sysaid-0.1.1/tests/test_users.py
```

### Comparing `ezapi-sysaid-0.1.0/.github/workflows/pytest.yml` & `ezapi-sysaid-0.1.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `ezapi-sysaid-0.1.0/.vscode/settings.json` & `ezapi-sysaid-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ezapi-sysaid-0.1.0/PKG-INFO` & `ezapi-sysaid-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 Metadata-Version: 2.1
 Name: ezapi-sysaid
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for SysAid REST API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
+Project-URL: repository, https://github.com/zehengl/ezapi-sysaid
+Project-URL: homepage, https://zehengl.github.io/ezapi-sysaid/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://cdn0.iconfinder.com/data/icons/online-shopping-fill-shoppers-features/512/24-hrs_service-512.png" alt="logo" height="128">
 </div>
 
 # ezapi-sysaid
 
 [![pytest](https://github.com/zehengl/ezapi-sysaid/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-sysaid/actions/workflows/pytest.yml)
 ![coding_style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - License](https://img.shields.io/pypi/l/ezapi-sysaid)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ezapi-sysaid)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/ezapi-sysaid)
+[![Downloads](https://pepy.tech/badge/ezapi-sysaid)](https://pepy.tech/project/ezapi-sysaid)
 
 A Python wrapper for SysAid REST API
 
 ## Install
 
 From [PyPi](https://pypi.org/project/ezapi-sysaid/)
 
     pip install ezapi-sysaid
 
 From [GitHub](https://github.com/zehengl/ezapi-sysaid)
 
     pip install git+https://github.com/zehengl/ezapi-sysaid.git
 
+## Usage
+
+Check out these [examples](https://zehengl.github.io/ezapi-sysaid/endpoints/).
+
 ## Credits
 
 - [Logo][1] by [Chanut is Industries][2]
 
 [1]: https://www.iconfinder.com/icons/7581528/24_hours_service_online_smartphone_support_application_message_icon
 [2]: https://www.iconfinder.com/Chanut-is
```

### Comparing `ezapi-sysaid-0.1.0/mkdocs.yml` & `ezapi-sysaid-0.1.1/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 site_name: ezapi-sysaid
 nav:
   - Home: index.md
+  - Endpoints:
+      - endpoints/index.md
+      - Users: endpoints/users.md
 theme:
   name: material
   favicon: https://cdn0.iconfinder.com/data/icons/online-shopping-fill-shoppers-features/512/24-hrs_service-512.png
   logo: https://cdn0.iconfinder.com/data/icons/online-shopping-fill-shoppers-features/512/24-hrs_service-512.png
   font:
     text: Roboto
   palette:
     - scheme: default
-      primary: indigo
-      accent: indigo
+      primary: green
+      accent: green
       toggle:
         icon: material/toggle-switch
         name: Switch to dark mode
     - scheme: slate
-      primary: indigo
-      accent: indigo
+      primary: green
+      accent: green
       toggle:
         icon: material/toggle-switch-off-outline
         name: Switch to light mode
   features:
     - header.autohide
     - content.code.copy
     - navigation.top
@@ -30,14 +33,15 @@
   - search
   - tags
   - minify:
       minify_html: true
   - git-revision-date-localized:
       type: timeago
       enable_creation_date: true
+  - section-index
 extra:
   social:
     - icon: fontawesome/brands/github
       link: https://github.com/zehengl
     - icon: fontawesome/brands/linkedin
       link: https://linkedin.com/in/zehengl
 markdown_extensions:
```

### Comparing `ezapi-sysaid-0.1.0/pyproject.toml` & `ezapi-sysaid-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "ezapi-sysaid"
 dynamic = ["version", "dependencies"]
-authors = [
-    { name = "Zeheng Li", email = "imzehengl@gmail.com" },
-]
-maintainers = [
-    { name = "Zeheng Li", email = "imzehengl@gmail.com" },
-]
+authors = [{ name = "Zeheng Li", email = "imzehengl@gmail.com" }]
+maintainers = [{ name = "Zeheng Li", email = "imzehengl@gmail.com" }]
 description = "A Python wrapper for SysAid REST API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
+[project.urls]
+repository = "https://github.com/zehengl/ezapi-sysaid"
+homepage = "https://zehengl.github.io/ezapi-sysaid/"
+
+
 [tool.setuptools_scm]
 
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 python_files = ["test_*.py"]
 addopts = ["--import-mode=importlib"]
```

### Comparing `ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/PKG-INFO` & `ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 Metadata-Version: 2.1
 Name: ezapi-sysaid
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for SysAid REST API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
+Project-URL: repository, https://github.com/zehengl/ezapi-sysaid
+Project-URL: homepage, https://zehengl.github.io/ezapi-sysaid/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://cdn0.iconfinder.com/data/icons/online-shopping-fill-shoppers-features/512/24-hrs_service-512.png" alt="logo" height="128">
 </div>
 
 # ezapi-sysaid
 
 [![pytest](https://github.com/zehengl/ezapi-sysaid/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-sysaid/actions/workflows/pytest.yml)
 ![coding_style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - License](https://img.shields.io/pypi/l/ezapi-sysaid)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ezapi-sysaid)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/ezapi-sysaid)
+[![Downloads](https://pepy.tech/badge/ezapi-sysaid)](https://pepy.tech/project/ezapi-sysaid)
 
 A Python wrapper for SysAid REST API
 
 ## Install
 
 From [PyPi](https://pypi.org/project/ezapi-sysaid/)
 
     pip install ezapi-sysaid
 
 From [GitHub](https://github.com/zehengl/ezapi-sysaid)
 
     pip install git+https://github.com/zehengl/ezapi-sysaid.git
 
+## Usage
+
+Check out these [examples](https://zehengl.github.io/ezapi-sysaid/endpoints/).
+
 ## Credits
 
 - [Logo][1] by [Chanut is Industries][2]
 
 [1]: https://www.iconfinder.com/icons/7581528/24_hours_service_online_smartphone_support_application_message_icon
 [2]: https://www.iconfinder.com/Chanut-is
```

### Comparing `ezapi-sysaid-0.1.0/src/ezapi_sysaid.egg-info/SOURCES.txt` & `ezapi-sysaid-0.1.1/src/ezapi_sysaid.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 mkdocs.yml
 pcufile.toml
 pyproject.toml
 requirements-dev.txt
 requirements-docs.txt
 requirements-test.txt
 requirements.txt
+.github/workflows/gh-deploy.yml
+.github/workflows/pcu.yml
 .github/workflows/pytest.yml
 .vscode/extensions.json
 .vscode/settings.json
 docs/index.md
+docs/endpoints/index.md
+docs/endpoints/users.md
 src/ezapi_sysaid.egg-info/PKG-INFO
 src/ezapi_sysaid.egg-info/SOURCES.txt
 src/ezapi_sysaid.egg-info/dependency_links.txt
 src/ezapi_sysaid.egg-info/requires.txt
 src/ezapi_sysaid.egg-info/top_level.txt
 src/sysaid/__init__.py
 src/sysaid/action_items.py
```

### Comparing `ezapi-sysaid-0.1.0/src/sysaid/__init__.py` & `ezapi-sysaid-0.1.1/src/sysaid/__init__.py`

 * *Files identical despite different names*

### Comparing `ezapi-sysaid-0.1.0/src/sysaid/assets.py` & `ezapi-sysaid-0.1.1/src/sysaid/assets.py`

 * *Files identical despite different names*

### Comparing `ezapi-sysaid-0.1.0/src/sysaid/filters.py` & `ezapi-sysaid-0.1.1/src/sysaid/filters.py`

 * *Files identical despite different names*

### Comparing `ezapi-sysaid-0.1.0/src/sysaid/service_requests.py` & `ezapi-sysaid-0.1.1/src/sysaid/service_requests.py`

 * *Files identical despite different names*

### Comparing `ezapi-sysaid-0.1.0/src/sysaid/users.py` & `ezapi-sysaid-0.1.1/src/sysaid/users.py`

 * *Files identical despite different names*

