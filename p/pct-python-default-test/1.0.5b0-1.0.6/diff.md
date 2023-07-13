# Comparing `tmp/pct_python_default_test-1.0.5b0.tar.gz` & `tmp/pct_python_default_test-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pct_python_default_test-1.0.5b0.tar", last modified: Tue Jul 11 20:36:03 2023, max compression
+gzip compressed data, was "pct_python_default_test-1.0.6.tar", last modified: Thu Jul 13 17:09:37 2023, max compression
```

## Comparing `pct_python_default_test-1.0.5b0.tar` & `pct_python_default_test-1.0.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.362866 pct_python_default_test-1.0.5b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/lib_detect_testenv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/lib_detect_testenv/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/lib_detect_testenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/lib_detect_testenv_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/lib_detect_testenv.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 20:36:03.000000 pct_python_default_test-1.0.5b0/pct_python_default_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.366866 pct_python_default_test-1.0.5b0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:36:03.370866 pct_python_default_test-1.0.5b0/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 20:35:17.000000 pct_python_default_test-1.0.5b0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.991490 pct_python_default_test-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.979489 pct_python_default_test-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-07-13 17:09:37.991490 pct_python_default_test-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/pct_python_default_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/pct_python_default_test/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:09:37.991490 pct_python_default_test-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/test_cli.py
```

### Comparing `pct_python_default_test-1.0.5b0/.coveragerc` & `pct_python_default_test-1.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/.docs/README_template.rst` & `pct_python_default_test-1.0.6/.docs/README_template.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-lib_detect_testenv
-==================
+pct_python_default_test
+=======================
 
 
-Version v2.0.5 as of 2023-07-11 see `Changelog`_
+Version v1.0.6 as of 2023-07-13 see `Changelog`_
 
 
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

### Comparing `pct_python_default_test-1.0.5b0/.docs/installation.rst` & `pct_python_default_test-1.0.6/.docs/installation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -3,43 +3,40 @@
 
 .. code-block::
 
     python -m pip --upgrade pip
     python -m pip --upgrade setuptools
 
 
-.. include:: ./installation_via_pypi.rst
+
 
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
-    python -m pip install --upgrade git+https://github.com/bitranox/lib_detect_testenv.git
+    python -m pip install --upgrade git+https://github.com/bitranox/pct_python_default_test.git
 
 
 - include it into Your requirements.txt:
 
 .. code-block::
 
     # Insert following line in Your requirements.txt:
-    # for the latest Release on pypi:
-    lib_detect_testenv
-
     # for the latest development version :
-    lib_detect_testenv @ git+https://github.com/bitranox/lib_detect_testenv.git
+    pct_python_default_test @ git+https://github.com/bitranox/pct_python_default_test.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
 - to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
-    $ git clone https://github.com/bitranox/lib_detect_testenv.git
-    $ cd lib_detect_testenv
+    $ git clone https://github.com/bitranox/pct_python_default_test.git
+    $ cd pct_python_default_test
     python -m pip install -e .[test]
 
 
 .. include:: ./installation_via_makefile.rst
```

### Comparing `pct_python_default_test-1.0.5b0/.github/workflows/codeql-analysis.yml` & `pct_python_default_test-1.0.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/.github/workflows/python-package.yml` & `pct_python_default_test-1.0.6/.github/workflows/python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./lib_detect_testenv/3rd_party_stubs"
+        MYPYPATH: "./pct_python_default_test/3rd_party_stubs"
 
         # coverage
         DO_COVERAGE: "True"
         DO_COVERAGE_UPLOAD_CODECOV: "True"
         DO_COVERAGE_UPLOAD_CODE_CLIMATE: "True"
 
         # package name
-        PACKAGE_NAME: "lib_detect_testenv"
+        PACKAGE_NAME: "pct_python_default_test"
         # the registered CLI Command
-        CLI_COMMAND: "lib_detect_testenv"
+        CLI_COMMAND: "pct_python_default_test"
         # the source file for rst_include (rebuild rst file includes)
         RST_INCLUDE_SOURCE: "./.docs/README_template.rst"
         # the target file for rst_include (rebuild rst file includes)
         RST_INCLUDE_TARGET: "./README.rst"
         # make Code Coverage Secret available in Environment
         CC_TEST_REPORTER_ID: ${{ secrets.CC_TEST_REPORTER_ID }}
         # make PyPi Password available in Environment
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

