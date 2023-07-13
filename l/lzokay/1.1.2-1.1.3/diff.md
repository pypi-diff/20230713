# Comparing `tmp/lzokay-1.1.2.tar.gz` & `tmp/lzokay-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lzokay-1.1.2.tar", last modified: Tue Aug  2 16:06:25 2022, max compression
+gzip compressed data, was "lzokay-1.1.3.tar", last modified: Thu Jul 13 17:43:36 2023, max compression
```

## Comparing `lzokay-1.1.2.tar` & `lzokay-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,45 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 16:06:25.507570 lzokay-1.1.2/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 16:06:25.496049 lzokay-1.1.2/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 16:06:25.503131 lzokay-1.1.2/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     4568 2022-08-02 16:05:26.000000 lzokay-1.1.2/.github/workflows/python.yml
--rw-r--r--   0 runner     (501) staff       (20)     1853 2022-08-02 16:05:26.000000 lzokay-1.1.2/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)       93 2022-08-02 16:05:26.000000 lzokay-1.1.2/.gitmodules
--rw-r--r--   0 runner     (501) staff       (20)     1087 2022-08-02 16:05:26.000000 lzokay-1.1.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       55 2022-08-02 16:05:26.000000 lzokay-1.1.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      731 2022-08-02 16:06:25.507810 lzokay-1.1.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)       39 2022-08-02 16:05:26.000000 lzokay-1.1.2/README.md
--rw-r--r--   0 runner     (501) staff       (20)   392571 2022-08-02 16:06:23.000000 lzokay-1.1.2/_lzokay.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2234 2022-08-02 16:05:26.000000 lzokay-1.1.2/_lzokay.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 16:06:25.504008 lzokay-1.1.2/lzokay/
--rw-r--r--   0 runner     (501) staff       (20)      251 2022-08-02 16:05:26.000000 lzokay-1.1.2/lzokay/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      176 2022-08-02 16:06:25.000000 lzokay-1.1.2/lzokay/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 16:06:25.506538 lzokay-1.1.2/lzokay.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      731 2022-08-02 16:06:25.000000 lzokay-1.1.2/lzokay.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      361 2022-08-02 16:06:25.000000 lzokay-1.1.2/lzokay.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-02 16:06:25.000000 lzokay-1.1.2/lzokay.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-02 16:05:54.000000 lzokay-1.1.2/lzokay.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       15 2022-08-02 16:06:25.000000 lzokay-1.1.2/lzokay.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      524 2022-08-02 16:05:26.000000 lzokay-1.1.2/lzokay_wrap.pxd
--rw-r--r--   0 runner     (501) staff       (20)      274 2022-08-02 16:05:26.000000 lzokay-1.1.2/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      747 2022-08-02 16:06:25.508731 lzokay-1.1.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     5066 2022-08-02 16:05:26.000000 lzokay-1.1.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 16:06:25.507089 lzokay-1.1.2/test/
--rw-r--r--   0 runner     (501) staff       (20)      434 2022-08-02 16:05:26.000000 lzokay-1.1.2/test/test_native.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.973441 lzokay-1.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/.github/
+-rw-rw-rw-   0        0        0      730 2023-07-13 17:41:58.000000 lzokay-1.1.3/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/.github/workflows/
+-rw-rw-rw-   0        0        0      618 2023-07-13 17:41:58.000000 lzokay-1.1.3/.github/workflows/dependabot.yml
+-rw-rw-rw-   0        0        0     4572 2023-07-13 17:41:58.000000 lzokay-1.1.3/.github/workflows/python.yml
+-rw-rw-rw-   0        0        0     1992 2023-07-13 17:41:58.000000 lzokay-1.1.3/.gitignore
+-rw-rw-rw-   0        0        0       96 2023-07-13 17:41:58.000000 lzokay-1.1.3/.gitmodules
+-rw-rw-rw-   0        0        0      432 2023-07-13 17:41:58.000000 lzokay-1.1.3/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1108 2023-07-13 17:41:58.000000 lzokay-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-13 17:41:58.000000 lzokay-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      786 2023-07-13 17:43:36.973441 lzokay-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-07-13 17:41:58.000000 lzokay-1.1.3/README.md
+-rw-rw-rw-   0        0        0   438357 2023-07-13 17:43:34.000000 lzokay-1.1.3/_lzokay.cpp
+-rw-rw-rw-   0        0        0     2329 2023-07-13 17:41:58.000000 lzokay-1.1.3/_lzokay.pyx
+-rw-rw-rw-   0        0        0      541 2023-07-13 17:41:58.000000 lzokay-1.1.3/lzokay_wrap.pxd
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.942191 lzokay-1.1.3/native/
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/native/lzokay/
+-rw-rw-rw-   0        0        0       41 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/.git
+-rw-rw-rw-   0        0        0     1705 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/CMakeLists.txt
+-rw-rw-rw-   0        0        0      111 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/Config.cmake.in
+-rw-rw-rw-   0        0        0     1097 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/LICENSE
+-rw-rw-rw-   0        0        0     1892 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/native/lzokay/lzokay-c/
+-rw-rw-rw-   0        0        0      204 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay-c/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1084 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay-c/lzokay-c.cpp
+-rw-rw-rw-   0        0        0      566 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay-c/lzokay-c.h
+-rw-rw-rw-   0        0        0    21184 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay.cpp
+-rw-rw-rw-   0        0        0     2558 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/lzokay.hpp
+-rw-rw-rw-   0        0        0     1305 2023-07-13 17:42:00.000000 lzokay-1.1.3/native/lzokay/test.cpp
+-rw-rw-rw-   0        0        0     1455 2023-07-13 17:41:58.000000 lzokay-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      137 2023-07-13 17:43:36.973441 lzokay-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     5173 2023-07-13 17:41:58.000000 lzokay-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.942191 lzokay-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.957816 lzokay-1.1.3/src/lzokay/
+-rw-rw-rw-   0        0        0      275 2023-07-13 17:41:58.000000 lzokay-1.1.3/src/lzokay/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay/version.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.973441 lzokay-1.1.3/src/lzokay.egg-info/
+-rw-rw-rw-   0        0        0      786 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 17:43:36.000000 lzokay-1.1.3/src/lzokay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 17:43:36.973441 lzokay-1.1.3/tests/
+-rw-rw-rw-   0        0        0      493 2023-07-13 17:41:58.000000 lzokay-1.1.3/tests/test_native.py
```

### Comparing `lzokay-1.1.2/.github/workflows/python.yml` & `lzokay-1.1.3/.github/workflows/python.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,166 @@
-name: Python Package
-
-on:
-  pull_request:
-  push:
-    branches:
-      - '*'
-    tags:
-      - '*'
-
-jobs:
-  build:
-    strategy:
-      fail-fast: false
-      matrix:
-        os:
-          - 'macos-latest'
-          - 'windows-latest'
-        python:
-          - '3.7'
-          - '3.8'
-          - '3.9'
-          - '3.10'
-          - '3.11-dev'
-
-    runs-on: ${{ matrix.os }}
-    name: Wheel for ${{ matrix.os }} (${{ matrix.python }})
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          submodules: 'recursive'
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "${{ matrix.python }}"
-     
-      - name: Install Python packages
-        run: python -m pip install --upgrade build pip
-
-      - name: build wheel
-        run: python -m build --wheel
-
-      - name: build sdist
-        run: python -m build --sdist
-        if: ${{ matrix.os == 'macos-latest' && matrix.python == '3.10' }}
-      
-      - name: Store the packages
-        uses: actions/upload-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist
-
-  linux-build:
-    strategy:
-      fail-fast: false
-      matrix:
-        python:
-          - 'cp37-cp37m'
-          - 'cp38-cp38'
-          - 'cp39-cp39'
-          - 'cp310-cp310'
-          - 'cp311-cp311'
-
-    runs-on: ubuntu-latest
-    container: quay.io/pypa/manylinux2014_x86_64
-    name: Wheel for Linux (${{ matrix.python }})
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          submodules: 'recursive'
-
-      - name: Avoid issues with Git's solution for CVE-2022-24765 breaking setuptools-scm
-        run: git config --global --add safe.directory $(pwd)
-
-      - run: /opt/python/${{ matrix.python }}/bin/python -m venv .venv
-     
-      - name: Install Python packages
-        run: .venv/bin/python -m pip install --upgrade build pip auditwheel
-
-      - name: build wheel
-        run: .venv/bin/python -m build --wheel
-
-      - name: multilinux stuff
-        run: |
-          .venv/bin/python -m auditwheel repair --plat manylinux2014_x86_64 dist/*-linux_x86_64.whl -w dist
-          rm dist/*-linux_x86_64.whl
-      
-      - name: Store the packages
-        uses: actions/upload-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist
-
-  test:
-    needs:
-      - build
-      - linux-build
-      
-    runs-on: ${{ matrix.os.image }}
-    name: ${{ matrix.os.name }} - Test Python ${{ matrix.python.version }}
-    strategy:
-      fail-fast: false
-      matrix:
-        os:
-          - {name: 'macOS', image: 'macos-latest', wheel: 'macosx_*'}
-          - {name: 'Windows', image: 'windows-latest', wheel: 'win_amd64'}
-          - {name: 'Linux', image: 'ubuntu-latest', wheel: 'manylinux2014_x86_64'}
-        python:
-          - {version: '3.7', wheel: 'cp37-cp37m'}
-          - {version: '3.8', wheel: 'cp38-cp38'}
-          - {version: '3.9', wheel: 'cp39-cp39'}
-          - {version: '3.10', wheel: 'cp310-cp310'}
-          - {version: '3.11-dev', wheel: 'cp311-cp311'}
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python.version }}
-
-      - name: Download all the dists
-        uses: actions/download-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist/
-            
-      - name: Install Python packages
-        run: python -m pip install --upgrade pip pytest
-
-      - name: install built wheel
-        run: python -m pip install dist/*-${{ matrix.python.wheel }}-*${{ matrix.os.wheel }}.whl
-        shell: bash
-
-      - name: test
-        run: python -m pytest
-        working-directory: test
-
-  pypi:
-    runs-on: 'ubuntu-latest'
-    needs:
-      - test
-
-    steps:
-      - name: Download all the dists
-        uses: actions/download-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist/
-
-      - name: Publish 📦 to TestPyPI
-        if: ${{ github.ref == 'refs/heads/main' }}
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          password: ${{ secrets.testpypi_password }}
-          repository_url: https://test.pypi.org/legacy/
-      
-      - name: Publish 📦 to PyPI
-        if: ${{ startsWith(github.ref, 'refs/tags/') }}
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          password: ${{ secrets.pypi_password }}
+name: Python Package
+
+on:
+  pull_request:
+  push:
+    branches:
+      - '*'
+    tags:
+      - '*'
+
+jobs:
+  build:
+    strategy:
+      fail-fast: false
+      matrix:
+        os:
+          - 'macos-latest'
+          - 'windows-latest'
+        python:
+          - '3.8'
+          - '3.9'
+          - '3.10'
+          - '3.11'
+          - '3.12.0-beta - 3.12.0'
+
+    runs-on: ${{ matrix.os }}
+    name: Wheel for ${{ matrix.os }} (${{ matrix.python }})
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+          submodules: 'recursive'
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "${{ matrix.python }}"
+     
+      - name: Install Python packages
+        run: python -m pip install --upgrade build pip
+
+      - name: Build
+        run: python -m build
+      
+      - name: Store the packages
+        uses: actions/upload-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist
+
+  linux-build:
+    strategy:
+      fail-fast: false
+      matrix:
+        python:
+          - 'cp38-cp38'
+          - 'cp39-cp39'
+          - 'cp310-cp310'
+          - 'cp311-cp311'
+          - 'cp312-cp312'
+
+    runs-on: ubuntu-latest
+    container: quay.io/pypa/manylinux2014_x86_64
+    name: Wheel for Linux (${{ matrix.python }})
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+          submodules: 'recursive'
+
+      - name: Avoid issues with Git's solution for CVE-2022-24765 breaking setuptools-scm
+        run: git config --global --add safe.directory $(pwd)
+
+      - run: /opt/python/${{ matrix.python }}/bin/python -m venv .venv
+     
+      - name: Install Python packages
+        run: .venv/bin/python -m pip install --upgrade build pip auditwheel setuptools
+
+      - name: build
+        run: .venv/bin/python -m build
+
+      - name: multilinux stuff
+        run: |
+          .venv/bin/python -m auditwheel repair --plat manylinux2014_x86_64 dist/*-linux_x86_64.whl -w dist
+          rm dist/*-linux_x86_64.whl
+      
+      - name: Store the packages
+        uses: actions/upload-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist
+
+  test:
+    needs:
+      - build
+      - linux-build
+      
+    runs-on: ${{ matrix.os.image }}
+    name: ${{ matrix.os.name }} - Test Python ${{ matrix.python.version }}
+    strategy:
+      fail-fast: false
+      matrix:
+        os:
+          - {name: 'macOS', image: 'macos-latest', wheel: 'macosx_*'}
+          - {name: 'Windows', image: 'windows-latest', wheel: 'win_amd64'}
+          - {name: 'Linux', image: 'ubuntu-latest', wheel: 'manylinux2014_x86_64'}
+        python:
+          - {version: '3.8', wheel: 'cp38-cp38'}
+          - {version: '3.9', wheel: 'cp39-cp39'}
+          - {version: '3.10', wheel: 'cp310-cp310'}
+          - {version: '3.11', wheel: 'cp311-cp311'}
+          - {version: '3.12.0-beta - 3.12.0', wheel: 'cp312-cp312'}
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python.version }}
+
+      - name: Download all the dists
+        uses: actions/download-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist/
+
+      - name: Install Python packages
+        run: python -m pip install --upgrade pip
+
+      - name: install built wheel
+        run: python -m pip install "$(ls dist/*-${{ matrix.python.wheel }}-*${{ matrix.os.wheel }}.whl)[test]"
+        shell: bash
+
+      - name: test
+        run: python -m pytest
+
+  pypi:
+    runs-on: 'ubuntu-latest'
+    needs:
+      - test
+
+    steps:
+      - name: Download all the dists
+        uses: actions/download-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist/
+
+      - name: Publish 📦 to TestPyPI
+        if: ${{ github.ref == 'refs/heads/main' }}
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.testpypi_password }}
+          repository-url: https://test.pypi.org/legacy/
+
+      - name: Publish 📦 to PyPI
+        if: ${{ startsWith(github.ref, 'refs/tags/') }}
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.pypi_password }}
```

### Comparing `lzokay-1.1.2/LICENSE` & `lzokay-1.1.3/native/lzokay/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-MIT License
-
-Copyright (c) 2021 Henrique Gemignani Passos Lima
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License
+
+Copyright (c) 2018 Jack Andersen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `lzokay-1.1.2/PKG-INFO` & `lzokay-1.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1
-Name: lzokay
-Version: 1.1.2
-Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
-Home-page: https://github.com/henriquegemignani/py-lzokay
-Author: Henrique Gemignani
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# py-lzokay
-Python bindings for LZ👌
+Metadata-Version: 2.1
+Name: lzokay
+Version: 1.1.3
+Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
+Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/henriquegemignani/py-lzokay
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# py-lzokay
+Python bindings for LZ👌
```

### Comparing `lzokay-1.1.2/_lzokay.cpp` & `lzokay-1.1.3/_lzokay.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-/* Generated by Cython 3.0.0a11 */
+/* Generated by Cython 3.0.0rc2 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "cmake_options": {
-            "dir": "/Users/runner/work/py-lzokay/py-lzokay/native/lzokay",
+            "dir": "D:\\a\\py-lzokay\\py-lzokay\\native\\lzokay",
             "targets": {
                 "lzokay": "lib"
             }
         },
         "depends": [],
         "extra_compile_args": [
-            "-std=c++17"
+            "-DUNICODE",
+            "/std:c++17",
+            "/MD"
         ],
         "language": "c++",
-        "name": "_lzokay",
+        "name": "lzokay._lzokay",
         "sources": [
             "_lzokay.pyx"
         ]
     },
-    "module_name": "_lzokay"
+    "module_name": "lzokay._lzokay"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
@@ -55,18 +57,18 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0a11"
+#define CYTHON_ABI "3_0_0rc2"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000AB
+#define CYTHON_HEX_VERSION 0x030000C2
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -192,26 +194,30 @@
   #undef CYTHON_METH_FASTCALL
   #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
   #ifndef CYTHON_PEP487_INIT_SUBCLASS
     #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
   #endif
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_MODULE_STATE
   #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 1
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
@@ -357,15 +363,15 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_GIL
-    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000)
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
   #endif
   #ifndef CYTHON_METH_FASTCALL
     #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
@@ -387,15 +393,15 @@
   #elif !defined(CYTHON_USE_TP_FINALIZE)
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #if PY_VERSION_HEX < 0x030600B1
     #undef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS 0
   #elif !defined(CYTHON_USE_DICT_VERSIONS)
-    #define CYTHON_USE_DICT_VERSIONS 1
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
@@ -435,14 +441,25 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
@@ -495,37 +512,57 @@
         #endif
     #endif
 #else
     #include <stdint.h>
     typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -541,23 +578,22 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_DefaultClassType PyClass_Type
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
@@ -566,18 +602,18 @@
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
     static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
         if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
@@ -595,39 +631,31 @@
         if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
         if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
         if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
         if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
         Py_XDECREF(kwds);
         Py_XDECREF(argcount);
         Py_XDECREF(posonlyargcount);
         Py_XDECREF(kwonlyargcount);
         Py_XDECREF(nlocals);
         Py_XDECREF(stacksize);
         Py_XDECREF(replace);
-        Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
 #elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
@@ -655,14 +683,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -673,14 +706,20 @@
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
@@ -874,15 +913,15 @@
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
 #elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
   #if PY_VERSION_HEX >= 0x030C0000
@@ -893,15 +932,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -911,19 +950,19 @@
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -994,25 +1033,30 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -1066,24 +1110,29 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
-#define __PYX_HAVE___lzokay
-#define __PYX_HAVE_API___lzokay
+#define __PYX_HAVE__lzokay___lzokay
+#define __PYX_HAVE_API__lzokay___lzokay
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "pythread.h"
 
     #if CYTHON_COMPILING_IN_PYPY
     #ifdef _MSC_VER
@@ -1184,14 +1233,15 @@
 static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
 {
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
 #endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -1209,14 +1259,60 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -1230,15 +1326,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1297,32 +1393,27 @@
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
 #if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
 #endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "_lzokay.pyx",
+  "<stringsource>",
   "contextvars.pxd",
   "array.pxd",
+  "_lzokay.pyx",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
@@ -1449,43 +1540,50 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1493,28 +1591,159 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
 
-/* TupleAndListFromArray.proto */
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif
+#endif
+#endif
+
+/* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
-static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* BuildPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char);
+
 /* IncludeStringH.proto */
 #include <string.h>
 
