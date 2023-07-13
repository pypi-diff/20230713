# Comparing `tmp/lib_programname-2.0.7.tar.gz` & `tmp/lib_programname-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_programname-2.0.7.tar", last modified: Wed Jul 12 19:23:37 2023, max compression
+gzip compressed data, was "lib_programname-2.0.8.tar", last modified: Thu Jul 13 17:14:47 2023, max compression
```

## Comparing `lib_programname-2.0.7.tar` & `lib_programname-2.0.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.101968 lib_programname-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.093968 lib_programname-2.0.7/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/badges_project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.085968 lib_programname-2.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.093968 lib_programname-2.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-12 19:22:50.000000 lib_programname-2.0.7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 19:22:50.000000 lib_programname-2.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 19:22:50.000000 lib_programname-2.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 19:22:50.000000 lib_programname-2.0.7/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 19:22:50.000000 lib_programname-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 19:22:50.000000 lib_programname-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-12 19:22:50.000000 lib_programname-2.0.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-12 19:23:37.101968 lib_programname-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 19:22:50.000000 lib_programname-2.0.7/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-12 19:23:24.000000 lib_programname-2.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 19:22:50.000000 lib_programname-2.0.7/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/lib_programname/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/lib_programname/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/lib_programname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/lib_programname_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/lib_programname.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-12 19:22:50.000000 lib_programname-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 19:22:50.000000 lib_programname-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 19:22:50.000000 lib_programname-2.0.7/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:23:37.101968 lib_programname-2.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.101968 lib_programname-2.0.7/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.346317 lib_programname-2.0.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/.docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/README_template.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/acknowledgment.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2097 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/badges.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/badges_project.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/commandline_help.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/contribute.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/description.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/installation_via_makefile.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      294 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/installation_via_pypi.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/licence_mit.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      395 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/tested_under.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/try_in_jupyter.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      204 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.334316 lib_programname-2.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2457 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.github/workflows/codeql-analysis.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8780 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-07-13 17:13:47.000000 lib_programname-2.0.8/CHANGES.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-07-13 17:13:47.000000 lib_programname-2.0.8/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-07-13 17:13:47.000000 lib_programname-2.0.8/CONTRIBUTING.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-13 17:13:47.000000 lib_programname-2.0.8/ISSUE_TEMPLATE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-07-13 17:13:47.000000 lib_programname-2.0.8/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-07-13 17:13:47.000000 lib_programname-2.0.8/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-07-13 17:13:47.000000 lib_programname-2.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-13 17:14:47.346317 lib_programname-2.0.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-13 17:13:47.000000 lib_programname-2.0.8/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10369 2023-07-13 17:13:47.000000 lib_programname-2.0.8/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-13 17:13:47.000000 lib_programname-2.0.8/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/lib_programname/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/lib_programname/3rd_party_stubs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/3rd_party_stubs/readme.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/__init__conf__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7510 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/lib_programname.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/lib_programname_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/lib_programname.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2541 2023-07-13 17:13:47.000000 lib_programname-2.0.8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-13 17:13:47.000000 lib_programname-2.0.8/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-07-13 17:13:47.000000 lib_programname-2.0.8/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:14:47.346317 lib_programname-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/tests/local_testscripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9587 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/lib_bash_functions.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_pytest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_testloop.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      878 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_testloop_windows.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/shellcheck.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5620 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/testing_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/test_cli.py
```

### Comparing `lib_programname-2.0.7/.coveragerc` & `lib_programname-2.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/.docs/README_template.rst` & `lib_programname-2.0.8/.docs/README_template.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 lib_programname
 ===============
 
 
-Version v2.0.7 as of 2023-07-12 see `Changelog`_
+Version v2.0.8 as of 2023-07-13 see `Changelog`_
 
 
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

### Comparing `lib_programname-2.0.7/.docs/badges.rst` & `lib_programname-2.0.8/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/.docs/badges_project.rst` & `lib_programname-2.0.8/.docs/badges_project.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/.docs/description.rst` & `lib_programname-2.0.8/.docs/description.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/.docs/installation.rst` & `lib_programname-2.0.8/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/.github/workflows/codeql-analysis.yml` & `lib_programname-2.0.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/.github/workflows/python-package.yml` & `lib_programname-2.0.8/.github/workflows/python-package.yml`

 * *Files 2% similar despite different names*

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

### Comparing `lib_programname-2.0.7/.gitignore` & `lib_programname-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/CHANGES.rst` & `lib_programname-2.0.8/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.8
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.7
 ---------
 2023-07-12:
     - also works now with symlinks
     - also works now with scripts and symlinks which do not have a ``py`` extension
     - clean ./tests/test_cli.py
```

### Comparing `lib_programname-2.0.7/CODE_OF_CONDUCT.md` & `lib_programname-2.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/CONTRIBUTING.md` & `lib_programname-2.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/ISSUE_TEMPLATE.md` & `lib_programname-2.0.8/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/LICENSE` & `lib_programname-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/Makefile` & `lib_programname-2.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/PKG-INFO` & `lib_programname-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib_programname
-Version: 2.0.7
+Version: 2.0.8
 Summary: get reliably the name of the executed script
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_programname
 Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_programname.git
 Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
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
 
 lib_programname
 ===============
 
 
