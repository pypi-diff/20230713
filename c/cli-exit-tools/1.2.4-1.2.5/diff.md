# Comparing `tmp/cli_exit_tools-1.2.4.tar.gz` & `tmp/cli_exit_tools-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_exit_tools-1.2.4.tar", last modified: Wed Jul 12 14:33:52 2023, max compression
+gzip compressed data, was "cli_exit_tools-1.2.5.tar", last modified: Thu Jul 13 17:11:56 2023, max compression
```

## Comparing `cli_exit_tools-1.2.4.tar` & `cli_exit_tools-1.2.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.373497 cli_exit_tools-1.2.4/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.361497 cli_exit_tools-1.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.373497 cli_exit_tools-1.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.377498 cli_exit_tools-1.2.4/cli_exit_tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/cli_exit_tools/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.377498 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.740480 cli_exit_tools-1.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-13 17:11:43.000000 cli_exit_tools-1.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/cli_exit_tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/cli_exit_tools/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/test_cli.py
```

### Comparing `cli_exit_tools-1.2.4/.coveragerc` & `cli_exit_tools-1.2.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/.docs/README_template.rst` & `cli_exit_tools-1.2.5/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 cli_exit_tools
 ==============
 
 
-Version v1.2.4 as of 2023-07-12 see `Changelog`_
+Version v1.2.5 as of 2023-07-13 see `Changelog`_
 
 
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

### Comparing `cli_exit_tools-1.2.4/.docs/badges.rst` & `cli_exit_tools-1.2.5/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/.docs/installation.rst` & `cli_exit_tools-1.2.5/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/.docs/usage.rst` & `cli_exit_tools-1.2.5/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/.github/workflows/codeql-analysis.yml` & `cli_exit_tools-1.2.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/.github/workflows/python-package.yml` & `cli_exit_tools-1.2.5/.github/workflows/python-package.yml`

 * *Files 6% similar despite different names*

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

### Comparing `cli_exit_tools-1.2.4/.gitignore` & `cli_exit_tools-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/CHANGES.rst` & `cli_exit_tools-1.2.5/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.5
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v1.2.4
 ---------
 2023-07-12:
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
 
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
```

### Comparing `cli_exit_tools-1.2.4/CODE_OF_CONDUCT.md` & `cli_exit_tools-1.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/CONTRIBUTING.md` & `cli_exit_tools-1.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/ISSUE_TEMPLATE.md` & `cli_exit_tools-1.2.5/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/LICENSE` & `cli_exit_tools-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/Makefile` & `cli_exit_tools-1.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/PKG-INFO` & `cli_exit_tools-1.2.5/cli_exit_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
-Name: cli_exit_tools
-Version: 1.2.4
+Name: cli-exit-tools
+Version: 1.2.5
 Summary: functions to exit an cli application properly
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/cli_exit_tools
 Project-URL: Documentation, https://github.com/bitranox/cli_exit_tools/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/cli_exit_tools.git
 Project-URL: Changelog, https://github.com/bitranox/cli_exit_tools/blob/master/CHANGES.rst
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
 
 cli_exit_tools
 ==============
 
 
-Version v1.2.4 as of 2023-07-12 see `Changelog`_
+Version v1.2.5 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -79,17 +79,17 @@
 - demo how to integrate into Your cli module (see usage)
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -409,26 +409,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.5
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v1.2.4
 ---------
 2023-07-12:
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
 
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
```

### Comparing `cli_exit_tools-1.2.4/PULL_REQUEST_TEMPLATE.md` & `cli_exit_tools-1.2.5/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/README.rst` & `cli_exit_tools-1.2.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cli_exit_tools
 ==============
 
 
-Version v1.2.4 as of 2023-07-12 see `Changelog`_
+Version v1.2.5 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -57,17 +57,17 @@
 - demo how to integrate into Your cli module (see usage)
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -387,26 +387,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.5
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v1.2.4
 ---------
 2023-07-12:
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
 
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
```

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools/3rd_party_stubs/readme.txt` & `cli_exit_tools-1.2.5/cli_exit_tools/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools/__init__.py` & `cli_exit_tools-1.2.5/cli_exit_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools/__init__conf__.py` & `cli_exit_tools-1.2.5/cli_exit_tools/__init__conf__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'cli_exit_tools'
 title = 'functions to exit an cli application properly'
-version = 'v1.2.4'
+version = 'v1.2.5'
 url = 'https://github.com/bitranox/cli_exit_tools'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'cli_exit_tools'
 
 
 def print_info() -> None:
     print("""\
 
 Info for cli_exit_tools:
 
     functions to exit an cli application properly
 
-    Version : v1.2.4
+    Version : v1.2.5
     Url     : https://github.com/bitranox/cli_exit_tools
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools.py` & `cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools_cli.py` & `cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools_cli.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools.egg-info/PKG-INFO` & `cli_exit_tools-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
-Name: cli-exit-tools
-Version: 1.2.4
+Name: cli_exit_tools
+Version: 1.2.5
 Summary: functions to exit an cli application properly
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/cli_exit_tools
 Project-URL: Documentation, https://github.com/bitranox/cli_exit_tools/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/cli_exit_tools.git
 Project-URL: Changelog, https://github.com/bitranox/cli_exit_tools/blob/master/CHANGES.rst
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
 
 cli_exit_tools
 ==============
 
 
-Version v1.2.4 as of 2023-07-12 see `Changelog`_
+Version v1.2.5 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -79,17 +79,17 @@
 - demo how to integrate into Your cli module (see usage)
 
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.7.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -409,26 +409,33 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.5
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+
 v1.2.4
 ---------
 2023-07-12:
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
 
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
```

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools.egg-info/SOURCES.txt` & `cli_exit_tools-1.2.5/cli_exit_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/cli_exit_tools.ipynb` & `cli_exit_tools-1.2.5/cli_exit_tools.ipynb`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/pyproject.toml` & `cli_exit_tools-1.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 name = "cli_exit_tools"
 authors = [
     {name = "Robert Nowotny", email = "bitranox@gmail.com"},
 ]
 description = "functions to exit an cli application properly"
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
     "lib_detect_testenv",
 ]
-version = "v1.2.4"
+version = "v1.2.5"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/cli_exit_tools"
 Documentation = "https://github.com/bitranox/cli_exit_tools/blob/master/README.rst"
 Repository = "https://github.com/bitranox/cli_exit_tools.git"
```

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/lib_bash_functions.sh` & `cli_exit_tools-1.2.5/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/run_pytest.sh` & `cli_exit_tools-1.2.5/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop.sh` & `cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop_windows.cmd` & `cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/shellcheck.sh` & `cli_exit_tools-1.2.5/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.4/tests/local_testscripts/testing_tools.py` & `cli_exit_tools-1.2.5/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

