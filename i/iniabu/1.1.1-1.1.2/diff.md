# Comparing `tmp/iniabu-1.1.1.tar.gz` & `tmp/iniabu-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iniabu-1.1.1.tar", last modified: Mon May  2 17:57:15 2022, max compression
+gzip compressed data, was "iniabu-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `iniabu-1.1.1.tar` & `iniabu-1.1.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0      135 2022-05-02 17:57:08.852711 iniabu-1.1.1/.bumpversion.cfg
--rw-r--r--   0        0        0       55 2022-05-02 17:57:08.852711 iniabu-1.1.1/.darglint
--rw-r--r--   0        0        0      316 2022-05-02 17:57:08.852711 iniabu-1.1.1/.flake8
--rw-r--r--   0        0        0     1235 2022-05-02 17:57:08.852711 iniabu-1.1.1/.github/workflows/package_testing.yml
--rw-r--r--   0        0        0      836 2022-05-02 17:57:08.852711 iniabu-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      560 2022-05-02 17:57:08.852711 iniabu-1.1.1/.gitignore
--rw-r--r--   0        0        0      388 2022-05-02 17:57:08.852711 iniabu-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3361 2022-05-02 17:57:08.852711 iniabu-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2137 2022-05-02 17:57:08.856711 iniabu-1.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    18092 2022-05-02 17:57:08.856711 iniabu-1.1.1/LICENSE
--rw-r--r--   0        0        0     4213 2022-05-02 17:57:08.856711 iniabu-1.1.1/README.rst
--rw-r--r--   0        0        0      176 2022-05-02 17:57:08.856711 iniabu-1.1.1/dev-requirements.txt
--rw-r--r--   0        0        0      211 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/api/elements.rst
--rw-r--r--   0        0        0      473 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/api/index.rst
--rw-r--r--   0        0        0      211 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/api/isotopes.rst
--rw-r--r--   0        0        0      257 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/api/main.rst
--rw-r--r--   0        0        0     1133 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/api/utilities.rst
--rw-r--r--   0        0        0     8753 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/background.rst
--rw-r--r--   0        0        0     1562 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/conf.py
--rw-r--r--   0        0        0     1138 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/config.rst
--rw-r--r--   0        0        0    12664 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/dev/index.rst
--rw-r--r--   0        0        0    42609 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/figures/int_norm.png
--rw-r--r--   0        0        0     2202 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/figures/int_norm.py
--rw-r--r--   0        0        0     3864 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/index.rst
--rw-r--r--   0        0        0    23244 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/intro.rst
--rw-r--r--   0        0        0    40536 2022-05-02 17:57:08.856711 iniabu-1.1.1/docs/jupyter_examples/astronomy_example.ipynb
--rw-r--r--   0        0        0   201882 2022-05-02 17:57:08.860711 iniabu-1.1.1/docs/jupyter_examples/cosmochemistry_example.ipynb
--rw-r--r--   0        0        0    49467 2022-05-02 17:57:08.860711 iniabu-1.1.1/docs/jupyter_examples/introduction.ipynb
--rw-r--r--   0        0        0       41 2022-05-02 17:57:08.860711 iniabu-1.1.1/docs/license.rst
--rw-r--r--   0        0        0      610 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/__init__.py
--rw-r--r--   0        0        0     1378 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/data/__init__.py
--rw-r--r--   0        0        0    30681 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/data/asplund09.py
--rw-r--r--   0        0        0    21701 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/data/lodders09.py
--rw-r--r--   0        0        0    35245 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/data/nist15.py
--rw-r--r--   0        0        0    85967 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/data/nist15_isomasses_all.py
--rw-r--r--   0        0        0     6047 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/elements.py
--rw-r--r--   0        0        0    12849 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/isotopes.py
--rw-r--r--   0        0        0    36829 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/main.py
--rw-r--r--   0        0        0    10974 2022-05-02 17:57:08.860711 iniabu-1.1.1/iniabu/utilities.py
--rw-r--r--   0        0        0     1916 2022-05-02 17:57:08.860711 iniabu-1.1.1/noxfile.py
--rw-r--r--   0        0        0     1473 2022-05-02 17:57:08.860711 iniabu-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        6 2022-05-02 17:57:08.860711 iniabu-1.1.1/requirements.txt
--rw-r--r--   0        0        0       36 2022-05-02 17:57:08.860711 iniabu-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      577 2022-05-02 17:57:08.860711 iniabu-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0       33 2022-05-02 17:57:08.860711 iniabu-1.1.1/tests/data/__init__.py
--rw-r--r--   0        0        0     2275 2022-05-02 17:57:08.860711 iniabu-1.1.1/tests/data/test_asplund09.py
--rw-r--r--   0        0        0     1965 2022-05-02 17:57:08.860711 iniabu-1.1.1/tests/data/test_lodders09.py
--rw-r--r--   0        0        0     3060 2022-05-02 17:57:08.860711 iniabu-1.1.1/tests/data/test_nist15.py
--rw-r--r--   0        0        0     7953 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_elements.py
--rw-r--r--   0        0        0      574 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_init.py
--rw-r--r--   0        0        0    11956 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_isotopes.py
--rw-r--r--   0        0        0     5328 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_main.py
--rw-r--r--   0        0        0     2988 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_main_bracket.py
--rw-r--r--   0        0        0     3865 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_main_delta.py
--rw-r--r--   0        0        0    10492 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_main_int_norm.py
--rw-r--r--   0        0        0    12057 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_main_ratios.py
--rw-r--r--   0        0        0     9870 2022-05-02 17:57:08.864712 iniabu-1.1.1/tests/test_utilities.py
--rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 iniabu-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      137 2023-07-13 10:24:36.751249 iniabu-1.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0       27 2023-07-13 10:24:36.751249 iniabu-1.1.2/.coveragerc
+-rw-r--r--   0        0        0       55 2023-07-13 10:24:36.751249 iniabu-1.1.2/.darglint
+-rw-r--r--   0        0        0      316 2023-07-13 10:24:36.751249 iniabu-1.1.2/.flake8
+-rw-r--r--   0        0        0     1594 2023-07-13 10:24:36.751249 iniabu-1.1.2/.github/workflows/package_testing.yml
+-rw-r--r--   0        0        0      837 2023-07-13 10:24:36.751249 iniabu-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      560 2023-07-13 10:24:36.751249 iniabu-1.1.2/.gitignore
+-rw-r--r--   0        0        0      387 2023-07-13 10:24:36.751249 iniabu-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      597 2023-07-13 10:24:36.751249 iniabu-1.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     3361 2023-07-13 10:24:36.751249 iniabu-1.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2137 2023-07-13 10:24:36.755249 iniabu-1.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    18092 2023-07-13 10:24:36.755249 iniabu-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4211 2023-07-13 10:24:36.755249 iniabu-1.1.2/README.rst
+-rw-r--r--   0        0        0      182 2023-07-13 10:24:36.755249 iniabu-1.1.2/dev-requirements.txt
+-rw-r--r--   0        0        0      211 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/api/elements.rst
+-rw-r--r--   0        0        0      473 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/api/index.rst
+-rw-r--r--   0        0        0      211 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/api/isotopes.rst
+-rw-r--r--   0        0        0      257 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/api/main.rst
+-rw-r--r--   0        0        0     1133 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/api/utilities.rst
+-rw-r--r--   0        0        0     8753 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/background.rst
+-rw-r--r--   0        0        0     1562 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/conf.py
+-rw-r--r--   0        0        0     1138 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/config.rst
+-rw-r--r--   0        0        0    12664 2023-07-13 10:24:36.755249 iniabu-1.1.2/docs/dev/index.rst
+-rw-r--r--   0        0        0    42609 2023-07-13 10:24:36.759249 iniabu-1.1.2/docs/figures/int_norm.png
+-rw-r--r--   0        0        0     2202 2023-07-13 10:24:36.759249 iniabu-1.1.2/docs/figures/int_norm.py
+-rw-r--r--   0        0        0     3862 2023-07-13 10:24:36.759249 iniabu-1.1.2/docs/index.rst
+-rw-r--r--   0        0        0    23245 2023-07-13 10:24:36.759249 iniabu-1.1.2/docs/intro.rst
+-rw-r--r--   0        0        0    40536 2023-07-13 10:24:36.759249 iniabu-1.1.2/docs/jupyter_examples/astronomy_example.ipynb
+-rw-r--r--   0        0        0   201882 2023-07-13 10:24:36.763249 iniabu-1.1.2/docs/jupyter_examples/cosmochemistry_example.ipynb
+-rw-r--r--   0        0        0    49467 2023-07-13 10:24:36.763249 iniabu-1.1.2/docs/jupyter_examples/introduction.ipynb
+-rw-r--r--   0        0        0       41 2023-07-13 10:24:36.763249 iniabu-1.1.2/docs/license.rst
+-rw-r--r--   0        0        0      610 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/__init__.py
+-rw-r--r--   0        0        0     1378 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/data/__init__.py
+-rw-r--r--   0        0        0    30681 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/data/asplund09.py
+-rw-r--r--   0        0        0    21701 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/data/lodders09.py
+-rw-r--r--   0        0        0    35245 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/data/nist15.py
+-rw-r--r--   0        0        0    85967 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/data/nist15_isomasses_all.py
+-rw-r--r--   0        0        0     6038 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/elements.py
+-rw-r--r--   0        0        0    12848 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/isotopes.py
+-rw-r--r--   0        0        0    36829 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/main.py
+-rw-r--r--   0        0        0    11002 2023-07-13 10:24:36.763249 iniabu-1.1.2/iniabu/utilities.py
+-rw-r--r--   0        0        0     1910 2023-07-13 10:24:36.763249 iniabu-1.1.2/noxfile.py
+-rw-r--r--   0        0        0     1439 2023-07-13 10:24:36.763249 iniabu-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-07-13 10:24:36.763249 iniabu-1.1.2/requirements.txt
+-rw-r--r--   0        0        0       36 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0       33 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/data/__init__.py
+-rw-r--r--   0        0        0     2275 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/data/test_asplund09.py
+-rw-r--r--   0        0        0     1965 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/data/test_lodders09.py
+-rw-r--r--   0        0        0     3060 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/data/test_nist15.py
+-rw-r--r--   0        0        0     7939 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_elements.py
+-rw-r--r--   0        0        0      574 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_init.py
+-rw-r--r--   0        0        0    11928 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_isotopes.py
+-rw-r--r--   0        0        0     5328 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_main.py
+-rw-r--r--   0        0        0     2988 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_main_bracket.py
+-rw-r--r--   0        0        0     3865 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_main_delta.py
+-rw-r--r--   0        0        0    10492 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_main_int_norm.py
+-rw-r--r--   0        0        0    12057 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_main_ratios.py
+-rw-r--r--   0        0        0     9870 2023-07-13 10:24:36.767249 iniabu-1.1.2/tests/test_utilities.py
+-rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 iniabu-1.1.2/PKG-INFO
```

### Comparing `iniabu-1.1.1/.github/workflows/python-publish.yml` & `iniabu-1.1.2/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: '3.6'
+        python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flit
     - name: Build and publish
       env:
         FLIT_USERNAME: '__token__'