+/* CIntToPyUnicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
+
+/* UnicodeConcatInPlace.proto */
+# if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
+    #if CYTHON_REFNANNY
+        #define __Pyx_PyUnicode_ConcatInPlace(left, right) __Pyx_PyUnicode_ConcatInPlaceImpl(&left, right, __pyx_refnanny)
+    #else
+        #define __Pyx_PyUnicode_ConcatInPlace(left, right) __Pyx_PyUnicode_ConcatInPlaceImpl(&left, right)
+    #endif
+    static CYTHON_INLINE PyObject *__Pyx_PyUnicode_ConcatInPlaceImpl(PyObject **p_left, PyObject *right
+        #if CYTHON_REFNANNY
+        , void* __pyx_refnanny
+        #endif
+    );
+#else
+#define __Pyx_PyUnicode_ConcatInPlace __Pyx_PyUnicode_Concat
+#endif
+#define __Pyx_PyUnicode_ConcatInPlaceSafe(left, right) ((unlikely((left) == Py_None) || unlikely((right) == Py_None)) ?\
+    PyNumber_InPlaceAdd(left, right) : __Pyx_PyUnicode_ConcatInPlace(left, right))
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* fastcall.proto */
@@ -1540,14 +1769,22 @@
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
+/* PyIntBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
+#else
+#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
+#endif
+
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
@@ -1559,42 +1796,14 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
-
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1615,26 +1824,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1662,99 +1871,43 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#if !CYTHON_VECTORCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if !CYTHON_VECTORCALL
-#if PY_VERSION_HEX >= 0x03080000
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()
-  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
-#else
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif
-#endif
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectFastCall.proto */
-#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
 /* RaiseUnexpectedTypeError.proto */
 static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-#if __STDC_VERSION__ >= 201112L
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0rc2
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0rc2
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
-#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_3_0_0rc2 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0rc2 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0rc2 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0rc2 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0rc2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0rc2 check_size);
 #endif
 
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportDottedModule.proto */
-static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
-
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* PyObjectCall2Args.proto */
@@ -1860,17 +2013,14 @@
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_CyFunctionType = 0;
-#endif
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
 #define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
@@ -2044,39 +2194,34 @@
     self->data.ob_item = (char*) items;
     __Pyx_SET_SIZE(self, n);
     self->allocated = newsize;
     return 0;
 }
 #endif
 
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* None.proto */
 #include <new>
 
 /* EnumClassDecl.proto */
 #if defined (_MSC_VER)
   #if _MSC_VER >= 1910
     #define __PYX_ENUM_CLASS_DECL enum
   #else
     #define __PYX_ENUM_CLASS_DECL
   #endif
 #else
   #define __PYX_ENUM_CLASS_DECL enum
 #endif
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
@@ -2105,385 +2250,339 @@
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
-#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_Occurred(), err1, err2)
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str);
-#else
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
-#endif
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self); /* proto*/
 
 /* Module declarations from "cpython.version" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "__builtin__" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.type" */
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
-#endif
 
 /* Module declarations from "libc.string" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "libc.stdio" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.object" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.ref" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.exc" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.module" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.mem" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.tuple" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.list" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.sequence" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.mapping" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.iterator" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.number" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.int" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "__builtin__" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.bool" */
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_ptype_7cpython_4bool_bool = 0;
-#endif
 
 /* Module declarations from "cpython.long" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.float" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "__builtin__" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.complex" */
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_ptype_7cpython_7complex_complex = 0;
-#endif
 
 /* Module declarations from "cpython.string" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.unicode" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.pyport" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.dict" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.instance" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.function" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.method" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.weakref" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.getargs" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.pythread" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.pystate" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.cobject" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.oldbuffer" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.set" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.buffer" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.bytes" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.pycapsule" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.contextvars" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "array" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "cpython.array" */
-#if !CYTHON_USE_MODULE_STATE
-static PyTypeObject *__pyx_ptype_7cpython_5array_array = 0;
-#endif
 static CYTHON_INLINE int __pyx_f_7cpython_5array_extend_buffer(arrayobject *, char *, Py_ssize_t); /*proto*/
 
 /* Module declarations from "libc.stdint" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
 /* Module declarations from "lzokay_wrap" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
 
-/* Module declarations from "_lzokay" */
-#if !CYTHON_USE_MODULE_STATE
-#endif
-static int __pyx_f_7_lzokay_compress_worst_size(PyObject *, int __pyx_skip_dispatch); /*proto*/
+/* Module declarations from "lzokay._lzokay" */
+static int __pyx_f_6lzokay_7_lzokay_compress_worst_size(PyObject *, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__Pyx_Enum_EResult_to_py(__PYX_ENUM_CLASS_DECL lzokay::EResult); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "_lzokay"
-extern int __pyx_module_is_main__lzokay;
-int __pyx_module_is_main__lzokay = 0;
+#define __Pyx_MODULE_NAME "lzokay._lzokay"
+extern int __pyx_module_is_main_lzokay___lzokay;
+int __pyx_module_is_main_lzokay___lzokay = 0;
 
-/* Implementation of "_lzokay" */
+/* Implementation of "lzokay._lzokay" */
 /* #### Code section: global_var ### */
+static PyObject *__pyx_builtin_ImportError;
+static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_MemoryError;
 /* #### Code section: string_decls ### */
+static const char __pyx_k_[] = ".";
 static const char __pyx_k_B[] = "B";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k__2[] = "*";
-static const char __pyx_k__10[] = "?";
+static const char __pyx_k__11[] = "?";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_code[] = "code";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_Error[] = "Error";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_bytes[] = "bytes";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_import[] = "__import__";
-static const char __pyx_k_lzokay[] = "_lzokay";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_return[] = "return";
+static const char __pyx_k_EResult[] = "EResult";
+static const char __pyx_k_Success[] = "Success";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_tobytes[] = "tobytes";
 static const char __pyx_k_compress[] = "compress";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_set_name[] = "__set_name__";
+static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_data_size[] = "data_size";
 static const char __pyx_k_metaclass[] = "__metaclass__";
+static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_data_bytes[] = "data_bytes";
 static const char __pyx_k_decompress[] = "decompress";
 static const char __pyx_k_lzokay_pyx[] = "_lzokay.pyx";
+static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
+static const char __pyx_k_lzokay_wrap[] = "lzokay_wrap";
 static const char __pyx_k_mro_entries[] = "__mro_entries__";
 static const char __pyx_k_InputOverrun[] = "InputOverrun";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_OutputOverrun[] = "OutputOverrun";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
+static const char __pyx_k_lzokay__lzokay[] = "lzokay._lzokay";
 static const char __pyx_k_result_mapping[] = "result_mapping";
 static const char __pyx_k_actual_out_size[] = "actual_out_size";
 static const char __pyx_k_InputNotConsumed[] = "InputNotConsumed";
 static const char __pyx_k_LookbehindOverrun[] = "LookbehindOverrun";
 static const char __pyx_k_curren_array_size[] = "curren_array_size";
 static const char __pyx_k_expected_out_size[] = "expected_out_size";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_compress_worst_size[] = "compress_worst_size";
 static const char __pyx_k_expected_output_size[] = "expected_output_size";
-#if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_n_u_B;
-static PyObject *__pyx_n_s_Error;
-static PyObject *__pyx_n_s_InputNotConsumed;
-static PyObject *__pyx_n_s_InputOverrun;
-static PyObject *__pyx_n_s_LookbehindOverrun;
-static PyObject *__pyx_n_s_MemoryError;
-static PyObject *__pyx_n_s_OutputOverrun;
-static PyObject *__pyx_n_s__10;
-static PyObject *__pyx_n_s__2;
-static PyObject *__pyx_n_s_actual_out_size;
-static PyObject *__pyx_n_s_array;
-static PyObject *__pyx_n_s_asyncio_coroutines;
-static PyObject *__pyx_n_s_b;
-static PyObject *__pyx_n_s_bytes;
-static PyObject *__pyx_n_s_class_getitem;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_code;
-static PyObject *__pyx_n_s_compress;
-static PyObject *__pyx_n_s_compress_worst_size;
-static PyObject *__pyx_n_s_curren_array_size;
-static PyObject *__pyx_n_s_data;
-static PyObject *__pyx_n_s_data_bytes;
-static PyObject *__pyx_n_s_data_size;
-static PyObject *__pyx_n_s_decompress;
-static PyObject *__pyx_n_s_dict;
-static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_expected_out_size;
-static PyObject *__pyx_n_s_expected_output_size;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_init_subclass;
-static PyObject *__pyx_n_s_initializing;
-static PyObject *__pyx_n_s_int;
-static PyObject *__pyx_n_s_is_coroutine;
-static PyObject *__pyx_n_s_lzokay;
-static PyObject *__pyx_kp_s_lzokay_pyx;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_metaclass;
-static PyObject *__pyx_n_s_module;
-static PyObject *__pyx_n_s_mro_entries;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_prepare;
-static PyObject *__pyx_n_s_qualname;
-static PyObject *__pyx_n_s_result_mapping;
-static PyObject *__pyx_n_s_return;
-static PyObject *__pyx_n_s_s;
-static PyObject *__pyx_n_s_set_name;
-static PyObject *__pyx_n_s_spec;
-static PyObject *__pyx_n_s_super;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_tobytes;
-#endif
+static const char __pyx_k_is_not_a_valid_EResult[] = " is not a valid EResult";
+static const char __pyx_k_enum_class_EResult_not_importabl[] = "enum class EResult not importable from lzokay_wrap. You are probably using a cpdef enum declared in a .pxd file that does not have a .py  or .pyx file.";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_7_lzokay_compress_worst_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s); /* proto */
-static PyObject *__pyx_pf_7_lzokay_2decompress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_expected_output_size); /* proto */
-static PyObject *__pyx_pf_7_lzokay_4compress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
-#if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_int_3;
-static PyObject *__pyx_int_16;
-static PyObject *__pyx_int_64;
-#endif
-#if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__9;
-#endif
+static PyObject *__pyx_pf_6lzokay_7_lzokay_compress_worst_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s); /* proto */
+static PyObject *__pyx_pf_6lzokay_7_lzokay_2decompress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_expected_output_size); /* proto */
+static PyObject *__pyx_pf_6lzokay_7_lzokay_4compress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
-#if CYTHON_USE_MODULE_STATE
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
   PyObject *__pyx_empty_bytes;
   PyObject *__pyx_empty_unicode;
   #ifdef __Pyx_CyFunction_USED
   PyTypeObject *__pyx_CyFunctionType;
   #endif
   #ifdef __Pyx_FusedFunction_USED
   PyTypeObject *__pyx_FusedFunctionType;
   #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyTypeObject *__pyx_ptype_7cpython_4bool_bool;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyTypeObject *__pyx_ptype_7cpython_7complex_complex;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyTypeObject *__pyx_ptype_7cpython_5array_array;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_u_B;
+  PyObject *__pyx_n_s_EResult;
   PyObject *__pyx_n_s_Error;
+  PyObject *__pyx_n_s_ImportError;
   PyObject *__pyx_n_s_InputNotConsumed;
   PyObject *__pyx_n_s_InputOverrun;
   PyObject *__pyx_n_s_LookbehindOverrun;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_n_s_OutputOverrun;
-  PyObject *__pyx_n_s__10;
+  PyObject *__pyx_n_s_Success;
+  PyObject *__pyx_n_s_ValueError;
+  PyObject *__pyx_n_s__11;
   PyObject *__pyx_n_s__2;
   PyObject *__pyx_n_s_actual_out_size;
   PyObject *__pyx_n_s_array;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b;
   PyObject *__pyx_n_s_bytes;
   PyObject *__pyx_n_s_class_getitem;
@@ -2494,23 +2593,26 @@
   PyObject *__pyx_n_s_curren_array_size;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_data_bytes;
   PyObject *__pyx_n_s_data_size;
   PyObject *__pyx_n_s_decompress;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_doc;
+  PyObject *__pyx_kp_u_enum_class_EResult_not_importabl;
   PyObject *__pyx_n_s_expected_out_size;
   PyObject *__pyx_n_s_expected_output_size;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_int;
   PyObject *__pyx_n_s_is_coroutine;
-  PyObject *__pyx_n_s_lzokay;
+  PyObject *__pyx_kp_u_is_not_a_valid_EResult;
+  PyObject *__pyx_n_s_lzokay__lzokay;
   PyObject *__pyx_kp_s_lzokay_pyx;
+  PyObject *__pyx_n_s_lzokay_wrap;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_n_s_module;
   PyObject *__pyx_n_s_mro_entries;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_prepare;
   PyObject *__pyx_n_s_qualname;
@@ -2518,40 +2620,51 @@
   PyObject *__pyx_n_s_return;
   PyObject *__pyx_n_s_s;
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_super;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_tobytes;
+  PyObject *__pyx_n_s_warn;
+  PyObject *__pyx_n_s_warnings;
   PyObject *__pyx_int_3;
   PyObject *__pyx_int_16;
   PyObject *__pyx_int_64;
-  PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__3;
-  PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__8;
-  PyObject *__pyx_codeobj__4;
-  PyObject *__pyx_codeobj__6;
-  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_codeobj__5;
+  PyObject *__pyx_codeobj__7;
+  PyObject *__pyx_codeobj__10;
 } __pyx_mstate;
 
