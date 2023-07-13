# Comparing `tmp/pyzenhub-0.3.1.tar.gz` & `tmp/pyzenhub-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzenhub-0.3.1.tar", last modified: Thu May 26 01:15:57 2022, max compression
+gzip compressed data, was "pyzenhub-0.3.2.tar", last modified: Thu Jul 13 16:38:59 2023, max compression
```

## Comparing `pyzenhub-0.3.1.tar` & `pyzenhub-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 01:15:57.127199 pyzenhub-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 01:15:57.119199 pyzenhub-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 01:15:57.123199 pyzenhub-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/.github/workflows/test_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/.github/workflows/test_typing.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-05-26 01:15:57.127199 pyzenhub-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 01:15:57.123199 pyzenhub-0.3.1/pyzenhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-05-26 01:15:56.000000 pyzenhub-0.3.1/pyzenhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-05-26 01:15:57.000000 pyzenhub-0.3.1/pyzenhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 01:15:56.000000 pyzenhub-0.3.1/pyzenhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 01:15:56.000000 pyzenhub-0.3.1/pyzenhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-26 01:15:56.000000 pyzenhub-0.3.1/pyzenhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-26 01:15:57.000000 pyzenhub-0.3.1/pyzenhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-05-26 01:15:57.127199 pyzenhub-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 01:15:57.123199 pyzenhub-0.3.1/zenhub/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-26 01:15:56.000000 pyzenhub-0.3.1/zenhub/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 01:15:57.127199 pyzenhub-0.3.1/zenhub/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     8759 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/epics.py
--rw-r--r--   0 runner    (1001) docker     (121)     9006 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/issues.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/milestones.py
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/release_report_issues.py
--rw-r--r--   0 runner    (1001) docker     (121)    12070 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/release_reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     7616 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/core/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-05-26 01:15:35.000000 pyzenhub-0.3.1/zenhub/utils.py
+drwxr-xr-x   0 gpenacastellanos   (503) staff       (20)        0 2023-07-13 16:38:59.755222 pyzenhub-0.3.2/
+drwxr-xr-x   0 gpenacastellanos   (503) staff       (20)        0 2023-07-13 16:38:59.699929 pyzenhub-0.3.2/.github/
+drwxr-xr-x   0 gpenacastellanos   (503) staff       (20)        0 2023-07-13 16:38:59.718118 pyzenhub-0.3.2/.github/workflows/
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     2949 2023-07-13 16:07:01.000000 pyzenhub-0.3.2/.github/workflows/test_pull_request.yml
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      465 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/.github/workflows/test_typing.yml
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1858 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/.gitignore
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      642 2023-07-13 15:56:21.000000 pyzenhub-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)       12 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/CHANGELOG.md
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      396 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1082 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/LICENSE.txt
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      127 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/MANIFEST.in
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     2969 2023-07-13 16:38:59.755970 pyzenhub-0.3.2/PKG-INFO
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1860 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/README.md
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      137 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/RELEASE.md
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      927 2023-07-13 15:58:28.000000 pyzenhub-0.3.2/pyproject.toml
+drwxr-xr-x   0 gpenacastellanos   (503) staff       (20)        0 2023-07-13 16:38:59.726796 pyzenhub-0.3.2/pyzenhub.egg-info/
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     2969 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/pyzenhub.egg-info/PKG-INFO
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      760 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/pyzenhub.egg-info/SOURCES.txt
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)        1 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/pyzenhub.egg-info/dependency_links.txt
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)        1 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/pyzenhub.egg-info/not-zip-safe
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)       63 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/pyzenhub.egg-info/requires.txt
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)        7 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/pyzenhub.egg-info/top_level.txt
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1357 2023-07-13 16:38:59.757906 pyzenhub-0.3.2/setup.cfg
+drwxr-xr-x   0 gpenacastellanos   (503) staff       (20)        0 2023-07-13 16:38:59.735606 pyzenhub-0.3.2/zenhub/
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1059 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/__init__.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      160 2023-07-13 16:38:59.000000 pyzenhub-0.3.2/zenhub/_version.py
+drwxr-xr-x   0 gpenacastellanos   (503) staff       (20)        0 2023-07-13 16:38:59.753204 pyzenhub-0.3.2/zenhub/core/
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1651 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/__init__.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1549 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/base.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     4835 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/dependencies.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     9283 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/epics.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)    10119 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/issues.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     2769 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/milestones.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     3086 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/rate.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     3099 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/release_report_issues.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)    10072 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/release_reports.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     8103 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/core/workspaces.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      215 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/exceptions.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     2787 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/models.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)      272 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/types.py
+-rw-r--r--   0 gpenacastellanos   (503) staff       (20)     1654 2023-07-13 15:44:08.000000 pyzenhub-0.3.2/zenhub/utils.py
```

### Comparing `pyzenhub-0.3.1/.github/workflows/test_pull_request.yml` & `pyzenhub-0.3.2/.github/workflows/test_pull_request.yml`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
     branches:
       - main
     tags:
       - "v*"
   pull_request:
     branches:
       - main
-  pull_request_target:
-    branches:
-      - main
   workflow_dispatch:
 
+
 jobs:
   pre-commit:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
           python-version: 3.9
       - name: Install package
-        run: pip install -e .
+        run: |
+          pip install --upgrade pip
+          pip install -e .
       - name: Install dependencies
         run: pip install pre-commit
       - name: Run pre-commit
         env:
           ZENHUB_TEST_TOKEN:  ${{ secrets.ZENHUB_TEST_TOKEN }}
         run: pre-commit run -a
 
@@ -35,41 +35,45 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
           python-version: 3.9
       - name: Install package
-        run: pip install -e .
+        run: |
+          pip install --upgrade pip
+          pip install -e .
       - name: Install dependencies
         run: pip install check-manifest
       - name: Run check
         run: check-manifest
 
   test:
     name: ${{ matrix.python }}
     runs-on: ubuntu-latest
     needs: pre-commit
     strategy:
       fail-fast: false
       matrix:
-        python: ["3.10"]
+        python: ["3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
       - name: Install package
-        run: pip install -e .
+        run: |
+          pip install --upgrade pip
+          pip install -e .
       - name: Install dependencies
         run: pip install pytest pytest-cov
       - name: Run pytest
         env:
           ZENHUB_TEST_TOKEN:  ${{ secrets.ZENHUB_TEST_TOKEN }}
-        run: pytest tests --cov=zenhub --cov-report term-missing
+        run: pytest tests --cov=zenhub --cov=tests --cov-report term-missing:skip-covered
       - uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
           name: codecov-umbrella
           fail_ci_if_error: true
           verbose: true
```

### Comparing `pyzenhub-0.3.1/.gitignore` & `pyzenhub-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyzenhub-0.3.1/.pre-commit-config.yaml` & `pyzenhub-0.3.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 -   repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     - id: isort
 -   repo: https://github.com/psf/black
     rev: 22.3.0
     hooks:
     - id: black
       pass_filenames: true
