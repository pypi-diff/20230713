# Comparing `tmp/audinterface-1.0.3.tar.gz` & `tmp/audinterface-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audinterface-1.0.3.tar", last modified: Tue Jun  6 13:30:20 2023, max compression
+gzip compressed data, was "audinterface-1.0.4.tar", last modified: Thu Jul 13 10:15:19 2023, max compression
```

## Comparing `audinterface-1.0.3.tar` & `audinterface-1.0.4.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.562342 audinterface-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.550342 audinterface-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.554342 audinterface-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-06 13:30:07.000000 audinterface-1.0.3/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-06 13:30:07.000000 audinterface-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 13:30:07.000000 audinterface-1.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 13:30:07.000000 audinterface-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 13:30:07.000000 audinterface-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-06 13:30:07.000000 audinterface-1.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-06 13:30:07.000000 audinterface-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-06 13:30:07.000000 audinterface-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-06-06 13:30:20.562342 audinterface-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-06 13:30:07.000000 audinterface-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.554342 audinterface-1.0.3/audinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/audinterface/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/audinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.554342 audinterface-1.0.3/audinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.550342 audinterface-1.0.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/api-src/audinterface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/api-src/audinterface.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/misc/
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-06 13:30:07.000000 audinterface-1.0.3/misc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 13:30:07.000000 audinterface-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-06 13:30:20.562342 audinterface-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 13:30:07.000000 audinterface-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.562342 audinterface-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    39773 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.541213 audinterface-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 10:15:02.000000 audinterface-1.0.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.529214 audinterface-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.533213 audinterface-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 10:15:02.000000 audinterface-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-13 10:15:02.000000 audinterface-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-13 10:15:02.000000 audinterface-1.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-13 10:15:02.000000 audinterface-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 10:15:02.000000 audinterface-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-13 10:15:19.541213 audinterface-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 10:15:02.000000 audinterface-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.533213 audinterface-1.0.4/audinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/audinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32332 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20091 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/audinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.533213 audinterface-1.0.4/audinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.529214 audinterface-1.0.4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/api-src/audinterface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/api-src/audinterface.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-13 10:15:02.000000 audinterface-1.0.4/misc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-13 10:15:02.000000 audinterface-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 10:15:02.000000 audinterface-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:15:19.541213 audinterface-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.541213 audinterface-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29831 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40495 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_utils.py
```

### Comparing `audinterface-1.0.3/.github/workflows/publish.yml` & `audinterface-1.0.4/.github/workflows/publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,23 @@
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install setuptools wheel twine
+        pip install build twine virtualenv
 
     # PyPI package
     - name: Build and publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