+#if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
 #else
 static struct PyModuleDef __pyx_moduledef;
 #endif
 
 #define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
 
 #define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
 
 #define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
 #endif
 /* #### Code section: module_state_clear ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_clear(PyObject *m) {
   __pyx_mstate *clear_module_state = __pyx_mstate(m);
   if (!clear_module_state) return 0;
   Py_CLEAR(clear_module_state->__pyx_d);
@@ -2566,22 +2679,27 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_7complex_complex);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_5array_array);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_u_B);
+  Py_CLEAR(clear_module_state->__pyx_n_s_EResult);
   Py_CLEAR(clear_module_state->__pyx_n_s_Error);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
   Py_CLEAR(clear_module_state->__pyx_n_s_InputNotConsumed);
   Py_CLEAR(clear_module_state->__pyx_n_s_InputOverrun);
   Py_CLEAR(clear_module_state->__pyx_n_s_LookbehindOverrun);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_n_s_OutputOverrun);
-  Py_CLEAR(clear_module_state->__pyx_n_s__10);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Success);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__11);
   Py_CLEAR(clear_module_state->__pyx_n_s__2);
   Py_CLEAR(clear_module_state->__pyx_n_s_actual_out_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
@@ -2592,23 +2710,26 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_curren_array_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_data_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_data_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_decompress);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enum_class_EResult_not_importabl);
   Py_CLEAR(clear_module_state->__pyx_n_s_expected_out_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_expected_output_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_int);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
-  Py_CLEAR(clear_module_state->__pyx_n_s_lzokay);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_is_not_a_valid_EResult);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lzokay__lzokay);
   Py_CLEAR(clear_module_state->__pyx_kp_s_lzokay_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lzokay_wrap);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_module);
   Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
@@ -2616,25 +2737,27 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
   Py_CLEAR(clear_module_state->__pyx_n_s_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_super);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_tobytes);
+  Py_CLEAR(clear_module_state->__pyx_n_s_warn);
+  Py_CLEAR(clear_module_state->__pyx_n_s_warnings);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_16);
   Py_CLEAR(clear_module_state->__pyx_int_64);
-  Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
-  Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2651,22 +2774,27 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_7complex_complex);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_5array_array);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_u_B);
+  Py_VISIT(traverse_module_state->__pyx_n_s_EResult);
   Py_VISIT(traverse_module_state->__pyx_n_s_Error);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
   Py_VISIT(traverse_module_state->__pyx_n_s_InputNotConsumed);
   Py_VISIT(traverse_module_state->__pyx_n_s_InputOverrun);
   Py_VISIT(traverse_module_state->__pyx_n_s_LookbehindOverrun);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_n_s_OutputOverrun);
-  Py_VISIT(traverse_module_state->__pyx_n_s__10);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Success);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__11);
   Py_VISIT(traverse_module_state->__pyx_n_s__2);
   Py_VISIT(traverse_module_state->__pyx_n_s_actual_out_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
@@ -2677,23 +2805,26 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_curren_array_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_data_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_data_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_decompress);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enum_class_EResult_not_importabl);
   Py_VISIT(traverse_module_state->__pyx_n_s_expected_out_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_expected_output_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_int);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
-  Py_VISIT(traverse_module_state->__pyx_n_s_lzokay);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_is_not_a_valid_EResult);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lzokay__lzokay);
   Py_VISIT(traverse_module_state->__pyx_kp_s_lzokay_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lzokay_wrap);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_module);
   Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
@@ -2701,54 +2832,166 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
   Py_VISIT(traverse_module_state->__pyx_n_s_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_super);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_tobytes);
+  Py_VISIT(traverse_module_state->__pyx_n_s_warn);
+  Py_VISIT(traverse_module_state->__pyx_n_s_warnings);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_16);
   Py_VISIT(traverse_module_state->__pyx_int_64);
-  Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
-  Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
-#if CYTHON_USE_MODULE_STATE
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
 #define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
 #define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
 #define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
 #ifdef __Pyx_CyFunction_USED
 #define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
 #endif
 #ifdef __Pyx_FusedFunction_USED
 #define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
 #endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_ptype_7cpython_4bool_bool __pyx_mstate_global->__pyx_ptype_7cpython_4bool_bool
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_ptype_7cpython_7complex_complex __pyx_mstate_global->__pyx_ptype_7cpython_7complex_complex
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_ptype_7cpython_5array_array __pyx_mstate_global->__pyx_ptype_7cpython_5array_array
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_u_B __pyx_mstate_global->__pyx_n_u_B
+#define __pyx_n_s_EResult __pyx_mstate_global->__pyx_n_s_EResult
 #define __pyx_n_s_Error __pyx_mstate_global->__pyx_n_s_Error
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
 #define __pyx_n_s_InputNotConsumed __pyx_mstate_global->__pyx_n_s_InputNotConsumed
 #define __pyx_n_s_InputOverrun __pyx_mstate_global->__pyx_n_s_InputOverrun
 #define __pyx_n_s_LookbehindOverrun __pyx_mstate_global->__pyx_n_s_LookbehindOverrun
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_n_s_OutputOverrun __pyx_mstate_global->__pyx_n_s_OutputOverrun
-#define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
+#define __pyx_n_s_Success __pyx_mstate_global->__pyx_n_s_Success
+#define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
+#define __pyx_n_s__11 __pyx_mstate_global->__pyx_n_s__11
 #define __pyx_n_s__2 __pyx_mstate_global->__pyx_n_s__2
 #define __pyx_n_s_actual_out_size __pyx_mstate_global->__pyx_n_s_actual_out_size
 #define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
 #define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
@@ -2759,23 +3002,26 @@
 #define __pyx_n_s_curren_array_size __pyx_mstate_global->__pyx_n_s_curren_array_size
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_data_bytes __pyx_mstate_global->__pyx_n_s_data_bytes
 #define __pyx_n_s_data_size __pyx_mstate_global->__pyx_n_s_data_size
 #define __pyx_n_s_decompress __pyx_mstate_global->__pyx_n_s_decompress
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
+#define __pyx_kp_u_enum_class_EResult_not_importabl __pyx_mstate_global->__pyx_kp_u_enum_class_EResult_not_importabl
 #define __pyx_n_s_expected_out_size __pyx_mstate_global->__pyx_n_s_expected_out_size
 #define __pyx_n_s_expected_output_size __pyx_mstate_global->__pyx_n_s_expected_output_size
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_int __pyx_mstate_global->__pyx_n_s_int
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
-#define __pyx_n_s_lzokay __pyx_mstate_global->__pyx_n_s_lzokay
+#define __pyx_kp_u_is_not_a_valid_EResult __pyx_mstate_global->__pyx_kp_u_is_not_a_valid_EResult
+#define __pyx_n_s_lzokay__lzokay __pyx_mstate_global->__pyx_n_s_lzokay__lzokay
 #define __pyx_kp_s_lzokay_pyx __pyx_mstate_global->__pyx_kp_s_lzokay_pyx
+#define __pyx_n_s_lzokay_wrap __pyx_mstate_global->__pyx_n_s_lzokay_wrap
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
 #define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
@@ -2783,999 +3029,460 @@
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
 #define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_tobytes __pyx_mstate_global->__pyx_n_s_tobytes
+#define __pyx_n_s_warn __pyx_mstate_global->__pyx_n_s_warn
+#define __pyx_n_s_warnings __pyx_mstate_global->__pyx_n_s_warnings
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_16 __pyx_mstate_global->__pyx_int_16
 #define __pyx_int_64 __pyx_mstate_global->__pyx_int_64
-#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
-#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
-#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
-#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
-#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
-#endif
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
 /* #### Code section: module_code ### */
 
-/* "_lzokay.pyx":41
- * 
- * 
- * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
- *     return s + s // 16 + 64 + 3
- * 
- */
-
-static PyObject *__pyx_pw_7_lzokay_1compress_worst_size(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static int __pyx_f_7_lzokay_compress_worst_size(PyObject *__pyx_v_s, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_t_3;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("compress_worst_size", 0);
-
-  /* "_lzokay.pyx":42
- * 
- * cpdef int compress_worst_size(s: int):
- *     return s + s // 16 + 64 + 3             # <<<<<<<<<<<<<<
- * 
+/* "EnumTypeToPy":132
  * 
- */
-  __pyx_t_1 = PyNumber_FloorDivide(__pyx_v_s, __pyx_int_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_s, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_64, 64, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_3, 3, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_3;
-  goto __pyx_L0;
-
-  /* "_lzokay.pyx":41
- * 
- * 
- * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
- *     return s + s // 16 + 64 + 3
+ * @cname("__Pyx_Enum_EResult_to_py")
+ * cdef __Pyx_Enum_EResult_to_py(EResult c_val):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_enum
  * 
  */
 
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_WriteUnraisable("_lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_7_lzokay_1compress_worst_size(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7_lzokay_compress_worst_size, "compress_worst_size(int s: int) -> int");
-static PyMethodDef __pyx_mdef_7_lzokay_1compress_worst_size = {"compress_worst_size", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7_lzokay_1compress_worst_size, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7_lzokay_compress_worst_size};
-static PyObject *__pyx_pw_7_lzokay_1compress_worst_size(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_s = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("compress_worst_size (wrapper)", 0);
-  {
-    #if CYTHON_USE_MODULE_STATE
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_s,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_s,0};
-    #endif
-    PyObject* values[1] = {0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress_worst_size") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v_s = ((PyObject*)values[0]);
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compress_worst_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 41, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("_lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyInt_Type), 0, "s", 1))) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7_lzokay_compress_worst_size(__pyx_self, __pyx_v_s);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_7_lzokay_compress_worst_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s) {
+static PyObject *__Pyx_Enum_EResult_to_py(__PYX_ENUM_CLASS_DECL lzokay::EResult __pyx_v_c_val) {
+  PyObject *__pyx_v___pyx_enum = 0;
+  PyObject *__pyx_v_warnings = NULL;
+  int __pyx_v_underlying_c_val;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("compress_worst_size", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_7_lzokay_compress_worst_size(__pyx_v_s, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "_lzokay.pyx":45
- * 
- * 
- * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
- *     data_size = len(data)
- * 
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_7_lzokay_3decompress(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7_lzokay_2decompress, "decompress(bytes data: bytes, int expected_output_size: int = None) -> bytes");
-static PyMethodDef __pyx_mdef_7_lzokay_3decompress = {"decompress", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7_lzokay_3decompress, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7_lzokay_2decompress};
-static PyObject *__pyx_pw_7_lzokay_3decompress(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_data = 0;
-  PyObject *__pyx_v_expected_output_size = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("decompress (wrapper)", 0);
-  {
-    #if CYTHON_USE_MODULE_STATE
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,&__pyx_n_s_expected_output_size,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,&__pyx_n_s_expected_output_size,0};
-    #endif
-    PyObject* values[2] = {0,0};
-    values[1] = ((PyObject*)((PyObject *)Py_None));
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_expected_output_size);
-          if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decompress") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
-      }
-    } else {
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_data = ((PyObject*)values[0]);
-    __pyx_v_expected_output_size = ((PyObject*)values[1]);
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decompress", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 45, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("_lzokay.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expected_output_size), (&PyInt_Type), 1, "expected_output_size", 1))) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7_lzokay_2decompress(__pyx_self, __pyx_v_data, __pyx_v_expected_output_size);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_7_lzokay_2decompress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_expected_output_size) {
-  Py_ssize_t __pyx_v_data_size;
-  size_t __pyx_v_curren_array_size;
-  size_t __pyx_v_actual_out_size;
-  arrayobject *__pyx_v_b = 0;
-  __PYX_ENUM_CLASS_DECL lzokay::EResult __pyx_v_code;
-  uint8_t const *__pyx_v_data_bytes;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
-  int __pyx_t_2;
-  size_t __pyx_t_3;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  uint8_t const *__pyx_t_6;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decompress", 0);
-
-  /* "_lzokay.pyx":46
- * 
- * def decompress(data: bytes, expected_output_size: int = None) -> bytes:
- *     data_size = len(data)             # <<<<<<<<<<<<<<
- * 
- *     cdef size_t curren_array_size = data_size
- */
-  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 46, __pyx_L1_error)
-  __pyx_v_data_size = __pyx_t_1;
-
-  /* "_lzokay.pyx":48
- *     data_size = len(data)
- * 
- *     cdef size_t curren_array_size = data_size             # <<<<<<<<<<<<<<
- *     if expected_output_size is not None:
- *         curren_array_size = expected_output_size
- */
-  __pyx_v_curren_array_size = __pyx_v_data_size;
-
-  /* "_lzokay.pyx":49
- * 
- *     cdef size_t curren_array_size = data_size
- *     if expected_output_size is not None:             # <<<<<<<<<<<<<<
- *         curren_array_size = expected_output_size
- * 
- */
-  __pyx_t_2 = (__pyx_v_expected_output_size != ((PyObject*)Py_None));
-  if (__pyx_t_2) {
-
-    /* "_lzokay.pyx":50
- *     cdef size_t curren_array_size = data_size
- *     if expected_output_size is not None:
- *         curren_array_size = expected_output_size             # <<<<<<<<<<<<<<
- * 
- *     cdef size_t actual_out_size = 0
- */
-    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_expected_output_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L1_error)
-    __pyx_v_curren_array_size = __pyx_t_3;
-
-    /* "_lzokay.pyx":49
- * 
- *     cdef size_t curren_array_size = data_size
- *     if expected_output_size is not None:             # <<<<<<<<<<<<<<
- *         curren_array_size = expected_output_size
- * 
- */
-  }
-
-  /* "_lzokay.pyx":52
- *         curren_array_size = expected_output_size
- * 
- *     cdef size_t actual_out_size = 0             # <<<<<<<<<<<<<<
- *     cdef array.array b = array.array('B')
- *     array.resize(b, curren_array_size)
- */
-  __pyx_v_actual_out_size = 0;
-
-  /* "_lzokay.pyx":53
- * 
- *     cdef size_t actual_out_size = 0
- *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
- *     array.resize(b, curren_array_size)
- * 
- */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_v_b = ((arrayobject *)__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_RefNannySetupContext("__Pyx_Enum_EResult_to_py", 0);
 
-  /* "_lzokay.pyx":54
- *     cdef size_t actual_out_size = 0
- *     cdef array.array b = array.array('B')
- *     array.resize(b, curren_array_size)             # <<<<<<<<<<<<<<
+  /* "EnumTypeToPy":137
  * 
- *     cdef c_EResult code = c_EResult.OutputOverrun
- */
-  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
-
-  /* "_lzokay.pyx":56
- *     array.resize(b, curren_array_size)
  * 
- *     cdef c_EResult code = c_EResult.OutputOverrun             # <<<<<<<<<<<<<<
- *     cdef const uint8_t* data_bytes = data
- *     while code == c_EResult.OutputOverrun:
+ *     try:             # <<<<<<<<<<<<<<
+ *         from lzokay_wrap import EResult as __pyx_enum
+ *     except ImportError:
  */
-  __pyx_v_code = lzokay::EResult::OutputOverrun;
-
-  /* "_lzokay.pyx":57
- * 
- *     cdef c_EResult code = c_EResult.OutputOverrun
- *     cdef const uint8_t* data_bytes = data             # <<<<<<<<<<<<<<
- *     while code == c_EResult.OutputOverrun:
- *         with nogil:
- */
-  __pyx_t_6 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_v_data_bytes = __pyx_t_6;
-
-  /* "_lzokay.pyx":58
- *     cdef c_EResult code = c_EResult.OutputOverrun
- *     cdef const uint8_t* data_bytes = data
- *     while code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
- *         with nogil:
- *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
- */
-  while (1) {
-    __pyx_t_2 = (__pyx_v_code == lzokay::EResult::OutputOverrun);
-    if (!__pyx_t_2) break;
-
-    /* "_lzokay.pyx":59
- *     cdef const uint8_t* data_bytes = data
- *     while code == c_EResult.OutputOverrun:
- *         with nogil:             # <<<<<<<<<<<<<<
- *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
- * 
- */
-    {
-        #ifdef WITH_THREAD
-        PyThreadState *_save;
-        _save = NULL;
-        Py_UNBLOCK_THREADS
-        __Pyx_FastGIL_Remember();
-        #endif
-        /*try:*/ {
-
-          /* "_lzokay.pyx":60
- *     while code == c_EResult.OutputOverrun:
- *         with nogil:
- *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)             # <<<<<<<<<<<<<<
- * 
- *         if code == c_EResult.OutputOverrun:
- */
-          __pyx_v_code = lzokay::decompress(__pyx_v_data_bytes, __pyx_v_data_size, __pyx_v_b->data.as_uchars, __pyx_v_curren_array_size, __pyx_v_actual_out_size);
-        }
-
-        /* "_lzokay.pyx":59
- *     cdef const uint8_t* data_bytes = data
- *     while code == c_EResult.OutputOverrun:
- *         with nogil:             # <<<<<<<<<<<<<<
- *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
- * 
- */
-        /*finally:*/ {
-          /*normal exit:*/{
-            #ifdef WITH_THREAD
-            __Pyx_FastGIL_Forget();
-            Py_BLOCK_THREADS
-            #endif
-            goto __pyx_L10;
-          }
-          __pyx_L10:;
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "EnumTypeToPy":138
+ * 
+ *     try:
+ *         from lzokay_wrap import EResult as __pyx_enum             # <<<<<<<<<<<<<<
+ *     except ImportError:
+ *         import warnings
+ */
+      __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_INCREF(__pyx_n_s_EResult);
+      __Pyx_GIVEREF(__pyx_n_s_EResult);
+      PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_EResult);
+      __pyx_t_5 = __Pyx_Import(__pyx_n_s_lzokay_wrap, __pyx_t_4, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = __Pyx_ImportFrom(__pyx_t_5, __pyx_n_s_EResult); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_4);
+      __pyx_v___pyx_enum = __pyx_t_4;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+      /* "EnumTypeToPy":137
+ * 
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         from lzokay_wrap import EResult as __pyx_enum
+ *     except ImportError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "EnumTypeToPy":139
+ *     try:
+ *         from lzokay_wrap import EResult as __pyx_enum
+ *     except ImportError:             # <<<<<<<<<<<<<<
+ *         import warnings
+ *         warnings.warn(
+ */
+    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
+    if (__pyx_t_6) {
+      __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_EResult_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 139, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_4);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "EnumTypeToPy":140
+ *         from lzokay_wrap import EResult as __pyx_enum
+ *     except ImportError:
+ *         import warnings             # <<<<<<<<<<<<<<
+ *         warnings.warn(
+ *             f"enum class EResult not importable from lzokay_wrap. "
+ */
+      __pyx_t_8 = __Pyx_ImportDottedModule(__pyx_n_s_warnings, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 140, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_v_warnings = __pyx_t_8;
+      __pyx_t_8 = 0;
+
+      /* "EnumTypeToPy":141
+ *     except ImportError:
+ *         import warnings
+ *         warnings.warn(             # <<<<<<<<<<<<<<
+ *             f"enum class EResult not importable from lzokay_wrap. "
+ *             "You are probably using a cpdef enum declared in a .pxd file that "
+ */
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_warnings, __pyx_n_s_warn); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 141, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_10 = NULL;
+      __pyx_t_6 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+        if (likely(__pyx_t_10)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+          __Pyx_INCREF(__pyx_t_10);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_9, function);
+          __pyx_t_6 = 1;
         }
-    }
-
-    /* "_lzokay.pyx":62
- *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
- * 
- *         if code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
- *             curren_array_size *= 2
- *             array.resize(b, curren_array_size)
- */
-    __pyx_t_2 = (__pyx_v_code == lzokay::EResult::OutputOverrun);
-    if (__pyx_t_2) {
+      }
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_enum_class_EResult_not_importabl};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L5_except_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "_lzokay.pyx":63
- * 
- *         if code == c_EResult.OutputOverrun:
- *             curren_array_size *= 2             # <<<<<<<<<<<<<<
- *             array.resize(b, curren_array_size)
- * 
+      /* "EnumTypeToPy":145
+ *             "You are probably using a cpdef enum declared in a .pxd file that "
+ *             "does not have a .py  or .pyx file.")
+ *         return <int>c_val             # <<<<<<<<<<<<<<
+ * 
+ *     if 0:
+ */
+      __Pyx_XDECREF(__pyx_r);
+      __pyx_t_8 = __Pyx_PyInt_From_int(((int)__pyx_v_c_val)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_r = __pyx_t_8;
+      __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      goto __pyx_L6_except_return;
+    }
+    goto __pyx_L5_except_error;
+
+    /* "EnumTypeToPy":137
+ * 
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         from lzokay_wrap import EResult as __pyx_enum
+ *     except ImportError:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L6_except_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+    __pyx_L8_try_end:;
+  }
+
+  /* "EnumTypeToPy":149
+ *     if 0:
+ *         pass
+ *     elif c_val == EResult.LookbehindOverrun:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.LookbehindOverrun
+ *     elif c_val == EResult.OutputOverrun:
+ */
+  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::LookbehindOverrun);
+  if (__pyx_t_11) {
+
+    /* "EnumTypeToPy":150
+ *         pass
+ *     elif c_val == EResult.LookbehindOverrun:
+ *         return __pyx_enum.LookbehindOverrun             # <<<<<<<<<<<<<<
+ *     elif c_val == EResult.OutputOverrun:
+ *         return __pyx_enum.OutputOverrun
  */
-      __pyx_v_curren_array_size = (__pyx_v_curren_array_size * 2);
-
-      /* "_lzokay.pyx":64
- *         if code == c_EResult.OutputOverrun:
- *             curren_array_size *= 2
- *             array.resize(b, curren_array_size)             # <<<<<<<<<<<<<<
- * 
- *     array.resize(b, actual_out_size)
- */
-      __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 64, __pyx_L1_error)
-
-      /* "_lzokay.pyx":62
- *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
- * 
- *         if code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
- *             curren_array_size *= 2
- *             array.resize(b, curren_array_size)
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_LookbehindOverrun); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_r = __pyx_t_7;
+    __pyx_t_7 = 0;
+    goto __pyx_L0;
+
+    /* "EnumTypeToPy":149
+ *     if 0:
+ *         pass
+ *     elif c_val == EResult.LookbehindOverrun:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.LookbehindOverrun
+ *     elif c_val == EResult.OutputOverrun:
  */
-    }
   }
 
-  /* "_lzokay.pyx":66
- *             array.resize(b, curren_array_size)
- * 
- *     array.resize(b, actual_out_size)             # <<<<<<<<<<<<<<
- * 
- *     if code in result_mapping:
- */
-  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 66, __pyx_L1_error)
-
-  /* "_lzokay.pyx":68
- *     array.resize(b, actual_out_size)
- * 
- *     if code in result_mapping:             # <<<<<<<<<<<<<<
- *         raise result_mapping[code]()
- * 
+  /* "EnumTypeToPy":151
+ *     elif c_val == EResult.LookbehindOverrun:
+ *         return __pyx_enum.LookbehindOverrun
+ *     elif c_val == EResult.OutputOverrun:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.OutputOverrun
+ *     elif c_val == EResult.InputOverrun:
+ */
+  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::OutputOverrun);
+  if (__pyx_t_11) {
+
+    /* "EnumTypeToPy":152
+ *         return __pyx_enum.LookbehindOverrun
+ *     elif c_val == EResult.OutputOverrun:
+ *         return __pyx_enum.OutputOverrun             # <<<<<<<<<<<<<<
+ *     elif c_val == EResult.InputOverrun:
+ *         return __pyx_enum.InputOverrun
  */
-  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 68, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_4, __pyx_t_7, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 68, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(__pyx_t_2)) {
-
-    /* "_lzokay.pyx":69
- * 
- *     if code in result_mapping:
- *         raise result_mapping[code]()             # <<<<<<<<<<<<<<
- * 
- *     return b.tobytes()
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 69, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 69, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = NULL;
-    __pyx_t_5 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-        __Pyx_INCREF(__pyx_t_8);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_9, function);
-        __pyx_t_5 = 1;
-      }
-    }
-    {
-      PyObject *__pyx_callargs[1] = {__pyx_t_8, };
-      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 69, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    }
-    __Pyx_Raise(__pyx_t_7, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 69, __pyx_L1_error)
-
-    /* "_lzokay.pyx":68
- *     array.resize(b, actual_out_size)
- * 
- *     if code in result_mapping:             # <<<<<<<<<<<<<<
- *         raise result_mapping[code]()
- * 
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_OutputOverrun); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_r = __pyx_t_7;
+    __pyx_t_7 = 0;
+    goto __pyx_L0;
+
+    /* "EnumTypeToPy":151
+ *     elif c_val == EResult.LookbehindOverrun:
+ *         return __pyx_enum.LookbehindOverrun
+ *     elif c_val == EResult.OutputOverrun:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.OutputOverrun
+ *     elif c_val == EResult.InputOverrun:
  */
   }
 
