# Comparing `tmp/lib_shopware6_api-2.0.3.tar.gz` & `tmp/lib_shopware6_api-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_shopware6_api-2.0.3.tar", last modified: Thu Jul 13 14:17:31 2023, max compression
+gzip compressed data, was "lib_shopware6_api-2.0.4.tar", last modified: Thu Jul 13 17:40:05 2023, max compression
```

## Comparing `lib_shopware6_api-2.0.3.tar` & `lib_shopware6_api-2.0.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.581505 lib_shopware6_api-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.573505 lib_shopware6_api-2.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    80717 2023-07-13 14:17:31.581505 lib_shopware6_api-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    79766 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/lib_shopware6_api/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/lib_shopware6_api/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_delivery_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    57284 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    80717 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:17:31.581505 lib_shopware6_api-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.545062 lib_shopware6_api-2.0.4/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.541062 lib_shopware6_api-2.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.545062 lib_shopware6_api-2.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    80805 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    79854 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.545062 lib_shopware6_api-2.0.4/lib_shopware6_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/lib_shopware6_api/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_delivery_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57284 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    80805 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/test_cli.py
```

### Comparing `lib_shopware6_api-2.0.3/.coveragerc` & `lib_shopware6_api-2.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/.docs/README_template.rst` & `lib_shopware6_api-2.0.4/.docs/README_template.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 lib_shopware6_api
 =================
 
 
-Version v2.0.3 as of 2023-07-13 see `Changelog`_
+Version v2.0.4 as of 2023-07-13 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
 .. include:: ./tested_under.rst
 
 ----
 
 .. include:: ./index.rst
```

### Comparing `lib_shopware6_api-2.0.3/.docs/badges.rst` & `lib_shopware6_api-2.0.4/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/.docs/installation.rst` & `lib_shopware6_api-2.0.4/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/.docs/usage.rst` & `lib_shopware6_api-2.0.4/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/.github/workflows/codeql-analysis.yml` & `lib_shopware6_api-2.0.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/.github/workflows/python-package.yml` & `lib_shopware6_api-2.0.4/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -76,25 +76,14 @@
       matrix:
         include:
           # https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-software
           # https://github.com/actions/setup-python/blob/main/docs/advanced-usage.md#available-versions-of-python-and-pypy
 
 
           - os: ubuntu-latest
-            python-version: "3.7"
-            env:
-              BUILD_DOCS: "False"
-              BUILD: "True"  
-              BUILD_TEST: "True"
-              MYPY_DO_TESTS: "True"
-              DO_SETUP_INSTALL: "True"
-              DO_SETUP_INSTALL_TEST: "True"
-              DO_CLI_TEST: "True"
-
-          - os: ubuntu-latest
             python-version: "3.8"
             env:
               BUILD_DOCS: "False"
               BUILD: "True"  
               BUILD_TEST: "True"
               MYPY_DO_TESTS: "True"
               DO_SETUP_INSTALL: "True"
```

### Comparing `lib_shopware6_api-2.0.3/.gitignore` & `lib_shopware6_api-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/CHANGES.rst` & `lib_shopware6_api-2.0.4/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.3
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api-2.0.3/CODE_OF_CONDUCT.md` & `lib_shopware6_api-2.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/CONTRIBUTING.md` & `lib_shopware6_api-2.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/ISSUE_TEMPLATE.md` & `lib_shopware6_api-2.0.4/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/LICENSE` & `lib_shopware6_api-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/Makefile` & `lib_shopware6_api-2.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/PKG-INFO` & `lib_shopware6_api-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib_shopware6_api
-Version: 2.0.3
+Version: 2.0.4
 Summary: use the shopware 6 api
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api
 =================
 
 
-Version v2.0.3 as of 2023-07-13 see `Changelog`_
+Version v2.0.4 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -76,17 +76,17 @@
 this might be a good example for Your own API Client Functions - to be further extended
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -1957,14 +1957,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.3
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api-2.0.3/PULL_REQUEST_TEMPLATE.md` & `lib_shopware6_api-2.0.4/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/README.rst` & `lib_shopware6_api-2.0.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_shopware6_api
 =================
 
 
-Version v2.0.3 as of 2023-07-13 see `Changelog`_
+Version v2.0.4 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -54,17 +54,17 @@
 this might be a good example for Your own API Client Functions - to be further extended
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -1935,14 +1935,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.3
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/3rd_party_stubs/readme.txt` & `lib_shopware6_api-2.0.4/lib_shopware6_api/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/__init__.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api_cli.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api_cli.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_currency.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_currency.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_delivery_time.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_delivery_time.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_media.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_media.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_product.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_product.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_tax.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_tax.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_unit.py` & `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_unit.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/PKG-INFO` & `lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib-shopware6-api
-Version: 2.0.3
+Version: 2.0.4
 Summary: use the shopware 6 api
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api
 =================
 
 
-Version v2.0.3 as of 2023-07-13 see `Changelog`_
+Version v2.0.4 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -76,17 +76,17 @@
 this might be a good example for Your own API Client Functions - to be further extended
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -1957,14 +1957,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.3
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/SOURCES.txt` & `lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/lib_shopware6_api.ipynb` & `lib_shopware6_api-2.0.4/lib_shopware6_api.ipynb`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/pyproject.toml` & `lib_shopware6_api-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 name = "lib_shopware6_api"
 authors = [
     {name = "Robert Nowotny", email = "bitranox@gmail.com"},
 ]
 description = "use the shopware 6 api"
 readme = "README.rst"
-requires-python = ">=3.7.0"
+requires-python = ">=3.8.0"
 keywords = [
 ]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -28,15 +28,15 @@
 dependencies = [
     "attrs>=21.3.0",
     "click",
     "cli_exit_tools",
     "lib_detect_testenv",
     "lib_shopware6_api_base",
 ]
-version = "v2.0.3"
+version = "v2.0.4"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_shopware6_api"
 Documentation = "https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_shopware6_api.git"
@@ -49,14 +49,15 @@
     "coloredlogs",
     "coverage",
     "flake8",
     "mypy ; platform_python_implementation != 'PyPy'",
     "pytest",
     "pytest-cov",
     "pytest-runner",
+    "readme_renderer",
 ]
 
 [project.scripts]
     lib_shopware6_api = "lib_shopware6_api.lib_shopware6_api_cli:cli_main"
 
 [tool.setuptools.package-data]
 lib_shopware6_api = [
```

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/lib_bash_functions.sh` & `lib_shopware6_api-2.0.4/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/run_pytest.sh` & `lib_shopware6_api-2.0.4/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop.sh` & `lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop_windows.cmd` & `lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/shellcheck.sh` & `lib_shopware6_api-2.0.4/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/local_testscripts/testing_tools.py` & `lib_shopware6_api-2.0.4/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.3/tests/test_cli.py` & `lib_shopware6_api-2.0.4/tests/test_cli.py`

 * *Files identical despite different names*

