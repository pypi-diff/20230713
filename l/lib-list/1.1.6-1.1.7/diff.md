# Comparing `tmp/lib_list-1.1.6.tar.gz` & `tmp/lib_list-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_list-1.1.6.tar", last modified: Fri Jun  3 21:36:52 2022, max compression
+gzip compressed data, was "lib_list-1.1.7.tar", last modified: Thu Jul 13 18:40:25 2023, max compression
```

## Comparing `lib_list-1.1.6.tar` & `lib_list-1.1.7.tar`

### file list

```diff
@@ -1,23 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 21:36:52.036041 lib_list-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-06-03 21:36:03.000000 lib_list-1.1.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-03 21:36:03.000000 lib_list-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-03 21:36:03.000000 lib_list-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7945 2022-06-03 21:36:52.036041 lib_list-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7304 2022-06-03 21:36:03.000000 lib_list-1.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 21:36:52.032041 lib_list-1.1.6/lib_list/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-06-03 21:36:03.000000 lib_list-1.1.6/lib_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-03 21:36:03.000000 lib_list-1.1.6/lib_list/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14243 2022-06-03 21:36:03.000000 lib_list-1.1.6/lib_list/lib_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-06-03 21:36:03.000000 lib_list-1.1.6/lib_list/lib_list_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 21:36:03.000000 lib_list-1.1.6/lib_list/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 21:36:52.036041 lib_list-1.1.6/lib_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7945 2022-06-03 21:36:51.000000 lib_list-1.1.6/lib_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-06-03 21:36:52.000000 lib_list-1.1.6/lib_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 21:36:51.000000 lib_list-1.1.6/lib_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-03 21:36:51.000000 lib_list-1.1.6/lib_list.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 21:36:49.000000 lib_list-1.1.6/lib_list.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-03 21:36:51.000000 lib_list-1.1.6/lib_list.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-03 21:36:51.000000 lib_list-1.1.6/lib_list.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-03 21:36:03.000000 lib_list-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-03 21:36:52.036041 lib_list-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-06-03 21:36:03.000000 lib_list-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 18:39:34.000000 lib_list-1.1.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.056002 lib_list-1.1.7/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 18:39:34.000000 lib_list-1.1.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.052002 lib_list-1.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.056002 lib_list-1.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 18:39:34.000000 lib_list-1.1.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-13 18:39:34.000000 lib_list-1.1.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 18:39:34.000000 lib_list-1.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-13 18:39:34.000000 lib_list-1.1.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 18:39:34.000000 lib_list-1.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 18:39:34.000000 lib_list-1.1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 18:39:34.000000 lib_list-1.1.7/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 18:39:34.000000 lib_list-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 18:39:34.000000 lib_list-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 18:39:34.000000 lib_list-1.1.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-13 18:40:25.060002 lib_list-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 18:39:34.000000 lib_list-1.1.7/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-07-13 18:39:34.000000 lib_list-1.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 18:39:34.000000 lib_list-1.1.7/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.056002 lib_list-1.1.7/lib_list/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/lib_list/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/lib_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/lib_list_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/lib_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-13 18:39:34.000000 lib_list-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 18:39:34.000000 lib_list-1.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 18:39:34.000000 lib_list-1.1.7/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:40:25.060002 lib_list-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/test_cli.py
```

### Comparing `lib_list-1.1.6/CHANGES.rst` & `lib_list-1.1.7/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.7
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+
 v1.1.6
 --------
 2022-03-25: implement github actions
 
 v1.1.5
 --------
 2020-10-09: service release
```

### Comparing `lib_list-1.1.6/LICENSE` & `lib_list-1.1.7/LICENSE`

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

### Comparing `lib_list-1.1.6/PKG-INFO` & `lib_list-1.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: lib_list
-Version: 1.1.6
+Version: 1.1.7
 Summary: some convenience functions for lists
-Home-page: https://github.com/bitranox/lib_list
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_list
+Project-URL: Documentation, https://github.com/bitranox/lib_list/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_list.git
+Project-URL: Changelog, https://github.com/bitranox/lib_list/blob/master/CHANGES.rst
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
 
 lib_list
 ========
 
 