-  /* "_lzokay.pyx":71
- *         raise result_mapping[code]()
- * 
- *     return b.tobytes()             # <<<<<<<<<<<<<<
- * 
- * 
+  /* "EnumTypeToPy":153
+ *     elif c_val == EResult.OutputOverrun:
+ *         return __pyx_enum.OutputOverrun
+ *     elif c_val == EResult.InputOverrun:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.InputOverrun
+ *     elif c_val == EResult.Error:
+ */
+  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::InputOverrun);
+  if (__pyx_t_11) {
+
+    /* "EnumTypeToPy":154
+ *         return __pyx_enum.OutputOverrun
+ *     elif c_val == EResult.InputOverrun:
+ *         return __pyx_enum.InputOverrun             # <<<<<<<<<<<<<<
+ *     elif c_val == EResult.Error:
+ *         return __pyx_enum.Error
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 71, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_8 = NULL;
-  __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_9, function);
-      __pyx_t_5 = 1;
-    }
-  }
-  {
-    PyObject *__pyx_callargs[1] = {__pyx_t_8, };
-    __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_InputOverrun); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  }
-  if (!(likely(PyBytes_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_7))) __PYX_ERR(0, 71, __pyx_L1_error)
-  __pyx_r = ((PyObject*)__pyx_t_7);
-  __pyx_t_7 = 0;
-  goto __pyx_L0;
-
-  /* "_lzokay.pyx":45
- * 
- * 
- * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
- *     data_size = len(data)
- * 
+    __pyx_r = __pyx_t_7;
+    __pyx_t_7 = 0;
+    goto __pyx_L0;
+
+    /* "EnumTypeToPy":153
+ *     elif c_val == EResult.OutputOverrun:
+ *         return __pyx_enum.OutputOverrun
+ *     elif c_val == EResult.InputOverrun:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.InputOverrun
+ *     elif c_val == EResult.Error:
  */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("_lzokay.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_b);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "_lzokay.pyx":74
- * 
- * 
- * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
- *     cdef const uint8_t* data_bytes = data
- *     cdef size_t data_size = len(data)
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_7_lzokay_5compress(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7_lzokay_4compress, "compress(bytes data: bytes) -> bytes");
-static PyMethodDef __pyx_mdef_7_lzokay_5compress = {"compress", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7_lzokay_5compress, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7_lzokay_4compress};
-static PyObject *__pyx_pw_7_lzokay_5compress(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_data = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("compress (wrapper)", 0);
-  {
-    #if CYTHON_USE_MODULE_STATE
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,0};
-    #else
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,0};
-    #endif
-    PyObject* values[1] = {0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress") < 0)) __PYX_ERR(0, 74, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v_data = ((PyObject*)values[0]);
   }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compress", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("_lzokay.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(0, 74, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7_lzokay_4compress(__pyx_self, __pyx_v_data);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
 
-static PyObject *__pyx_pf_7_lzokay_4compress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data) {
-  uint8_t const *__pyx_v_data_bytes;
-  size_t __pyx_v_data_size;
-  size_t __pyx_v_expected_out_size;
-  arrayobject *__pyx_v_b = 0;
-  __PYX_ENUM_CLASS_DECL lzokay::EResult __pyx_v_code;
-  size_t __pyx_v_actual_out_size;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  uint8_t const *__pyx_t_1;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("compress", 0);
-
-  /* "_lzokay.pyx":75
- * 
- * def compress(data: bytes) -> bytes:
- *     cdef const uint8_t* data_bytes = data             # <<<<<<<<<<<<<<
- *     cdef size_t data_size = len(data)
- *     cdef size_t expected_out_size = compress_worst_size(data_size)
- */
-  __pyx_t_1 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_v_data_bytes = __pyx_t_1;
-
-  /* "_lzokay.pyx":76
- * def compress(data: bytes) -> bytes:
- *     cdef const uint8_t* data_bytes = data
- *     cdef size_t data_size = len(data)             # <<<<<<<<<<<<<<
- *     cdef size_t expected_out_size = compress_worst_size(data_size)
- * 
- */
-  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 76, __pyx_L1_error)
-  __pyx_v_data_size = __pyx_t_2;
-
-  /* "_lzokay.pyx":77
- *     cdef const uint8_t* data_bytes = data
- *     cdef size_t data_size = len(data)
- *     cdef size_t expected_out_size = compress_worst_size(data_size)             # <<<<<<<<<<<<<<
- * 
- *     cdef array.array b = array.array('B')
+  /* "EnumTypeToPy":155
+ *     elif c_val == EResult.InputOverrun:
+ *         return __pyx_enum.InputOverrun
+ *     elif c_val == EResult.Error:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.Error
+ *     elif c_val == EResult.Success:
+ */
+  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::Error);
+  if (__pyx_t_11) {
+
+    /* "EnumTypeToPy":156
+ *         return __pyx_enum.InputOverrun
+ *     elif c_val == EResult.Error:
+ *         return __pyx_enum.Error             # <<<<<<<<<<<<<<
+ *     elif c_val == EResult.Success:
+ *         return __pyx_enum.Success
  */
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(PyInt_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_v_expected_out_size = __pyx_f_7_lzokay_compress_worst_size(((PyObject*)__pyx_t_3), 0);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-  /* "_lzokay.pyx":79
- *     cdef size_t expected_out_size = compress_worst_size(data_size)
- * 
- *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
- *     array.resize(b, expected_out_size)
- * 
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_Error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_r = __pyx_t_7;
+    __pyx_t_7 = 0;
+    goto __pyx_L0;
+
+    /* "EnumTypeToPy":155
+ *     elif c_val == EResult.InputOverrun:
+ *         return __pyx_enum.InputOverrun
+ *     elif c_val == EResult.Error:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.Error
+ *     elif c_val == EResult.Success:
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_v_b = ((arrayobject *)__pyx_t_3);
-  __pyx_t_3 = 0;
+  }
 
-  /* "_lzokay.pyx":80
- * 
- *     cdef array.array b = array.array('B')
- *     array.resize(b, expected_out_size)             # <<<<<<<<<<<<<<
- * 
- *     # Results from c_compress
+  /* "EnumTypeToPy":157
+ *     elif c_val == EResult.Error:
+ *         return __pyx_enum.Error
+ *     elif c_val == EResult.Success:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.Success
+ *     elif c_val == EResult.InputNotConsumed:
+ */
+  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::Success);
+  if (__pyx_t_11) {
+
+    /* "EnumTypeToPy":158
+ *         return __pyx_enum.Error
+ *     elif c_val == EResult.Success:
+ *         return __pyx_enum.Success             # <<<<<<<<<<<<<<
+ *     elif c_val == EResult.InputNotConsumed:
+ *         return __pyx_enum.InputNotConsumed
  */
-  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_expected_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 80, __pyx_L1_error)
-
-  /* "_lzokay.pyx":84
- *     # Results from c_compress
- *     cdef c_EResult code
- *     cdef size_t actual_out_size = 0             # <<<<<<<<<<<<<<
- * 
- *     with nogil:
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_Success); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_r = __pyx_t_7;
+    __pyx_t_7 = 0;
+    goto __pyx_L0;
+
+    /* "EnumTypeToPy":157
+ *     elif c_val == EResult.Error:
+ *         return __pyx_enum.Error
+ *     elif c_val == EResult.Success:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.Success
+ *     elif c_val == EResult.InputNotConsumed:
  */
-  __pyx_v_actual_out_size = 0;
+  }
 
-  /* "_lzokay.pyx":86
- *     cdef size_t actual_out_size = 0
- * 
- *     with nogil:             # <<<<<<<<<<<<<<
- *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
- * 
+  /* "EnumTypeToPy":159
+ *     elif c_val == EResult.Success:
+ *         return __pyx_enum.Success
+ *     elif c_val == EResult.InputNotConsumed:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.InputNotConsumed
+ *     else:
  */
-  {
-      #ifdef WITH_THREAD
-      PyThreadState *_save;
-      _save = NULL;
-      Py_UNBLOCK_THREADS
-      __Pyx_FastGIL_Remember();
-      #endif
-      /*try:*/ {
+  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::InputNotConsumed);
+  if (likely(__pyx_t_11)) {
 
-        /* "_lzokay.pyx":87
- * 
- *     with nogil:
- *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)             # <<<<<<<<<<<<<<
- * 
- *     array.resize(b, actual_out_size)
+    /* "EnumTypeToPy":160
+ *         return __pyx_enum.Success
+ *     elif c_val == EResult.InputNotConsumed:
+ *         return __pyx_enum.InputNotConsumed             # <<<<<<<<<<<<<<
+ *     else:
+ *         underlying_c_val = <int>c_val
  */
-        __pyx_v_code = lzokay::compress(__pyx_v_data_bytes, __pyx_v_data_size, __pyx_v_b->data.as_uchars, __pyx_v_expected_out_size, __pyx_v_actual_out_size);
-      }
-
-      /* "_lzokay.pyx":86
- *     cdef size_t actual_out_size = 0
- * 
- *     with nogil:             # <<<<<<<<<<<<<<
- *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
- * 
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_InputNotConsumed); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_r = __pyx_t_7;
+    __pyx_t_7 = 0;
+    goto __pyx_L0;
+
+    /* "EnumTypeToPy":159
+ *     elif c_val == EResult.Success:
+ *         return __pyx_enum.Success
+ *     elif c_val == EResult.InputNotConsumed:             # <<<<<<<<<<<<<<
+ *         return __pyx_enum.InputNotConsumed
+ *     else:
  */
-      /*finally:*/ {
-        /*normal exit:*/{
-          #ifdef WITH_THREAD
-          __Pyx_FastGIL_Forget();
-          Py_BLOCK_THREADS
-          #endif
-          goto __pyx_L5;
-        }
-        __pyx_L5:;
-      }
   }
 
-  /* "_lzokay.pyx":89
- *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
- * 
- *     array.resize(b, actual_out_size)             # <<<<<<<<<<<<<<
- * 
- *     if code in result_mapping:
- */
-  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 89, __pyx_L1_error)
-
-  /* "_lzokay.pyx":91
- *     array.resize(b, actual_out_size)
- * 
- *     if code in result_mapping:             # <<<<<<<<<<<<<<
- *         raise result_mapping[code]()
+  /* "EnumTypeToPy":162
+ *         return __pyx_enum.InputNotConsumed
+ *     else:
+ *         underlying_c_val = <int>c_val             # <<<<<<<<<<<<<<
+ *         raise ValueError(f"{underlying_c_val} is not a valid EResult")
  * 
  */