```

### Comparing `iniabu-1.1.1/.gitignore` & `iniabu-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/CODE_OF_CONDUCT.md` & `iniabu-1.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/CONTRIBUTING.md` & `iniabu-1.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/LICENSE` & `iniabu-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/README.rst` & `iniabu-1.1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     :alt: Documentation Status
 .. image:: https://img.shields.io/pypi/v/iniabu?color=informational
     :target: https://pypi.org/project/iniabu/
     :alt: PyPi
 .. image:: https://github.com/galactic-forensics/iniabu/workflows/tests/badge.svg?branch=main
     :target: https://github.com/galactic-forensics/iniabu
     :alt: tests
-.. image:: https://coveralls.io/repos/github/galactic-forensics/iniabu/badge.svg?branch=main
-    :target: https://coveralls.io/github/galactic-forensics/iniabu?branch=main
-    :alt: coverage
+.. image:: https://codecov.io/gh/galactic-forensics/iniabu/branch/main/graph/badge.svg?token=P2SJEANE6S
+    :target: https://codecov.io/gh/galactic-forensics/iniabu
+    :alt: Code coverage
 .. image:: https://img.shields.io/badge/License-GPL%20v2-blue.svg
     :target: https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html
     :alt: License: GPL v2
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code style: black
```

### Comparing `iniabu-1.1.1/docs/api/utilities.rst` & `iniabu-1.1.2/docs/api/utilities.rst`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/background.rst` & `iniabu-1.1.2/docs/background.rst`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/conf.py` & `iniabu-1.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 sys.path.append("../")
 
 # -- Project information -----------------------------------------------------
 
 project = "iniabu"
 author = "Reto Trappitsch"
 copyright = f"2020-2022, {author}"
