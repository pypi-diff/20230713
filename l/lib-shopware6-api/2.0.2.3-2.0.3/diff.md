# Comparing `tmp/lib_shopware6_api-2.0.2.3.tar.gz` & `tmp/lib_shopware6_api-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_shopware6_api-2.0.2.3.tar", last modified: Wed Jun 29 23:23:04 2022, max compression
+gzip compressed data, was "lib_shopware6_api-2.0.3.tar", last modified: Thu Jul 13 14:17:31 2023, max compression
```

## Comparing `lib_shopware6_api-2.0.2.3.tar` & `lib_shopware6_api-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 23:23:04.847515 lib_shopware6_api-2.0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    79682 2022-06-29 23:23:04.847515 lib_shopware6_api-2.0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    79035 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 23:23:04.847515 lib_shopware6_api-2.0.2.3/lib_shopware6_api/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/lib_shopware6_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/lib_shopware6_api_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_currency.py
--rw-r--r--   0 runner    (1001) docker     (121)     4227 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_delivery_time.py
--rw-r--r--   0 runner    (1001) docker     (121)    57284 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_media.py
--rw-r--r--   0 runner    (1001) docker     (121)    26121 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     5082 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_tax.py
--rw-r--r--   0 runner    (1001) docker     (121)     2583 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 23:23:04.847515 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    79682 2022-06-29 23:23:04.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-06-29 23:23:04.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 23:23:04.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-06-29 23:23:04.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 23:23:02.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-29 23:23:04.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-29 23:23:04.000000 lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-29 23:23:04.847515 lib_shopware6_api-2.0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-06-29 23:20:22.000000 lib_shopware6_api-2.0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.581505 lib_shopware6_api-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.573505 lib_shopware6_api-2.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    80717 2023-07-13 14:17:31.581505 lib_shopware6_api-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    79766 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/lib_shopware6_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/lib_shopware6_api/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_delivery_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57284 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api/sub_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    80717 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 14:17:31.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/lib_shopware6_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:17:31.581505 lib_shopware6_api-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:31.577505 lib_shopware6_api-2.0.3/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 14:14:44.000000 lib_shopware6_api-2.0.3/tests/test_cli.py
```

### Comparing `lib_shopware6_api-2.0.2.3/LICENSE` & `lib_shopware6_api-2.0.3/LICENSE`

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

### Comparing `lib_shopware6_api-2.0.2.3/PKG-INFO` & `lib_shopware6_api-2.0.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: lib_shopware6_api
-Version: 2.0.2.3
-Summary: use the shopware 6 api
-Home-page: https://github.com/bitranox/lib_shopware6_api
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
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
 lib_shopware6_api
 =================
 
 
-Version v2.0.2.3 as of 2022-06-30 see `Changelog`_
+Version v2.0.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
@@ -41,30 +23,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-shopware6-api?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_shopware6_api
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_shopware6_api
    :target: https://codecov.io/gh/bitranox/lib_shopware6_api
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_shopware6_api?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_shopware6_api
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_shopware6_api?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_shopware6_api?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_shopware6_api?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_shopware6_api
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_shopware6_api/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_shopware6_api
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-shopware6-api
    :target: https://pypi.org/project/lib-shopware6-api/
@@ -72,22 +51,22 @@
 
 shopware6 higher level API client, based on `lib_shopware_api_base <https://github.com/bitranox/lib_shopware6_api_base>`_
 
 this might be a good example for Your own API Client Functions - to be further extended
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_shopware6_api>`_, flake8 style checking ,mypy static type checking ,
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -1857,14 +1836,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_shopware6_api
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_shopware6_api[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_shopware6_api.git
 
@@ -1880,22 +1866,22 @@
     # for the latest development version :
     lib_shopware6_api @ git+https://github.com/bitranox/lib_shopware6_api.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_shopware6_api.git
     $ cd lib_shopware6_api
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -1949,14 +1935,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.3
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
+v2.0.2.4
+---------
+2023-06-30:
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
 v2.0.2.3
 ---------
 2022-06-30: specify correct "attr" version in requirements
 
 v2.0.2.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
```

### Comparing `lib_shopware6_api-2.0.2.3/README.rst` & `lib_shopware6_api-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,38 @@
+Metadata-Version: 2.1
+Name: lib_shopware6_api
+Version: 2.0.3
+Summary: use the shopware 6 api
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api
+Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api.git
+Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api/blob/master/CHANGES.rst
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
 lib_shopware6_api
 =================
 
 
