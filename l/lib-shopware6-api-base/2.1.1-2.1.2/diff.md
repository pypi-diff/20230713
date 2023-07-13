# Comparing `tmp/lib_shopware6_api_base-2.1.1.tar.gz` & `tmp/lib_shopware6_api_base-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_shopware6_api_base-2.1.1.tar", last modified: Thu Jul 13 10:30:58 2023, max compression
+gzip compressed data, was "lib_shopware6_api_base-2.1.2.tar", last modified: Thu Jul 13 17:35:42 2023, max compression
```

## Comparing `lib_shopware6_api_base-2.1.1.tar` & `lib_shopware6_api_base-2.1.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.395977 lib_shopware6_api_base-2.1.1/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.391977 lib_shopware6_api_base-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.395977 lib_shopware6_api_base-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    74216 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    73225 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.395977 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    59849 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    74216 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.739866 lib_shopware6_api_base-2.1.2/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.735866 lib_shopware6_api_base-2.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.739866 lib_shopware6_api_base-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    74304 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    73313 2023-07-13 17:35:29.000000 lib_shopware6_api_base-2.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59849 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    74304 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/test_cli.py
```

### Comparing `lib_shopware6_api_base-2.1.1/.coveragerc` & `lib_shopware6_api_base-2.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/.docs/README_template.rst` & `lib_shopware6_api_base-2.1.2/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.1 as of 2023-07-13 see `Changelog`_
+Version v2.1.2 as of 2023-07-13 see `Changelog`_
 
 
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

### Comparing `lib_shopware6_api_base-2.1.1/.docs/badges.rst` & `lib_shopware6_api_base-2.1.2/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/.docs/installation.rst` & `lib_shopware6_api_base-2.1.2/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/.docs/usage.rst` & `lib_shopware6_api_base-2.1.2/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/.github/workflows/codeql-analysis.yml` & `lib_shopware6_api_base-2.1.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/.github/workflows/python-package.yml` & `lib_shopware6_api_base-2.1.2/.github/workflows/python-package.yml`

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

### Comparing `lib_shopware6_api_base-2.1.1/.gitignore` & `lib_shopware6_api_base-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/CHANGES.rst` & `lib_shopware6_api_base-2.1.2/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.2
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.1.1
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api_base-2.1.1/CODE_OF_CONDUCT.md` & `lib_shopware6_api_base-2.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/CONTRIBUTING.md` & `lib_shopware6_api_base-2.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/ISSUE_TEMPLATE.md` & `lib_shopware6_api_base-2.1.2/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/LICENSE` & `lib_shopware6_api_base-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/Makefile` & `lib_shopware6_api_base-2.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/PKG-INFO` & `lib_shopware6_api_base-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib_shopware6_api_base
-Version: 2.1.1
+Version: 2.1.2
 Summary: python3 base API client for shopware6
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api_base
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api_base.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api_base/blob/master/CHANGES.rst
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
 
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.1 as of 2023-07-13 see `Changelog`_
+Version v2.1.2 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -81,17 +81,17 @@
 On github it can be only tested on linux, because we can not run a docker shopware container service on MacOS or Windows.
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -1994,14 +1994,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.2
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.1.1
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api_base-2.1.1/PULL_REQUEST_TEMPLATE.md` & `lib_shopware6_api_base-2.1.2/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/README.rst` & `lib_shopware6_api_base-2.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.1 as of 2023-07-13 see `Changelog`_
+Version v2.1.2 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -59,17 +59,17 @@
 On github it can be only tested on linux, because we can not run a docker shopware container service on MacOS or Windows.
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -1972,14 +1972,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.2
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.1.1
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/3rd_party_stubs/readme.txt` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__conf__.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_shopware6_api_base'
 title = 'python3 base API client for shopware6'
-version = 'v2.1.1'
+version = 'v2.1.2'
 url = 'https://github.com/bitranox/lib_shopware6_api_base'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_shopware6_api_base'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_shopware6_api_base:
 
     python3 base API client for shopware6
 
-    Version : v2.1.1
+    Version : v2.1.2
     Url     : https://github.com/bitranox/lib_shopware6_api_base
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_classes.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_classes.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_cli.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_cli.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/PKG-INFO` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib-shopware6-api-base
-Version: 2.1.1
+Version: 2.1.2
 Summary: python3 base API client for shopware6
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api_base
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api_base.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api_base/blob/master/CHANGES.rst
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
 
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.1 as of 2023-07-13 see `Changelog`_
+Version v2.1.2 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -81,17 +81,17 @@
 On github it can be only tested on linux, because we can not run a docker shopware container service on MacOS or Windows.
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -1994,14 +1994,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.2
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.1.1
 ---------
 2023-07-13:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove setup.cfg
     - remove setup.py
```

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/SOURCES.txt` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.ipynb` & `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.ipynb`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/pyproject.toml` & `lib_shopware6_api_base-2.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 name = "lib_shopware6_api_base"
 authors = [
     {name = "Robert Nowotny", email = "bitranox@gmail.com"},
 ]
 description = "python3 base API client for shopware6"
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
@@ -31,15 +31,15 @@
     "cli_exit_tools",
     "lib_detect_testenv",
     "oauthlib",
     "pprint3x",
     "requests",
     "requests_oauthlib",
 ]
-version = "v2.1.1"
+version = "v2.1.2"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_shopware6_api_base"
 Documentation = "https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_shopware6_api_base.git"
@@ -53,14 +53,15 @@
     "coverage",
     "flake8",
     "mypy ; platform_python_implementation != 'PyPy'",
     "pprint3x",
     "pytest",
     "pytest-cov",
     "pytest-runner",
+    "readme_renderer",
 ]
 
 [project.scripts]
     lib_shopware6_api_base = "lib_shopware6_api_base.lib_shopware6_api_base_cli:cli_main"
 
 [tool.setuptools.package-data]
 lib_shopware6_api_base = [
```

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/lib_bash_functions.sh` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_pytest.sh` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop.sh` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop_windows.cmd` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/shellcheck.sh` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/local_testscripts/testing_tools.py` & `lib_shopware6_api_base-2.1.2/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.1/tests/test_cli.py` & `lib_shopware6_api_base-2.1.2/tests/test_cli.py`

 * *Files identical despite different names*