-        python setup.py sdist bdist_wheel
+        python -m build
         python -m twine upload dist/*
 
     # Documentation
     - name: Install doc dependencies
       run: |
         sudo apt-get update
         sudo apt-get install --no-install-recommends --yes libsndfile1 sox
@@ -58,15 +58,15 @@
         CHANGELOG=$(git diff -U0 HEAD^ HEAD | grep '^[+][\* ]' | sed 's/\+//')
         # Support for multiline, see
         # https://github.com/actions/create-release/pull/11#issuecomment-640071918
         CHANGELOG="${CHANGELOG//'%'/'%25'}"
         CHANGELOG="${CHANGELOG//$'\n'/'%0A'}"
         CHANGELOG="${CHANGELOG//$'\r'/'%0D'}"
         echo "Got changelog: $CHANGELOG"
-        echo "::set-output name=body::$CHANGELOG"
+        run echo "body=$CHANGELOG" >> $GITHUB_OUTPUT
 
     - name: Create release on Github
       id: create_release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
```

### Comparing `audinterface-1.0.3/.github/workflows/test.yml` & `audinterface-1.0.4/.github/workflows/doc.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-name: Test
+name: Documentation
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
+        os: [ ubuntu-latest ]
+        python-version: [ '3.8' ]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Cache emodb
       uses: actions/cache@v3
       with:
@@ -25,38 +25,25 @@
         key: emodb-1.3.0
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
-    - name: Prepare Ubuntu
+    - name: Ubuntu - install libsndfile1
       run: |
         sudo apt-get update
-        sudo apt-get install --no-install-recommends --yes libsndfile1 sox
-      if: matrix.os == 'ubuntu-latest'
+        sudo apt-get install --no-install-recommends --yes libsndfile1
 
-    - name: Install dependencies
+    - name: Install package
       run: |
-        python -V
         python -m pip install --upgrade pip
         pip install -r requirements.txt
-        pip install -r docs/requirements.txt
-        pip install -r tests/requirements.txt
 
-    - name: Test with pytest
-      run: |
-        python -m pytest
-
-    - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v1
-      with:
-        token: ${{ secrets.CODECOV_TOKEN }}
-        file: ./coverage.xml
-      if: matrix.os == 'ubuntu-latest'
+    - name: Install docs requirements
+      run: pip install -r docs/requirements.txt
 
     - name: Test building documentation
-      run: |
-        python -m sphinx docs/ docs/_build/ -b html -W
-        # Disbale link check until new release is done
-        # python -m sphinx docs/ build/sphinx/html -b linkcheck
-      if: matrix.os == 'ubuntu-latest'
+      run: python -m sphinx docs/ docs/_build/ -b html -W
+
+    - name: Check links in documentation
+      run: python -m sphinx docs/ docs/_build/ -b linkcheck -W
```

### Comparing `audinterface-1.0.3/CHANGELOG.rst` & `audinterface-1.0.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.4 (2023/07/13)
+--------------------------
+
+* Changed: require ``audmath>=1.3.0``
+* Changed: require ``audiofile>=1.3.0``
+* Changed: always evenly round
+  ``start`` and ``end``
+  to samples
+  in ``audinterface.utils.read_signal()``
+* Fixed: process functions
+  that work on segments
+  are now always processing the identical signal
+  independent if they get the signal as input,
+  like ``audinterface.Process.process_signal()``,
+  or a file,
+  like ``audinterface.Process.process_file()``
+
+
 Version 1.0.3 (2023/06/06)
 --------------------------
 
 * Added: ``cache_root`` argument
   to ``audinterface.Segment.process_index()``
```

### Comparing `audinterface-1.0.3/CONTRIBUTING.rst` & `audinterface-1.0.4/CONTRIBUTING.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,109 +1,121 @@
 Contributing
 ============
 
 Everyone is invited to contribute to this project.
 Feel free to create a `pull request`_ .
-If you find errors, omissions, inconsistencies or other things
-that need improvement, please create an issue_.
+If you find errors,
+omissions,
+inconsistencies,
+or other things
+that need improvement,
+please create an issue_.
 
 .. _issue: https://github.com/audeering/audinterface/issues/new/
 .. _pull request: https://github.com/audeering/audinterface/compare/
 
 
 Development Installation
 ------------------------
 
-Instead of pip-installing the latest release from PyPI,
+Instead of pip-installing the latest release from PyPI_,
 you should get the newest development version from Github_::
 
-    git clone https://github.com/audeering/audinterface/
-    cd audinterface
-    # Create virutal environment for this project
-    # e.g.
-    # virtualenv --python="python3"  $HOME/.envs/audinterface
-    # source $HOME/.envs/audinterface/bin/activate
-    pip install -r requirements.txt
+   git clone https://github.com/audeering/audinterface/
+   cd audinterface
+   # Create virtual environment for this project
+   # e.g.
+   # virtualenv --python="python3"  $HOME/.envs/audinterface
+   # source $HOME/.envs/audinterface/bin/activate
+   pip install -r requirements.txt
 
-.. _Github: https://github.com/audeering/audinterface
 
-This way, your installation always stays up-to-date,
+This way,
+your installation always stays up-to-date,
 even if you pull new changes from the Github repository.
 
+.. _PyPI: https://pypi.org/project/audinterface/
+.. _Github: https://github.com/audeering/audinterface/
+
 
 Coding Convention
 -----------------
 
 We follow the PEP8_ convention for Python code
-and check for correct syntax with flake8_.
-Exceptions are defined under the ``[flake8]`` section
-in :file:`setup.cfg`.
+and check for correct syntax with ruff_.
+In addition,
+we check for common spelling errors with codespell_.
+Both tools and possible exceptions
+are defined in :file:`pyproject.toml`.
 
 The checks are executed in the CI using `pre-commit`_.
 You can enable those checks locally by executing::
 
     pip install pre-commit  # consider system wide installation
     pre-commit install
     pre-commit run --all-files
 
-Afterwards flake8_ is executed
+Afterwards ruff_ and codespell_ are executed
 every time you create a commit.
 
-You can also install flake8_
+You can also install ruff_ and codespell_
 and call it directly::
 
-    pip install flake8  # consider system wide installation
-    flake8
+    pip install ruff codespell  # consider system wide installation
+    ruff check .
+    codespell
 
 It can be restricted to specific folders::
 
-    flake8 audfoo/ tests/
+    ruff check audfoo/ tests/
+    codespell audfoo/ tests/
+
 
+.. _codespell: https://github.com/codespell-project/codespell/
 .. _PEP8: http://www.python.org/dev/peps/pep-0008/
-.. _flake8: https://flake8.pycqa.org/en/latest/index.html
 .. _pre-commit: https://pre-commit.com
+.. _ruff: https://beta.ruff.rs
 
 
 Building the Documentation
 --------------------------
 
 If you make changes to the documentation,
 you can re-create the HTML pages using Sphinx_.
 You can install it and a few other necessary packages with::
 
-    pip install -r requirements.txt
-    pip install -r docs/requirements.txt
+   pip install -r docs/requirements.txt
 
 To create the HTML pages, use::
 
-	python -m sphinx docs/ build/sphinx/html -b html
+   python -m sphinx docs/ build/sphinx/html -b html
 
 The generated files will be available
 in the directory :file:`build/sphinx/html/`.
 
 It is also possible to automatically check if all links are still valid::
 
-    python -m sphinx docs/ build/sphinx/linkcheck -b linkcheck
+   python -m sphinx docs/ build/sphinx/html -b linkcheck
 
-.. _Sphinx: http://sphinx-doc.org/
+.. _Sphinx: http://sphinx-doc.org
 
 
 Running the Tests
 -----------------
 
 You'll need pytest_ for that.
 It can be installed with::
 
-    pip install -r tests/requirements.txt
+   pip install -r tests/requirements.txt
 
 To execute the tests, simply run::
 
-    python -m pytest
+   python -m pytest
 
-.. _pytest: https://pytest.org/
+.. _pytest: https://pytest.org
 
 
 Creating a New Release
 ----------------------
 
 New releases are made using the following steps:
```

### Comparing `audinterface-1.0.3/LICENSE` & `audinterface-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.3/README.rst` & `audinterface-1.0.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 to apply any machine learning model
 or digital signal processing algorithm
 to audio files or databases_.
 
 Have a look at the installation_ and usage_ instructions.
 
 .. _databases: https://audeering.github.io/audformat/
-.. _installation: https://audeering.github.io/audinterface/install.html
+.. _installation: https://audeering.github.io/audinterface/installation.html
 .. _usage: https://audeering.github.io/audinterface/usage.html
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/audinterface/workflows/Test/badge.svg
     :target: https://github.com/audeering/audinterface/actions?query=workflow%3ATest
     :alt: Test status
-.. |coverage| image:: https://codecov.io/gh/audeering/audinterface/branch/master/graph/badge.svg?token=dNAlTQNVBt
+.. |coverage| image:: https://codecov.io/gh/audeering/audinterface/branch/main/graph/badge.svg?token=dNAlTQNVBt
     :target: https://codecov.io/gh/audeering/audinterface/
     :alt: code coverage
 .. |docs| image:: https://img.shields.io/pypi/v/audinterface?label=docs
     :target: https://audeering.github.io/audinterface/
     :alt: audinterface's documentation
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
-    :target: https://github.com/audeering/audinterface/blob/master/LICENSE
+    :target: https://github.com/audeering/audinterface/blob/main/LICENSE
     :alt: audinterface's MIT license
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/audinterface.svg
     :target: https://pypi.org/project/audinterface/
     :alt: audinterfaces's supported Python versions
```

### Comparing `audinterface-1.0.3/audinterface/__init__.py` & `audinterface-1.0.4/audinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.3/audinterface/core/feature.py` & `audinterface-1.0.4/audinterface/core/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 import pandas as pd
 
 import audeer
 import audformat
 
 from audinterface.core.process import Process
 from audinterface.core.segment import Segment
-from audinterface.core.typing import (
-    Timestamp,
-    Timestamps,
-)
+from audinterface.core.typing import Timestamp
+from audinterface.core.typing import Timestamps
 import audinterface.core.utils as utils
 
 
 def deprecated_process_func_applies_sliding_window_default_value(
 ) -> typing.Callable:
     """Deprecate default value of process_func_applies_sliding_window."""
     def _deprecated(func):
@@ -120,15 +118,15 @@
             if ``True``
             the processing function receives
             whole files or segments and is responsible
             for applying a sliding window itself.
             If ``False``,
             the sliding window is applied internally
             and the processing function
-            receives invidual frames instead.
+            receives individual frames instead.
             Applies only if
             features are extracted in a framewise manner
             (see ``win_dur`` and ``hop_dur``)
         sampling_rate: sampling rate in Hz.
             If ``None`` it will call ``process_func`` with the actual
             sampling rate of the signal
         resample: if ``True`` enforces given sampling rate by resampling
@@ -672,15 +670,14 @@
         return frame.values.T.reshape(self.num_channels, self.num_features, -1)
 
     def _reshape_3d(
             self,
             features: typing.Union[np.ndarray, pd.Series]
     ):
         r"""Reshape to [n_channels, n_features, n_frames]."""
-
         features = np.array(features)
         features = np.atleast_1d(features)
 
         if self.process.process_func_is_mono:
             # when mono processing is turned on
             # the channel dimension has to be 1,
             # so we would usually omit it,
```

### Comparing `audinterface-1.0.3/audinterface/core/process.py` & `audinterface-1.0.4/audinterface/core/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 import pandas as pd
 
 import audeer
 import audformat
 
 from audinterface.core import utils
 from audinterface.core.segment import Segment
-from audinterface.core.typing import (
-    Timestamp,
-    Timestamps,
-)
+from audinterface.core.typing import Timestamp
+from audinterface.core.typing import Timestamps
 
 
 class Process:
     r"""Processing interface.
 
     Args:
         process_func: processing function,
@@ -721,15 +719,14 @@
     def _process_signal_from_index_wo_segment(
             self,
             signal: np.ndarray,
             sampling_rate: int,
             index: pd.Index,
     ) -> pd.Series:
         r"""Like process_signal_from_index, but does not apply segmentation."""
-
         if index.empty:
             return pd.Series(None, index=index, dtype=object)
 
         skip_file_level = (
                 isinstance(index, pd.MultiIndex) and
                 len(index.levels) == 2
         )
@@ -834,15 +831,14 @@
             sampling_rate: int,
             *,
             idx: int = 0,
             root: str = None,
             file: str = None,
     ) -> typing.Any:
         r"""Call processing function, possibly pass special args."""
-
         signal, sampling_rate = utils.preprocess_signal(
             signal,
             sampling_rate,
             self.sampling_rate,
             self.resample,
             self.channels,
             self.mixdown,
```

### Comparing `audinterface-1.0.3/audinterface/core/process_with_context.py` & `audinterface-1.0.4/audinterface/core/process_with_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,14 @@
         ends: typing.Sequence[int],
         *,
         idx: int = 0,
         root: str = None,
         file: str = None,
     ) -> typing.Any:
         r"""Call processing function, possibly pass special args."""
-
         signal, sampling_rate = utils.preprocess_signal(
             signal,
             sampling_rate,
             self.sampling_rate,
             self.resample,
             self.channels,
             self.mixdown,
@@ -354,14 +353,16 @@
         signal. However, if channel selection, mixdown and/or resampling
         is enabled, the signal will be first remixed and resampled if the
         input sampling rate does not fit the expected sampling rate.
 
         Args:
             signal: signal values
             sampling_rate: sampling rate in Hz
+            starts: sequence with start values
+            ends: sequence with end values
 
         Returns:
             Processed signal
 
         Raises:
             RuntimeError: if sampling rates do not match
             RuntimeError: if channel selection is invalid
```

### Comparing `audinterface-1.0.3/audinterface/core/segment.py` & `audinterface-1.0.4/audinterface/core/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,23 @@
 import numpy as np
 import pandas as pd
 
 import audeer
 import audformat
 
 from audinterface.core import utils
-from audinterface.core.typing import (
-    Timestamp,
-    Timestamps,
-)
+from audinterface.core.typing import Timestamp
+from audinterface.core.typing import Timestamps
 
 
 def create_process_func(
         process_func: typing.Optional[typing.Callable[..., pd.MultiIndex]],
         invert: bool,
 ) -> typing.Callable[..., pd.MultiIndex]:
     r"""Create processing function."""
-
     if process_func is None:
         def process_func(signal, sr, **kwargs):
             return utils.signal_index()
 
     if invert:
         def process_func_invert(signal, sr, **kwargs):
             index = process_func(signal, sr, **kwargs)
```

### Comparing `audinterface-1.0.3/audinterface/core/utils.py` & `audinterface-1.0.4/audinterface/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 import typing
 
 import numpy as np
 import pandas as pd
 
 import audeer
 import audformat
+import audiofile as af
 import audmath
 import audresample
-import audiofile as af
 
-from audinterface.core.typing import (
-    Timestamp,
-    Timestamps,
-)
+from audinterface.core.typing import Timestamp
+from audinterface.core.typing import Timestamps
 
 
 def assert_index(obj: pd.Index):
     r"""Check if index is conform to audformat."""
-
     if isinstance(obj, pd.MultiIndex) and len(obj.levels) == 2:
 
         if obj.has_duplicates:
             max_display = 10
             duplicates = obj[obj.duplicated()]
             msg_tail = '\n...' if len(duplicates) > max_display else ''
             msg_duplicates = '\n'.join(
@@ -60,29 +57,28 @@
                 "Level 'end' must contain values of type 'timedelta64[ns]'."
             )
     else:
         audformat.assert_index(obj)
 
 
 def is_scalar(value: typing.Any) -> bool:
-    r"""Check if value is scalar"""
+    r"""Check if value is scalar."""
     return (value is not None) and \
            (isinstance(value, str) or not hasattr(value, '__len__'))
 
 
 def preprocess_signal(
         signal: np.ndarray,
         sampling_rate: int,
         expected_rate: int,
         resample: bool,
         channels: typing.Union[int, typing.Sequence[int]],
         mixdown: bool,
 ) -> (np.ndarray, int):
     r"""Pre-process signal."""
-
     signal = np.atleast_2d(signal)
 
     if channels is not None or mixdown:
         signal = audresample.remix(signal, channels, mixdown)
 
     if expected_rate is not None and sampling_rate != expected_rate:
         if resample:
@@ -162,17 +158,17 @@
         sampling_rate: int,
         start: pd.Timedelta,
         end: pd.Timedelta,
 ) -> typing.Tuple[int, int]:
     if pd.isna(end):
         end = pd.to_timedelta(signal.shape[-1] / sampling_rate, unit='s')
     max_i = signal.shape[-1]
-    start_i = int(round(start.total_seconds() * sampling_rate))
+    start_i = audmath.samples(start.total_seconds(), sampling_rate)
     start_i = min(start_i, max_i)
-    end_i = int(round(end.total_seconds() * sampling_rate))
+    end_i = audmath.samples(end.total_seconds(), sampling_rate)
     end_i = min(end_i, max_i)
     return start_i, end_i
 
 
 def segments_to_indices(
         signal: np.ndarray,
         sampling_rate: int,
```

### Comparing `audinterface-1.0.3/audinterface.egg-info/SOURCES.txt` & `audinterface-1.0.4/audinterface.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+.flake8
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.rst
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
-.github/workflows/flake8.yml
+.github/workflows/doc.yml
+.github/workflows/linter.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 audinterface/__init__.py
 audinterface.egg-info/PKG-INFO
 audinterface.egg-info/SOURCES.txt
 audinterface.egg-info/dependency_links.txt
 audinterface.egg-info/requires.txt
```

### Comparing `audinterface-1.0.3/docs/_templates/autosummary/class.rst` & `audinterface-1.0.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.3/docs/api-src/audinterface.rst` & `audinterface-1.0.4/docs/api-src/audinterface.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.3/docs/conf.py` & `audinterface-1.0.4/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from datetime import date
 import os
 import shutil
-import subprocess
+
+import toml
 
 import audeer
 
 
+config = toml.load(audeer.path('..', 'pyproject.toml'))
+
+
 # Project -----------------------------------------------------------------
-project = 'audinterface'
+project = config['project']['name']
 copyright = f'2020-{date.today().year} audEERING GmbH'
-author = 'Johannes Wagner, Hagen Wierstorf, Andreas Triantafyllopoulos'
-# The x.y.z version read from tags
-try:
-    version = subprocess.check_output(['git', 'describe', '--tags',
-                                       '--always'])
-    version = version.decode().strip()
-except Exception:
-    version = '<unknown>'
-title = f'{project} Documentation'
+author = ', '.join(author['name'] for author in config['project']['authors'])
+version = audeer.git_repo_version()
+title = 'Documentation'
 
 
 # General -----------------------------------------------------------------
 master_doc = 'index'
 extensions = []
 source_suffix = '.rst'
 exclude_patterns = [
```

### Comparing `audinterface-1.0.3/docs/index.rst` & `audinterface-1.0.4/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-.. audinterface documentation master file
-
 .. include:: ../README.rst
 
 .. toctree::
     :caption: Getting started
     :maxdepth: 2
     :hidden:
```

### Comparing `audinterface-1.0.3/docs/usage.rst` & `audinterface-1.0.4/docs/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     df
 
 To calculate features with a sliding window,
 we create a new interface
 and set a window and hop duration.
 By setting
 ``process_func_applies_sliding_window=False``
-the windowing is automatically handeled
+the windowing is automatically handled
 and single frames are passed on to the processing function.
 
 .. jupyter-execute::
 
     interface = audinterface.Feature(
         ['mean', 'std'],
         process_func=features,
```

### Comparing `audinterface-1.0.3/misc/logo.png` & `audinterface-1.0.4/misc/logo.png`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.3/tests/test_feature.py` & `audinterface-1.0.4/tests/test_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 
-import audiofile
 import numpy as np
 import pandas as pd
 import pytest
 
 import audeer
 import audformat
-import audinterface
+import audiofile
 import audiofile as af
 
+import audinterface
+
 
 SAMPLING_RATE = 8000
 NUM_CHANNELS = 2
 NUM_FEATURES = 3
 NUM_FRAMES = 5
 SIGNAL_1D = np.ones((1, SAMPLING_RATE))
 SIGNAL_2D = np.ones((NUM_CHANNELS, SAMPLING_RATE))
```

### Comparing `audinterface-1.0.3/tests/test_process.py` & `audinterface-1.0.4/tests/test_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 
-import audiofile
-import audiofile as af
 import numpy as np
 import pandas as pd
 import pytest
 
 import audeer
-import audinterface
 import audformat
+import audiofile
+import audiofile as af
 import audobject
 
+import audinterface
+
+
+def identity(signal, sampling_rate):
+    return signal
+
 
 def signal_duration(signal, sampling_rate):
     return signal.shape[1] / sampling_rate
 
 
 def signal_max(signal, sampling_rate):
     return np.max(signal)
@@ -297,14 +302,36 @@
             1.0,
             2.0,
             False,
             None,
             False,
             1.0,
         ),
+        # Test for certain `start`, `end` values
+        # that were failing before
+        # https://github.com/audeering/audinterface/issues/123
+        (
+            identity,
+            None,
+            np.concatenate(
+                [
+                    np.zeros((1, 18240)),
+                    np.ones((1, 6720)),
+                    np.zeros((1, 23040)),
+                ],
+                axis=1,
+            ),
+            16000,
+            pd.Timedelta('0 days 00:00:01.140000'),
+            pd.Timedelta('0 days 00:00:01.560000'),
+            True,
+            None,
+            False,
+            np.ones((1, 6720), 'float32'),
+        ),
     ],
 )
 def test_process_file(
     tmpdir,
     process_func,
     segment,
     signal,
@@ -335,27 +362,29 @@
 
     # test absolute path
     y = process.process_file(
         path,
         start=start,
         end=end,
     )
+
     np.testing.assert_almost_equal(
-        y.values, expected_output, decimal=4,
+        y.values[0], expected_output, decimal=4,
     )
 
     # test relative path
     y = process.process_file(
         file,
         start=start,
         end=end,
         root=root,
     )
+
     np.testing.assert_almost_equal(
-        y.values, expected_output, decimal=4,
+        y.values[0], expected_output, decimal=4,
     )
 
 
 @pytest.mark.parametrize(
     'process_func, num_files, signal, sampling_rate, starts, ends, '
     'expected_output',
     [
@@ -1475,15 +1504,15 @@
     expected = pd.Series(
         [((idx, file, root), (idx, file, root))
          for idx, (file, _, _) in enumerate(index)],
         index,
     )
     pd.testing.assert_series_equal(y, expected)
 
-    # explicitely pass special arguments
+    # explicitly pass special arguments
 
     process = audinterface.Process(
         process_func=process_func,
         process_func_args={'idx': 99, 'file': 'my/file', 'root': None},
         num_workers=num_workers,
     )
     y = process.process_index(index, root=root)
```

### Comparing `audinterface-1.0.3/tests/test_process_with_context.py` & `audinterface-1.0.4/tests/test_process_with_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import audformat
-import audinterface
 import audiofile
 
+import audinterface
+
 
 def signal_max(signal, sampling_rate):
     return np.max(signal)
 
 
 def signal_max_with_context(signal, sampling_rate, starts, ends):
     result = np.zeros(len(starts))
@@ -338,15 +339,15 @@
     for idx in range(num_files):
         file = files[idx]
         for _ in range(num_frames):
             values.append((idx, file, root))
     expected = pd.Series(values, index)
     pd.testing.assert_series_equal(y, expected)
 
-    # explicitely pass special arguments
+    # explicitly pass special arguments
 
     process = audinterface.ProcessWithContext(
         process_func=process_func,
         process_func_args={'idx': 99, 'file': 'my/file', 'root': None},
     )
     y = process.process_index(index, root=root)
     expected = pd.Series([(99, 'my/file', None)] * len(index), index)
```

### Comparing `audinterface-1.0.3/tests/test_segment.py` & `audinterface-1.0.4/tests/test_segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import audformat
-import audinterface
 import audiofile as af
 
+import audinterface
+
 
 SAMPLING_RATE = 8000
 SIGNAL = np.ones((3, SAMPLING_RATE * 10))
 SIGNAL_DUR = pd.to_timedelta(SIGNAL.shape[-1] / SAMPLING_RATE, unit='s')
 STARTS = pd.timedelta_range('0s', '10s', 3)
 ENDS = STARTS + pd.to_timedelta('1s')
 INDEX = audinterface.utils.signal_index(STARTS, ENDS)
```

### Comparing `audinterface-1.0.3/tests/test_utils.py` & `audinterface-1.0.4/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import re
 
 import numpy as np
 import pandas as pd
 import pytest
 
+import audeer
 import audformat
+import audiofile
+
 import audinterface
 
 
 def to_array(value):
     if value is not None:
         if isinstance(value, (pd.Series, pd.DataFrame, pd.Index)):
             value = value.tolist()
@@ -127,14 +130,53 @@
             ).tolist() == ends
         else:
             assert index.get_level_values(
                 audformat.define.IndexField.END
             ).tolist() == [pd.NaT] * len(starts)
 
 
+def test_read_audio(tmpdir):
+
+    # Ensures that we apply the same rounding
+    # when reading with `audinterface.utils.read_audio()`
+    # with `start` and `end`
+    # or when using `start` and `end` with `process_signal()`.
+
+    # Use critical `start` and `end` values
+    # as reported in
+    # https://github.com/audeering/audinterface/issues/123
+    start = pd.Timedelta('0 days 00:00:01.140000')
+    end = pd.Timedelta('0 days 00:00:01.560000')
+
+    sampling_rate = 16000
+    signal = np.zeros((1, 3 * sampling_rate))
+
+    # Use `audinterface.core.utils.segment_to_indices()` as ground truth
+    start_i, end_i = audinterface.core.utils.segment_to_indices(
+        signal,
+        sampling_rate,
+        start,
+        end,
+    )
+    signal[:, start_i:end_i] = 0.9
+
+    audio_file = audeer.path(tmpdir, 'signal.wav')
+    audiofile.write(audio_file, signal, sampling_rate)
+
+    signal, _ = audinterface.utils.read_audio(
+        audio_file,
+        start=start,
+        end=end,
+    )
+    expected_signal, _ = audiofile.read(audio_file, always_2d=True)
+    expected_signal = expected_signal[:, start_i:end_i]
+
+    np.testing.assert_array_equal(signal, expected_signal)
+
+
 @pytest.mark.parametrize(
     'signal, sampling_rate, win_dur, hop_dur, expected',
     [
         # empty
         (
             np.array([]),
             1, 1, 1,
```

