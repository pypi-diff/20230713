# Comparing `tmp/igittigitt-2.1.2.tar.gz` & `tmp/igittigitt-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/igittigitt-2.1.2.tar", last modified: Sat Jun 25 16:00:02 2022, max compression
+gzip compressed data, was "igittigitt-2.1.3.tar", last modified: Thu Jul 13 17:51:28 2023, max compression
```

## Comparing `igittigitt-2.1.2.tar` & `igittigitt-2.1.3.tar`

### file list

```diff
@@ -1,24 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:00:02.000000 igittigitt-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2022-06-25 15:59:17.000000 igittigitt-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-06-25 15:59:17.000000 igittigitt-2.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    20363 2022-06-25 16:00:02.000000 igittigitt-2.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt/
--rw-r--r--   0 runner    (1001) docker     (121)    24984 2022-06-25 15:59:17.000000 igittigitt-2.1.2/igittigitt/igittigitt.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 15:59:17.000000 igittigitt-2.1.2/igittigitt/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-06-25 15:59:17.000000 igittigitt-2.1.2/igittigitt/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-25 15:59:17.000000 igittigitt-2.1.2/igittigitt/conf_igittigitt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-06-25 15:59:17.000000 igittigitt-2.1.2/igittigitt/igittigitt_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-06-25 15:59:17.000000 igittigitt-2.1.2/igittigitt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-25 15:59:17.000000 igittigitt-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-25 15:59:17.000000 igittigitt-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    19673 2022-06-25 15:59:17.000000 igittigitt-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20363 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 16:00:02.000000 igittigitt-2.1.2/igittigitt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 16:00:01.000000 igittigitt-2.1.2/igittigitt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-25 16:00:02.000000 igittigitt-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-25 15:59:17.000000 igittigitt-2.1.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.489839 igittigitt-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-13 17:50:34.000000 igittigitt-2.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:50:34.000000 igittigitt-2.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:50:34.000000 igittigitt-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:50:34.000000 igittigitt-2.1.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:50:34.000000 igittigitt-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:50:34.000000 igittigitt-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:50:34.000000 igittigitt-2.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-13 17:51:28.505839 igittigitt-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:50:34.000000 igittigitt-2.1.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-07-13 17:50:34.000000 igittigitt-2.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:50:34.000000 igittigitt-2.1.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/igittigitt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/igittigitt/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/conf_igittigitt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/igittigitt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/igittigitt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/igittigitt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-13 17:50:34.000000 igittigitt-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 17:50:34.000000 igittigitt-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:50:34.000000 igittigitt-2.1.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:51:28.505839 igittigitt-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/default_pattern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/default_pattern/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/default_pattern/.config/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/default_pattern/.config/git/ignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/default_pattern/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/default_pattern/git/ignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/.test_gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/.test_gitignore_empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/.test_venv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/.test_venv/some_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/.test_gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/excluded/excluded.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/excluded_not/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/excluded_not/sub_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/excluded_not.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/not_excluded2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/not_excluded2/sub_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/not_excluded2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/test__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/.test_gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/example/test__pycache__/excluded/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/test__pycache__/excluded/excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/excluded/excluded/excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/some_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/example_negation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/example_negation/foo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example_negation/foo/bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example_negation/foo/bar/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example_negation/foo/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example_negation/foo/other/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/testing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/tests/target_expected/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/.test_gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/tests/target_expected/not_excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded/.test_gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded/excluded_not.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded/not_excluded2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/test_pytest.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `igittigitt-2.1.2/CHANGES.rst` & `igittigitt-2.1.3/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v2.1.2
 -------
 2022-06-25:
     - set __all__ accordingly
     - point out limitations in Readme
     - integrate github actions
     - adjusting tests: patterns ending with a point can not match on windows
```

### Comparing `igittigitt-2.1.2/PKG-INFO` & `igittigitt-2.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: igittigitt
-Version: 2.1.2
+Version: 2.1.3
 Summary: A spec-compliant gitignore parser for Python
-Home-page: https://github.com/bitranox/igittigitt
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/igittigitt
+Project-URL: Documentation, https://github.com/bitranox/igittigitt/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/igittigitt.git
+Project-URL: Changelog, https://github.com/bitranox/igittigitt/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 igittigitt
 ==========
 
 
-Version v2.1.2 as of 2022-06-25 see `Changelog`_
+Version v2.1.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
@@ -43,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/igittigitt?label=PyPI%20Package
    :target: https://badge.fury.io/py/igittigitt
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/igittigitt
    :target: https://codecov.io/gh/bitranox/igittigitt
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/igittigitt?branch=master
-   :target: https://bettercodehub.com/results/bitranox/igittigitt
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/igittigitt?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/igittigitt/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/igittigitt?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/igittigitt/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/igittigitt?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/igittigitt/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/igittigitt
+.. |snyk| image:: https://snyk.io/test/github/bitranox/igittigitt/badge.svg
    :target: https://snyk.io/test/github/bitranox/igittigitt
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/igittigitt
    :target: https://pypi.org/project/igittigitt/
