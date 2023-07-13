# Comparing `tmp/lib_detect_testenv-2.0.5.tar.gz` & `tmp/lib_detect_testenv-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_detect_testenv-2.0.5.tar", last modified: Tue Jul 11 20:56:14 2023, max compression
+gzip compressed data, was "lib_detect_testenv-2.0.6.tar", last modified: Thu Jul 13 16:44:45 2023, max compression
```

## Comparing `lib_detect_testenv-2.0.5.tar` & `lib_detect_testenv-2.0.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.980442 lib_detect_testenv-2.0.5/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.976442 lib_detect_testenv-2.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.980442 lib_detect_testenv-2.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.980442 lib_detect_testenv-2.0.5/lib_detect_testenv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/lib_detect_testenv/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 20:56:14.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/lib_detect_testenv.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:56:14.984442 lib_detect_testenv-2.0.5/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 20:55:28.000000 lib_detect_testenv-2.0.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.491191 lib_detect_testenv-2.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/lib_detect_testenv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/lib_detect_testenv/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/test_cli.py
```

### Comparing `lib_detect_testenv-2.0.5/.coveragerc` & `lib_detect_testenv-2.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/.docs/README_template.rst` & `lib_detect_testenv-2.0.6/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 lib_detect_testenv
 ==================
 
 
-Version v2.0.5 as of 2023-07-11 see `Changelog`_
+Version v2.0.6 as of 2023-07-13 see `Changelog`_
 
 
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

### Comparing `lib_detect_testenv-2.0.5/.docs/badges.rst` & `lib_detect_testenv-2.0.6/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/.docs/installation.rst` & `lib_detect_testenv-2.0.6/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/.docs/usage.rst` & `lib_detect_testenv-2.0.6/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/.github/workflows/codeql-analysis.yml` & `lib_detect_testenv-2.0.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/.github/workflows/python-package.yml` & `lib_detect_testenv-2.0.6/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -85,25 +85,14 @@
               DO_SETUP_INSTALL: "True"
               DO_SETUP_INSTALL_TEST: "True"
               # Test registered CLI Command
               DO_CLI_TEST: "True"
 
 
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

### Comparing `lib_detect_testenv-2.0.5/.gitignore` & `lib_detect_testenv-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/CHANGES.rst` & `lib_detect_testenv-2.0.6/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.5
 ---------
 2023-07-11:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove mypy.ini
     - remove pytest.ini
     - remove setup.cfg
     - remove setup.py
     - remove .bettercodehub.yml
     - remove .travis.yml
     - update black config
+    - clean ./tests/test_cli.py
 
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
```

### Comparing `lib_detect_testenv-2.0.5/CODE_OF_CONDUCT.md` & `lib_detect_testenv-2.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/CONTRIBUTING.md` & `lib_detect_testenv-2.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/ISSUE_TEMPLATE.md` & `lib_detect_testenv-2.0.6/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/LICENSE` & `lib_detect_testenv-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/Makefile` & `lib_detect_testenv-2.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/PKG-INFO` & `lib_detect_testenv-2.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib_detect_testenv
-Version: 2.0.5
+Version: 2.0.6
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_detect_testenv
 Project-URL: Documentation, https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_detect_testenv.git
 Project-URL: Changelog, https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst
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
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.5 as of 2023-07-11 see `Changelog`_
+Version v2.0.6 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -74,17 +74,17 @@
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -159,14 +159,18 @@
         True if docrunner is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert False == is_doctest_active(arg_string="")
+        >>> assert True == is_doctest_active(arg_string="docrunner.py")
+        >>> assert True == is_doctest_active(arg_string="doctest.py")
+
         """
 
 - detect if pytest is active
 
 .. code-block:: python
 
     def is_pytest_active(arg_string: Optional[str] = None) -> bool:
@@ -184,14 +188,17 @@
         True if pytest is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert True == is_pytest_active(arg_string='pytest.py')
+        >>> assert True == is_pytest_active(arg_string='/pytest/__main__.py')
+
         """
 
 - detect if setup.py is active
 
 .. code-block:: python
 
     def is_setup_active(arg_string: Optional[str] = None) -> bool:
@@ -209,14 +216,17 @@
         True if setup.py is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert False == is_setup_active(arg_string="")
