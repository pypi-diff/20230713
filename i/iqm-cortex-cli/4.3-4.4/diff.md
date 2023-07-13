# Comparing `tmp/iqm-cortex-cli-4.3.tar.gz` & `tmp/iqm-cortex-cli-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-cortex-cli-4.3.tar", last modified: Wed Jun 28 09:22:48 2023, max compression
+gzip compressed data, was "iqm-cortex-cli-4.4.tar", last modified: Thu Jul 13 07:33:42 2023, max compression
```

## Comparing `iqm-cortex-cli-4.3.tar` & `iqm-cortex-cli-4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.681371 iqm-cortex-cli-4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.685371 iqm-cortex-cli-4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.685371 iqm-cortex-cli-4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.681371 iqm-cortex-cli-4.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.685371 iqm-cortex-cli-4.3/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.685371 iqm-cortex-cli-4.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.681371 iqm-cortex-cli-4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/src/cortex_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/src/cortex_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/src/cortex_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/src/cortex_cli/cortex_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/src/cortex_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/src/cortex_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/src/cortex_cli/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-28 09:22:48.000000 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-28 09:22:48.000000 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 09:22:48.000000 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-28 09:22:48.000000 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-28 09:22:48.000000 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 09:22:48.000000 iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/cortex_cli_auth_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/cortex_cli_auth_logout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/cortex_cli_auth_status_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/cortex_cli_init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/cortex_cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:22:48.689371 iqm-cortex-cli-4.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tests/token_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-28 09:22:14.000000 iqm-cortex-cli-4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/src/cortex_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/cortex_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_auth_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_auth_logout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_auth_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/token_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tox.ini
```

### Comparing `iqm-cortex-cli-4.3/.github/workflows/ci.yml` & `iqm-cortex-cli-4.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/.github/workflows/publish.yml` & `iqm-cortex-cli-4.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/.github/workflows/tag_and_release.yml` & `iqm-cortex-cli-4.4/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/CHANGELOG.rst` & `iqm-cortex-cli-4.4/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 4.4
+===========
+
+* Support relative paths during init `#52 <https://github.com/iqm-finland/cortex-cli/pull/52>`_
+
+
 Version 4.3
 ===========
 
 * Fix logging for multi-user systems `#48 <https://github.com/iqm-finland/cortex-cli/pull/48>`_
 
 Version 4.2
 ===========
```

### Comparing `iqm-cortex-cli-4.3/DEVELOPMENT.rst` & `iqm-cortex-cli-4.4/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/LICENSE.rst` & `iqm-cortex-cli-4.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/PKG-INFO` & `iqm-cortex-cli-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.3
+Version: 4.4
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-4.3/README.rst` & `iqm-cortex-cli-4.4/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/Makefile` & `iqm-cortex-cli-4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/_static/images/favicon.ico` & `iqm-cortex-cli-4.4/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/_static/images/logo.png` & `iqm-cortex-cli-4.4/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/_templates/autosummary-class-template.rst` & `iqm-cortex-cli-4.4/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/_templates/autosummary-module-template.rst` & `iqm-cortex-cli-4.4/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/_templates/page.html` & `iqm-cortex-cli-4.4/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/_templates/versioning.html` & `iqm-cortex-cli-4.4/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/docs/conf.py` & `iqm-cortex-cli-4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/pyproject.toml` & `iqm-cortex-cli-4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.9, <3.11"
 dependencies = [
-    "click >= 7.1.2",
+    "click >= 7.1.2, < 8.1.4",  # upper limit until https://github.com/pallets/click/issues/2558 is fixed
     "jsonschema >= 4.6.0",
     "mechanize >= 0.4.8",
     "psutil >= 5.9.2",
     "pydantic >= 1.10.2, < 2.0",
     "python-daemon >= 2.3.0",
     "requests >= 2.26.0"
 ]
```

### Comparing `iqm-cortex-cli-4.3/src/cortex_cli/__init__.py` & `iqm-cortex-cli-4.4/src/cortex_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/src/cortex_cli/auth.py` & `iqm-cortex-cli-4.4/src/cortex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/src/cortex_cli/cortex_cli.py` & `iqm-cortex-cli-4.4/src/cortex_cli/cortex_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from datetime import datetime, timedelta
 import json
 import logging
 import os
 from pathlib import Path
 import platform
 import sys