```

### Comparing `pyzenhub-0.3.1/LICENSE.txt` & `pyzenhub-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyzenhub-0.3.1/PKG-INFO` & `pyzenhub-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pyzenhub
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python bindings to the Zenhub API
 Home-page: https://github.com/goanpeca/pyzenhub
 Author: Gonzalo Pena-Castellanos
 Author-email: goanpeca@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/goanpeca/pyzenhub
 Project-URL: Tracker, https://github.com/goanpeca/pyzenhub/issues
 Project-URL: Changelog, https://github.com/goanpeca/pyzenhub/blob/main/CHANGELOG.md
 Keywords: zenhub,api
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -29,46 +28,58 @@
 # PyZenHub
 
 Python bindings to the Zenhub API.
 
 ## Project status
 
 [![License](https://img.shields.io/pypi/l/pyzenhub.svg?color=green)](https://github.com/goanpeca/pyzenhub/raw/main/LICENSE.txt)
-[![PyPI](https://img.shields.io/pypi/v/pyzenhub.svg?color=green)](https://pypi.org/project/puzenhub)
+[![PyPI](https://img.shields.io/pypi/v/pyzenhub.svg?color=green)](https://pypi.org/project/pyzenhub)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/pyzenhub.svg?color=green)](https://python.org)
-[![PR Test](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml/badge.svg?branch=main)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml)
+[![Tests](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml/badge.svg?branch=main)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml)
+[![Typing](https://github.com/goanpeca/pyzenhub/actions/workflows/test_typing.yml/badge.svg)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_typing.yml)
 [![codecov](https://codecov.io/gh/goanpeca/pyzenhub/branch/main/graph/badge.svg?token=dcsjgl1sOi)](https://codecov.io/gh/goanpeca/pyzenhub)
 
 ## Usage
 
 ```python
 from zenhub import Zenhub
 
-zh = Zenhub(<zenhub_token>)
-zh.get_epics(<repo_id>)
+zh = Zenhub('<zenhub_token>')
+zh.get_epics('<repo_id>')  # Dictionary
 ```
 
-For enterprise installs:
+Return models instead of dictionaries
 
 ```python
 from zenhub import Zenhub
 
-zh = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>)
-zh.get_epics(<repo_id>)
+zh = Zenhub('<zenhub_token>', return_models=True)
+zh.get_epics('<repo_id>')  # Pydantic model!
 ```
 
-To select the enterprise version use the `enterprise` parameter. 
+*Methods will always return dates as `datetime.datetime` objects, not strings.*
+
+### For enterprise installs
+
+```python
+from zenhub import Zenhub
+
+zh = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>')
+zh.get_epics('<repo_id>')
+```
+
+To select the enterprise version use the `enterprise` parameter.
 
 ```python
 from zenhub import Zenhub
 
-zh2 = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>, enterprise=2)
-zh.get_epics(<repo_id>)
+zh2 = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>', enterprise=2)
+zh.get_epics('<repo_id>')
 
-zh3 = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>, enterprise=3)
-zh.get_epics(<repo_id>)
+zh3 = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>', enterprise=3)
+zh.get_epics('<repo_id>')
 ```
 
 ## Documentation
 
 See [ZenHub official API documentation](https://github.com/ZenHubIO/API).
```

### Comparing `pyzenhub-0.3.1/README.md` & `pyzenhub-0.3.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 # PyZenHub
 
 Python bindings to the Zenhub API.
 
 ## Project status
 
 [![License](https://img.shields.io/pypi/l/pyzenhub.svg?color=green)](https://github.com/goanpeca/pyzenhub/raw/main/LICENSE.txt)
-[![PyPI](https://img.shields.io/pypi/v/pyzenhub.svg?color=green)](https://pypi.org/project/puzenhub)
+[![PyPI](https://img.shields.io/pypi/v/pyzenhub.svg?color=green)](https://pypi.org/project/pyzenhub)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/pyzenhub.svg?color=green)](https://python.org)
-[![PR Test](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml/badge.svg?branch=main)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml)
+[![Tests](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml/badge.svg?branch=main)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml)
+[![Typing](https://github.com/goanpeca/pyzenhub/actions/workflows/test_typing.yml/badge.svg)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_typing.yml)
 [![codecov](https://codecov.io/gh/goanpeca/pyzenhub/branch/main/graph/badge.svg?token=dcsjgl1sOi)](https://codecov.io/gh/goanpeca/pyzenhub)
 
 ## Usage
 
 ```python
 from zenhub import Zenhub
 
-zh = Zenhub(<zenhub_token>)
-zh.get_epics(<repo_id>)
+zh = Zenhub('<zenhub_token>')
+zh.get_epics('<repo_id>')  # Dictionary
 ```
 
-For enterprise installs:
+Return models instead of dictionaries
 
 ```python
 from zenhub import Zenhub
 
-zh = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>)
-zh.get_epics(<repo_id>)
+zh = Zenhub('<zenhub_token>', return_models=True)
+zh.get_epics('<repo_id>')  # Pydantic model!
 ```
 
-To select the enterprise version use the `enterprise` parameter. 
+*Methods will always return dates as `datetime.datetime` objects, not strings.*
+
+### For enterprise installs
+
+```python
+from zenhub import Zenhub
+
+zh = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>')
+zh.get_epics('<repo_id>')
+```
+
+To select the enterprise version use the `enterprise` parameter.
 
 ```python
 from zenhub import Zenhub
 
-zh2 = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>, enterprise=2)
-zh.get_epics(<repo_id>)
+zh2 = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>', enterprise=2)
+zh.get_epics('<repo_id>')
 
-zh3 = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>, enterprise=3)
-zh.get_epics(<repo_id>)
+zh3 = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>', enterprise=3)
+zh.get_epics('<repo_id>')
 ```
 
 ## Documentation
 
 See [ZenHub official API documentation](https://github.com/ZenHubIO/API).
```

### Comparing `pyzenhub-0.3.1/pyproject.toml` & `pyzenhub-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyzenhub-0.3.1/pyzenhub.egg-info/PKG-INFO` & `pyzenhub-0.3.2/pyzenhub.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pyzenhub
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python bindings to the Zenhub API
 Home-page: https://github.com/goanpeca/pyzenhub
 Author: Gonzalo Pena-Castellanos
 Author-email: goanpeca@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/goanpeca/pyzenhub
 Project-URL: Tracker, https://github.com/goanpeca/pyzenhub/issues
 Project-URL: Changelog, https://github.com/goanpeca/pyzenhub/blob/main/CHANGELOG.md
 Keywords: zenhub,api
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -29,46 +28,58 @@
 # PyZenHub
 
 Python bindings to the Zenhub API.
 
 ## Project status
 
 [![License](https://img.shields.io/pypi/l/pyzenhub.svg?color=green)](https://github.com/goanpeca/pyzenhub/raw/main/LICENSE.txt)
-[![PyPI](https://img.shields.io/pypi/v/pyzenhub.svg?color=green)](https://pypi.org/project/puzenhub)
+[![PyPI](https://img.shields.io/pypi/v/pyzenhub.svg?color=green)](https://pypi.org/project/pyzenhub)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/pyzenhub.svg?color=green)](https://python.org)
-[![PR Test](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml/badge.svg?branch=main)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml)
+[![Tests](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml/badge.svg?branch=main)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_pull_request.yml)
+[![Typing](https://github.com/goanpeca/pyzenhub/actions/workflows/test_typing.yml/badge.svg)](https://github.com/goanpeca/pyzenhub/actions/workflows/test_typing.yml)
 [![codecov](https://codecov.io/gh/goanpeca/pyzenhub/branch/main/graph/badge.svg?token=dcsjgl1sOi)](https://codecov.io/gh/goanpeca/pyzenhub)
 
 ## Usage
 
 ```python
 from zenhub import Zenhub
 
-zh = Zenhub(<zenhub_token>)
-zh.get_epics(<repo_id>)
+zh = Zenhub('<zenhub_token>')
+zh.get_epics('<repo_id>')  # Dictionary
 ```
 
-For enterprise installs:
+Return models instead of dictionaries
 
 ```python
 from zenhub import Zenhub
 
-zh = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>)
-zh.get_epics(<repo_id>)
+zh = Zenhub('<zenhub_token>', return_models=True)
+zh.get_epics('<repo_id>')  # Pydantic model!
 ```
 
-To select the enterprise version use the `enterprise` parameter. 
+*Methods will always return dates as `datetime.datetime` objects, not strings.*
+
+### For enterprise installs
+
+```python
+from zenhub import Zenhub
+
+zh = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>')
+zh.get_epics('<repo_id>')
+```
+
+To select the enterprise version use the `enterprise` parameter.
 
 ```python
 from zenhub import Zenhub
 
-zh2 = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>, enterprise=2)
-zh.get_epics(<repo_id>)
+zh2 = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>', enterprise=2)
+zh.get_epics('<repo_id>')
 
-zh3 = Zenhub(<zenhub_token>, base_url=<enterprise-api-endpoint>, enterprise=3)
-zh.get_epics(<repo_id>)
+zh3 = Zenhub('<zenhub_token>', base_url='<enterprise-api-endpoint>', enterprise=3)
+zh.get_epics('<repo_id>')
 ```
 
 ## Documentation
 
 See [ZenHub official API documentation](https://github.com/ZenHubIO/API).
```

### Comparing `pyzenhub-0.3.1/pyzenhub.egg-info/SOURCES.txt` & `pyzenhub-0.3.2/pyzenhub.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,10 +24,11 @@
 zenhub/utils.py
 zenhub/core/__init__.py
 zenhub/core/base.py
 zenhub/core/dependencies.py
 zenhub/core/epics.py
 zenhub/core/issues.py
 zenhub/core/milestones.py
+zenhub/core/rate.py
 zenhub/core/release_report_issues.py
 zenhub/core/release_reports.py
 zenhub/core/workspaces.py
```

### Comparing `pyzenhub-0.3.1/setup.cfg` & `pyzenhub-0.3.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 description = Python bindings to the Zenhub API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/goanpeca/pyzenhub
 author = Gonzalo Pena-Castellanos
 author_email = goanpeca@gmail.com
 license = MIT
-license_file = LICENSE.txt
+license_files = LICENSE.txt
 classifiers = 
 	Development Status :: 5 - Production/Stable
-	Environment :: X11 Applications :: Qt
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
@@ -27,15 +26,15 @@
 	Tracker = https://github.com/goanpeca/pyzenhub/issues
 	Changelog = https://github.com/goanpeca/pyzenhub/blob/main/CHANGELOG.md
 
 [options]
 packages = find:
 install_requires = 
 	packaging
-	pydantic>=1.5.1
+	pydantic<2
 	requests
 	types-requests
 	typing_extensions
 python_requires = >=3.8
 include_package_data = True
 setup_requires = 
 	setuptools-scm
```

### Comparing `pyzenhub-0.3.1/zenhub/__init__.py` & `pyzenhub-0.3.2/zenhub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzenhub-0.3.1/zenhub/core/__init__.py` & `pyzenhub-0.3.2/zenhub/core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """ZenHub API."""
+from typing import Optional
+
 import requests
 
 from ..types import URLString
 from .dependencies import DependenciesMixin
 from .epics import EpicsMixin
 from .issues import IssuesMixin
 from .milestones import MilestonesMixin
+from .rate import RateMixin
 from .release_report_issues import ReleaseReportIssuesMixin
 from .release_reports import ReleaseReportsMixin
 from .workspaces import WorkspacesMixin
 
 # Constants
 DEFAULT_BASE_URL: URLString = "https://api.zenhub.com"
 
@@ -18,34 +21,42 @@
     IssuesMixin,
     EpicsMixin,
     WorkspacesMixin,
     MilestonesMixin,
     DependenciesMixin,
     ReleaseReportsMixin,
     ReleaseReportIssuesMixin,
+    RateMixin,
 ):
     """Zenhub API wrapper."""
 
     _HEADERS = {
         "Content-Type": "application/json",
         "User-Agent": "ZenHub Python Client",
     }
 
     def __init__(
         self,
         token: str,
         base_url: URLString = DEFAULT_BASE_URL,
         enterprise: int = 2,
+        return_models: bool = False,
     ):
         """ZenHub API wrapper."""
         self._session = requests.Session()
+        self._repo_id: Optional[int] = None
+
+        if base_url == DEFAULT_BASE_URL:
+            self._repo_id = 262640661  # Use ZenHub's default repo ID
+
         if enterprise == 3 and base_url != DEFAULT_BASE_URL:
             if base_url.endswith("/"):
                 base_url = base_url + "api"
             else:
                 base_url = base_url + "/api"
 
         self._base_url = base_url
+        self._output_models = return_models
 
         # Setup
         self._session.headers.update(self._HEADERS)
         self._session.headers.update({"X-Authentication-Token": token})
```

### Comparing `pyzenhub-0.3.1/zenhub/core/base.py` & `pyzenhub-0.3.2/zenhub/core/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+from typing import Optional
+
 import requests
 
 from ..types import URLString
 from ..utils import parse_response_contents
 
 
 class BaseMixin:
     _session: requests.Session
     _base_url: URLString
+    _repo_id: Optional[int]
+    _output_models: bool
 
     def _make_url(self, url: URLString) -> URLString:
         """Create full api url."""
         return f"{self._base_url}{url}"
 
     def _get(self, url: URLString) -> dict:
         """Send GET request with given url."""
```

### Comparing `pyzenhub-0.3.1/zenhub/core/dependencies.py` & `pyzenhub-0.3.2/zenhub/core/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """ZenHub dependencies methods."""
+from typing import Union
+
 from ..models import Dependencies, Dependency
 from .base import BaseMixin
 
 
 class DependenciesMixin(BaseMixin):
-    def get_dependencies(self, repo_id: int) -> dict:
+    def get_dependencies(self, repo_id: int) -> Union[Dependencies, dict]:
         """
         Get Dependencies for a Repository.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        dict
+        Dependencies or dict
             Dictionary of dependencies. See example below.
 
         .. code-block:: python
             {
                 "dependencies": [
                     {
                         "blocking": {
@@ -44,26 +46,30 @@
                 ]
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-dependencies-for-a-repository
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/dependencies
         url = f"/p1/repositories/{repo_id}/dependencies"
         data = self._get(url)
-        return Dependencies.parse_obj(data).dict(include=data.keys())
+        model = Dependencies.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
     def create_dependency(
         self,
         blocking_repo_id: int,
         blocking_issue_number: int,
         blocked_repo_id: int,
         blocked_issue_number: int,
-    ) -> dict:
+    ) -> Union[Dependency, dict]:
         """
         Create a dependency.
 
         Parameters
         ----------
         blocking_repo_id: int
             ID of the repository, not its full name of the blocking issue.
@@ -72,15 +78,15 @@
         blocked_repo_id: int
             ID of the repository, not its full name of the blocked issue.
         blocked_issue_number: int
             Blocked issue number.
 
         Returns
         -------
-        dict
+        Dependency or dict
             Example response.
 
         .. code-block:: python
             {
                 "blocking": {
                     "repo_id": 92563409,
                     "issue_number": 14
@@ -91,28 +97,32 @@
                 }
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#create-a-dependency
         """
+        self._repo_id = blocked_repo_id
         # POST /p1/dependencies
         url = "/p1/dependencies"
         body = {
             "blocking": {
                 "repo_id": blocking_repo_id,
                 "issue_number": blocking_issue_number,
             },
             "blocked": {
                 "repo_id": blocked_repo_id,
                 "issue_number": blocked_issue_number,
             },
         }
         data = self._post(url, body)
-        return Dependency.parse_obj(data).dict(include=data.keys())
+        model = Dependency.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
     def remove_dependency(
         self,
         blocking_repo_id: int,
         blocking_issue_number: int,
         blocked_repo_id: int,
         blocked_issue_number: int,
@@ -136,14 +146,15 @@
         bool
             ``True`` if the dependency was removed.
 
         Note
         ----
         https://github.com/ZenHubIO/API#remove-a-dependency
         """
+        self._repo_id = blocked_repo_id
         # DELETE /p1/dependencies
         url = "/p1/dependencies"
         body = {
             "blocking": {
                 "repo_id": blocking_repo_id,
                 "issue_number": blocking_issue_number,
             },
```

### Comparing `pyzenhub-0.3.1/zenhub/core/epics.py` & `pyzenhub-0.3.2/zenhub/core/epics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """ZenHub epics methods."""
-from typing import Iterable
+from typing import Iterable, Union
 
 from ..models import AddRemoveIssuesEpic, EpicData, Epics, Issue
 from .base import BaseMixin
 
 
 class EpicsMixin(BaseMixin):
-    def get_epics(self, repo_id: int) -> dict:
+    def get_epics(self, repo_id: int) -> Union[Epics, dict]:
         """
         Get all Epics for a repository.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        dict
+        Epics or dict
             See example response below.
 
         .. code-block:: python
             {
                 "epic_issues": [
                     {
                         "issue_number": 3953,
@@ -42,33 +42,39 @@
           number, repository ID, and GitHub issue URL is provided for each
           Epic.
         - If an issue is only an issue belonging to an Epic (and not a parent
           Epic), it is not considered an Epic and won’t be included in the return
           array.
         https://github.com/ZenHubIO/API#get-epics-for-a-repository
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/epics
         url = f"/p1/repositories/{repo_id}/epics"
         data = self._get(url)
-        return Epics.parse_obj(data).dict(include=data.keys())
+        model = Epics.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
-    def get_epic_data(self, repo_id: int, epic_id: int) -> dict:
+    def get_epic_data(
+        self, repo_id: int, epic_id: int
+    ) -> Union[EpicData, dict]:
         """
         Get all Epics for a repository.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
         epic_id : int
             Github issue number of the epic.
 
         Returns
         -------
-        dict
+        EpicData or dict
             See example response below.
 
         .. code-block:: python
             {
                 "total_epic_estimates": {"value": 60},
                 "estimate": {"value": 10},
                 "pipeline": {
@@ -138,18 +144,22 @@
                 ]
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-epic-data
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/epics/:epic_id
         url = f"/p1/repositories/{repo_id}/epics/{epic_id}"
         data = self._get(url)
-        return EpicData.parse_obj(data).dict(include=data.keys())
+        model = EpicData.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
     def convert_epic_to_issue(self, repo_id: int, issue_number: int) -> bool:
         """
         Converts an Epic back to a regular issue.
 
         Parameters
         ----------
@@ -163,14 +173,15 @@
         bool
             ``True`` if successful.
 
         Note
         ----
         https://github.com/ZenHubIO/API#convert-an-epic-to-an-issue
         """
+        self._repo_id = repo_id
         # POST /p1/repositories/:repo_id/epics/:issue_number/convert_to_issue
         url = (
             f"/p1/repositories/{repo_id}/epics/{issue_number}/convert_to_issue"
         )
         data = self._post(url)
         return True if data == {} else False
 
@@ -195,29 +206,30 @@
         bool
             ``True`` if successful.
 
         Note
         ----
         https://github.com/ZenHubIO/API#convert-issue-to-epic
         """
+        self._repo_id = repo_id
         # POST /p1/repositories/:repo_id/issues/:issue_number/convert_to_epic
         url = (
             f"/p1/repositories/{repo_id}/issues/{issue_number}/convert_to_epic"
         )
         body = {"issues": issues}
         data = self._post(url, body=body)
         return bool(data)
 
     def add_or_remove_issues_to_epic(
         self,
         repo_id: int,
         issue_number: int,
         remove_issues: Iterable[Issue] = (),
         add_issues: Iterable[Issue] = (),
-    ) -> dict:
+    ) -> Union[AddRemoveIssuesEpic, dict]:
         """
         Bulk add or remove issues to an Epic.
 
         The result returns which issue was added or removed from the Epic.
 
         Parameters
         ----------
@@ -228,15 +240,15 @@
         remove_issues: Iterable[Issue]
             Issues to remove from epic.
         add_issues: Iterable[Issue]
             Issues to add to epic.
 
         Returns
         -------
-        dict
+        AddRemoveIssuesEpic or dict
             Example response.
 
         .. code-block:: python
             {
                 "removed_issues": [
                     {"repo_id": 3887883, "issue_number": 3}
                 ],
@@ -246,15 +258,19 @@
                 ]
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#add-or-remove-issues-to-epic
         """
+        self._repo_id = repo_id
         # POST /p1/repositories/:repo_id/epics/:issue_number/update_issues
         url = f"/p1/repositories/{repo_id}/epics/{issue_number}/update_issues"
         body = {
             "remove_issues": list(remove_issues),
             "add_issues": list(add_issues),
         }
         data = self._post(url, body=body)
-        return AddRemoveIssuesEpic.parse_obj(data).dict(include=data.keys())
+        model = AddRemoveIssuesEpic.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
```

### Comparing `pyzenhub-0.3.1/zenhub/core/issues.py` & `pyzenhub-0.3.2/zenhub/core/issues.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 """ZenHub issues methods."""
-from typing import Union
+from typing import List, Optional, Union
 
-from ..models import Estimate, IssueData
+from ..models import (
+    Estimate,
+    EstimateIssueEvent,
+    Event,
+    IssueData,
+    TransferIssueEvent,
+)
 from ..types import Base64String, IssuePosition
 from .base import BaseMixin
 
 
 class IssuesMixin(BaseMixin):
-    def get_issue_data(self, repo_id: int, issue_number: int) -> dict:
+    def get_issue_data(
+        self, repo_id: int, issue_number: int
+    ) -> Union[IssueData, dict]:
         """
         Get the data for a specific issue.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
         issue_number : int
             Repository issue number.
 
         Returns
         -------
-        dict
+        IssueData or dict
             The issue data dictionary. See example response below.
 
         .. code-block:: python
             {
                 "estimate": {
                     "value": 8
                 },
@@ -66,33 +74,39 @@
         - Reopened issues might take up to one minute to show up in the
           correct Pipeline.
         - ``pipelines`` contains all pipelines in all Workspaces this issue
           is in.
 
         https://github.com/ZenHubIO/API#get-issue-data
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/issues/:issue_number
         url = f"/p1/repositories/{repo_id}/issues/{issue_number}"
         data = self._get(url)
-        return IssueData.parse_obj(data).dict(include=data.keys())
+        model = IssueData.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
-    def get_issue_events(self, repo_id: int, issue_number: int) -> dict:
+    def get_issue_events(
+        self, repo_id: int, issue_number: int
+    ) -> Union[List[Event], List[dict]]:
         """
         Get the events for an issue.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
         issue_number : int
             Repository issue number.
 
         Returns
         -------
-        dict
+        List of Event or List of dict
             See example response below.
 
         .. code-block:: python
             [
                 {
                     "user_id": 16717,
                     "type": "estimateIssue",
@@ -150,17 +164,30 @@
         - Type can be either estimateIssue or transferIssue. The values before
           and after the event are included in the event data.
         - transferIssue events include a workspace_id indicating in which
           Workspace the transfer occurred.
 
         https://github.com/ZenHubIO/API#get-issue-events
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/issues/:issue_number/events
         url = f"/p1/repositories/{repo_id}/issues/{issue_number}/events"
-        return self._get(url)
+        events: List[dict] = self._get(url)  # type: ignore
+        event_models: List[Event] = []
+        for event in events:
+            event_model: Optional[Event] = None
+            if event["type"] == "estimateIssue":
+                event_model = EstimateIssueEvent.parse_obj(event)
+            elif event["type"] == "transferIssue":
+                event_model = TransferIssueEvent.parse_obj(event)
+
+            if event_model:
+                event_models.append(event_model)
+
+        return event_models if self._output_models else events
 
     def move_issue(
         self,
         workspace_id: Base64String,
         repo_id: int,
         issue_number: int,
         pipeline_id: Base64String,
@@ -182,20 +209,22 @@
         position : int
             Can be specified as top or bottom, or a 0-based position in the
             Pipeline such as 1, which would be the second position in the
             Pipeline.
 
         Returns
         -------
-        ``True`` if successful.
+        bool
+            ``True`` if successful.
 
         Note
         ----
         https://github.com/ZenHubIO/API#move-an-issue-between-pipelines
         """
+        self._repo_id = repo_id
         # POST /p2/workspaces/:workspace_id/repositories/:repo_id/issues/:issue_number/moves
         url = (
             f"/p2/workspaces/{workspace_id}/repositories/"
             f"{repo_id}/issues/{issue_number}/moves"
         )
         body = {"pipeline_id": pipeline_id, "position": position}
         return True if self._post(url, body) == {} else False
@@ -221,51 +250,58 @@
         position : int or IssuePosition
             Can be specified as top or bottom, or a 0-based position in the
             Pipeline such as 1, which would be the second position in the
             Pipeline.
 
         Returns
         -------
-        ``True`` if successful.
+        bool
+            ``True`` if successful.
 
         Note
         ----
         https://github.com/ZenHubIO/API#move-an-issue-between-pipelines-in-the-oldest-workspace
         """
+        self._repo_id = repo_id
         # POST /p1/repositories/:repo_id/issues/:issue_number/moves
         url = f"/p1/repositories/{repo_id}/issues/{issue_number}/moves"
         body = {"pipeline_id": pipeline_id, "position": position}
         return True if self._post(url, body) == {} else False
 
     def set_issue_estimate(
         self, repo_id: int, issue_number: int, estimate: int
-    ) -> dict:
+    ) -> Union[Estimate, dict]:
         """
         Set Issue Estimate.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
         issue_number : int
             Repository issue number.
         estimate : int
             The estimate for the issue.
 
         Returns
         -------
-        Dict. See example response below.
+        Estimate or dict.
+            See example response below.
 
         .. code-block:: python
             {
                 "estimate": 15,
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#set-issue-estimate
         """
+        self._repo_id = repo_id
         # PUT /p1/repositories/:repo_id/issues/:issue_number/estimate
         url = f"/p1/repositories/{repo_id}/issues/{issue_number}/estimate"
         body = {"estimate": estimate}
         data = self._put(url, body)
-        return Estimate.parse_obj(data).dict(include=data.keys())
+        model = Estimate.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
```

### Comparing `pyzenhub-0.3.1/zenhub/core/milestones.py` & `pyzenhub-0.3.2/zenhub/core/milestones.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,95 @@
 """ZenHub milestone methods."""
 import datetime
+from typing import Union
 
 from ..models import MilestoneDate
 from ..utils import date_to_string
 from .base import BaseMixin
 
 
 class MilestonesMixin(BaseMixin):
     def set_milestone_start_date(
         self,
         repo_id: int,
         milestone_number: int,
         start_date: datetime.datetime,
-    ) -> dict:
+    ) -> Union[MilestoneDate, dict]:
         """
         Set milestone start date.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
         milestone_number : int
             ID of the milestone, not its full name.
         start_date : datetime.datetime
             Start date of the milestone.
 
         Returns
         -------
-        dict
+        MilestoneDate or dict
             The milestone with the new start date. See example below.
 
         .. code-block:: python
             {
                 "start_date": "2010-11-13T01:38:56.842Z",
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#set-milestone-start-date
         """
+        self._repo_id = repo_id
         # POST /p1/repositories/:repo_id/milestones/:milestone_number/start_date
         url = (
             f"/p1/repositories/{repo_id}/milestones/"
             f"{milestone_number}/start_date"
         )
         body = {"start_date": date_to_string(start_date)}
         data = self._post(url, body)
-        return MilestoneDate.parse_obj(data).dict(include=data.keys())
+        model = MilestoneDate.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
     def get_milestone_start_date(
         self, repo_id: int, milestone_number: int
-    ) -> dict:
+    ) -> Union[MilestoneDate, dict]:
         """
         Get milestone start date.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
         milestone_number : int
             ID of the milestone, not its full name.
         start_date : datetime.datetime
             Start date of the milestone.
 
         Returns
         -------
-        dict
+        MilestoneDate or dict
             The milestone with the current start date. See example below.
 
         .. code-block:: python
             {
                 "start_date": "2010-11-13T01:38:56.842Z",
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-milestone-start-date
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/milestones/:milestone_number/start_date
         url = (
             f"/p1/repositories/{repo_id}/milestones/"
             f"{milestone_number}/start_date"
         )
         data = self._get(url)
-        return MilestoneDate.parse_obj(data).dict(include=data.keys())
+        model = MilestoneDate.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
```

### Comparing `pyzenhub-0.3.1/zenhub/core/release_report_issues.py` & `pyzenhub-0.3.2/zenhub/core/release_report_issues.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 """ZenHub release report issues methods."""
 
-from typing import Iterable, List
+from typing import Iterable, List, Union
 
 from ..models import AddRemoveIssue, Issue
 from ..types import Base64String
 from .base import BaseMixin
 
 
 class ReleaseReportIssuesMixin(BaseMixin):
     def get_release_report_issues(
         self, release_id: Base64String
-    ) -> List[dict]:
+    ) -> Union[List[Issue], List[dict]]:
         """
         Get all the Issues for a Release Report.
 
         Parameters
         ----------
         release_id : Base64String
             The unique string identifier of the Release Report.
 
         Returns
         -------
-        List of dictionaries. See example response below.
+        List of Issue or List of dictionaries
+            See example response below.
 
         .. code-block:: python
             [
                 { "repo_id": 103707262, "issue_number": 2 },
                 { "repo_id": 103707262, "issue_number": 3 },
             ]
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-all-the-issues-for-a-release-report
         """
         # GET /p1/reports/release/:release_id/issues
         url = f"/p1/reports/release/{release_id}/issues"
-        return [
-            Issue.parse_obj(item).dict(include=item.keys())
-            for item in self._get(url)
-        ]
+        if self._output_models:
+            return [Issue.parse_obj(item) for item in self._get(url)]
+        else:
+            return [
+                Issue.parse_obj(item).dict(include=item.keys())
+                for item in self._get(url)
+            ]
 
     def add_or_remove_issues_from_release_report(
         self,
         release_id: Base64String,
         add_issues: Iterable[Issue] = (),
         remove_issues: Iterable[Issue] = (),
-    ) -> dict:
+    ) -> Union[AddRemoveIssue, dict]:
         """
         Add or Remove Issues to or from a Release Report.
 
         Adding and removing issues can be done in the same request by
         providing both ``add_issues`` and ``remove_issues`` parameters.
 
         Parameters
@@ -61,15 +65,15 @@
             keys to add to the Release Report.
         remove_issues : Iterable of Issue
             An iterable of dictionaries with ``repo_id`` and ``issue_number``
             keys to remove from the Release Report.
 
         Returns
         -------
-        dict
+        AddRemoveIssue or dict
             The added or removed issues. See example response below.
 
         .. code-block:: python
             {
                 "added": [{ "repo_id": 103707262, "issue_number": 3 }],
                 "removed": [],
             }
@@ -81,8 +85,11 @@
         # PATCH /p1/reports/release/:release_id/issues
         url = f"/p1/reports/release/{release_id}/issues"
         body = {
             'add_issues': list(add_issues),
             'remove_issues': list(remove_issues),
         }
         data = self._patch(url, body=body)
-        return AddRemoveIssue.parse_obj(data).dict(include=data.keys())
+        model = AddRemoveIssue.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
```

### Comparing `pyzenhub-0.3.1/zenhub/core/release_reports.py` & `pyzenhub-0.3.2/zenhub/core/release_reports.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """ZenHub release reports methods."""
 import datetime
-from typing import Iterable, List, Optional
+from typing import Iterable, List, Optional, Union
 
-from ..models import AddRemoveIssue, Issue, ReleaseReport
+from ..models import ReleaseReport
 from ..types import Base64String, ReportState
 from ..utils import check_dates, date_to_string
 from .base import BaseMixin
 
 
 class ReleaseReportsMixin(BaseMixin):
     def create_release_report(
         self,
         repo_id: int,
         title: str,
         start_date: datetime.datetime,
         desired_end_date: datetime.datetime,
         description: str = "",
         repositories: Iterable[int] = (),
-    ) -> dict:
+    ) -> Union[ReleaseReport, dict]:
         """
         Create a Release Report.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
@@ -35,15 +35,15 @@
             Start date of the Release Report. The default is ''.
         repositories : Iterable of int, optional
             List of repository IDs to include in the Release Report.
             The default is ().
 
         Returns
         -------
-        ReleaseReportWithRepositories
+        ReleaseReport or dict
             The created Release Report. See example response below.
 
         .. code-block:: python
             {
                 "release_id": "59dff4f508399a35a276a1ea",
                 "title": "Great title",
                 "description": "Amazing description",
@@ -55,14 +55,15 @@
                 "repositories": [103707262]
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#create-a-release-report
         """
+        self._repo_id = repo_id
         check_dates(start_date, desired_end_date)
         # POST /p1/repositories/:repo_id/reports/release
         url = f"/p1/repositories/{repo_id}/reports/release"
         body = {
             "title": title,
             "start_date": date_to_string(start_date),
             "desired_end_date": date_to_string(desired_end_date),
@@ -70,28 +71,33 @@
         if description:
             body["description"] = description
 
         if repositories:
             body["repositories"] = list(repositories)  # type: ignore [assignment]
 
         data = self._post(url, body)
-        return ReleaseReport.parse_obj(data).dict(include=data.keys())
+        model = ReleaseReport.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
-    def get_release_report(self, release_id: Base64String) -> dict:
+    def get_release_report(
+        self, release_id: Base64String
+    ) -> Union[ReleaseReport, dict]:
         """
         Get a Release Report.
 
         Parameters
         ----------
         release_id : Base64String
             The unique string identifier of the Release Report.
 
         Returns
         -------
-        dict
+        ReleaseReport or dict
             The requested Release Report. See example response below.
 
         .. code-block:: python
             {
                 "release_id": "59d3cd520a430a6344fd3bdb",
                 "title": "Test release",
                 "description": "",
@@ -105,28 +111,33 @@
         Note
         ----
         https://github.com/ZenHubIO/API#get-a-release-report
         """
         # GET /p1/reports/release/:release_id
         url = f"/p1/reports/release/{release_id}"
         data = self._get(url)
-        return ReleaseReport.parse_obj(data).dict(include=data.keys())
-
-    def get_release_reports(self, repo_id: int) -> List[dict]:
+        model = ReleaseReport.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
+
+    def get_release_reports(
+        self, repo_id: int
+    ) -> Union[List[ReleaseReport], List[dict]]:
         """
         Get Release Reports for a Repository.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        List of dictionaries. See example response below.
+        List of ReleaseReport or List of dict. See example response below.
 
         .. code-block:: python
             [
                 {
                     "release_id": "59cbf2fde010f7a5207406e8",
                     "title": "Great title for release 1",
                     "description": "Great description for release",
@@ -148,31 +159,34 @@
                 }
             ]
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-release-reports-for-a-repository
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/reports/releases
         url = f"/p1/repositories/{repo_id}/reports/releases"
-        data = [
-            ReleaseReport.parse_obj(item).dict(include=item.keys())
-            for item in self._get(url)
-        ]
-        return data
+        if self._output_models:
+            return [ReleaseReport.parse_obj(item) for item in self._get(url)]
+        else:
+            return [
+                ReleaseReport.parse_obj(item).dict(include=item.keys())
+                for item in self._get(url)
+            ]
 
     def edit_release_report(
         self,
         release_id: Base64String,
         title: str,
         start_date: datetime.datetime,
         desired_end_date: datetime.datetime,
         description: str = '',
         state: Optional[ReportState] = None,
-    ) -> dict:
+    ) -> Union[ReleaseReport, dict]:
         """
         Edit a Release Report.
 
         Parameters
         ----------
         release_id : Base64String
             The unique string identifier of the Release Report.
@@ -185,15 +199,15 @@
         description : str, optional
             Start date of the Release Report. The default is ''.
         state : ReportState, optional
             The state the Release Report. The default is None.
 
         Returns
         -------
-        dict
+        ReleaseReport or dict
             The created Release Report. See example response below.
 
         .. code-block:: python
             {
                 "release_id": "59d3d6438b3f16667f9e7174",
                 "title": "Amazing title",
                 "description": "Amazing description",
@@ -221,15 +235,18 @@
         if state is not None:
             if state in ["open", "closed"]:
                 body["state"] = state
             else:
                 raise ValueError("`state` must be 'open' or 'closed'")
 
         data = self._patch(url, body)
-        return ReleaseReport.parse_obj(data).dict(include=data.keys())
+        model = ReleaseReport.parse_obj(data)
+        return (
+            model if self._output_models else model.dict(include=data.keys())
+        )
 
     def add_repo_to_release_report(
         self, release_id: Base64String, repo_id: int
     ) -> bool:
         """
         Add a Repository to a Release Report.
 
@@ -238,20 +255,22 @@
         release_id : Base64String
             The unique string identifier of the Release Report.
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        ``True`` if successful.
+        bool
+            ``True`` if successful.
 
         Note
         ----
         https://github.com/ZenHubIO/API#add-a-repository-to-a-release-report
         """
+        self._repo_id = repo_id
         # POST /p1/reports/release/:release_id/repository/:repo_id
         url = f"/p1/reports/release/{release_id}/repository/{repo_id}"
         return True if self._post(url) == {} else False
 
     def remove_repo_from_release_report(
         self, release_id: Base64String, repo_id: int
     ) -> bool:
@@ -263,98 +282,19 @@
         release_id : Base64String
             The unique string identifier of the Release Report.
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        ``True`` if successful.
+        bool
+            ``True`` if successful.
 
         Note
         ----
         A release must always have at least one repository.
         https://github.com/ZenHubIO/API#remove-a-repository-from-a-release-report
         """
+        self._repo_id = repo_id
         # DELETE /p1/reports/release/:release_id/repository/:repo_id
         url = f"/p1/reports/release/{release_id}/repository/{repo_id}"
         return True if self._delete(url) == {} else False
-
-    # --- Release Report Issues
-    # ------------------------------------------------------------------------
-    def get_release_report_issues(
-        self, release_id: Base64String
-    ) -> List[dict]:
-        """
-        Get all the Issues for a Release Report.
-
-        Parameters
-        ----------
-        release_id : Base64String
-            The unique string identifier of the Release Report.
-
-        Returns
-        -------
-        List of dictionaries. See example response below.
-
-        .. code-block:: python
-            [
-                { "repo_id": 103707262, "issue_number": 2 },
-                { "repo_id": 103707262, "issue_number": 3 },
-            ]
-
-        Note
-        ----
-        https://github.com/ZenHubIO/API#get-all-the-issues-for-a-release-report
-        """
-        # GET /p1/reports/release/:release_id/issues
-        url = f"/p1/reports/release/{release_id}/issues"
-        return [
-            Issue.parse_obj(item).dict(include=item.keys())
-            for item in self._get(url)
-        ]
-
-    def add_or_remove_issues_from_release_report(
-        self,
-        release_id: Base64String,
-        add_issues: Iterable[Issue] = (),
-        remove_issues: Iterable[Issue] = (),
-    ) -> dict:
-        """
-        Add or Remove Issues to or from a Release Report.
-
-        Adding and removing issues can be done in the same request by
-        providing both ``add_issues`` and ``remove_issues`` parameters.
-
-        Parameters
-        ----------
-        release_id : Base64String
-            The unique string identifier of the Release Report.
-        add_issues : Iterable of Issue
-            An iterable of dictionaries with ``repo_id`` and ``issue_number``
-            keys to add to the Release Report.
-        remove_issues : Iterable of Issue
-            An iterable of dictionaries with ``repo_id`` and ``issue_number``
-            keys to remove from the Release Report.
-
-        Returns
-        -------
-        dict
-            The added or removed issues. See example response below.
-
-        .. code-block:: python
-            {
-                "added": [{ "repo_id": 103707262, "issue_number": 3 }],
-                "removed": [],
-            }
-
-        Note
-        ----
-        https://github.com/ZenHubIO/API#add-or-remove-issues-to-or-from-a-release-report
-        """
-        # PATCH /p1/reports/release/:release_id/issues
-        url = f"/p1/reports/release/{release_id}/issues"
-        body = {
-            'add_issues': list(add_issues),
-            'remove_issues': list(remove_issues),
-        }
-        data = self._patch(url, body)
-        return AddRemoveIssue.parse_obj(data).dict(include=data.keys())
```

### Comparing `pyzenhub-0.3.1/zenhub/core/workspaces.py` & `pyzenhub-0.3.2/zenhub/core/workspaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """ZenHub workspace methods."""
-from typing import List
+from typing import List, Union
 
 from ..models import Board, Workspace
 from ..types import Base64String
 from .base import BaseMixin
 
 
 class WorkspacesMixin(BaseMixin):
-    def get_workspaces(self, repo_id: int) -> List[dict]:
+    def get_workspaces(
+        self, repo_id: int
+    ) -> Union[List[dict], List[Workspace]]:
         """
         Gets all Workspaces containing ``repo_id``.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
@@ -37,39 +39,43 @@
                 }
             ]
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-zenhub-workspaces-for-a-repository
         """
+        self._repo_id = repo_id
         # GET /p2/repositories/:repo_id/workspaces
         url = f"/p2/repositories/{repo_id}/workspaces"
         data = self._get(url)
-        return [
-            Workspace.parse_obj(workspace).dict(include=workspace.keys())
-            for workspace in data
-        ]
+        if self._output_models:
+            return [Workspace.parse_obj(workspace) for workspace in data]
+        else:
+            return [
+                Workspace.parse_obj(workspace).dict(include=workspace.keys())
+                for workspace in data
+            ]
 
     def get_repository_board(
         self, workspace_id: Base64String, repo_id: int
-    ) -> dict:
+    ) -> Union[dict, Board]:
         """
         Get ZenHub Board data for a repository (``repo_id``) within the
         Workspace (``workspace_id``).
 
         Parameters
         ----------
         workspace_id : Base64String
             Workspace unique string identifier.
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        Dictionary with board information.
+        Dictionary or model with board information.
             Zenhub workspace board listing pipelines and issues. See example
             response below.
 
         .. code-block:: python
             {
                 "pipelines": [
                     {
@@ -126,33 +132,37 @@
                 ]
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-a-zenhub-board-for-a-repository
         """
+        self._repo_id = repo_id
         # GET /p2/workspaces/:workspace_id/repositories/:repo_id/board
         url = f"/p2/workspaces/{workspace_id}/repositories/{repo_id}/board"
         data = self._get(url)
-        return Board.parse_obj(data).dict(
-            include=data.keys(), exclude_none=True
+        model = Board.parse_obj(data)
+        return (
+            model
+            if self._output_models
+            else model.dict(include=data.keys(), exclude_none=True)
         )
 
-    def get_oldest_repository_board(self, repo_id: int) -> dict:
+    def get_oldest_repository_board(self, repo_id: int) -> Union[dict, Board]:
         """
         Get the oldest ZenHub board for a repository.
 
         Parameters
         ----------
         repo_id : int
             ID of the repository, not its full name.
 
         Returns
         -------
-        Dictionary with board information.
+        Dictionary or model with board information.
             Zenhub workspace board listing pipelines and issues. See example
             response below.
 
         .. code-block:: python
             {
                 "pipelines": [
                     {
@@ -209,13 +219,17 @@
                 ]
             }
 
         Note
         ----
         https://github.com/ZenHubIO/API#get-the-oldest-zenhub-board-for-a-repository
         """
+        self._repo_id = repo_id
         # GET /p1/repositories/:repo_id/board
         url = f"/p1/repositories/{repo_id}/board"
         data = self._get(url)
-        return Board.parse_obj(data).dict(
-            include=data.keys(), exclude_none=True
+        model = Board.parse_obj(data)
+        return (
+            model
+            if self._output_models
+            else model.dict(include=data.keys(), exclude_none=True)
         )
```

### Comparing `pyzenhub-0.3.1/zenhub/models.py` & `pyzenhub-0.3.2/zenhub/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,59 @@
 """ZenHub API pydantic models."""
+import datetime
 from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
-from .types import Base64String, ISO8601DateString, IssuePosition, URLString
+from .types import (
+    Base64String,
+    ISO8601DateString,
+    IssueEventType,
+    IssuePosition,
+    ReportState,
+    Seconds,
+    URLString,
+)
+
+
+class IssueEstimate(BaseModel):
+    value: int
+
+
+class PipelineName(BaseModel):
+    name: str
+
+
+class Event(BaseModel):
+    user_id: int
+    type: IssueEventType
+    created_at: datetime.datetime
+
+
+class EstimateIssueEvent(Event):
+    from_estimate: Optional[IssueEstimate]
+    to_estimate: Optional[IssueEstimate]
+
+
+class TransferIssueEvent(Event):
+    from_pipeline: Optional[PipelineName]
+    to_pipeline: Optional[PipelineName]
+    workspace_id: Optional[Base64String]
 
 
 class PlusOnes(BaseModel):
     created_at: ISO8601DateString
 
 
 class Pipeline(BaseModel):
     name: str
     pipeline_id: Base64String
     workspace_id: Base64String
 
 
-class IssueEstimate(BaseModel):
-    value: int
-
-
 class IssueData(BaseModel):
     estimate: Optional[IssueEstimate]
     repo_id: Optional[int]
     is_epic: bool
     plus_ones: List[PlusOnes]
     pipeline: Optional[Pipeline]
     pipelines: Optional[List[Pipeline]]
@@ -48,15 +78,15 @@
     release_id: Base64String
     title: str
     description: str
     start_date: ISO8601DateString
     desired_end_date: ISO8601DateString
     created_at: ISO8601DateString
     closed_at: Optional[ISO8601DateString]
-    state: str
+    state: ReportState
     repositories: Optional[List[int]]
 
 
 class Dependency(BaseModel):
     blocking: Issue
     blocked: Issue
 
@@ -78,15 +108,15 @@
 
 class Estimate(BaseModel):
     estimate: int
 
 
 class PipelineIssue(BaseModel):
     issue_number: int
-    estimate: Optional[dict]  # FIXME: IssueEstimate
+    estimate: Optional[IssueEstimate]
     position: Union[IssuePosition, int]
     is_epic: bool
 
 
 class BoardPipeline(BaseModel):
     id: Base64String
     name: str
@@ -109,7 +139,13 @@
 
 class EpicData(BaseModel):
     total_epic_estimates: IssueEstimate
     estimate: Optional[IssueEstimate]
     pipeline: Pipeline
     pipelines: List[Pipeline]
     issues: List[Issue]
+
+
+class RateLimit(BaseModel):
+    limit: int
+    used: int
+    reset: Seconds
```

### Comparing `pyzenhub-0.3.1/zenhub/utils.py` & `pyzenhub-0.3.2/zenhub/utils.py`

 * *Files identical despite different names*