### Comparing `pct_python_default_test-1.0.5b0/.gitignore` & `pct_python_default_test-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/CHANGES.rst` & `pct_python_default_test-1.0.6/CHANGES.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 Changelog
-=========
+---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
-v2.0.5
+v1.0.6
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
+v1.0.5
 ---------
-2023-07-11:
+2023-xx-xx:
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
 
-v2.0.4
+v1.0.4
 ---------
-2023-06-26: suppress upload of .egg files to pypi.org
+2023-06-26:
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
 
-v2.0.3
+v1.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
-    - add python 3.11 tests
-    - update to pypy 3.9 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
 
-v2.0.2.2
----------
-2022-06-02: update to github actions checkout@v3 and setup-python@v3
-
-v2.0.2.1
+v1.0.2
 --------
-2022-06-01: update github actions test matrix
+2022-05-20: update github actions test matrix to python 3.10
 
-v2.0.2
+v1.0.1
 --------
 2022-03-29: remedy mypy Untyped decorator makes function "cli_info" untyped
 
-v2.0.1
---------
-2022-03-25: fix github actions windows test
-
-v2.0.0
--------
-2021-11-23:
-    - add "setup.py test" detection
-
-v1.0.2
--------
-2021-11-22:
-    - remove second github action yml
-    - fix "setup.py test"
+v1.0.0
+---------
+2022-03-25: remove listdir of ./dist, moved to lib_cicd_github
 
-v1.0.1
-------
-2021-11-21: implement github actions
+v0.1.1
+---------
+2020-08-01: fix pypi deploy
 
-v1.0.0
-------
-2021-11-19: initial release
+v0.1.0
+--------
+2020-07-31:
+    - change1
+    - change2
+    - ...
```

### Comparing `pct_python_default_test-1.0.5b0/CODE_OF_CONDUCT.md` & `pct_python_default_test-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/CONTRIBUTING.md` & `pct_python_default_test-1.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/ISSUE_TEMPLATE.md` & `pct_python_default_test-1.0.6/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/LICENSE` & `pct_python_default_test-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/Makefile` & `pct_python_default_test-1.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/PULL_REQUEST_TEMPLATE.md` & `pct_python_default_test-1.0.6/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/lib_detect_testenv/3rd_party_stubs/readme.txt` & `pct_python_default_test-1.0.6/pct_python_default_test/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/lib_detect_testenv/lib_detect_testenv_cli.py` & `pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 # OWN
 import cli_exit_tools
 
 # PROJ
 try:
     from . import __init__conf__
-    from . import lib_detect_testenv
+    from . import pct_python_default_test
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
     # imports for doctest
     import __init__conf__  # type: ignore  # pragma: no cover
