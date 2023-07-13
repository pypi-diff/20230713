# Comparing `tmp/pprint3x-3.10.4.2.tar.gz` & `tmp/pprint3x-3.10.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pprint3x-3.10.4.2.tar", last modified: Thu Jun  2 08:42:18 2022, max compression
+gzip compressed data, was "pprint3x-3.10.4.3.tar", last modified: Thu Jul 13 11:09:23 2023, max compression
```

## Comparing `pprint3x-3.10.4.2.tar` & `pprint3x-3.10.4.3.tar`

### file list

```diff
@@ -1,22 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 08:42:18.500279 pprint3x-3.10.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8164 2022-06-02 08:42:18.500279 pprint3x-3.10.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7521 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 08:42:18.496279 pprint3x-3.10.4.2/pprint3x/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/pprint3x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/pprint3x/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23898 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/pprint3x/pprint3x.py
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/pprint3x/pprint3x.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/pprint3x/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 08:42:18.496279 pprint3x-3.10.4.2/pprint3x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8164 2022-06-02 08:42:17.000000 pprint3x-3.10.4.2/pprint3x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-06-02 08:42:18.000000 pprint3x-3.10.4.2/pprint3x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 08:42:17.000000 pprint3x-3.10.4.2/pprint3x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 08:42:16.000000 pprint3x-3.10.4.2/pprint3x.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-02 08:42:18.000000 pprint3x-3.10.4.2/pprint3x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-02 08:42:18.000000 pprint3x-3.10.4.2/pprint3x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-06-02 08:42:18.500279 pprint3x-3.10.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-06-02 08:41:30.000000 pprint3x-3.10.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.385937 pprint3x-3.10.4.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.373937 pprint3x-3.10.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.385937 pprint3x-3.10.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-07-13 11:09:10.000000 pprint3x-3.10.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.385937 pprint3x-3.10.4.3/pprint3x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/pprint3x/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x/pprint3x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x/pprint3x.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/pprint3x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-13 11:09:23.000000 pprint3x-3.10.4.3/pprint3x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-13 11:09:23.000000 pprint3x-3.10.4.3/pprint3x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:09:23.000000 pprint3x-3.10.4.3/pprint3x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-13 11:09:23.000000 pprint3x-3.10.4.3/pprint3x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 11:09:23.000000 pprint3x-3.10.4.3/pprint3x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pprint3x.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:23.389937 pprint3x-3.10.4.3/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-07-13 11:08:37.000000 pprint3x-3.10.4.3/tests/test_pprint.py
```

### Comparing `pprint3x-3.10.4.2/LICENSE` & `pprint3x-3.10.4.3/LICENSE`

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

### Comparing `pprint3x-3.10.4.2/PKG-INFO` & `pprint3x-3.10.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pprint3x
-Version: 3.10.4.2
+Version: 3.10.4.3
 Summary: backport of pprint from python 3.11
-Home-page: https://github.com/bitranox/pprint3x
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/pprint3x
+Project-URL: Documentation, https://github.com/bitranox/pprint3x/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/pprint3x.git
+Project-URL: Changelog, https://github.com/bitranox/pprint3x/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 pprint3x
 ========
 
 
-Version v3.10.4.2 as of 2022-06-02 see `Changelog`_
+Version v3.10.4.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/pprint3x?label=PyPI%20Package
    :target: https://badge.fury.io/py/pprint3x
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/pprint3x
    :target: https://codecov.io/gh/bitranox/pprint3x
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/pprint3x?branch=master
-   :target: https://bettercodehub.com/results/bitranox/pprint3x
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/pprint3x?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/pprint3x/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/pprint3x?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/pprint3x/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/pprint3x?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/pprint3x/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/pprint3x
+.. |snyk| image:: https://snyk.io/test/github/bitranox/pprint3x/badge.svg
    :target: https://snyk.io/test/github/bitranox/pprint3x
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pprint3x
    :target: https://pypi.org/project/pprint3x/