-version = "1.1.1"
+version = "1.1.2"
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `iniabu-1.1.1/docs/config.rst` & `iniabu-1.1.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/dev/index.rst` & `iniabu-1.1.2/docs/dev/index.rst`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/figures/int_norm.png` & `iniabu-1.1.2/docs/figures/int_norm.png`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/figures/int_norm.py` & `iniabu-1.1.2/docs/figures/int_norm.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/index.rst` & `iniabu-1.1.2/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     :alt: Documentation Status
 .. image:: https://img.shields.io/pypi/v/iniabu?color=informational
     :target: https://pypi.org/project/iniabu/
     :alt: PyPi
 .. image:: https://github.com/galactic-forensics/iniabu/workflows/tests/badge.svg?branch=main
     :target: https://github.com/galactic-forensics/iniabu
     :alt: tests
-.. image:: https://coveralls.io/repos/github/galactic-forensics/iniabu/badge.svg?branch=main
-    :target: https://coveralls.io/github/galactic-forensics/iniabu?branch=main
-    :alt: coverage
+.. image:: https://codecov.io/gh/galactic-forensics/iniabu/branch/main/graph/badge.svg?token=P2SJEANE6S
+    :target: https://codecov.io/gh/galactic-forensics/iniabu
+    :alt: Code coverage
 .. image:: https://img.shields.io/badge/License-GPL%20v2-blue.svg
     :target: https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html
     :alt: License: GPL v2
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code style: black
```