-  __pyx_t_3 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_5, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(__pyx_t_6)) {
+  /*else*/ {
+    __pyx_v_underlying_c_val = ((int)__pyx_v_c_val);
 
-    /* "_lzokay.pyx":92
- * 
- *     if code in result_mapping:
- *         raise result_mapping[code]()             # <<<<<<<<<<<<<<
+    /* "EnumTypeToPy":163
+ *     else:
+ *         underlying_c_val = <int>c_val
+ *         raise ValueError(f"{underlying_c_val} is not a valid EResult")             # <<<<<<<<<<<<<<
  * 
- *     return b.tobytes()
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_underlying_c_val, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_7, __pyx_kp_u_is_not_a_valid_EResult); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = NULL;
-    __pyx_t_4 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_4 = 1;
-      }
-    }
-    {
-      PyObject *__pyx_callargs[1] = {__pyx_t_7, };
-      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    }
-    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 92, __pyx_L1_error)
-
-    /* "_lzokay.pyx":91
- *     array.resize(b, actual_out_size)
- * 
- *     if code in result_mapping:             # <<<<<<<<<<<<<<
- *         raise result_mapping[code]()
- * 
- */
-  }
-
-  /* "_lzokay.pyx":94
- *         raise result_mapping[code]()
- * 
- *     return b.tobytes()             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = NULL;
-  __pyx_t_4 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_7);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
-      __pyx_t_4 = 1;
-    }
-  }
-  {
-    PyObject *__pyx_callargs[1] = {__pyx_t_7, };
-    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_Raise(__pyx_t_7, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __PYX_ERR(0, 163, __pyx_L1_error)
   }
-  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_5))) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_r = ((PyObject*)__pyx_t_5);
-  __pyx_t_5 = 0;
-  goto __pyx_L0;
 
-  /* "_lzokay.pyx":74
+  /* "EnumTypeToPy":132
  * 
+ * @cname("__Pyx_Enum_EResult_to_py")
+ * cdef __Pyx_Enum_EResult_to_py(EResult c_val):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_enum
  * 
- * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
- *     cdef const uint8_t* data_bytes = data
- *     cdef size_t data_size = len(data)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("_lzokay.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_EResult_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_b);
+  __Pyx_XDECREF(__pyx_v___pyx_enum);
+  __Pyx_XDECREF(__pyx_v_warnings);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
@@ -4081,16 +3788,16 @@
  * 
  *         def __getbuffer__(self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
 /* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_7cpython_5array_5array_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_7cpython_5array_5array_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
+CYTHON_UNUSED static int __pyx_pw_7cpython_5array_5array_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
+CYTHON_UNUSED static int __pyx_pw_7cpython_5array_5array_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
   __pyx_r = __pyx_pf_7cpython_5array_5array___getbuffer__(((arrayobject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
 
   /* function exit code */
@@ -4329,16 +4036,16 @@
  * 
  *         def __releasebuffer__(self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             PyObject_Free(info.shape)
  * 
  */
 
 /* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_7cpython_5array_5array_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_7cpython_5array_5array_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
+CYTHON_UNUSED static void __pyx_pw_7cpython_5array_5array_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
+CYTHON_UNUSED static void __pyx_pw_7cpython_5array_5array_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
   __pyx_pf_7cpython_5array_5array_2__releasebuffer__(((arrayobject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -4723,263 +4430,1138 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
+/* "lzokay/_lzokay.pyx":41
+ * 
+ * 
+ * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
+ *     return s + s // 16 + 64 + 3
+ * 
+ */
+
+static PyObject *__pyx_pw_6lzokay_7_lzokay_1compress_worst_size(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static int __pyx_f_6lzokay_7_lzokay_compress_worst_size(PyObject *__pyx_v_s, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("compress_worst_size", 0);
+
+  /* "lzokay/_lzokay.pyx":42
+ * 
+ * cpdef int compress_worst_size(s: int):
+ *     return s + s // 16 + 64 + 3             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = PyNumber_FloorDivide(__pyx_v_s, __pyx_int_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyNumber_Add(__pyx_v_s, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_64, 64, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_3, 3, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(3, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_3;
+  goto __pyx_L0;
+
+  /* "lzokay/_lzokay.pyx":41
+ * 
+ * 
+ * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
+ *     return s + s // 16 + 64 + 3
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("lzokay._lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6lzokay_7_lzokay_1compress_worst_size(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6lzokay_7_lzokay_compress_worst_size, "compress_worst_size(int s: int) -> int");
+static PyMethodDef __pyx_mdef_6lzokay_7_lzokay_1compress_worst_size = {"compress_worst_size", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6lzokay_7_lzokay_1compress_worst_size, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6lzokay_7_lzokay_compress_worst_size};
+static PyObject *__pyx_pw_6lzokay_7_lzokay_1compress_worst_size(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_s = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("compress_worst_size (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_s,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 41, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress_worst_size") < 0)) __PYX_ERR(3, 41, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_s = ((PyObject*)values[0]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("compress_worst_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(3, 41, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("lzokay._lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyInt_Type), 0, "s", 1))) __PYX_ERR(3, 41, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6lzokay_7_lzokay_compress_worst_size(__pyx_self, __pyx_v_s);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6lzokay_7_lzokay_compress_worst_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("compress_worst_size", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_f_6lzokay_7_lzokay_compress_worst_size(__pyx_v_s, 0); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(3, 41, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("lzokay._lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "lzokay/_lzokay.pyx":45
+ * 
+ * 
+ * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
+ *     data_size = len(data)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6lzokay_7_lzokay_3decompress(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6lzokay_7_lzokay_2decompress, "decompress(bytes data: bytes, int expected_output_size: int = None) -> bytes");
+static PyMethodDef __pyx_mdef_6lzokay_7_lzokay_3decompress = {"decompress", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6lzokay_7_lzokay_3decompress, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6lzokay_7_lzokay_2decompress};
+static PyObject *__pyx_pw_6lzokay_7_lzokay_3decompress(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_data = 0;
+  PyObject *__pyx_v_expected_output_size = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("decompress (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,&__pyx_n_s_expected_output_size,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject*)((PyObject *)Py_None));
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 45, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_expected_output_size);
+          if (value) { values[1] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 45, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decompress") < 0)) __PYX_ERR(3, 45, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_data = ((PyObject*)values[0]);
+    __pyx_v_expected_output_size = ((PyObject*)values[1]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("decompress", 0, 1, 2, __pyx_nargs); __PYX_ERR(3, 45, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("lzokay._lzokay.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(3, 45, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expected_output_size), (&PyInt_Type), 1, "expected_output_size", 1))) __PYX_ERR(3, 45, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6lzokay_7_lzokay_2decompress(__pyx_self, __pyx_v_data, __pyx_v_expected_output_size);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6lzokay_7_lzokay_2decompress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_expected_output_size) {
+  Py_ssize_t __pyx_v_data_size;
+  size_t __pyx_v_curren_array_size;
+  size_t __pyx_v_actual_out_size;
+  arrayobject *__pyx_v_b = 0;
+  __PYX_ENUM_CLASS_DECL lzokay::EResult __pyx_v_code;
+  uint8_t const *__pyx_v_data_bytes;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
+  size_t __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  uint8_t const *__pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("decompress", 0);
+
+  /* "lzokay/_lzokay.pyx":46
+ * 
+ * def decompress(data: bytes, expected_output_size: int = None) -> bytes:
+ *     data_size = len(data)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef size_t curren_array_size = data_size
+ */
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(3, 46, __pyx_L1_error)
+  __pyx_v_data_size = __pyx_t_1;
+
+  /* "lzokay/_lzokay.pyx":48
+ *     data_size = len(data)
+ * 
+ *     cdef size_t curren_array_size = data_size             # <<<<<<<<<<<<<<
+ *     if expected_output_size is not None:
+ *         curren_array_size = expected_output_size
+ */
+  __pyx_v_curren_array_size = __pyx_v_data_size;
+
+  /* "lzokay/_lzokay.pyx":49
+ * 
+ *     cdef size_t curren_array_size = data_size
+ *     if expected_output_size is not None:             # <<<<<<<<<<<<<<
+ *         curren_array_size = expected_output_size
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_expected_output_size != ((PyObject*)Py_None));
+  if (__pyx_t_2) {
+
+    /* "lzokay/_lzokay.pyx":50
+ *     cdef size_t curren_array_size = data_size
+ *     if expected_output_size is not None:
+ *         curren_array_size = expected_output_size             # <<<<<<<<<<<<<<
+ * 
+ *     cdef size_t actual_out_size = 0
+ */
+    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_expected_output_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(3, 50, __pyx_L1_error)
+    __pyx_v_curren_array_size = __pyx_t_3;
+
+    /* "lzokay/_lzokay.pyx":49
+ * 
+ *     cdef size_t curren_array_size = data_size
+ *     if expected_output_size is not None:             # <<<<<<<<<<<<<<
+ *         curren_array_size = expected_output_size
+ * 
+ */
+  }
+
+  /* "lzokay/_lzokay.pyx":52
+ *         curren_array_size = expected_output_size
+ * 
+ *     cdef size_t actual_out_size = 0             # <<<<<<<<<<<<<<
+ *     cdef array.array b = array.array('B')
+ *     array.resize(b, curren_array_size)
+ */
+  __pyx_v_actual_out_size = 0;
+
+  /* "lzokay/_lzokay.pyx":53
+ * 
+ *     cdef size_t actual_out_size = 0
+ *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
+ *     array.resize(b, curren_array_size)
+ * 
+ */
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_b = ((arrayobject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "lzokay/_lzokay.pyx":54
+ *     cdef size_t actual_out_size = 0
+ *     cdef array.array b = array.array('B')
+ *     array.resize(b, curren_array_size)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef c_EResult code = c_EResult.OutputOverrun
+ */
+  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(3, 54, __pyx_L1_error)
+
+  /* "lzokay/_lzokay.pyx":56
+ *     array.resize(b, curren_array_size)
+ * 
+ *     cdef c_EResult code = c_EResult.OutputOverrun             # <<<<<<<<<<<<<<
+ *     cdef const uint8_t* data_bytes = data
+ *     while code == c_EResult.OutputOverrun:
+ */
+  __pyx_v_code = lzokay::EResult::OutputOverrun;
+
+  /* "lzokay/_lzokay.pyx":57
+ * 
+ *     cdef c_EResult code = c_EResult.OutputOverrun
+ *     cdef const uint8_t* data_bytes = data             # <<<<<<<<<<<<<<
+ *     while code == c_EResult.OutputOverrun:
+ *         with nogil:
+ */
+  __pyx_t_6 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(3, 57, __pyx_L1_error)
+  __pyx_v_data_bytes = __pyx_t_6;
+
+  /* "lzokay/_lzokay.pyx":58
+ *     cdef c_EResult code = c_EResult.OutputOverrun
+ *     cdef const uint8_t* data_bytes = data
+ *     while code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
+ *         with nogil:
+ *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
+ */
+  while (1) {
+    __pyx_t_2 = (__pyx_v_code == lzokay::EResult::OutputOverrun);
+    if (!__pyx_t_2) break;
+
+    /* "lzokay/_lzokay.pyx":59
+ *     cdef const uint8_t* data_bytes = data
+ *     while code == c_EResult.OutputOverrun:
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
+ * 
+ */
+    {
+        #ifdef WITH_THREAD
+        PyThreadState *_save;
+        _save = NULL;
+        Py_UNBLOCK_THREADS
+        __Pyx_FastGIL_Remember();
+        #endif
+        /*try:*/ {
+
+          /* "lzokay/_lzokay.pyx":60
+ *     while code == c_EResult.OutputOverrun:
+ *         with nogil:
+ *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)             # <<<<<<<<<<<<<<
+ * 
+ *         if code == c_EResult.OutputOverrun:
+ */
+          __pyx_v_code = lzokay::decompress(__pyx_v_data_bytes, __pyx_v_data_size, __pyx_v_b->data.as_uchars, __pyx_v_curren_array_size, __pyx_v_actual_out_size);
+        }
+
+        /* "lzokay/_lzokay.pyx":59
+ *     cdef const uint8_t* data_bytes = data
+ *     while code == c_EResult.OutputOverrun:
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
+ * 
+ */
+        /*finally:*/ {
+          /*normal exit:*/{
+            #ifdef WITH_THREAD
+            __Pyx_FastGIL_Forget();
+            Py_BLOCK_THREADS
+            #endif
+            goto __pyx_L10;
+          }
+          __pyx_L10:;
+        }
+    }
+
+    /* "lzokay/_lzokay.pyx":62
+ *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
+ * 
+ *         if code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
+ *             curren_array_size *= 2
+ *             array.resize(b, curren_array_size)
+ */
+    __pyx_t_2 = (__pyx_v_code == lzokay::EResult::OutputOverrun);
+    if (__pyx_t_2) {
+
+      /* "lzokay/_lzokay.pyx":63
+ * 
+ *         if code == c_EResult.OutputOverrun:
+ *             curren_array_size *= 2             # <<<<<<<<<<<<<<
+ *             array.resize(b, curren_array_size)
+ * 
+ */
+      __pyx_v_curren_array_size = (__pyx_v_curren_array_size * 2);
+
+      /* "lzokay/_lzokay.pyx":64
+ *         if code == c_EResult.OutputOverrun:
+ *             curren_array_size *= 2
+ *             array.resize(b, curren_array_size)             # <<<<<<<<<<<<<<
+ * 
+ *     array.resize(b, actual_out_size)
+ */
+      __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(3, 64, __pyx_L1_error)
+
+      /* "lzokay/_lzokay.pyx":62
+ *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
+ * 
+ *         if code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
+ *             curren_array_size *= 2
+ *             array.resize(b, curren_array_size)
+ */
+    }
+  }
+
+  /* "lzokay/_lzokay.pyx":66
+ *             array.resize(b, curren_array_size)
+ * 
+ *     array.resize(b, actual_out_size)             # <<<<<<<<<<<<<<
+ * 
+ *     if code in result_mapping:
+ */
+  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(3, 66, __pyx_L1_error)
+
+  /* "lzokay/_lzokay.pyx":68
+ *     array.resize(b, actual_out_size)
+ * 
+ *     if code in result_mapping:             # <<<<<<<<<<<<<<
+ *         raise result_mapping[code]()
+ * 
+ */
+  __pyx_t_4 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_4, __pyx_t_7, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(3, 68, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (unlikely(__pyx_t_2)) {
+
+    /* "lzokay/_lzokay.pyx":69
+ * 
+ *     if code in result_mapping:
+ *         raise result_mapping[code]()             # <<<<<<<<<<<<<<
+ * 
+ *     return b.tobytes()
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 69, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_8 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 69, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 69, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = NULL;
+    __pyx_t_5 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_9, function);
+        __pyx_t_5 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_8, };
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 69, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    }
+    __Pyx_Raise(__pyx_t_7, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __PYX_ERR(3, 69, __pyx_L1_error)
+
+    /* "lzokay/_lzokay.pyx":68
+ *     array.resize(b, actual_out_size)
+ * 
+ *     if code in result_mapping:             # <<<<<<<<<<<<<<
+ *         raise result_mapping[code]()
+ * 
+ */
+  }
+
+  /* "lzokay/_lzokay.pyx":71
+ *         raise result_mapping[code]()
+ * 
+ *     return b.tobytes()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_8 = NULL;
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_9, function);
+      __pyx_t_5 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_8, };
+    __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 71, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  }
+  if (!(likely(PyBytes_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_7))) __PYX_ERR(3, 71, __pyx_L1_error)
+  __pyx_r = ((PyObject*)__pyx_t_7);
+  __pyx_t_7 = 0;
+  goto __pyx_L0;
+
+  /* "lzokay/_lzokay.pyx":45
+ * 
+ * 
+ * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
+ *     data_size = len(data)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("lzokay._lzokay.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_b);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "lzokay/_lzokay.pyx":74
+ * 
+ * 
+ * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
+ *     cdef const uint8_t* data_bytes = data
+ *     cdef size_t data_size = len(data)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6lzokay_7_lzokay_5compress(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6lzokay_7_lzokay_4compress, "compress(bytes data: bytes) -> bytes");
+static PyMethodDef __pyx_mdef_6lzokay_7_lzokay_5compress = {"compress", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6lzokay_7_lzokay_5compress, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6lzokay_7_lzokay_4compress};
+static PyObject *__pyx_pw_6lzokay_7_lzokay_5compress(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_data = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("compress (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 74, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress") < 0)) __PYX_ERR(3, 74, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_data = ((PyObject*)values[0]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("compress", 1, 1, 1, __pyx_nargs); __PYX_ERR(3, 74, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("lzokay._lzokay.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(3, 74, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6lzokay_7_lzokay_4compress(__pyx_self, __pyx_v_data);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6lzokay_7_lzokay_4compress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data) {
+  uint8_t const *__pyx_v_data_bytes;
+  size_t __pyx_v_data_size;
+  size_t __pyx_v_expected_out_size;
+  arrayobject *__pyx_v_b = 0;
+  __PYX_ENUM_CLASS_DECL lzokay::EResult __pyx_v_code;
+  size_t __pyx_v_actual_out_size;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  uint8_t const *__pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("compress", 0);
+
+  /* "lzokay/_lzokay.pyx":75
+ * 
+ * def compress(data: bytes) -> bytes:
+ *     cdef const uint8_t* data_bytes = data             # <<<<<<<<<<<<<<
+ *     cdef size_t data_size = len(data)
+ *     cdef size_t expected_out_size = compress_worst_size(data_size)
+ */
+  __pyx_t_1 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(3, 75, __pyx_L1_error)
+  __pyx_v_data_bytes = __pyx_t_1;
+
+  /* "lzokay/_lzokay.pyx":76
+ * def compress(data: bytes) -> bytes:
+ *     cdef const uint8_t* data_bytes = data
+ *     cdef size_t data_size = len(data)             # <<<<<<<<<<<<<<
+ *     cdef size_t expected_out_size = compress_worst_size(data_size)
+ * 
+ */
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(3, 76, __pyx_L1_error)
+  __pyx_v_data_size = __pyx_t_2;
+
+  /* "lzokay/_lzokay.pyx":77
+ *     cdef const uint8_t* data_bytes = data
+ *     cdef size_t data_size = len(data)
+ *     cdef size_t expected_out_size = compress_worst_size(data_size)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef array.array b = array.array('B')
+ */
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(3, 77, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_6lzokay_7_lzokay_compress_worst_size(((PyObject*)__pyx_t_3), 0); if (unlikely(__pyx_t_4 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(3, 77, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_expected_out_size = __pyx_t_4;
+
+  /* "lzokay/_lzokay.pyx":79
+ *     cdef size_t expected_out_size = compress_worst_size(data_size)
+ * 
+ *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
+ *     array.resize(b, expected_out_size)
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_v_b = ((arrayobject *)__pyx_t_3);
+  __pyx_t_3 = 0;
+
+  /* "lzokay/_lzokay.pyx":80
+ * 
+ *     cdef array.array b = array.array('B')
+ *     array.resize(b, expected_out_size)             # <<<<<<<<<<<<<<
+ * 
+ *     # Results from c_compress
+ */
+  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_expected_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 80, __pyx_L1_error)
+
+  /* "lzokay/_lzokay.pyx":84
+ *     # Results from c_compress
+ *     cdef c_EResult code
+ *     cdef size_t actual_out_size = 0             # <<<<<<<<<<<<<<
+ * 
+ *     with nogil:
+ */
+  __pyx_v_actual_out_size = 0;
+
+  /* "lzokay/_lzokay.pyx":86
+ *     cdef size_t actual_out_size = 0
+ * 
+ *     with nogil:             # <<<<<<<<<<<<<<
+ *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
+ * 
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      _save = NULL;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "lzokay/_lzokay.pyx":87
+ * 
+ *     with nogil:
+ *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)             # <<<<<<<<<<<<<<
+ * 
+ *     array.resize(b, actual_out_size)
+ */
+        __pyx_v_code = lzokay::compress(__pyx_v_data_bytes, __pyx_v_data_size, __pyx_v_b->data.as_uchars, __pyx_v_expected_out_size, __pyx_v_actual_out_size);
+      }
+
+      /* "lzokay/_lzokay.pyx":86
+ *     cdef size_t actual_out_size = 0
+ * 
+ *     with nogil:             # <<<<<<<<<<<<<<
+ *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
+ * 
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "lzokay/_lzokay.pyx":89
+ *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
+ * 
+ *     array.resize(b, actual_out_size)             # <<<<<<<<<<<<<<
+ * 
+ *     if code in result_mapping:
+ */
+  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 89, __pyx_L1_error)
+
+  /* "lzokay/_lzokay.pyx":91
+ *     array.resize(b, actual_out_size)
+ * 
+ *     if code in result_mapping:             # <<<<<<<<<<<<<<
+ *         raise result_mapping[code]()
+ * 
+ */
+  __pyx_t_3 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_5, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(3, 91, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(__pyx_t_6)) {
+
+    /* "lzokay/_lzokay.pyx":92
+ * 
+ *     if code in result_mapping:
+ *         raise result_mapping[code]()             # <<<<<<<<<<<<<<
+ * 
+ *     return b.tobytes()
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 92, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 92, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 92, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = NULL;
+    __pyx_t_4 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[1] = {__pyx_t_7, };
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 92, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
+    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __PYX_ERR(3, 92, __pyx_L1_error)
+
+    /* "lzokay/_lzokay.pyx":91
+ *     array.resize(b, actual_out_size)
+ * 
+ *     if code in result_mapping:             # <<<<<<<<<<<<<<
+ *         raise result_mapping[code]()
+ * 
+ */
+  }
+
+  /* "lzokay/_lzokay.pyx":94
+ *         raise result_mapping[code]()
+ * 
+ *     return b.tobytes()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_7 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_7, };
+    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 94, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  }
+  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_5))) __PYX_ERR(3, 94, __pyx_L1_error)
+  __pyx_r = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "lzokay/_lzokay.pyx":74
+ * 
+ * 
+ * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
+ *     cdef const uint8_t* data_bytes = data
+ *     cdef size_t data_size = len(data)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("lzokay._lzokay.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_b);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  #if CYTHON_USE_MODULE_STATE
-  {0, __pyx_k_B, sizeof(__pyx_k_B), 0, 1, 0, 1},
-  {0, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
-  {0, __pyx_k_InputNotConsumed, sizeof(__pyx_k_InputNotConsumed), 0, 0, 1, 1},
-  {0, __pyx_k_InputOverrun, sizeof(__pyx_k_InputOverrun), 0, 0, 1, 1},
-  {0, __pyx_k_LookbehindOverrun, sizeof(__pyx_k_LookbehindOverrun), 0, 0, 1, 1},
-  {0, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
-  {0, __pyx_k_OutputOverrun, sizeof(__pyx_k_OutputOverrun), 0, 0, 1, 1},
-  {0, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
-  {0, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
-  {0, __pyx_k_actual_out_size, sizeof(__pyx_k_actual_out_size), 0, 0, 1, 1},
-  {0, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
-  {0, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-  {0, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
-  {0, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
-  {0, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
-  {0, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {0, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
-  {0, __pyx_k_compress, sizeof(__pyx_k_compress), 0, 0, 1, 1},
-  {0, __pyx_k_compress_worst_size, sizeof(__pyx_k_compress_worst_size), 0, 0, 1, 1},
-  {0, __pyx_k_curren_array_size, sizeof(__pyx_k_curren_array_size), 0, 0, 1, 1},
-  {0, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {0, __pyx_k_data_bytes, sizeof(__pyx_k_data_bytes), 0, 0, 1, 1},
-  {0, __pyx_k_data_size, sizeof(__pyx_k_data_size), 0, 0, 1, 1},
-  {0, __pyx_k_decompress, sizeof(__pyx_k_decompress), 0, 0, 1, 1},
-  {0, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-  {0, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {0, __pyx_k_expected_out_size, sizeof(__pyx_k_expected_out_size), 0, 0, 1, 1},
-  {0, __pyx_k_expected_output_size, sizeof(__pyx_k_expected_output_size), 0, 0, 1, 1},
-  {0, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {0, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
-  {0, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
-  {0, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
-  {0, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-  {0, __pyx_k_lzokay, sizeof(__pyx_k_lzokay), 0, 0, 1, 1},
-  {0, __pyx_k_lzokay_pyx, sizeof(__pyx_k_lzokay_pyx), 0, 0, 1, 0},
-  {0, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {0, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-  {0, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
-  {0, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
-  {0, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {0, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-  {0, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-  {0, __pyx_k_result_mapping, sizeof(__pyx_k_result_mapping), 0, 0, 1, 1},
-  {0, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
-  {0, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
-  {0, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
-  {0, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
-  {0, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
-  {0, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {0, __pyx_k_tobytes, sizeof(__pyx_k_tobytes), 0, 0, 1, 1},
-  #else
-  {&__pyx_n_u_B, __pyx_k_B, sizeof(__pyx_k_B), 0, 1, 0, 1},
-  {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
-  {&__pyx_n_s_InputNotConsumed, __pyx_k_InputNotConsumed, sizeof(__pyx_k_InputNotConsumed), 0, 0, 1, 1},
-  {&__pyx_n_s_InputOverrun, __pyx_k_InputOverrun, sizeof(__pyx_k_InputOverrun), 0, 0, 1, 1},
-  {&__pyx_n_s_LookbehindOverrun, __pyx_k_LookbehindOverrun, sizeof(__pyx_k_LookbehindOverrun), 0, 0, 1, 1},
-  {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
-  {&__pyx_n_s_OutputOverrun, __pyx_k_OutputOverrun, sizeof(__pyx_k_OutputOverrun), 0, 0, 1, 1},
-  {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
-  {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
-  {&__pyx_n_s_actual_out_size, __pyx_k_actual_out_size, sizeof(__pyx_k_actual_out_size), 0, 0, 1, 1},
-  {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
-  {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-  {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
-  {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
-  {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_code, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
-  {&__pyx_n_s_compress, __pyx_k_compress, sizeof(__pyx_k_compress), 0, 0, 1, 1},
-  {&__pyx_n_s_compress_worst_size, __pyx_k_compress_worst_size, sizeof(__pyx_k_compress_worst_size), 0, 0, 1, 1},
-  {&__pyx_n_s_curren_array_size, __pyx_k_curren_array_size, sizeof(__pyx_k_curren_array_size), 0, 0, 1, 1},
-  {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {&__pyx_n_s_data_bytes, __pyx_k_data_bytes, sizeof(__pyx_k_data_bytes), 0, 0, 1, 1},
-  {&__pyx_n_s_data_size, __pyx_k_data_size, sizeof(__pyx_k_data_size), 0, 0, 1, 1},
-  {&__pyx_n_s_decompress, __pyx_k_decompress, sizeof(__pyx_k_decompress), 0, 0, 1, 1},
-  {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-  {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_expected_out_size, __pyx_k_expected_out_size, sizeof(__pyx_k_expected_out_size), 0, 0, 1, 1},
-  {&__pyx_n_s_expected_output_size, __pyx_k_expected_output_size, sizeof(__pyx_k_expected_output_size), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
-  {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
-  {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-  {&__pyx_n_s_lzokay, __pyx_k_lzokay, sizeof(__pyx_k_lzokay), 0, 0, 1, 1},
-  {&__pyx_kp_s_lzokay_pyx, __pyx_k_lzokay_pyx, sizeof(__pyx_k_lzokay_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-  {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
-  {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-  {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-  {&__pyx_n_s_result_mapping, __pyx_k_result_mapping, sizeof(__pyx_k_result_mapping), 0, 0, 1, 1},
-  {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
-  {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
-  {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
-  {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
-  {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_tobytes, __pyx_k_tobytes, sizeof(__pyx_k_tobytes), 0, 0, 1, 1},
-  #endif
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
+    {&__pyx_n_u_B, __pyx_k_B, sizeof(__pyx_k_B), 0, 1, 0, 1},
+    {&__pyx_n_s_EResult, __pyx_k_EResult, sizeof(__pyx_k_EResult), 0, 0, 1, 1},
+    {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s_InputNotConsumed, __pyx_k_InputNotConsumed, sizeof(__pyx_k_InputNotConsumed), 0, 0, 1, 1},
+    {&__pyx_n_s_InputOverrun, __pyx_k_InputOverrun, sizeof(__pyx_k_InputOverrun), 0, 0, 1, 1},
+    {&__pyx_n_s_LookbehindOverrun, __pyx_k_LookbehindOverrun, sizeof(__pyx_k_LookbehindOverrun), 0, 0, 1, 1},
+    {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
+    {&__pyx_n_s_OutputOverrun, __pyx_k_OutputOverrun, sizeof(__pyx_k_OutputOverrun), 0, 0, 1, 1},
+    {&__pyx_n_s_Success, __pyx_k_Success, sizeof(__pyx_k_Success), 0, 0, 1, 1},
+    {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+    {&__pyx_n_s__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 1, 1},
+    {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
+    {&__pyx_n_s_actual_out_size, __pyx_k_actual_out_size, sizeof(__pyx_k_actual_out_size), 0, 0, 1, 1},
+    {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
+    {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
+    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_code, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
+    {&__pyx_n_s_compress, __pyx_k_compress, sizeof(__pyx_k_compress), 0, 0, 1, 1},
+    {&__pyx_n_s_compress_worst_size, __pyx_k_compress_worst_size, sizeof(__pyx_k_compress_worst_size), 0, 0, 1, 1},
+    {&__pyx_n_s_curren_array_size, __pyx_k_curren_array_size, sizeof(__pyx_k_curren_array_size), 0, 0, 1, 1},
+    {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+    {&__pyx_n_s_data_bytes, __pyx_k_data_bytes, sizeof(__pyx_k_data_bytes), 0, 0, 1, 1},
+    {&__pyx_n_s_data_size, __pyx_k_data_size, sizeof(__pyx_k_data_size), 0, 0, 1, 1},
+    {&__pyx_n_s_decompress, __pyx_k_decompress, sizeof(__pyx_k_decompress), 0, 0, 1, 1},
+    {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+    {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
+    {&__pyx_kp_u_enum_class_EResult_not_importabl, __pyx_k_enum_class_EResult_not_importabl, sizeof(__pyx_k_enum_class_EResult_not_importabl), 0, 1, 0, 0},
+    {&__pyx_n_s_expected_out_size, __pyx_k_expected_out_size, sizeof(__pyx_k_expected_out_size), 0, 0, 1, 1},
+    {&__pyx_n_s_expected_output_size, __pyx_k_expected_output_size, sizeof(__pyx_k_expected_output_size), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_is_not_a_valid_EResult, __pyx_k_is_not_a_valid_EResult, sizeof(__pyx_k_is_not_a_valid_EResult), 0, 1, 0, 0},
+    {&__pyx_n_s_lzokay__lzokay, __pyx_k_lzokay__lzokay, sizeof(__pyx_k_lzokay__lzokay), 0, 0, 1, 1},
+    {&__pyx_kp_s_lzokay_pyx, __pyx_k_lzokay_pyx, sizeof(__pyx_k_lzokay_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_lzokay_wrap, __pyx_k_lzokay_wrap, sizeof(__pyx_k_lzokay_wrap), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
+    {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
+    {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
+    {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
+    {&__pyx_n_s_result_mapping, __pyx_k_result_mapping, sizeof(__pyx_k_result_mapping), 0, 0, 1, 1},
+    {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
+    {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
+    {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_tobytes, __pyx_k_tobytes, sizeof(__pyx_k_tobytes), 0, 0, 1, 1},
+    {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
+    {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 163, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 120, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "_lzokay.pyx":53
+  /* "lzokay/_lzokay.pyx":53
  * 
  *     cdef size_t actual_out_size = 0
  *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
  *     array.resize(b, curren_array_size)
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_u_B); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_u_B); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "_lzokay.pyx":41
+  /* "lzokay/_lzokay.pyx":41
  * 
  * 
  * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
  *     return s + s // 16 + 64 + 3
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_s); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 41, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress_worst_size, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_s); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(3, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress_worst_size, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(3, 41, __pyx_L1_error)
 
-  /* "_lzokay.pyx":45
+  /* "lzokay/_lzokay.pyx":45
  * 
  * 
  * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
  *     data_size = len(data)
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(8, __pyx_n_s_data, __pyx_n_s_expected_output_size, __pyx_n_s_data_size, __pyx_n_s_curren_array_size, __pyx_n_s_actual_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_data_bytes); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_decompress, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_tuple__7 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__6 = PyTuple_Pack(8, __pyx_n_s_data, __pyx_n_s_expected_output_size, __pyx_n_s_data_size, __pyx_n_s_curren_array_size, __pyx_n_s_actual_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_data_bytes); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_decompress, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(3, 45, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(3, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "_lzokay.pyx":74
+  /* "lzokay/_lzokay.pyx":74
  * 
  * 
  * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     cdef const uint8_t* data_bytes = data
  *     cdef size_t data_size = len(data)
  */
-  __pyx_tuple__8 = PyTuple_Pack(7, __pyx_n_s_data, __pyx_n_s_data_bytes, __pyx_n_s_data_size, __pyx_n_s_expected_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_actual_out_size); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(7, __pyx_n_s_data, __pyx_n_s_data_bytes, __pyx_n_s_data_size, __pyx_n_s_expected_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_actual_out_size); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(3, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(3, 74, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
-  #if CYTHON_USE_MODULE_STATE
-  if (__Pyx_InitString(__pyx_string_tab[0], &__pyx_n_u_B) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[1], &__pyx_n_s_Error) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[2], &__pyx_n_s_InputNotConsumed) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[3], &__pyx_n_s_InputOverrun) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[4], &__pyx_n_s_LookbehindOverrun) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[5], &__pyx_n_s_MemoryError) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[6], &__pyx_n_s_OutputOverrun) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[7], &__pyx_n_s__10) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[8], &__pyx_n_s__2) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[9], &__pyx_n_s_actual_out_size) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[10], &__pyx_n_s_array) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[11], &__pyx_n_s_asyncio_coroutines) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[12], &__pyx_n_s_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[13], &__pyx_n_s_bytes) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[14], &__pyx_n_s_class_getitem) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[15], &__pyx_n_s_cline_in_traceback) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[16], &__pyx_n_s_code) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[17], &__pyx_n_s_compress) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[18], &__pyx_n_s_compress_worst_size) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[19], &__pyx_n_s_curren_array_size) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[20], &__pyx_n_s_data) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[21], &__pyx_n_s_data_bytes) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[22], &__pyx_n_s_data_size) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[23], &__pyx_n_s_decompress) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[24], &__pyx_n_s_dict) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[25], &__pyx_n_s_doc) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[26], &__pyx_n_s_expected_out_size) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[27], &__pyx_n_s_expected_output_size) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[28], &__pyx_n_s_import) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[29], &__pyx_n_s_init_subclass) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[30], &__pyx_n_s_initializing) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[31], &__pyx_n_s_int) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[32], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[33], &__pyx_n_s_lzokay) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[34], &__pyx_kp_s_lzokay_pyx) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[35], &__pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[36], &__pyx_n_s_metaclass) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[37], &__pyx_n_s_module) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[38], &__pyx_n_s_mro_entries) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[39], &__pyx_n_s_name) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[40], &__pyx_n_s_prepare) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[41], &__pyx_n_s_qualname) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[42], &__pyx_n_s_result_mapping) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[43], &__pyx_n_s_return) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[44], &__pyx_n_s_s) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[45], &__pyx_n_s_set_name) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[46], &__pyx_n_s_spec) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[47], &__pyx_n_s_super) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[48], &__pyx_n_s_test) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[49], &__pyx_n_s_tobytes) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  #endif
-  #if !CYTHON_USE_MODULE_STATE
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  #endif
-  __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(3, 1, __pyx_L1_error);
+  __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(3, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
@@ -5031,44 +5613,37 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT(arrayobject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 69, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_0rc2(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0rc2(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_0rc2); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5244,14 +5819,17 @@
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__lzokay(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -5269,440 +5847,441 @@
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_lzokay", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #elif CYTHON_COMPILING_IN_LIMITED_API
-  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely(!__pyx_m)) __PYX_ERR(3, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    Py_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _lzokay pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(3, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely(!__pyx_m)) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__lzokay(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
-  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(3, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
   /*--- Initialize various global constants etc. ---*/
-  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   stringtab_initialized = 1;
-  if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitGlobals() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
-  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main__lzokay) {
-    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_module_is_main_lzokay___lzokay) {
+    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
-    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "_lzokay")) {
-      if (unlikely((PyDict_SetItemString(modules, "_lzokay", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(3, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "lzokay._lzokay")) {
+      if (unlikely((PyDict_SetItemString(modules, "lzokay._lzokay", __pyx_m) < 0))) __PYX_ERR(3, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(3, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-  if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_patch_abc() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
 
-  /* "_lzokay.pyx":2
+  /* "lzokay/_lzokay.pyx":2
  * from cpython cimport array
  * import array             # <<<<<<<<<<<<<<
  * from libc.stdint cimport uint8_t
  * 
  */
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_array, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_array, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_array, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_array, __pyx_t_2) < 0) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lzokay.pyx":12
+  /* "lzokay/_lzokay.pyx":12
  * 
  * 
  * class LookbehindOverrun(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_LookbehindOverrun, __pyx_n_s_LookbehindOverrun, (PyObject *) NULL, __pyx_n_s_lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_LookbehindOverrun, __pyx_n_s_LookbehindOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 12, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(3, 12, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_LookbehindOverrun, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_LookbehindOverrun, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LookbehindOverrun, __pyx_t_2) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LookbehindOverrun, __pyx_t_2) < 0) __PYX_ERR(3, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "_lzokay.pyx":16
+  /* "lzokay/_lzokay.pyx":16
  * 
  * 
  * class OutputOverrun(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_OutputOverrun, __pyx_n_s_OutputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_OutputOverrun, __pyx_n_s_OutputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__pyx_t_4 != __pyx_t_3) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 16, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(3, 16, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_OutputOverrun, __pyx_t_4, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_OutputOverrun, __pyx_t_4, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_OutputOverrun, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_OutputOverrun, __pyx_t_3) < 0) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_lzokay.pyx":20
+  /* "lzokay/_lzokay.pyx":20
  * 
  * 
  * class InputOverrun(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_5 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_5, __pyx_n_s_InputOverrun, __pyx_n_s_InputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_5, __pyx_n_s_InputOverrun, __pyx_n_s_InputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__pyx_t_5 != __pyx_t_4) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 20, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(3, 20, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_InputOverrun, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_InputOverrun, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputOverrun, __pyx_t_4) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputOverrun, __pyx_t_4) < 0) __PYX_ERR(3, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_lzokay.pyx":24
+  /* "lzokay/_lzokay.pyx":24
  * 
  * 
  * class Error(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_2, __pyx_n_s_Error, __pyx_n_s_Error, (PyObject *) NULL, __pyx_n_s_lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_2, __pyx_n_s_Error, __pyx_n_s_Error, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__pyx_t_2 != __pyx_t_5) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_4, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(0, 24, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_4, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(3, 24, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_Error, __pyx_t_2, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_Error, __pyx_t_2, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Error, __pyx_t_5) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Error, __pyx_t_5) < 0) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lzokay.pyx":28
+  /* "lzokay/_lzokay.pyx":28
  * 
  * 
  * class InputNotConsumed(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_InputNotConsumed, __pyx_n_s_InputNotConsumed, (PyObject *) NULL, __pyx_n_s_lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_InputNotConsumed, __pyx_n_s_InputNotConsumed, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(3, 28, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InputNotConsumed, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InputNotConsumed, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputNotConsumed, __pyx_t_2) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputNotConsumed, __pyx_t_2) < 0) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "_lzokay.pyx":33
+  /* "lzokay/_lzokay.pyx":33
  * 
  * result_mapping = {
  *     c_EResult.LookbehindOverrun: LookbehindOverrun,             # <<<<<<<<<<<<<<
  *     c_EResult.OutputOverrun: OutputOverrun,
  *     c_EResult.InputOverrun: InputOverrun,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::LookbehindOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Enum_EResult_to_py(lzokay::EResult::LookbehindOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LookbehindOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LookbehindOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_lzokay.pyx":34
+  /* "lzokay/_lzokay.pyx":34
  * result_mapping = {
  *     c_EResult.LookbehindOverrun: LookbehindOverrun,
  *     c_EResult.OutputOverrun: OutputOverrun,             # <<<<<<<<<<<<<<
  *     c_EResult.InputOverrun: InputOverrun,
  *     c_EResult.Error: Error,
  */
-  __pyx_t_5 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::OutputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Enum_EResult_to_py(lzokay::EResult::OutputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_OutputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_OutputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_lzokay.pyx":35
+  /* "lzokay/_lzokay.pyx":35
  *     c_EResult.LookbehindOverrun: LookbehindOverrun,
  *     c_EResult.OutputOverrun: OutputOverrun,
  *     c_EResult.InputOverrun: InputOverrun,             # <<<<<<<<<<<<<<
  *     c_EResult.Error: Error,
  *     c_EResult.InputNotConsumed: InputNotConsumed,
  */
-  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::InputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Enum_EResult_to_py(lzokay::EResult::InputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_lzokay.pyx":36
+  /* "lzokay/_lzokay.pyx":36
  *     c_EResult.OutputOverrun: OutputOverrun,
  *     c_EResult.InputOverrun: InputOverrun,
  *     c_EResult.Error: Error,             # <<<<<<<<<<<<<<
  *     c_EResult.InputNotConsumed: InputNotConsumed,
  * }
  */
-  __pyx_t_5 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::Error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Enum_EResult_to_py(lzokay::EResult::Error); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_lzokay.pyx":37
+  /* "lzokay/_lzokay.pyx":37
  *     c_EResult.InputOverrun: InputOverrun,
  *     c_EResult.Error: Error,
  *     c_EResult.InputNotConsumed: InputNotConsumed,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::InputNotConsumed); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Enum_EResult_to_py(lzokay::EResult::InputNotConsumed); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputNotConsumed); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputNotConsumed); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_result_mapping, __pyx_t_3) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_result_mapping, __pyx_t_3) < 0) __PYX_ERR(3, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "_lzokay.pyx":41
+  /* "lzokay/_lzokay.pyx":41
  * 
  * 
  * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
  *     return s + s // 16 + 64 + 3
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_s, __pyx_n_s_int) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7_lzokay_1compress_worst_size, 0, __pyx_n_s_compress_worst_size, NULL, __pyx_n_s_lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_s, __pyx_n_s_int) < 0) __PYX_ERR(3, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_1compress_worst_size, 0, __pyx_n_s_compress_worst_size, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress_worst_size, __pyx_t_5) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress_worst_size, __pyx_t_5) < 0) __PYX_ERR(3, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_lzokay.pyx":45
+  /* "lzokay/_lzokay.pyx":45
  * 
  * 
  * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
  *     data_size = len(data)
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_expected_output_size, __pyx_n_s_int) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7_lzokay_3decompress, 0, __pyx_n_s_decompress, NULL, __pyx_n_s_lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_expected_output_size, __pyx_n_s_int) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_3decompress, 0, __pyx_n_s_decompress, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__7);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__8);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decompress, __pyx_t_3) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decompress, __pyx_t_3) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "_lzokay.pyx":74
+  /* "lzokay/_lzokay.pyx":74
  * 
  * 
  * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     cdef const uint8_t* data_bytes = data
  *     cdef size_t data_size = len(data)
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7_lzokay_5compress, 0, __pyx_n_s_compress, NULL, __pyx_n_s_lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 74, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_5compress, 0, __pyx_n_s_compress, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress, __pyx_t_5) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress, __pyx_t_5) < 0) __PYX_ERR(3, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_lzokay.pyx":1
+  /* "lzokay/_lzokay.pyx":1
  * from cpython cimport array             # <<<<<<<<<<<<<<
  * import array
  * from libc.stdint cimport uint8_t
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_5) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "array.pxd":172
- *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
- * 
- * cdef inline void zero(array self):             # <<<<<<<<<<<<<<
- *     """ set all elements of array to zero. """
- *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
- */
-
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init _lzokay", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init lzokay._lzokay", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init _lzokay");
+    PyErr_SetString(PyExc_ImportError, "init lzokay._lzokay");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -5710,15 +6289,15 @@
   return;
   #endif
 }
 /* #### Code section: cleanup_globals ### */
 /* #### Code section: cleanup_module ### */
 /* #### Code section: main_method ### */
 /* #### Code section: utility_code_pragmas ### */
-#if _MSC_VER
+#ifdef _MSC_VER
 #pragma warning( push )
 /* Warning 4127: conditional expression is constant
  * Cython uses constant conditional expressions to allow in inline functions to be optimized at
  * compile-time, so this warning is not useful
  */
 #pragma warning( disable : 4127 )
 #endif
@@ -5741,216 +6320,1214 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
-    CYTHON_MAYBE_UNUSED_VAR(intval);
-    CYTHON_MAYBE_UNUSED_VAR(inplace);
-    CYTHON_UNUSED_VAR(zerodivision_check);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long x;
-        long a = PyInt_AS_LONG(op1);
-        
-            x = (long)((unsigned long)a + b);
-            if (likely((x^a) >= 0 || (x^b) >= 0))
-                return PyInt_FromLong(x);
-            return PyLong_Type.tp_as_number->nb_add(op1, op2);
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
     }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-#ifdef HAVE_LONG_LONG
-        const PY_LONG_LONG llb = intval;
-        PY_LONG_LONG lla, llx;
 #endif
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (unlikely(size == 0)) {
-            return __Pyx_NewRef(op2);
-        }
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
-        } else {
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
-            }
-        }
-                x = a + b;
-            return PyLong_FromLong(x);
-#ifdef HAVE_LONG_LONG
-        long_long:
-                llx = lla + llb;
-            return PyLong_FromLongLong(llx);
-#endif
-        
-        
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
     }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        double a = __pyx_PyFloat_AsDouble(op1);
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
 #else
-        double a = PyFloat_AS_DOUBLE(op1);
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
 #endif
-            double result;
-            
-            PyFPE_START_PROTECT("add", return NULL)
-            result = ((double)a) + (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
     }
-    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
 }
 #endif
 
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
     tstate->curexc_traceback = tb;
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+#endif
 }
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
     *type = tstate->curexc_type;
     *value = tstate->curexc_value;
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
+/* PyObjectGetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro))
+        return tp->tp_getattro(obj, attr_name);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_getattr))
+        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
+#endif
+    return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-    else state = (PyGILState_STATE)-1;
-#endif
-    CYTHON_UNUSED_VAR(clineno);
-    CYTHON_UNUSED_VAR(lineno);
-    CYTHON_UNUSED_VAR(filename);
-    CYTHON_MAYBE_UNUSED_VAR(nogil);
     __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
+    return result;
+}
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
+        PyErr_Format(PyExc_NameError,
+#if PY_MAJOR_VERSION >= 3
+            "name '%U' is not defined", name);
+#else
+            "name '%.200s' is not defined", PyString_AS_STRING(name));
+#endif
+    }
+    return result;
+}
+
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *module = 0;
+    PyObject *empty_dict = 0;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (unlikely(!py_import))
+        goto bad;
+    if (!from_list) {
+        empty_list = PyList_New(0);
+        if (unlikely(!empty_list))
+            goto bad;
+        from_list = empty_list;
+    }
+    #endif
+    empty_dict = PyDict_New();
+    if (unlikely(!empty_dict))
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
+                module = PyImport_ImportModuleLevelObject(
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (unlikely(!py_level))
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
+            #endif
+        }
+    }
+bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    return module;
+}
+
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        const char* module_name_str = 0;
+        PyObject* module_name = 0;
+        PyObject* module_dot = 0;
+        PyObject* full_name = 0;
+        PyErr_Clear();
+        module_name_str = PyModule_GetName(module);
+        if (unlikely(!module_name_str)) { goto modbad; }
+        module_name = PyUnicode_FromString(module_name_str);
+        if (unlikely(!module_name)) { goto modbad; }
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u_);
+        if (unlikely(!module_dot)) { goto modbad; }
+        full_name = PyUnicode_Concat(module_dot, name);
+        if (unlikely(!full_name)) { goto modbad; }
+        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+        {
+            PyObject *modules = PyImport_GetModuleDict();
+            if (unlikely(!modules))
+                goto modbad;
+            value = PyObject_GetItem(modules, full_name);
+        }
+        #else
+        value = PyImport_GetModule(full_name);
+        #endif
+      modbad:
+        Py_XDECREF(full_name);
+        Py_XDECREF(module_dot);
+        Py_XDECREF(module_name);
+    }
+    if (unlikely(!value)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
+    }
+    return value;
+}
+
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
     #else
-    ctx = PyUnicode_FromString(name);
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
     #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
     } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
     }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__2;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* PyFunctionFastCall */
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectCallMethO */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
+#endif
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
+    }
+#endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+}
+
+/* CIntToDigits */
+static const char DIGIT_PAIRS_10[2*10*10+1] = {
+    "00010203040506070809"
+    "10111213141516171819"
+    "20212223242526272829"
+    "30313233343536373839"
+    "40414243444546474849"
+    "50515253545556575859"
+    "60616263646566676869"
+    "70717273747576777879"
+    "80818283848586878889"
+    "90919293949596979899"
+};
+static const char DIGIT_PAIRS_8[2*8*8+1] = {
+    "0001020304050607"
+    "1011121314151617"
+    "2021222324252627"
+    "3031323334353637"
+    "4041424344454647"
+    "5051525354555657"
+    "6061626364656667"
+    "7071727374757677"
+};
+static const char DIGITS_HEX[2*16+1] = {
+    "0123456789abcdef"
+    "0123456789ABCDEF"
+};
+
+/* BuildPyUnicode */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char) {
+    PyObject *uval;
+    Py_ssize_t uoffset = ulength - clength;
+#if CYTHON_USE_UNICODE_INTERNALS
+    Py_ssize_t i;
+#if CYTHON_PEP393_ENABLED
+    void *udata;
+    uval = PyUnicode_New(ulength, 127);
+    if (unlikely(!uval)) return NULL;
+    udata = PyUnicode_DATA(uval);
+#else
+    Py_UNICODE *udata;
+    uval = PyUnicode_FromUnicode(NULL, ulength);
+    if (unlikely(!uval)) return NULL;
+    udata = PyUnicode_AS_UNICODE(uval);
+#endif
+    if (uoffset > 0) {
+        i = 0;
+        if (prepend_sign) {
+            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, 0, '-');
+            i++;
+        }
+        for (; i < uoffset; i++) {
+            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, i, padding_char);
+        }
+    }
+    for (i=0; i < clength; i++) {
+        __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, uoffset+i, chars[i]);
+    }
+#else
+    {
+        PyObject *sign = NULL, *padding = NULL;
+        uval = NULL;
+        if (uoffset > 0) {
+            prepend_sign = !!prepend_sign;
+            if (uoffset > prepend_sign) {
+                padding = PyUnicode_FromOrdinal(padding_char);
+                if (likely(padding) && uoffset > prepend_sign + 1) {
+                    PyObject *tmp;
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
+                    if (unlikely(!repeat)) goto done_or_error;
+                    tmp = PyNumber_Multiply(padding, repeat);
+                    Py_DECREF(repeat);
+                    Py_DECREF(padding);
+                    padding = tmp;
+                }
+                if (unlikely(!padding)) goto done_or_error;
+            }
+            if (prepend_sign) {
+                sign = PyUnicode_FromOrdinal('-');
+                if (unlikely(!sign)) goto done_or_error;
+            }
+        }
+        uval = PyUnicode_DecodeASCII(chars, clength, NULL);
+        if (likely(uval) && padding) {
+            PyObject *tmp = PyNumber_Add(padding, uval);
+            Py_DECREF(uval);
+            uval = tmp;
+        }
+        if (likely(uval) && sign) {
+            PyObject *tmp = PyNumber_Add(sign, uval);
+            Py_DECREF(uval);
+            uval = tmp;
+        }
+done_or_error:
+        Py_XDECREF(padding);
+        Py_XDECREF(sign);
+    }
+#endif
+    return uval;
+}
+
+/* CIntToPyUnicode */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char) {
+    char digits[sizeof(int)*3+2];
+    char *dpos, *end = digits + sizeof(int)*3+2;
+    const char *hex_digits = DIGITS_HEX;
+    Py_ssize_t length, ulength;
+    int prepend_sign, last_one_off;
+    int remaining;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (format_char == 'X') {
+        hex_digits += 16;
+        format_char = 'x';
+    }
+    remaining = value;
+    last_one_off = 0;
+    dpos = end;
+    do {
+        int digit_pos;
+        switch (format_char) {
+        case 'o':
+            digit_pos = abs((int)(remaining % (8*8)));
+            remaining = (int) (remaining / (8*8));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 8);
+            break;
+        case 'd':
+            digit_pos = abs((int)(remaining % (10*10)));
+            remaining = (int) (remaining / (10*10));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 10);
+            break;
+        case 'x':
+            *(--dpos) = hex_digits[abs((int)(remaining % 16))];
+            remaining = (int) (remaining / 16);
+            break;
+        default:
+            assert(0);
+            break;
+        }
+    } while (unlikely(remaining != 0));
+    assert(!last_one_off || *dpos == '0');
+    dpos += last_one_off;
+    length = end - dpos;
+    ulength = length;
+    prepend_sign = 0;
+    if (!is_unsigned && value <= neg_one) {
+        if (padding_char == ' ' || width <= length + 1) {
+            *(--dpos) = '-';
+            ++length;
+        } else {
+            prepend_sign = 1;
+        }
+        ++ulength;
+    }
+    if (width > ulength) {
+        ulength = width;
+    }
+    if (ulength == 1) {
+        return PyUnicode_FromOrdinal(*dpos);
+    }
+    return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
+}
+
+/* UnicodeConcatInPlace */
+# if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
+static int
+__Pyx_unicode_modifiable(PyObject *unicode)
+{
+    if (Py_REFCNT(unicode) != 1)
+        return 0;
+    if (!PyUnicode_CheckExact(unicode))
+        return 0;
+    if (PyUnicode_CHECK_INTERNED(unicode))
+        return 0;
+    return 1;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_ConcatInPlaceImpl(PyObject **p_left, PyObject *right
+        #if CYTHON_REFNANNY
+        , void* __pyx_refnanny
+        #endif
+    ) {
+    PyObject *left = *p_left;
+    Py_ssize_t left_len, right_len, new_len;
+    if (unlikely(__Pyx_PyUnicode_READY(left) == -1))
+        return NULL;
+    if (unlikely(__Pyx_PyUnicode_READY(right) == -1))
+        return NULL;
+    left_len = PyUnicode_GET_LENGTH(left);
+    if (left_len == 0) {
+        Py_INCREF(right);
+        return right;
+    }
+    right_len = PyUnicode_GET_LENGTH(right);
+    if (right_len == 0) {
+        Py_INCREF(left);
+        return left;
+    }
+    if (unlikely(left_len > PY_SSIZE_T_MAX - right_len)) {
+        PyErr_SetString(PyExc_OverflowError,
+                        "strings are too large to concat");
+        return NULL;
+    }
+    new_len = left_len + right_len;
+    if (__Pyx_unicode_modifiable(left)
+            && PyUnicode_CheckExact(right)
+            && PyUnicode_KIND(right) <= PyUnicode_KIND(left)
+            && !(PyUnicode_IS_ASCII(left) && !PyUnicode_IS_ASCII(right))) {
+        __Pyx_GIVEREF(*p_left);
+        if (unlikely(PyUnicode_Resize(p_left, new_len) != 0)) {
+            __Pyx_GOTREF(*p_left);
+            return NULL;
+        }
+        __Pyx_INCREF(*p_left);
+        _PyUnicode_FastCopyCharacters(*p_left, left_len, right, 0, right_len);
+        return *p_left;
+    } else {
+        return __Pyx_PyUnicode_Concat(left, right);
+    }
+  }
 #endif
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* TupleAndListFromArray */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
     PyObject *v;
     Py_ssize_t i;
     for (i = 0; i < length; i++) {
         v = dest[i] = src[i];
@@ -6150,14 +7727,147 @@
             return kwvalues[i];
         }
     }
     return NULL;  // not found (no exception set)
 }
 #endif
 