+        >>> assert True == is_setup_active(arg_string="setup.py")
+
         """
 
 - detect if "setup.py test" is active
 
 .. code-block:: python
 
     def is_setup_test_active(arg_string: Optional[str] = None) -> bool:
@@ -234,14 +244,18 @@
         True if "setup.py test" is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert False == is_setup_test_active('')
+        >>> assert False == is_setup_test_active('setup.py')
+        >>> assert True == is_setup_test_active('setup.py test')
+
         """
 
 - add a path to the syspath
 
 .. code-block:: python
 
     def add_path_to_syspath(path_to_append: PathLikeOrString) -> None:
@@ -412,26 +426,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.5
 ---------
 2023-07-11:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove mypy.ini
     - remove pytest.ini
     - remove setup.cfg
     - remove setup.py
     - remove .bettercodehub.yml
     - remove .travis.yml
     - update black config
+    - clean ./tests/test_cli.py
 
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
```

### Comparing `lib_detect_testenv-2.0.5/PULL_REQUEST_TEMPLATE.md` & `lib_detect_testenv-2.0.6/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/README.rst` & `lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,34 @@
+Metadata-Version: 2.1
+Name: lib-detect-testenv
+Version: 2.0.6
+Summary: detects if pytest or doctest or pyrunner on pycharm is running
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_detect_testenv
+Project-URL: Documentation, https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_detect_testenv.git
+Project-URL: Changelog, https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8.0
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
 lib_detect_testenv
 ==================
 
 
-Version v2.0.5 as of 2023-07-11 see `Changelog`_
+Version v2.0.6 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -52,17 +74,17 @@
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -137,14 +159,18 @@
         True if docrunner is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert False == is_doctest_active(arg_string="")
+        >>> assert True == is_doctest_active(arg_string="docrunner.py")
+        >>> assert True == is_doctest_active(arg_string="doctest.py")
+
         """
 
 - detect if pytest is active
 
 .. code-block:: python
 
     def is_pytest_active(arg_string: Optional[str] = None) -> bool:
@@ -162,14 +188,17 @@
         True if pytest is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert True == is_pytest_active(arg_string='pytest.py')
+        >>> assert True == is_pytest_active(arg_string='/pytest/__main__.py')
+
         """
 
 - detect if setup.py is active
 
 .. code-block:: python
 
     def is_setup_active(arg_string: Optional[str] = None) -> bool:
@@ -187,14 +216,17 @@
         True if setup.py is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert False == is_setup_active(arg_string="")
+        >>> assert True == is_setup_active(arg_string="setup.py")
+
         """
 
 - detect if "setup.py test" is active
 
 .. code-block:: python
 
     def is_setup_test_active(arg_string: Optional[str] = None) -> bool:
@@ -212,14 +244,18 @@
         True if "setup.py test" is detected
 
 
         Exceptions
         ----------
         none
 
+        >>> assert False == is_setup_test_active('')
+        >>> assert False == is_setup_test_active('setup.py')
+        >>> assert True == is_setup_test_active('setup.py test')
+
         """
 
 - add a path to the syspath
 
 .. code-block:: python
 
     def add_path_to_syspath(path_to_append: PathLikeOrString) -> None:
@@ -390,26 +426,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.5
 ---------
 2023-07-11:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove mypy.ini
     - remove pytest.ini
     - remove setup.cfg
     - remove setup.py
     - remove .bettercodehub.yml
     - remove .travis.yml
     - update black config
+    - clean ./tests/test_cli.py
 
 v2.0.4
 ---------
 2023-06-26: suppress upload of .egg files to pypi.org
 
 v2.0.3
 ---------