### Comparing `iniabu-1.1.1/docs/intro.rst` & `iniabu-1.1.2/docs/intro.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ======================
 
 
 Dependencies
 ------------
 
 This package is tested
-with python versions 3.6 - 3.9.
+with python versions 3.7 - 3.10.
 It might work on older python version as well,
 however,
 compatibility is not guaranteed.
 
 The only dependency at the moment
 for running the ``iniabu`` package
 is ``numpy``.
```

### Comparing `iniabu-1.1.1/docs/jupyter_examples/astronomy_example.ipynb` & `iniabu-1.1.2/docs/jupyter_examples/astronomy_example.ipynb`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/jupyter_examples/cosmochemistry_example.ipynb` & `iniabu-1.1.2/docs/jupyter_examples/cosmochemistry_example.ipynb`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/docs/jupyter_examples/introduction.ipynb` & `iniabu-1.1.2/docs/jupyter_examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/iniabu/__init__.py` & `iniabu-1.1.2/iniabu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .main import IniAbu
 
 ini = IniAbu()
 inimf = IniAbu(unit="mass_fraction")
 inilog = IniAbu(unit="num_log")
 
 # Package information
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 __title__ = "iniabu"
 __description__ = (
     "Read solar system abundances and automatically calculate various "
     "metrics, e.g., delta-values, dex, etc."
 )
```

### Comparing `iniabu-1.1.1/iniabu/data/__init__.py` & `iniabu-1.1.2/iniabu/data/__init__.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/iniabu/data/asplund09.py` & `iniabu-1.1.2/iniabu/data/asplund09.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/iniabu/data/lodders09.py` & `iniabu-1.1.2/iniabu/data/lodders09.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/iniabu/data/nist15.py` & `iniabu-1.1.2/iniabu/data/nist15.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/iniabu/data/nist15_isomasses_all.py` & `iniabu-1.1.2/iniabu/data/nist15_isomasses_all.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/iniabu/elements.py` & `iniabu-1.1.2/iniabu/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         is returned.
 
         :return: Atomic numbers of all isotopes
         :rtype: ndarray,list<ndarray>
         """
         ret_arr = []
         for ele in self._eles:
-            ret_arr.append(np.array(self._ele_dict[ele][1], dtype=np.int))
+            ret_arr.append(np.array(self._ele_dict[ele][1], dtype=int))
         return return_list_simplifier(ret_arr)
 
     @property
     def iso_abu_rel(self):
         """Get relative abundance of all isotopes.
 
         Returns a list with the relative abundances of all isotopes of the given