+/* PyIntBinop */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_MAYBE_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long x;
+        long a = PyInt_AS_LONG(op1);
+        
+            x = (long)((unsigned long)a + (unsigned long)b);
+            if (likely((x^a) >= 0 || (x^b) >= 0))
+                return PyInt_FromLong(x);
+            return PyLong_Type.tp_as_number->nb_add(op1, op2);
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        const long b = intval;
+        long a, x;
+#ifdef HAVE_LONG_LONG
+        const PY_LONG_LONG llb = intval;
+        PY_LONG_LONG lla, llx;
+#endif
+        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
+            return __Pyx_NewRef(op2);
+        }
+        if (likely(__Pyx_PyLong_IsCompact(op1))) {
+            a = __Pyx_PyLong_CompactValue(op1);
+        } else {
+            const digit* digits = __Pyx_PyLong_Digits(op1);
+            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
+            switch (size) {
+                case -2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
+            }
+        }
+                x = a + b;
+            return PyLong_FromLong(x);
+#ifdef HAVE_LONG_LONG
+        long_long:
+                llx = lla + llb;
+            return PyLong_FromLongLong(llx);
+#endif
+        
+        
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
+        double a = PyFloat_AS_DOUBLE(op1);
+#endif
+            double result;
+            
+            PyFPE_START_PROTECT("add", return NULL)
+            result = ((double)a) + (double)b;
+            PyFPE_END_PROTECT(result)
+            return PyFloat_FromDouble(result);
+    }
+    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
+}
+#endif
+
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
@@ -6333,109 +8043,14 @@
         "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
         ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* PyObjectGetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