@@ -84,22 +85,22 @@
 * ``pprint.pp`` has been added to pretty-print objects with dictionary
   keys being sorted with their insertion order by default. Parameter
   *sort_dicts* has been added to ``pprint.pprint``, ``pprint.pformat`` and
   ``pprint.PrettyPrinter``. Contributed by Rémi Lapeyre in Python 3.8.
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/pprint3x>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/pprint3x/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -164,14 +165,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade pprint3x
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade pprint3x[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/pprint3x.git
 
@@ -187,22 +195,22 @@
     # for the latest development version :
     pprint3x @ git+https://github.com/bitranox/pprint3x.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/pprint3x.git
     $ cd pprint3x
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -252,14 +260,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.3
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - remove travis config
+    - remove bettercodehub config
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v3.10.4.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v3.10.4.1
 ---------
 2022-06-01: update github actions test matrix
```

### Comparing `pprint3x-3.10.4.2/README.rst` & `pprint3x-3.10.4.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 pprint3x
 ========
 
 
-Version v3.10.4.2 as of 2022-06-02 see `Changelog`_
+Version v3.10.4.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
@@ -23,30 +23,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/pprint3x?label=PyPI%20Package
    :target: https://badge.fury.io/py/pprint3x
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/pprint3x
    :target: https://codecov.io/gh/bitranox/pprint3x
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/pprint3x?branch=master
-   :target: https://bettercodehub.com/results/bitranox/pprint3x
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/pprint3x?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/pprint3x/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/pprint3x?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/pprint3x/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/pprint3x?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/pprint3x/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/pprint3x
+.. |snyk| image:: https://snyk.io/test/github/bitranox/pprint3x/badge.svg
    :target: https://snyk.io/test/github/bitranox/pprint3x
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pprint3x
    :target: https://pypi.org/project/pprint3x/
@@ -66,22 +63,22 @@
 * ``pprint.pp`` has been added to pretty-print objects with dictionary
   keys being sorted with their insertion order by default. Parameter
   *sort_dicts* has been added to ``pprint.pprint``, ``pprint.pformat`` and
   ``pprint.PrettyPrinter``. Contributed by Rémi Lapeyre in Python 3.8.
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/pprint3x>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/pprint3x/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -146,14 +143,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade pprint3x
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade pprint3x[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/pprint3x.git
 
@@ -169,22 +173,22 @@
     # for the latest development version :
     pprint3x @ git+https://github.com/bitranox/pprint3x.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/pprint3x.git
     $ cd pprint3x
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -234,14 +238,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.3
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - remove travis config
+    - remove bettercodehub config
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v3.10.4.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v3.10.4.1
 ---------
 2022-06-01: update github actions test matrix
```

### Comparing `pprint3x-3.10.4.2/pprint3x/pprint3x.py` & `pprint3x-3.10.4.3/pprint3x/pprint3x.py`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.2/pprint3x/pprint3x.pyi` & `pprint3x-3.10.4.3/pprint3x/pprint3x.pyi`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.2/pprint3x.egg-info/PKG-INFO` & `pprint3x-3.10.4.3/pprint3x.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pprint3x
-Version: 3.10.4.2
+Version: 3.10.4.3
 Summary: backport of pprint from python 3.11
-Home-page: https://github.com/bitranox/pprint3x
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/pprint3x
+Project-URL: Documentation, https://github.com/bitranox/pprint3x/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/pprint3x.git
+Project-URL: Changelog, https://github.com/bitranox/pprint3x/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 pprint3x
 ========
 
 
-Version v3.10.4.2 as of 2022-06-02 see `Changelog`_
+Version v3.10.4.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/pprint3x?label=PyPI%20Package
    :target: https://badge.fury.io/py/pprint3x
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/pprint3x
    :target: https://codecov.io/gh/bitranox/pprint3x
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/pprint3x?branch=master
-   :target: https://bettercodehub.com/results/bitranox/pprint3x
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/pprint3x?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/pprint3x/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/pprint3x?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/pprint3x/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/pprint3x?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/pprint3x/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/pprint3x
+.. |snyk| image:: https://snyk.io/test/github/bitranox/pprint3x/badge.svg
    :target: https://snyk.io/test/github/bitranox/pprint3x
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pprint3x
    :target: https://pypi.org/project/pprint3x/
@@ -84,22 +85,22 @@
 * ``pprint.pp`` has been added to pretty-print objects with dictionary
   keys being sorted with their insertion order by default. Parameter
   *sort_dicts* has been added to ``pprint.pprint``, ``pprint.pformat`` and
   ``pprint.PrettyPrinter``. Contributed by Rémi Lapeyre in Python 3.8.
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/pprint3x>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/pprint3x/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -164,14 +165,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade pprint3x
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade pprint3x[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/pprint3x.git
 
@@ -187,22 +195,22 @@
     # for the latest development version :
     pprint3x @ git+https://github.com/bitranox/pprint3x.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/pprint3x.git
     $ cd pprint3x
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -252,14 +260,30 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.3
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+    - remove travis config
+    - remove bettercodehub config
+    - remove "better code" badges
+    - remove python 3.6 tests
+    - adding python 3.11 tests
+    - update pypy tests to 3.9
+
 v3.10.4.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v3.10.4.1
 ---------
 2022-06-01: update github actions test matrix
```