@@ -109,15 +109,15 @@
         "mass_fractions" as units, relative abundances will also be in mass fractions.
 
         :return: Relative abundance of all isotopes
         :rtype: ndarray,list<ndarray>
         """
         ret_arr = []
         for ele in self._eles:
-            ret_arr.append(np.array(self._ele_dict[ele][2], dtype=np.float))
+            ret_arr.append(np.array(self._ele_dict[ele][2], dtype=float))
         return return_list_simplifier(ret_arr)
 
     @property
     def iso_abu_solar(self):
         """Get solar abundances of all isotopes.
 
         Returns a list with the solar abundances of all isotopes of the given element.
@@ -126,15 +126,15 @@
         is not available, these values will be filled with ``np.nan``.
 
         :return: Relative abundance of all isotopes
         :rtype: ndarray,list<ndarray>
         """
         ret_arr = []
         for ele in self._eles:
-            ret_arr.append(np.array(self._ele_dict[ele][3], dtype=np.float))
+            ret_arr.append(np.array(self._ele_dict[ele][3], dtype=float))
         return return_list_simplifier(ret_arr)
 
     @property
     def mass(self):
         """Get the mass of an element.
 
         Returns the mass of an element depending on the specified composition. The mass
```

### Comparing `iniabu-1.1.1/iniabu/isotopes.py` & `iniabu-1.1.2/iniabu/isotopes.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 
         if all_av:
             isos = self._isos_all
         else:
             isos = self._isos
 
         for iso in isos:
-
             try:
                 ret_arr.append(self._iso_dict[iso][0])
             except KeyError:
                 ret_arr.append(0)  # isotope has no relative abundance - unstable
         ret_arr = np.array(ret_arr)
         return return_list_simplifier(ret_arr)
```

### Comparing `iniabu-1.1.1/iniabu/main.py` & `iniabu-1.1.2/iniabu/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,16 @@
         self._ele_dict_mf, self._iso_dict_mf = utilities.make_mf_dict(self._ele_dict)
 
         self._database = db
 
         # print message on what was loaded:
         if not self._is_initializing:
             print(
-                f"iniabu loaded database: '{self.database}', current units: "
-                f"'{self.unit}'"
+                f"iniabu loaded database: {self.database!r}, current units: "
+                f"{self.unit!r}"
             )
 
     @property
     def ele_dict(self):
         """Get the element dictionary.
 
         The dictionary keys are element symbols, e.g., "H". The entries for the element
```

### Comparing `iniabu-1.1.1/iniabu/utilities.py` & `iniabu-1.1.2/iniabu/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     iso_entries = []
     for key in element_dict.keys():
         for it, iso in enumerate(element_dict[key][1]):
             iso_keys.append(f"{key}-{iso}")
             rel_abu = element_dict[key][2][it]
             ss_abu = element_dict[key][3][it]
             iso_entries.append([rel_abu, ss_abu])
-    return dict(zip(iso_keys, iso_entries))
+    return dict(zip(iso_keys, iso_entries))  # noqa: B905
 
 
 def make_log_abu_dict(element_dict):
     """Make element and isotope dictionaries for logarithmic abundances.
 
     This routine takes an element dictionary with linear abundances, normed to Si
     equals 1e6, and returns new dictionaries with logarithmic abundances, normed to
@@ -229,15 +229,15 @@
             np.log10(rel_a * ss_abu_lin / abu_h) + 12.0 for rel_a in rel_abu
         ]
         tmp_entry.append(iso_ss_abu_log)
         # append to full list
         ele_entries.append(tmp_entry)
 
     # form new dictionary
-    element_dict_log = dict(zip(ele_keys, ele_entries))
+    element_dict_log = dict(zip(ele_keys, ele_entries))  # noqa: B905
 
     # isotope dictionary
     isotope_dict_log = make_iso_dict(element_dict_log)
 
     return element_dict_log, isotope_dict_log