-}
-#endif
-
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
-/* GetBuiltinName */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
-    if (unlikely(!result) && !PyErr_Occurred()) {
-        PyErr_Format(PyExc_NameError,
-#if PY_MAJOR_VERSION >= 3
-            "name '%U' is not defined", name);
-#else
-            "name '%.200s' is not defined", PyString_AS_STRING(name));
-#endif
-    }
-    return result;
-}
-
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -6592,238 +8207,18 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
-/* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-
-/* PyObjectCallMethO */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectFastCall */
-static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
-    PyObject *argstuple;
-    PyObject *result;
-    size_t i;
-    argstuple = PyTuple_New((Py_ssize_t)nargs);
-    if (unlikely(!argstuple)) return NULL;
-    for (i = 0; i < nargs; i++) {
-        Py_INCREF(args[i]);
-        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
-    }
-    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
-    Py_DECREF(argstuple);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
-    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (nargs == 0 && kwargs == NULL) {
-#ifdef __Pyx_CyFunction_USED
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
-    }
-    else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
-    }
-#endif
-    #if PY_VERSION_HEX < 0x030800B1
-    #if CYTHON_FAST_PYCCALL
-    if (PyCFunction_Check(func)) {
-        if (kwargs) {
-            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
-        } else {
-            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
-        }
-    }
-    #if PY_VERSION_HEX >= 0x030700A1
-    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
-        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
-    }
-    #endif
-    #endif
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
-    }
-    #endif
-    #endif
-    #if CYTHON_VECTORCALL
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
-    }
-    #endif
-    if (nargs == 0) {
-        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
-    }
-    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
-}
-
-/* PyObjectCallOneArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *args[2] = {NULL, arg};
-    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     key_value = __Pyx_PyIndex_AsSsize_t(index);
     if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
         return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
     }
     if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
         __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
@@ -6860,189 +8255,30 @@
     if (likely(sm && sm->sq_item)) {
         return __Pyx_PyObject_GetIndex(obj, key);
     }
     return __Pyx_PyObject_GetItem_Slow(obj, key);
 }
 #endif
 
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    CYTHON_UNUSED_VAR(cause);
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY ||  CYTHON_COMPILING_IN_LIMITED_API
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
                  expected, obj_type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0rc2
+#define __PYX_HAVE_RT_ImportType_3_0_0rc2
+static PyTypeObject *__Pyx_ImportType_3_0_0rc2(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0rc2 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -7088,226 +8324,36 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0rc2 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0rc2 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *module = 0;
-    PyObject *empty_dict = 0;
-    PyObject *empty_list = 0;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (unlikely(!py_import))
-        goto bad;
-    if (!from_list) {
-        empty_list = PyList_New(0);
-        if (unlikely(!empty_list))
-            goto bad;
-        from_list = empty_list;
-    }
-    #endif
-    empty_dict = PyDict_New();
-    if (unlikely(!empty_dict))
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                #if CYTHON_COMPILING_IN_LIMITED_API
-                module = PyImport_ImportModuleLevelObject(
-                    name, empty_dict, empty_dict, from_list, 1);
-                #else
-                module = PyImport_ImportModuleLevelObject(
-                    name, __pyx_d, empty_dict, from_list, 1);
-                #endif
-                if (unlikely(!module)) {
-                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (unlikely(!py_level))
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            #if CYTHON_COMPILING_IN_LIMITED_API
-            module = PyImport_ImportModuleLevelObject(
-                name, empty_dict, empty_dict, from_list, level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, __pyx_d, empty_dict, from_list, level);
-            #endif
-            #endif
-        }
-    }
-bad:
-    Py_XDECREF(empty_dict);
-    Py_XDECREF(empty_list);
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    return module;
-}
-
-/* ImportDottedModule */
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
-    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
-    if (unlikely(PyErr_Occurred())) {
-        PyErr_Clear();
-    }
-    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
-        partial_name = name;
-    } else {
-        slice = PySequence_GetSlice(parts_tuple, 0, count);
-        if (unlikely(!slice))
-            goto bad;
-        sep = PyUnicode_FromStringAndSize(".", 1);
-        if (unlikely(!sep))
-            goto bad;
-        partial_name = PyUnicode_Join(sep, slice);
-    }
-    PyErr_Format(
-#if PY_MAJOR_VERSION < 3
-        PyExc_ImportError,
-        "No module named '%s'", PyString_AS_STRING(partial_name));
-#else
-#if PY_VERSION_HEX >= 0x030600B1
-        PyExc_ModuleNotFoundError,
-#else
-        PyExc_ImportError,
-#endif
-        "No module named '%U'", partial_name);
-#endif
-bad:
-    Py_XDECREF(sep);
-    Py_XDECREF(slice);
-    Py_XDECREF(partial_name);
-    return NULL;
-}
-#endif
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
-    PyObject *imported_module;
-#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
-    PyObject *modules = PyImport_GetModuleDict();
-    if (unlikely(!modules))
-        return NULL;
-    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
-    Py_XINCREF(imported_module);
-#else
-    imported_module = PyImport_GetModule(name);
-#endif
-    return imported_module;
-}
-#endif
-static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
-#if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__2;
-    CYTHON_UNUSED_VAR(parts_tuple);
-    from_list = PyList_New(1);
-    if (unlikely(!from_list))
-        return NULL;
-    Py_INCREF(star);
-    PyList_SET_ITEM(from_list, 0, star);
-    module = __Pyx_Import(name, from_list, 0);
-    Py_DECREF(from_list);
-    return module;
-#else
-    Py_ssize_t i, nparts;
-    PyObject *imported_module;
-    PyObject *module = __Pyx_Import(name, NULL, 0);
-    if (!parts_tuple || unlikely(!module))
-        return module;
-    imported_module = __Pyx__ImportDottedModule_Lookup(name);
-    if (likely(imported_module)) {
-        Py_DECREF(module);
-        return imported_module;
-    }
-    PyErr_Clear();
-    nparts = PyTuple_GET_SIZE(parts_tuple);
-    for (i=1; i < nparts && module; i++) {
-        PyObject *part, *submodule;
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        part = PyTuple_GET_ITEM(parts_tuple, i);
-#else
-        part = PySequence_ITEM(parts_tuple, i);
-#endif
-        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
-#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-        Py_DECREF(part);
-#endif
-        Py_DECREF(module);
-        module = submodule;
-    }
-    if (likely(module))
-        return module;
-    return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
-#endif
-}
-static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
-    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
-    if (likely(module)) {
-        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
-        if (likely(spec)) {
-            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
-            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
-                Py_DECREF(spec);
-                spec = NULL;
-            }
-            Py_XDECREF(unsafe);
-        }
-        if (likely(!spec)) {
-            PyErr_Clear();
-            return module;
-        }
-        Py_DECREF(spec);
-        Py_DECREF(module);
-    } else if (PyErr_Occurred()) {
-        PyErr_Clear();
-    }
-#endif
-    return __Pyx__ImportDottedModule(name, parts_tuple);
-}
-
 /* Py3UpdateBases */
 static PyObject*
 __Pyx_PEP560_update_bases(PyObject *bases)
 {
     Py_ssize_t i, j, size_bases;
     PyObject *base, *meth, *new_base, *result, *new_bases = NULL;
     size_bases = PyTuple_GET_SIZE(bases);
@@ -7648,16 +8694,16 @@
     return result;
 }
 
 /* FixUpExtensionType */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
 #if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    (void) spec;