-Version v2.0.7 as of 2023-07-12 see `Changelog`_
+Version v2.0.8 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -128,17 +128,17 @@
     /Users/tester/testme
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -297,14 +297,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.8
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.7
 ---------
 2023-07-12:
     - also works now with symlinks
     - also works now with scripts and symlinks which do not have a ``py`` extension
     - clean ./tests/test_cli.py
```

### Comparing `lib_programname-2.0.7/PULL_REQUEST_TEMPLATE.md` & `lib_programname-2.0.8/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/README.rst` & `lib_programname-2.0.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_programname
 ===============
 
 
-Version v2.0.7 as of 2023-07-12 see `Changelog`_
+Version v2.0.8 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -106,17 +106,17 @@
     /Users/tester/testme
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -275,14 +275,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.8
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.7
 ---------
 2023-07-12:
     - also works now with symlinks
     - also works now with scripts and symlinks which do not have a ``py`` extension
     - clean ./tests/test_cli.py
```

### Comparing `lib_programname-2.0.7/lib_programname/3rd_party_stubs/readme.txt` & `lib_programname-2.0.8/lib_programname/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/lib_programname/__init__.py` & `lib_programname-2.0.8/lib_programname/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/lib_programname/__init__conf__.py` & `lib_programname-2.0.8/lib_programname/__init__conf__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_programname'
 title = 'get reliably the name of the executed script'
-version = 'v2.0.7'
+version = 'v2.0.8'
 url = 'https://github.com/bitranox/lib_programname'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_programname'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_programname:
 
     get reliably the name of the executed script
 
-    Version : v2.0.7
+    Version : v2.0.8
     Url     : https://github.com/bitranox/lib_programname
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_programname-2.0.7/lib_programname/lib_programname.py` & `lib_programname-2.0.8/lib_programname/lib_programname.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/lib_programname/lib_programname_cli.py` & `lib_programname-2.0.8/lib_programname/lib_programname_cli.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/lib_programname.egg-info/PKG-INFO` & `lib_programname-2.0.8/lib_programname.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lib-programname
-Version: 2.0.7
+Version: 2.0.8
 Summary: get reliably the name of the executed script
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_programname
 Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_programname.git
 Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
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
 
 lib_programname
 ===============
 
 
-Version v2.0.7 as of 2023-07-12 see `Changelog`_
+Version v2.0.8 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -128,17 +128,17 @@
     /Users/tester/testme
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -297,14 +297,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.8
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v2.0.7
 ---------
 2023-07-12:
     - also works now with symlinks
     - also works now with scripts and symlinks which do not have a ``py`` extension
     - clean ./tests/test_cli.py
```

### Comparing `lib_programname-2.0.7/lib_programname.egg-info/SOURCES.txt` & `lib_programname-2.0.8/lib_programname.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/lib_programname.ipynb` & `lib_programname-2.0.8/lib_programname.ipynb`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/pyproject.toml` & `lib_programname-2.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 name = "lib_programname"
 authors = [
     {name = "Robert Nowotny", email = "bitranox@gmail.com"},
 ]
 description = "get reliably the name of the executed script"
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
@@ -26,15 +26,15 @@
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
     "lib_detect_testenv",
 ]
-version = "v2.0.7"
+version = "v2.0.8"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_programname"
 Documentation = "https://github.com/bitranox/lib_programname/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_programname.git"
```

### Comparing `lib_programname-2.0.7/tests/local_testscripts/lib_bash_functions.sh` & `lib_programname-2.0.8/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/local_testscripts/run_pytest.sh` & `lib_programname-2.0.8/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/local_testscripts/run_testloop.sh` & `lib_programname-2.0.8/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_programname-2.0.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/local_testscripts/run_testloop_windows.cmd` & `lib_programname-2.0.8/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/local_testscripts/shellcheck.sh` & `lib_programname-2.0.8/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/local_testscripts/testing_tools.py` & `lib_programname-2.0.8/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.7/tests/test_cli.py` & `lib_programname-2.0.8/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 logger = logging.getLogger()
 package_dir = "lib_programname"
 cli_filename = "lib_programname_cli.py"
 
 path_cli_command = pathlib.Path(__file__).resolve().parent.parent / package_dir / cli_filename
 
 
-def call_cli_command(commandline_args: str = "") -> bool:
-    command = " ".join([sys.executable, str(path_cli_command), commandline_args])
+def call_cli_command(commandline_args: str = '') -> bool:
+    command = ' '.join([sys.executable, str(path_cli_command), commandline_args])
     try:
         subprocess.run(command, shell=True, check=True)
     except subprocess.CalledProcessError:
         return False
     return True
 
 
 def test_cli_commands() -> None:
-    assert not call_cli_command("--unknown_option")
-    assert call_cli_command("--version")
-    assert call_cli_command("-h")
-    assert call_cli_command("info")
-    assert call_cli_command("--traceback info")
+    assert not call_cli_command('--unknown_option')
+    assert call_cli_command('--version')
+    assert call_cli_command('-h')
+    assert call_cli_command('info')
+    assert call_cli_command('--traceback info')
```