@@ -199,22 +198,22 @@
 - synonyms:
     ugh, brr, ugh devil, yuck
 - origin
     probably covering for: o God, ogottogott
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/igittigitt>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/igittigitt/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -418,14 +417,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade igittigitt
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade igittigitt[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/igittigitt.git
 
@@ -441,22 +447,22 @@
     # for the latest development version :
     igittigitt @ git+https://github.com/bitranox/igittigitt.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/igittigitt.git
     $ cd igittigitt
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -510,14 +516,35 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v2.1.2
 -------
 2022-06-25:
     - set __all__ accordingly
     - point out limitations in Readme
     - integrate github actions
     - adjusting tests: patterns ending with a point can not match on windows
@@ -606,9 +633,7 @@
     - implement black codestyle
 
 v0.0.1
 --------
 2020-08-12: initial release
     - fork from https://github.com/mherrmann/gitignore_parser
 
-
-
```

### Comparing `igittigitt-2.1.2/igittigitt/igittigitt.py` & `igittigitt-2.1.3/igittigitt/igittigitt.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.2/igittigitt/igittigitt_cli.py` & `igittigitt-2.1.3/igittigitt/igittigitt_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
 @click.version_option(
     version=__init__conf__.version,
     prog_name=__init__conf__.shell_command,
     message=f"{__init__conf__.shell_command} version {__init__conf__.version}",
 )
 @click.option(
     "--traceback/--no-traceback",
@@ -44,22 +44,22 @@
     help="return traceback information on cli",
 )
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
 
 
-@cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)
+@cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)  # type: ignore
 def cli_info() -> None:
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()  # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `igittigitt-2.1.2/igittigitt/__init__.py` & `igittigitt-2.1.3/igittigitt/__init__.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.2/LICENSE` & `igittigitt-2.1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 1990-2022 Robert Nowotny
+Copyright (c) 1990-2023 Robert Nowotny
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `igittigitt-2.1.2/README.rst` & `igittigitt-2.1.3/igittigitt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,38 @@
+Metadata-Version: 2.1
+Name: igittigitt
+Version: 2.1.3
+Summary: A spec-compliant gitignore parser for Python
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/igittigitt
+Project-URL: Documentation, https://github.com/bitranox/igittigitt/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/igittigitt.git
+Project-URL: Changelog, https://github.com/bitranox/igittigitt/blob/master/CHANGES.rst
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
 igittigitt
 ==========
 
 
-Version v2.1.2 as of 2022-06-25 see `Changelog`_
+Version v2.1.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
@@ -23,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/igittigitt?label=PyPI%20Package
    :target: https://badge.fury.io/py/igittigitt
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/igittigitt
    :target: https://codecov.io/gh/bitranox/igittigitt
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/igittigitt?branch=master
-   :target: https://bettercodehub.com/results/bitranox/igittigitt
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/igittigitt?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/igittigitt/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/igittigitt?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/igittigitt/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/igittigitt?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/igittigitt/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/igittigitt
+.. |snyk| image:: https://snyk.io/test/github/bitranox/igittigitt/badge.svg
    :target: https://snyk.io/test/github/bitranox/igittigitt
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/igittigitt
    :target: https://pypi.org/project/igittigitt/
@@ -179,22 +198,22 @@
 - synonyms:
     ugh, brr, ugh devil, yuck
 - origin
     probably covering for: o God, ogottogott
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/igittigitt>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/igittigitt/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -398,14 +417,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade igittigitt
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade igittigitt[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/igittigitt.git
 
@@ -421,22 +447,22 @@
     # for the latest development version :
     igittigitt @ git+https://github.com/bitranox/igittigitt.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/igittigitt.git
     $ cd igittigitt
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -490,14 +516,35 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v2.1.2
 -------
 2022-06-25:
     - set __all__ accordingly
     - point out limitations in Readme
     - integrate github actions
     - adjusting tests: patterns ending with a point can not match on windows
```

### Comparing `igittigitt-2.1.2/igittigitt.egg-info/PKG-INFO` & `igittigitt-2.1.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,16 @@
-Metadata-Version: 2.1
-Name: igittigitt
-Version: 2.1.2
-Summary: A spec-compliant gitignore parser for Python
-Home-page: https://github.com/bitranox/igittigitt
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 igittigitt
 ==========
 
 
-Version v2.1.2 as of 2022-06-25 see `Changelog`_
+Version v2.1.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
@@ -43,30 +23,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/igittigitt?label=PyPI%20Package
    :target: https://badge.fury.io/py/igittigitt
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/igittigitt
    :target: https://codecov.io/gh/bitranox/igittigitt
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/igittigitt?branch=master
-   :target: https://bettercodehub.com/results/bitranox/igittigitt
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/igittigitt?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/igittigitt/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/igittigitt?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/igittigitt/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/igittigitt?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/igittigitt/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/igittigitt
+.. |snyk| image:: https://snyk.io/test/github/bitranox/igittigitt/badge.svg
    :target: https://snyk.io/test/github/bitranox/igittigitt
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/igittigitt
    :target: https://pypi.org/project/igittigitt/
@@ -199,22 +176,22 @@
 - synonyms:
     ugh, brr, ugh devil, yuck
 - origin
     probably covering for: o God, ogottogott
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/igittigitt>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/igittigitt/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -418,14 +395,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade igittigitt
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade igittigitt[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/igittigitt.git
 
@@ -441,22 +425,22 @@
     # for the latest development version :
     igittigitt @ git+https://github.com/bitranox/igittigitt.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/igittigitt.git
     $ cd igittigitt
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -510,14 +494,35 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v2.1.2
 -------
 2022-06-25:
     - set __all__ accordingly
     - point out limitations in Readme
     - integrate github actions
     - adjusting tests: patterns ending with a point can not match on windows
@@ -606,9 +611,7 @@
     - implement black codestyle
 
 v0.0.1
 --------
 2020-08-12: initial release
     - fork from https://github.com/mherrmann/gitignore_parser
 
-
-
```