-    (void) type;
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
 #else
     const PyType_Slot *slot = spec->slots;
     while (slot && slot->slot && slot->slot != Py_tp_members)
         slot++;
     if (slot && slot->slot == Py_tp_members) {
         int changed = 0;
 #if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
@@ -7810,15 +8856,15 @@
               spec->basicsize) < 0) {
             goto bad;
         }
         goto done;
     }
     if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
     PyErr_Clear();
-    (void) module;
+    CYTHON_UNUSED_VAR(module);
     cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
     if (unlikely(!cached_type)) goto bad;
     if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
     if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
 done:
     Py_DECREF(abi_module);
     assert(cached_type == NULL || PyType_Check(cached_type));
@@ -8457,17 +9503,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -8699,27 +9750,30 @@
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #endif
 static int __pyx_CyFunction_init(PyObject *module) {
 #if CYTHON_USE_TYPE_SPECS
     __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
 #else
-    (void) module;
+    CYTHON_UNUSED_VAR(module);
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
 #endif
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
 }
@@ -8760,20 +9814,21 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
@@ -9023,52 +10078,14 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -9088,48 +10105,53 @@
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9143,108 +10165,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -9257,14 +10351,52 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
@@ -9284,48 +10416,53 @@
             return (size_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) >= 2 * PyLong_SHIFT)) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(size_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) >= 2 * PyLong_SHIFT)) {
+                                return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) >= 3 * PyLong_SHIFT)) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) >= 3 * PyLong_SHIFT)) {
+                                return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) >= 4 * PyLong_SHIFT)) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) >= 4 * PyLong_SHIFT)) {
+                                return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9339,108 +10476,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(size_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(size_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(size_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(size_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(size_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(size_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             size_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (size_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (size_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (size_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (size_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (size_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(size_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((size_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(size_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((size_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((size_t) 1) << (sizeof(size_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (size_t) -1;
         }
     } else {
         size_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (size_t) -1;
         val = __Pyx_PyInt_As_size_t(tmp);
@@ -9462,15 +10671,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__10));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__11));
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
@@ -9533,48 +10742,53 @@
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9588,108 +10802,180 @@
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
             if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
             } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -9877,15 +11163,14 @@
     if (!*str)
         return -1;
     if (PyObject_Hash(*str) == -1)
         return -1;
     return 0;
 }
 #endif
-#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION >= 3
         __Pyx_InitString(*t, t->p);
         #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
@@ -9899,15 +11184,14 @@
         if (PyObject_Hash(*t->p) == -1)
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
-#endif
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
@@ -10071,21 +11355,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -10146,15 +11428,15 @@
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
 /* #### Code section: utility_code_pragmas_end ### */
-#if _MSV_VER
+#ifdef _MSC_VER
 #pragma warning( pop )
 #endif
 
 
 
 /* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `lzokay-1.1.2/_lzokay.pyx` & `lzokay-1.1.3/_lzokay.pyx`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-from cpython cimport array
-import array
-from libc.stdint cimport uint8_t
-
-from lzokay_wrap cimport (
-    decompress as c_decompress,
-    compress as c_compress,
-    EResult as c_EResult,
-)
-
-
-class LookbehindOverrun(Exception):
-    pass
-
-
-class OutputOverrun(Exception):
-    pass
-
-
-class InputOverrun(Exception):
-    pass
-
-
-class Error(Exception):
-    pass
-
-
-class InputNotConsumed(Exception):
-    pass
-
-
-result_mapping = {
-    c_EResult.LookbehindOverrun: LookbehindOverrun,
-    c_EResult.OutputOverrun: OutputOverrun,
-    c_EResult.InputOverrun: InputOverrun,
-    c_EResult.Error: Error,
-    c_EResult.InputNotConsumed: InputNotConsumed,
-}
-
-
-cpdef int compress_worst_size(s: int):
-    return s + s // 16 + 64 + 3
-
-
-def decompress(data: bytes, expected_output_size: int = None) -> bytes:
-    data_size = len(data)
-
-    cdef size_t curren_array_size = data_size
-    if expected_output_size is not None:
-        curren_array_size = expected_output_size
-    
-    cdef size_t actual_out_size = 0    
-    cdef array.array b = array.array('B')
-    array.resize(b, curren_array_size)
-    
-    cdef c_EResult code = c_EResult.OutputOverrun
-    cdef const uint8_t* data_bytes = data
-    while code == c_EResult.OutputOverrun:
-        with nogil:
-            code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
-
-        if code == c_EResult.OutputOverrun:
-            curren_array_size *= 2
-            array.resize(b, curren_array_size)
-    
-    array.resize(b, actual_out_size)
-
-    if code in result_mapping:
-        raise result_mapping[code]()
-
-    return b.tobytes()
-
-    
-def compress(data: bytes) -> bytes:
-    cdef const uint8_t* data_bytes = data
-    cdef size_t data_size = len(data)
-    cdef size_t expected_out_size = compress_worst_size(data_size)
-
-    cdef array.array b = array.array('B')
-    array.resize(b, expected_out_size)
-    
-    # Results from c_compress
-    cdef c_EResult code
-    cdef size_t actual_out_size = 0
-
-    with nogil:
-        code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
-    
-    array.resize(b, actual_out_size)
-
-    if code in result_mapping:
-        raise result_mapping[code]()
-
-    return b.tobytes()
-
+from cpython cimport array
+import array
+from libc.stdint cimport uint8_t
+
+from lzokay_wrap cimport (
+    decompress as c_decompress,
+    compress as c_compress,
+    EResult as c_EResult,
+)
+
+
+class LookbehindOverrun(Exception):
+    pass
+
+
+class OutputOverrun(Exception):
+    pass
+
+
+class InputOverrun(Exception):
+    pass
+
+
+class Error(Exception):
+    pass
+
+
+class InputNotConsumed(Exception):
+    pass
+
+
+result_mapping = {
+    c_EResult.LookbehindOverrun: LookbehindOverrun,
+    c_EResult.OutputOverrun: OutputOverrun,
+    c_EResult.InputOverrun: InputOverrun,
+    c_EResult.Error: Error,
+    c_EResult.InputNotConsumed: InputNotConsumed,
+}
+
+
+cpdef int compress_worst_size(s: int):
+    return s + s // 16 + 64 + 3
+
+
+def decompress(data: bytes, expected_output_size: int = None) -> bytes:
+    data_size = len(data)
+
+    cdef size_t curren_array_size = data_size
+    if expected_output_size is not None:
+        curren_array_size = expected_output_size
+    
+    cdef size_t actual_out_size = 0    
+    cdef array.array b = array.array('B')
+    array.resize(b, curren_array_size)
+    
+    cdef c_EResult code = c_EResult.OutputOverrun
+    cdef const uint8_t* data_bytes = data
+    while code == c_EResult.OutputOverrun:
+        with nogil:
+            code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
+
+        if code == c_EResult.OutputOverrun:
+            curren_array_size *= 2
+            array.resize(b, curren_array_size)
+    
+    array.resize(b, actual_out_size)
+
+    if code in result_mapping:
+        raise result_mapping[code]()
+
+    return b.tobytes()
+
+    
+def compress(data: bytes) -> bytes:
+    cdef const uint8_t* data_bytes = data
+    cdef size_t data_size = len(data)
+    cdef size_t expected_out_size = compress_worst_size(data_size)
+
+    cdef array.array b = array.array('B')
+    array.resize(b, expected_out_size)
+    
+    # Results from c_compress
+    cdef c_EResult code
+    cdef size_t actual_out_size = 0
+
+    with nogil:
+        code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
+    
+    array.resize(b, actual_out_size)
+
+    if code in result_mapping:
+        raise result_mapping[code]()
+
+    return b.tobytes()
+
```

### Comparing `lzokay-1.1.2/lzokay.egg-info/PKG-INFO` & `lzokay-1.1.3/src/lzokay.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1
-Name: lzokay
-Version: 1.1.2
-Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
-Home-page: https://github.com/henriquegemignani/py-lzokay
-Author: Henrique Gemignani
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# py-lzokay
-Python bindings for LZ👌
+Metadata-Version: 2.1
+Name: lzokay
+Version: 1.1.3
+Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
+Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/henriquegemignani/py-lzokay
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# py-lzokay
+Python bindings for LZ👌
```