```

### Comparing `iniabu-1.1.1/noxfile.py` & `iniabu-1.1.2/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import nox
 
 
 nox.options.sessions = "lint", "safety", "tests", "xdoctest"
 
 package = "iniabu"
 locations = "iniabu", "tests", "noxfile.py", "docs/conf.py"
-python_suite = ["3.10", "3.9", "3.8", "3.7", "3.6"]
-python_main = "3.10"
+python_suite = ["3.11", "3.10", "3.9", "3.8"]
+python_main = "3.11"
 
 
 @nox.session(python=python_main)
 def build(session):
     """Pack iniabu for release on PyPi."""
     session.install("flit")
     session.run("flit", "build")
```

### Comparing `iniabu-1.1.1/pyproject.toml` & `iniabu-1.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 
 [tool.flit.metadata]
 module = "iniabu"
 author = "Reto Trappitsch"
 author-email = "reto@galactic-forensics.space"
 home-page = "https://github.com/galactic-forensics/iniabu"
 requires = ["numpy"]
-requires-python=">=3.6"
+requires-python=">=3.8"
 description-file="README.rst"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
@@ -30,21 +29,22 @@
     "darglint>=1.5.1",
     "flake8",
     "flake8-bandit",
     "flake8-black",
     "flake8-bugbear",
     "flake8-docstrings",
     "flake8-import-order",
-    "bandit<=1.7.2",
+    "bandit"
 ]
 doc = [
     "sphinx",
     "sphinx_rtd_theme"
 ]
 test = [
+    "hypothesis",
     "pytest>=6.0",
     "pytest-cov",
     "pytest-mock",
     "pytest-sugar"
 ]
 
 [tool.flit.metadata.urls]
```

### Comparing `iniabu-1.1.1/tests/conftest.py` & `iniabu-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/data/test_asplund09.py` & `iniabu-1.1.2/tests/data/test_asplund09.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/data/test_lodders09.py` & `iniabu-1.1.2/tests/data/test_lodders09.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/data/test_nist15.py` & `iniabu-1.1.2/tests/data/test_nist15.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/test_elements.py` & `iniabu-1.1.2/tests/test_elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,20 +208,20 @@
     ele1=st.sampled_from(list(iniabu.data.lodders09_elements.keys())),
     ele2=st.sampled_from(list(iniabu.data.lodders09_elements.keys())),
 )
 def test_z(ini_default, ele1, ele2):
     """Get the number of protons for element."""
     z_ele = iniabu.data.elements_z[ele1]
     ret_val = ini_default.ele[ele1].z
-    assert isinstance(ret_val, np.int64)
+    assert ret_val.dtype == int
     assert ret_val == z_ele
 
     z_eles = np.array([z_ele, iniabu.data.elements_z[ele2]])
     ret_val = ini_default.ele[[ele1, ele2]].z
-    assert ret_val.dtype == np.int64
+    assert ret_val.dtype == int
     np.testing.assert_equal(ret_val, z_eles)
 
 
 def test_element_naming_case_sensitivity(ini_default):
     """Call element with any capitalization."""
     assert ini_default.ele["ti"].name == "Ti"
     assert ini_default.ele["tI"].name == "Ti"
```

### Comparing `iniabu-1.1.1/tests/test_init.py` & `iniabu-1.1.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/test_isotopes.py` & `iniabu-1.1.2/tests/test_isotopes.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 @given(
     iso1=st.sampled_from(list(iniabu.data.lodders09_isotopes.keys())),
     iso2=st.sampled_from(list(iniabu.data.lodders09_isotopes.keys())),
 )
 def test_a(ini_default, iso1, iso2):
     """Return mass number of isotope (what is actually put in already)."""
     ret_val = ini_default.iso[iso1].a
-    assert isinstance(ret_val, np.int64)
+    assert ret_val.dtype == int
     assert ret_val == int(iso1.split("-")[1])
 
     ret_val = ini_default.iso[[iso1, iso2]].a
-    assert ret_val.dtype == np.int64
+    assert ret_val.dtype == int
     np.testing.assert_equal(
         ret_val,
         np.array([int(iso1.split("-")[1]), int(iso2.split("-")[1])]),
     )
 
 
 def test_a_all(ini_default):
