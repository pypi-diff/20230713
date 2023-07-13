# Comparing `tmp/lib_shopware6_api_base-2.1.0.tar.gz` & `tmp/lib_shopware6_api_base-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_shopware6_api_base-2.1.0.tar", last modified: Wed Jun 28 22:17:37 2023, max compression
+gzip compressed data, was "lib_shopware6_api_base-2.1.1.tar", last modified: Thu Jul 13 10:30:58 2023, max compression
```

## Comparing `lib_shopware6_api_base-2.1.0.tar` & `lib_shopware6_api_base-2.1.1.tar`

### file list

```diff
@@ -1,32 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:17:37.951975 lib_shopware6_api_base-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    73220 2023-06-28 22:17:37.951975 lib_shopware6_api_base-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    72550 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:17:37.951975 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/conf_shopware6_api_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    59849 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:17:37.951975 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    73220 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 22:17:37.000000 lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-28 22:17:37.951975 lib_shopware6_api_base-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:17:37.951975 lib_shopware6_api_base-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-28 22:16:27.000000 lib_shopware6_api_base-2.1.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.395977 lib_shopware6_api_base-2.1.1/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.391977 lib_shopware6_api_base-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.395977 lib_shopware6_api_base-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    74216 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    73225 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.395977 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59849 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    74216 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 10:30:58.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:58.399977 lib_shopware6_api_base-2.1.1/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 10:29:38.000000 lib_shopware6_api_base-2.1.1/tests/test_cli.py
```

### Comparing `lib_shopware6_api_base-2.1.0/CHANGES.rst` & `lib_shopware6_api_base-2.1.1/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.1
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
 v2.1.0
 ---------
 2023-06-28:
-    - get rid of TRAVIS
-    - update github actions
     - introduce additional header fields
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
 
 v2.0.9
 ---------
 2022-07-04: support additional query parameters for patch, post ,put and delete requests
 
 v2.0.8
 ---------
```

### Comparing `lib_shopware6_api_base-2.1.0/LICENSE` & `lib_shopware6_api_base-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/PKG-INFO` & `lib_shopware6_api_base-2.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: lib_shopware6_api_base
-Version: 2.1.0
-Summary: python3 base API client for shopware6
-Home-page: https://github.com/bitranox/lib_shopware6_api_base
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.0 as of 2023-06-29 see `Changelog`_
+Version v2.1.1 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -53,15 +35,15 @@
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api_base/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_shopware6_api_base?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_shopware6_api_base
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_shopware6_api_base/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_shopware6_api_base
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-shopware6-api-base
    :target: https://pypi.org/project/lib-shopware6-api-base/
@@ -1888,14 +1870,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_shopware6_api_base
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_shopware6_api_base[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_shopware6_api_base.git
 
@@ -1911,22 +1900,22 @@
     # for the latest development version :
     lib_shopware6_api_base @ git+https://github.com/bitranox/lib_shopware6_api_base.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_shopware6_api_base.git
     $ cd lib_shopware6_api_base
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -1983,20 +1972,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.1
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
 v2.1.0
 ---------
 2023-06-28:
-    - get rid of TRAVIS
-    - update github actions
     - introduce additional header fields
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
 
 v2.0.9
 ---------
 2022-07-04: support additional query parameters for patch, post ,put and delete requests
 
 v2.0.8
 ---------
```

### Comparing `lib_shopware6_api_base-2.1.0/README.rst` & `lib_shopware6_api_base-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,34 @@
+Metadata-Version: 2.1
+Name: lib_shopware6_api_base
+Version: 2.1.1
+Summary: python3 base API client for shopware6
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api_base
+Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api_base.git
+Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api_base/blob/master/CHANGES.rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7.0
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.0 as of 2023-06-29 see `Changelog`_
+Version v2.1.1 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -35,15 +57,15 @@
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api_base/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_shopware6_api_base?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_shopware6_api_base
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_shopware6_api_base/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_shopware6_api_base
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-shopware6-api-base
    :target: https://pypi.org/project/lib-shopware6-api-base/
@@ -1870,14 +1892,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_shopware6_api_base
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_shopware6_api_base[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_shopware6_api_base.git
 
@@ -1893,22 +1922,22 @@
     # for the latest development version :
     lib_shopware6_api_base @ git+https://github.com/bitranox/lib_shopware6_api_base.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_shopware6_api_base.git
     $ cd lib_shopware6_api_base
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -1965,20 +1994,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.1
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
 v2.1.0
 ---------
 2023-06-28:
-    - get rid of TRAVIS
-    - update github actions
     - introduce additional header fields
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
 
 v2.0.9
 ---------
 2022-07-04: support additional query parameters for patch, post ,put and delete requests
 
 v2.0.8
 ---------
```

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/__init__.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/conf_shopware6_api_base_classes.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_classes.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_cli.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
@@ -45,13 +45,13 @@
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()      # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.0/lib_shopware6_api_base.egg-info/PKG-INFO` & `lib_shopware6_api_base-2.1.1/lib_shopware6_api_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: lib-shopware6-api-base
-Version: 2.1.0
+Version: 2.1.1
 Summary: python3 base API client for shopware6
-Home-page: https://github.com/bitranox/lib_shopware6_api_base
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api_base
+Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api_base.git
+Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api_base/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.0 as of 2023-06-29 see `Changelog`_
+Version v2.1.1 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -53,15 +57,15 @@
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api_base/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_shopware6_api_base?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_shopware6_api_base
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_shopware6_api_base/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_shopware6_api_base
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-shopware6-api-base
    :target: https://pypi.org/project/lib-shopware6-api-base/
@@ -1888,14 +1892,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_shopware6_api_base
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_shopware6_api_base[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_shopware6_api_base.git
 
@@ -1911,22 +1922,22 @@
     # for the latest development version :
     lib_shopware6_api_base @ git+https://github.com/bitranox/lib_shopware6_api_base.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_shopware6_api_base.git
     $ cd lib_shopware6_api_base
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -1983,20 +1994,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.1
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
 v2.1.0
 ---------
 2023-06-28:
-    - get rid of TRAVIS
-    - update github actions
     - introduce additional header fields
+    - update black config
+    - remove travis config
+    - remove bettercodehub config
+    - do not upload .egg files to pypi.org
+    - update github actions : checkout@v3 and setup-python@v4
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
 
 v2.0.9
 ---------
 2022-07-04: support additional query parameters for patch, post ,put and delete requests
 
 v2.0.8
 ---------
```