```

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv/3rd_party_stubs/readme.txt` & `lib_detect_testenv-2.0.6/lib_detect_testenv/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv/__init__.py` & `lib_detect_testenv-2.0.6/lib_detect_testenv/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv/__init__conf__.py` & `lib_detect_testenv-2.0.6/lib_detect_testenv/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_detect_testenv'
 title = 'detects if pytest or doctest or pyrunner on pycharm is running'
-version = 'v2.0.5'
+version = 'v2.0.6'
 url = 'https://github.com/bitranox/lib_detect_testenv'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_detect_testenv'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_detect_testenv:
 
     detects if pytest or doctest or pyrunner on pycharm is running
 
-    Version : v2.0.5
+    Version : v2.0.6
     Url     : https://github.com/bitranox/lib_detect_testenv
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv.py` & `lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     True if docrunner is detected
 
 
     Exceptions
     ----------
     none
 
+    >>> assert False == is_doctest_active(arg_string="")
+    >>> assert True == is_doctest_active(arg_string="docrunner.py")
+    >>> assert True == is_doctest_active(arg_string="doctest.py")
+
     """
     # is_doctest_active}}}
 
     arg_string = _get_sys_argv_str(arg_string)
     if "docrunner.py" in arg_string or "doctest.py" in arg_string:
         return True
     return False
@@ -94,24 +98,27 @@
     True if pytest is detected
 
 
     Exceptions
     ----------
     none
 
+    >>> assert True == is_pytest_active(arg_string='pytest.py')
+    >>> assert True == is_pytest_active(arg_string='/pytest/__main__.py')
+
     """
     # is_pytest_active}}}
 
     arg_string = _get_sys_argv_str(arg_string)
     # this is used in our tests when we test cli-commands
     if os.getenv("PYTEST_IS_RUNNING"):
         return True
     if ("pytest.py" in arg_string) or ("/pytest/__main__.py" in arg_string):
         return True
-    return False
+    return False            # pragma: no cover
 
 
 # is_setup_active{{{
 def is_setup_active(arg_string: Optional[str] = None) -> bool:
     """
     returns True if "setup.py" is detected
 
@@ -126,14 +133,17 @@
     True if setup.py is detected
 
 
     Exceptions
     ----------
     none
 
+    >>> assert False == is_setup_active(arg_string="")
+    >>> assert True == is_setup_active(arg_string="setup.py")
+
     """
     # is_setup_active}}}
     arg_string = _get_sys_argv_str(arg_string)
     return "setup.py" in arg_string
 
 
 # is_setup_test_active{{{
@@ -152,14 +162,18 @@
     True if "setup.py test" is detected
 
 
     Exceptions
     ----------
     none
 
+    >>> assert False == is_setup_test_active('')
+    >>> assert False == is_setup_test_active('setup.py')
+    >>> assert True == is_setup_test_active('setup.py test')
+
     """
     # is_setup_test_active}}}
     arg_string = _get_sys_argv_str(arg_string)
     if "setup.py" in arg_string:
         arg_string_remaining = arg_string.split("setup.py")[1].strip()
         if arg_string_remaining.startswith("test"):
             return True
```

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv/lib_detect_testenv_cli.py` & `lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv_cli.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv.egg-info/SOURCES.txt` & `lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/lib_detect_testenv.ipynb` & `lib_detect_testenv-2.0.6/lib_detect_testenv.ipynb`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/pyproject.toml` & `lib_detect_testenv-2.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 name = "lib_detect_testenv"
 authors = [
     {name = "Robert Nowotny", email = "bitranox@gmail.com"},
 ]
 description = "detects if pytest or doctest or pyrunner on pycharm is running"
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
@@ -25,15 +25,15 @@
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
 ]
-version = "v2.0.5"
+version = "v2.0.6"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_detect_testenv"
 Documentation = "https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_detect_testenv.git"
```

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/lib_bash_functions.sh` & `lib_detect_testenv-2.0.6/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/run_pytest.sh` & `lib_detect_testenv-2.0.6/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop.sh` & `lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/run_testloop_windows.cmd` & `lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/shellcheck.sh` & `lib_detect_testenv-2.0.6/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/local_testscripts/testing_tools.py` & `lib_detect_testenv-2.0.6/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.5/tests/test_cli.py` & `lib_detect_testenv-2.0.6/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,12 @@
         subprocess.run(command, shell=True, check=True)
     except subprocess.CalledProcessError:
         return False
     return True
 
 
 def test_cli_commands() -> None:
-    # due to a bug in python 3.8.1 with setup.py test on travis we need to cancel the click tests there !
-    if sys.version_info < (3, 8, 1) or sys.version_info >= (3, 8, 2):
-        assert not call_cli_command("--unknown_option")
-        assert call_cli_command("--version")
-        assert call_cli_command("-h")
-        assert call_cli_command("info")
-        assert call_cli_command("--traceback info")
+    assert not call_cli_command("--unknown_option")
+    assert call_cli_command("--version")
+    assert call_cli_command("-h")
+    assert call_cli_command("info")
+    assert call_cli_command("--traceback info")
```