@@ -242,21 +242,21 @@
     iso1=st.sampled_from(list(iniabu.data.lodders09_isotopes.keys())),
     iso2=st.sampled_from(list(iniabu.data.lodders09_isotopes.keys())),
 )
 def test_z(ini_default, iso1, iso2):
     """Get the number of protons for element."""
     z_ele = iniabu.data.elements_z[iso1.split("-")[0]]
     ret_val = ini_default.iso[iso1].z
-    assert isinstance(ret_val, np.int64)
+    assert ret_val.dtype == int
     assert ret_val == z_ele
 
     # list
     z_eles = np.array([z_ele, iniabu.data.elements_z[iso2.split("-")[0]]])
     ret_val = ini_default.iso[[iso1, iso2]].z
-    assert ret_val.dtype == np.int64
+    assert ret_val.dtype == int
     np.testing.assert_equal(ret_val, z_eles)
 
 
 def test_z_all(ini_default):
     """Ensure that we get more back when calling for z of all isotopes of element."""
     ele = "H"
     default_list = ini_default.iso[ele].z
```

### Comparing `iniabu-1.1.1/tests/test_main.py` & `iniabu-1.1.2/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     # change unit
     ini.unit = unit
     # now load the nist database for example
     db_new = "nist"
     ini.database = db_new
 
     spy_print.assert_called_with(
-        f"iniabu loaded database: '{db_new}', current " f"units: '{unit}'"
+        f"iniabu loaded database: {db_new!r}, current " f"units: {unit!r}"
     )
 
 
 # TEST THE DICTIONARIES #
 
 
 def test_ele_dict(ini_default):
```

### Comparing `iniabu-1.1.1/tests/test_main_bracket.py` & `iniabu-1.1.2/tests/test_main_bracket.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/test_main_delta.py` & `iniabu-1.1.2/tests/test_main_delta.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/test_main_int_norm.py` & `iniabu-1.1.2/tests/test_main_int_norm.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/test_main_ratios.py` & `iniabu-1.1.2/tests/test_main_ratios.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/tests/test_utilities.py` & `iniabu-1.1.2/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `iniabu-1.1.1/PKG-INFO` & `iniabu-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: iniabu
-Version: 1.1.1
+Version: 1.1.2
 Summary: Solar System initial abundance package.
 Home-page: https://github.com/galactic-forensics/iniabu
 Author: Reto Trappitsch
 Author-email: reto@galactic-forensics.space
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: numpy
 Requires-Dist: darglint>=1.5.1 ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flake8-bandit ; extra == "dev"
 Requires-Dist: flake8-black ; extra == "dev"
 Requires-Dist: flake8-bugbear ; extra == "dev"
 Requires-Dist: flake8-docstrings ; extra == "dev"
 Requires-Dist: flake8-import-order ; extra == "dev"
-Requires-Dist: bandit<=1.7.2 ; extra == "dev"
+Requires-Dist: bandit ; extra == "dev"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
+Requires-Dist: hypothesis ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: pytest-sugar ; extra == "test"
 Project-URL: Documentation, https://iniabu.readthedocs.io
 Provides-Extra: dev
 Provides-Extra: doc
@@ -47,17 +47,17 @@
     :alt: Documentation Status
 .. image:: https://img.shields.io/pypi/v/iniabu?color=informational
     :target: https://pypi.org/project/iniabu/
     :alt: PyPi
 .. image:: https://github.com/galactic-forensics/iniabu/workflows/tests/badge.svg?branch=main
     :target: https://github.com/galactic-forensics/iniabu
     :alt: tests
-.. image:: https://coveralls.io/repos/github/galactic-forensics/iniabu/badge.svg?branch=main
-    :target: https://coveralls.io/github/galactic-forensics/iniabu?branch=main
-    :alt: coverage
+.. image:: https://codecov.io/gh/galactic-forensics/iniabu/branch/main/graph/badge.svg?token=P2SJEANE6S
+    :target: https://codecov.io/gh/galactic-forensics/iniabu
+    :alt: Code coverage
 .. image:: https://img.shields.io/badge/License-GPL%20v2-blue.svg
     :target: https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html
     :alt: License: GPL v2
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code style: black
```