+from typing import Any, Optional
 
 import click
 from psutil import Process
 from pydantic import ValidationError
 import requests
 from requests.exceptions import ConnectionError, Timeout  # pylint: disable=redefined-builtin
 
@@ -77,14 +78,30 @@
     if verbose:
         logger.setLevel(logging.DEBUG)
         return logging.DEBUG
     logger.setLevel(logging.INFO)
     return logging.INFO
 
 
+class ResolvedPath(click.Path):
+    """A click parameter type for a resolved path.
+    Normal ``click.Path(resolve_path=True)`` fails under Windows running python <= 3.9.
+    See https://github.com/pallets/click/issues/2466
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def convert(self, value: Any, param: Optional[click.Parameter], ctx: Optional[click.Context]) -> Any:
+        abspath = Path(value).absolute()
+        # fsdecode to ensure that the return value is a str.
+        # (with click<8.0.3 Path.convert will return Path if passed a Path)
+        return os.fsdecode(super().convert(abspath, param, ctx))
+
+
 def _read_json(path: str) -> dict:
     """Read a JSON file.
 
     Args:
         path: path to the file to read
     Raises:
         click.FileError: if file is not a valid JSON file
@@ -123,15 +140,15 @@
 
     # File exists, so user must either overwrite or enter a new path
     while True:
         msg = f"{click.style('File at given path already exists. Overwrite?', fg='red')}"
         if click.confirm(msg, default=None):
             return path
 
-        new_path = click.prompt('New file path', type=click.Path(dir_okay=False, writable=True))
+        new_path = click.prompt('New file path', type=ResolvedPath(dir_okay=False, writable=True, resolve_path=True))
 
         if new_path == path:
             continue
         return new_path
 
 
 def _validate_config_file(config_file: str) -> ConfigFile:
@@ -289,23 +306,23 @@
 
 @cortex_cli.command()
 @click.option(
     '--config-file',
     prompt='Where to save config',
     callback=_validate_path,
     default=CortexCliCommand.default_config_path,
-    type=click.Path(dir_okay=False, writable=True),
+    type=ResolvedPath(dir_okay=False, writable=True, resolve_path=True),
     help='Location where the configuration file will be saved.',
 )
 @click.option(
     '--tokens-file',
     prompt='Where to save auth tokens',
     callback=_validate_path,
     default=CortexCliCommand.default_tokens_path,
-    type=click.Path(dir_okay=False, writable=True),
+    type=ResolvedPath(dir_okay=False, writable=True, resolve_path=True),
     help='Location where the tokens file will be saved.',
 )
 @click.option(
     '--auth-server-url',
     prompt='Authentication server URL',
     callback=_validate_auth_server_url,
     help='Authentication server URL.',
@@ -370,15 +387,15 @@
     return
 
 
 @auth.command()
 @click.option(
     '--config-file',
     default=CortexCliCommand.default_config_path,
-    type=click.Path(exists=True, dir_okay=False),
+    type=ResolvedPath(exists=True, dir_okay=False, resolve_path=True),
     help='Location of the configuration file to be used.',
 )
 @click.option('-v', '--verbose', is_flag=True, help='Print extra information.')
 def status(config_file, verbose) -> None:
     """Check status of authentication."""
     _set_log_level_by_verbosity(verbose)
 
@@ -507,15 +524,15 @@
     return False
 
 
 @auth.command()
 @click.option(
     '--config-file',
     default=CortexCliCommand.default_config_path,
-    type=click.Path(exists=True, dir_okay=False),
+    type=ResolvedPath(exists=True, dir_okay=False, resolve_path=True),
     help='Location of the configuration file to be used.',
 )
 @click.option('--username', help='Username for authentication.')
 @click.option('--password', help='Password for authentication.')
 @click.option(
     '--refresh-period', default=REFRESH_PERIOD, show_default=True, help='How often to refresh tokens (in seconds).'
 )
@@ -605,15 +622,17 @@
     else:
         logger.info('Starting token manager daemon...')
         daemonize_token_manager(refresh_period, config)
 
 
 @auth.command()
 @click.option(
-    '--config-file', type=click.Path(exists=True, dir_okay=False), default=CortexCliCommand.default_config_path
+    '--config-file',
+    type=ResolvedPath(exists=True, dir_okay=False, resolve_path=True),
+    default=CortexCliCommand.default_config_path,
 )
 @click.option('--keep-tokens', is_flag=True, default=False, help="Don't delete tokens file, but kill token manager.")
 @click.option('-f', '--force', is_flag=True, default=False, help="Don't ask for confirmation.")
 def logout(config_file: str, keep_tokens: str, force: bool) -> None:
     """Either logout completely, or just stop token manager while keeping tokens file."""
     config = _validate_config_file(config_file)
     auth_server_url, realm, client_id = config.auth_server_url, config.realm, config.client_id
```

### Comparing `iqm-cortex-cli-4.3/src/cortex_cli/models.py` & `iqm-cortex-cli-4.4/src/cortex_cli/models.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/src/cortex_cli/token_manager.py` & `iqm-cortex-cli-4.4/src/cortex_cli/token_manager.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/PKG-INFO` & `iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.3
+Version: 4.4
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-4.3/src/iqm_cortex_cli.egg-info/SOURCES.txt` & `iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tag-from-pipeline.sh` & `iqm-cortex-cli-4.4/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/auth_test.py` & `iqm-cortex-cli-4.4/tests/auth_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/conftest.py` & `iqm-cortex-cli-4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/cortex_cli_auth_login_test.py` & `iqm-cortex-cli-4.4/tests/cortex_cli_auth_login_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,32 @@
 
 import json
 import os
 
 from click.testing import CliRunner
 import mechanize  # type: ignore
 from mockito import ANY, mock, unstub, when
+import pytest
 
 from cortex_cli.cortex_cli import cortex_cli
 from tests.conftest import expect_token_is_valid, make_token, prepare_tokens
 
 
-def test_auth_login_succeeds(config_dict, credentials):
+@pytest.mark.parametrize('absolute_path', [True, False])
+def test_auth_login_succeeds(config_dict, credentials, absolute_path):
     """
     Tests that ``cortex auth login`` performs authentication and saves tokens.
     """
     expected_tokens = prepare_tokens(300, 3600, **credentials)
 
     runner = CliRunner()
     with runner.isolated_filesystem():
         config_dict['username'] = credentials['username']
+        if absolute_path:
+            config_dict['tokens_file'] = os.path.join(os.getcwd(), config_dict['tokens_file'])  # use absolute path
         with open('config.json', 'w', encoding='UTF-8') as file:
             file.write(json.dumps(config_dict))
 
         result = runner.invoke(
             cortex_cli,
             [
                 'auth',
```

### Comparing `iqm-cortex-cli-4.3/tests/cortex_cli_auth_logout_test.py` & `iqm-cortex-cli-4.4/tests/cortex_cli_auth_logout_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/cortex_cli_auth_status_test.py` & `iqm-cortex-cli-4.4/tests/cortex_cli_auth_status_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/cortex_cli_init_test.py` & `iqm-cortex-cli-4.4/tests/cortex_cli_init_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,27 +25,30 @@
 import pytest
 
 from cortex_cli.cortex_cli import cortex_cli
 from tests.conftest import expect_process_terminate, prepare_auth_server_urls
 
 
 @pytest.mark.parametrize('first_option', ['--config-file', '--tokens-file', '--auth-server-url', '--client-id'])
-def test_init_saves_config_file(config_dict, first_option):
+@pytest.mark.parametrize('absolute_path', [True, False])
+def test_init_saves_config_file(config_dict, first_option, tmp_path, absolute_path):
     """
     Tests that ``cortex init`` produces config file.
 
     Having different options as first one is tested since it can affect the initialization of ``click.Context``.
     Specifying ``realm`` before ``auth-server-url`` is not allowed, so that case is not included.
     """
     prepare_auth_server_urls(config_dict)
     runner = CliRunner()
-    with runner.isolated_filesystem():
+    with runner.isolated_filesystem(temp_dir=tmp_path):
         options_map = {
-            '--config-file': 'config.json',
-            '--tokens-file': config_dict['tokens_file'],
+            '--config-file': os.path.join(os.getcwd(), 'config.json') if absolute_path else 'config.json',
+            '--tokens-file': os.path.join(os.getcwd(), config_dict['tokens_file'])
+            if absolute_path
+            else config_dict['tokens_file'],
             '--auth-server-url': config_dict['auth_server_url'],
             '--realm': config_dict['realm'],
             '--client-id': config_dict['client_id'],
         }
         result = runner.invoke(
             cortex_cli,
             [
@@ -55,25 +58,27 @@
                 *itertools.chain.from_iterable([item for item in options_map.items() if item[0] != first_option]),
             ],
         )
         assert result.exit_code == 0
         assert 'Cortex CLI initialized successfully' in result.output
         with open('config.json', 'r', encoding='utf-8') as config_file:
             loaded_config = json.load(config_file)
+            tmp_tokens_path = os.path.join(os.getcwd(), config_dict['tokens_file'])
+            config_dict['tokens_file'] = tmp_tokens_path  # update path to current temporary dir created by CliRunner
             assert loaded_config == config_dict
     unstub()
 
 
-def test_init_overwrites_config_file(config_dict):
+def test_init_overwrites_config_file(config_dict, tmp_path):
     """
     Tests that ``cortex init`` prompts to overwrite, and overwrites existing config file.
     """
     prepare_auth_server_urls(config_dict)
     runner = CliRunner()
-    with runner.isolated_filesystem():
+    with runner.isolated_filesystem(temp_dir=tmp_path):
         old_config_dict = config_dict.copy()
         old_config_dict['auth_server_url'] = 'https://to.be.overwritten.com'
         old_config_dict['username'] = 'to_be_overwritten'
         with open('config.json', 'w', encoding='UTF-8') as file:
             file.write(json.dumps(old_config_dict))
 
         result = runner.invoke(
@@ -93,26 +98,28 @@
             ],
             input='y',
         )
         assert result.exit_code == 0
         assert 'already exists. Overwrite?' in result.output
         with open('config.json', 'r', encoding='utf-8') as config_file:
             loaded_config = json.load(config_file)
+            tmp_tokens_path = os.path.join(os.getcwd(), config_dict['tokens_file'])
+            config_dict['tokens_file'] = tmp_tokens_path  # update path to current temporary dir created by CliRunner
             assert loaded_config == config_dict
             assert loaded_config != old_config_dict
     unstub()
 
 
-def test_init_kills_daemon_and_removes_token_file(config_dict, tokens_dict):
+def test_init_kills_daemon_and_removes_token_file(config_dict, tokens_dict, tmp_path):
     """
     Tests that ``cortex init`` kills active token manager daemon and removes old token file.
     """
     prepare_auth_server_urls(config_dict)
     runner = CliRunner()
-    with runner.isolated_filesystem():
+    with runner.isolated_filesystem(temp_dir=tmp_path):
         # emulate a running daemon by storing a real PID
         tokens_dict['pid'] = os.getpid()
 
         tokens_file_path = 'tokens.json'
         with open(tokens_file_path, 'w', encoding='UTF-8') as file:
             file.write(json.dumps(tokens_dict))
 
@@ -136,22 +143,22 @@
         )
         assert not Path(tokens_file_path).is_file()
         assert result.exit_code == 0
         assert 'will be killed' in result.output
     unstub()
 
 
-def test_init_warns_user_if_auth_server_url_is_invalid(config_dict):
+def test_init_warns_user_if_auth_server_url_is_invalid(config_dict, tmp_path):
     """
     Tests that ``cortex init`` prompts user to either accept invalid auth server URL or to enter another one.
     """
     invalid_url = 'http://invalid.com'
     prepare_auth_server_urls(config_dict, invalid_url)
     runner = CliRunner()
-    with runner.isolated_filesystem():
+    with runner.isolated_filesystem(temp_dir=tmp_path):
         result = runner.invoke(
             cortex_cli,
             [
                 'init',
                 '--config-file',
                 'config.json',
                 '--tokens-file',
@@ -166,27 +173,29 @@
             input='y\ny\n',  # User accepts auth_server_url and realm (realm can not be accessed either)
         )
         assert result.exit_code == 0
         assert f'No auth server could be accessed with URL {invalid_url}' in result.output
         assert 'Do you still want to use it?' in result.output
         with open('config.json', 'r', encoding='utf-8') as config_file:
             loaded_config = json.load(config_file)
+            tmp_tokens_path = os.path.join(os.getcwd(), config_dict['tokens_file'])
+            config_dict['tokens_file'] = tmp_tokens_path  # update path to current temporary dir created by CliRunner
             assert loaded_config == {**config_dict, 'auth_server_url': invalid_url}
     unstub()
 
 
-def test_init_warns_user_if_realm_is_invalid(config_dict):
+def test_init_warns_user_if_realm_is_invalid(config_dict, tmp_path):
     """
     Tests that ``cortex init`` prompts user to either accept invalid realm or to enter another one.
     """
     valid_url = config_dict['auth_server_url']
     invalid_realm = 'invalid'
     prepare_auth_server_urls(config_dict, invalid_realm=invalid_realm)
     runner = CliRunner()
-    with runner.isolated_filesystem():
+    with runner.isolated_filesystem(temp_dir=tmp_path):
         result = runner.invoke(
             cortex_cli,
             [
                 'init',
                 '--config-file',
                 'config.json',
                 '--tokens-file',
@@ -201,26 +210,28 @@
             input='y\n',  # User accepts the realm
         )
         assert result.exit_code == 0
         assert f'No auth realm could be accessed with URL {valid_url}/realms/{invalid_realm}' in result.output
         assert 'Do you still want to use it?' in result.output
         with open('config.json', 'r', encoding='utf-8') as config_file:
             loaded_config = json.load(config_file)
+            tmp_tokens_path = os.path.join(os.getcwd(), config_dict['tokens_file'])
+            config_dict['tokens_file'] = tmp_tokens_path  # update path to current temporary dir created by CliRunner
             assert loaded_config == {**config_dict, 'realm': invalid_realm}
     unstub()
 
 
-def test_init_lets_user_to_enter_correct_auth_server_url_if_the_original_is_invalid(config_dict):
+def test_init_lets_user_to_enter_correct_auth_server_url_if_the_original_is_invalid(config_dict, tmp_path):
     """
     Tests that ``cortex init`` prompts user to enter another URL if the original is invalid.
     """
     invalid_url = 'http://invalid.com'
     prepare_auth_server_urls(config_dict, invalid_url)
     runner = CliRunner()
-    with runner.isolated_filesystem():
+    with runner.isolated_filesystem(temp_dir=tmp_path):
         result = runner.invoke(
             cortex_cli,
             [
                 'init',
                 '--config-file',
                 'config.json',
                 '--tokens-file',
@@ -235,9 +246,11 @@
             input=f'\n{config_dict["auth_server_url"]}\n',  # User rejects the invalid URL and enters another one
         )
         assert result.exit_code == 0
         assert f'No auth server could be accessed with URL {invalid_url}' in result.output
         assert 'Do you still want to use it?' in result.output
         with open('config.json', 'r', encoding='utf-8') as config_file:
             loaded_config = json.load(config_file)
+            tmp_tokens_path = os.path.join(os.getcwd(), config_dict['tokens_file'])
+            config_dict['tokens_file'] = tmp_tokens_path  # update path to current temporary dir created by CliRunner
             assert loaded_config == config_dict
     unstub()
```

### Comparing `iqm-cortex-cli-4.3/tests/cortex_cli_test.py` & `iqm-cortex-cli-4.4/tests/cortex_cli_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/resources/tokens.json` & `iqm-cortex-cli-4.4/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tests/token_manager_test.py` & `iqm-cortex-cli-4.4/tests/token_manager_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.3/tox.ini` & `iqm-cortex-cli-4.4/tox.ini`

 * *Files identical despite different names*