-Version v1.1.6 as of 2022-06-03 see `Changelog`_
+Version v1.1.7 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
@@ -41,51 +45,48 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-list?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_list
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_list
    :target: https://codecov.io/gh/bitranox/lib_list
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_list?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_list
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_list?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_list/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_list?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_list/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_list?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_list/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_list
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_list/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_list
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-list
    :target: https://pypi.org/project/lib-list/
    :alt: PyPI - Downloads
 
 some convenience functions for lists
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_list>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_list/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -144,14 +145,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_list
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_list[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_list.git
 
@@ -167,22 +175,22 @@
     # for the latest development version :
     lib_list @ git+https://github.com/bitranox/lib_list.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_list.git
     $ cd lib_list
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -233,14 +241,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.7
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+
 v1.1.6
 --------
 2022-03-25: implement github actions
 
 v1.1.5
 --------
 2020-10-09: service release
```

### Comparing `lib_list-1.1.6/README.rst` & `lib_list-1.1.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 lib_list
 ========
 
 
-Version v1.1.6 as of 2022-06-03 see `Changelog`_
+Version v1.1.7 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
@@ -23,51 +23,48 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-list?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_list
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_list
    :target: https://codecov.io/gh/bitranox/lib_list
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_list?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_list
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_list?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_list/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_list?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_list/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_list?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_list/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_list
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_list/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_list
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-list
    :target: https://pypi.org/project/lib-list/
    :alt: PyPI - Downloads
 
 some convenience functions for lists
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_list>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_list/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -126,14 +123,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_list
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_list[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_list.git
 
@@ -149,22 +153,22 @@
     # for the latest development version :
     lib_list @ git+https://github.com/bitranox/lib_list.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_list.git
     $ cd lib_list
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -215,14 +219,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.7
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+
 v1.1.6
 --------
 2022-03-25: implement github actions
 
 v1.1.5
 --------
 2020-10-09: service release
```

### Comparing `lib_list-1.1.6/lib_list/lib_list.py` & `lib_list-1.1.7/lib_list/lib_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,14 @@
         return l_elements
 
     ls_results: List[str] = []
     for s_element in l_elements:
         if isinstance(s_element, str):
             if fnmatch.fnmatch(s_element, s_fnmatch_searchpattern):
                 ls_results.append(s_element)
-            else:
-                continue
     return ls_results
 
 
 def get_list_elements_containing(l_elements: List[Any], s_search_string: str) -> List[str]:
     """get list elements of type str which contain the searchstring
 
     >>> get_list_elements_containing([], 'bc')
```

### Comparing `lib_list-1.1.6/lib_list/lib_list_cli.py` & `lib_list-1.1.7/lib_list/lib_list_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,32 +27,32 @@
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
 
 
-@cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)
+@cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)      # type: ignore
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

### Comparing `lib_list-1.1.6/lib_list.egg-info/PKG-INFO` & `lib_list-1.1.7/lib_list.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: lib-list
-Version: 1.1.6
+Version: 1.1.7
 Summary: some convenience functions for lists
-Home-page: https://github.com/bitranox/lib_list
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_list
+Project-URL: Documentation, https://github.com/bitranox/lib_list/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_list.git
+Project-URL: Changelog, https://github.com/bitranox/lib_list/blob/master/CHANGES.rst
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
 
 lib_list
 ========
 
 
-Version v1.1.6 as of 2022-06-03 see `Changelog`_
+Version v1.1.7 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
@@ -41,51 +45,48 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-list?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_list
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_list
    :target: https://codecov.io/gh/bitranox/lib_list
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_list?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_list
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_list?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_list/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_list?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_list/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_list?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_list/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_list
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_list/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_list
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-list
    :target: https://pypi.org/project/lib-list/
    :alt: PyPI - Downloads
 
 some convenience functions for lists
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_list>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_list/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -144,14 +145,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_list
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_list[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_list.git
 
@@ -167,22 +175,22 @@
     # for the latest development version :
     lib_list @ git+https://github.com/bitranox/lib_list.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_list.git
     $ cd lib_list
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -233,14 +241,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.7
+---------
+2023-07-13:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+
 v1.1.6
 --------
 2022-03-25: implement github actions
 
 v1.1.5
 --------
 2020-10-09: service release
```