-Version v2.0.2.3 as of 2022-06-30 see `Changelog`_
+Version v2.0.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
@@ -23,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-shopware6-api?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_shopware6_api
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_shopware6_api
    :target: https://codecov.io/gh/bitranox/lib_shopware6_api
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_shopware6_api?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_shopware6_api
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_shopware6_api?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_shopware6_api?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_shopware6_api?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_shopware6_api
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_shopware6_api/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_shopware6_api
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-shopware6-api
    :target: https://pypi.org/project/lib-shopware6-api/
@@ -54,22 +73,22 @@
 
 shopware6 higher level API client, based on `lib_shopware_api_base <https://github.com/bitranox/lib_shopware6_api_base>`_
 
 this might be a good example for Your own API Client Functions - to be further extended
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_shopware6_api>`_, flake8 style checking ,mypy static type checking ,
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -1839,14 +1858,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_shopware6_api
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_shopware6_api[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_shopware6_api.git
 
@@ -1862,22 +1888,22 @@
     # for the latest development version :
     lib_shopware6_api @ git+https://github.com/bitranox/lib_shopware6_api.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_shopware6_api.git
     $ cd lib_shopware6_api
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -1931,14 +1957,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.3
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
+v2.0.2.4
+---------
+2023-06-30:
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
 v2.0.2.3
 ---------
 2022-06-30: specify correct "attr" version in requirements
 
 v2.0.2.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
```

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/__init__.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/lib_shopware6_api.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/lib_shopware6_api_cli.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/lib_shopware6_api_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)   # type: ignore
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
@@ -47,13 +47,13 @@
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()    # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_currency.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_currency.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_delivery_time.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_delivery_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
         >>> # Test
         >>> my_api.get_delivery_times_sorted_by_min_days()
         [{'name': '...', 'id': '...', 'position': 10}, ...]
 
         """
         # get_delivery_times_sorted_by_min_days}}}
-        days = {"day": 1, "week": 7, "month": 31, "year": 365}
+        days = {"hour": 0.0416667, "day": 1, "week": 7, "month": 31, "year": 365}
         payload = dal.Criteria()
         payload.includes["delivery_time"] = ["id", "name", "min", "unit"]
         l_dict_delivery_times = self.search_delivery_times(payload=payload)
         l_dict_delivery_times = sorted(l_dict_delivery_times, key=lambda dt: dt["min"] * days[dt["unit"]])  # type: ignore
         position = 10
         for delivery_time in l_dict_delivery_times:
             delivery_time["position"] = position
```

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_media.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_media.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_product.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_product.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_tax.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_tax.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api/sub_unit.py` & `lib_shopware6_api-2.0.3/lib_shopware6_api/sub_unit.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.2.3/lib_shopware6_api.egg-info/PKG-INFO` & `lib_shopware6_api-2.0.3/lib_shopware6_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: lib-shopware6-api
-Version: 2.0.2.3
+Version: 2.0.3
 Summary: use the shopware 6 api
-Home-page: https://github.com/bitranox/lib_shopware6_api
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api
+Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api.git
+Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api/blob/master/CHANGES.rst
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
 
 lib_shopware6_api
 =================
 
 
-Version v2.0.2.3 as of 2022-06-30 see `Changelog`_
+Version v2.0.3 as of 2023-07-13 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-shopware6-api?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_shopware6_api
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_shopware6_api
    :target: https://codecov.io/gh/bitranox/lib_shopware6_api
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_shopware6_api?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_shopware6_api
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_shopware6_api?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_shopware6_api?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_shopware6_api?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_shopware6_api
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_shopware6_api/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_shopware6_api
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-shopware6-api
    :target: https://pypi.org/project/lib-shopware6-api/
@@ -72,22 +73,22 @@
 
 shopware6 higher level API client, based on `lib_shopware_api_base <https://github.com/bitranox/lib_shopware6_api_base>`_
 
 this might be a good example for Your own API Client Functions - to be further extended
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_shopware6_api>`_, flake8 style checking ,mypy static type checking ,
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -1857,14 +1858,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_shopware6_api
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_shopware6_api[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_shopware6_api.git
 
@@ -1880,22 +1888,22 @@
     # for the latest development version :
     lib_shopware6_api @ git+https://github.com/bitranox/lib_shopware6_api.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_shopware6_api.git
     $ cd lib_shopware6_api
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -1949,14 +1957,37 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.3
+---------
+2023-07-13:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove setup.cfg
+    - remove setup.py
+    - update black config
+    - clean ./tests/test_cli.py
+
+v2.0.2.4
+---------
+2023-06-30:
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
 v2.0.2.3
 ---------
 2022-06-30: specify correct "attr" version in requirements
 
 v2.0.2.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
```