-    import lib_detect_testenv  # type: ignore  # pragma: no cover
+    import pct_python_default_test  # type: ignore  # pragma: no cover
 
 # CONSTANTS
 CLICK_CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 def info() -> None:
     """
@@ -34,15 +34,15 @@
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
-        # lib_detect_testenv.main()
+        pct_python_default_test.main()
 
 
 @cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)  # type: ignore
 def cli_info() -> None:
     """get program informations"""
     info()
```

### Comparing `pct_python_default_test-1.0.5b0/pyproject.toml` & `pct_python_default_test-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,52 +2,46 @@
 requires = ['setuptools', 'setuptools-scm']
 build-backend = "setuptools.build_meta"
 
 [project]
 # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 name = "pct_python_default_test"
 authors = [
-    {name = "put Your Name here", email = "some_email_address@gmail.com"},
+    {name = "Robert Nowotny", email = "bitranox@gmail.com"},
 ]
 description = "a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template"
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
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
 ]
-version = "v1.0.5b"
+version = "v1.0.6"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
-Homepage = "https://github.com/bitranox/lib_detect_testenv"
-Documentation = "https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst"
-Repository = "https://github.com/bitranox/lib_detect_testenv.git"
-Changelog = "https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst"
+Homepage = "https://github.com/bitranox/pct_python_default_test"
+Documentation = "https://github.com/bitranox/pct_python_default_test/blob/master/README.rst"
+Repository = "https://github.com/bitranox/pct_python_default_test.git"
+Changelog = "https://github.com/bitranox/pct_python_default_test/blob/master/CHANGES.rst"
 
 [project.optional-dependencies]
 test = [
     "black",
     "codecov",
     "coloredlogs",
     "coverage",
@@ -56,18 +50,18 @@
     "pytest",
     "pytest-cov",
     "pytest-runner",
     "readme_renderer",
 ]
 
 [project.scripts]
-    lib_detect_testenv = "lib_detect_testenv.lib_detect_testenv_cli:cli_main"
+    pct_python_default_test = "pct_python_default_test.pct_python_default_test_cli:cli_main"
 
 [tool.setuptools.package-data]
-lib_detect_testenv = [
+pct_python_default_test = [
     "py.typed",
     "*.pyi",
     "__init__.pyi",
 ]
 
 [tool.black]
 line-length = 160
```

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/lib_bash_functions.sh` & `pct_python_default_test-1.0.6/tests/local_testscripts/lib_bash_functions.sh`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 function cleanup() {
   trap '' 2 # disable Ctrl+C
   delete_virtual_environment
   clean_caches
   # delete the link to commandline interface
-  rm -f  /usr/local/bin/lib_detect_testenv
+  rm -f  /usr/local/bin/pct_python_default_test
   cd "${save_dir}" || exit
   trap 2 # enable Ctrl+C
 }
 
 
 function run_black() {
   # run black for *.py files
@@ -228,30 +228,30 @@
   fi
 }
 
 
 function test_commandline_interface_venv() {
   my_banner "test commandline interface on virtual environment"
 
-  clr_green "issuing command : /usr/local/bin/lib_detect_testenv --version"
-  if ! "/usr/local/bin/lib_detect_testenv" --version; then
+  clr_green "issuing command : /usr/local/bin/pct_python_default_test --version"
+  if ! "/usr/local/bin/pct_python_default_test" --version; then
     my_banner_warning "test commandline interface on virtual environment ERROR"
     beep
     sleep "${sleeptime_on_error}"
     return 1
   fi
 }
 
 
 function test_commandline_interface_venv_old() {
   # this will fail if rotek lib directory is in the path - keep this as a reminder
   my_banner "test commandline interface on virtual environment"
 
-  clr_green "issuing command : $HOME/venv/local/bin/lib_detect_testenv --version"
-  if ! "$HOME/venv/local/bin/lib_detect_testenv" --version; then
+  clr_green "issuing command : $HOME/venv/local/bin/pct_python_default_test --version"
+  if ! "$HOME/venv/local/bin/pct_python_default_test" --version; then
     my_banner_warning "test commandline interface on virtual environment ERROR"
     beep
     sleep "${sleeptime_on_error}"
     return 1
   fi
 }
```

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/run_pytest.sh` & `pct_python_default_test-1.0.6/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop.sh` & `pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/run_testloop_windows.cmd` & `pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/shellcheck.sh` & `pct_python_default_test-1.0.6/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/tests/local_testscripts/testing_tools.py` & `pct_python_default_test-1.0.6/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.5b0/tests/test_cli.py` & `pct_python_default_test-1.0.6/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # STDLIB
 import logging
-import os
 import pathlib
 import subprocess
 import sys
 
 logger = logging.getLogger()
-package_dir = "lib_detect_testenv"
-cli_filename = "lib_detect_testenv_cli.py"
-os.environ["PYTEST_IS_RUNNING"] = "True"  # to be able to detect pytest when running the cli command
+package_dir = "pct_python_default_test"
+cli_filename = "pct_python_default_test_cli.py"
 
 path_cli_command = pathlib.Path(__file__).resolve().parent.parent / package_dir / cli_filename
 
 
 def call_cli_command(commandline_args: str = "") -> bool:
     command = " ".join([sys.executable, str(path_cli_command), commandline_args])
     try:
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

