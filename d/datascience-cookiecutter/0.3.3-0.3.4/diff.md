# Comparing `tmp/datascience_cookiecutter-0.3.3.tar.gz` & `tmp/datascience_cookiecutter-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.3.3.tar", last modified: Sun Jul  2 18:39:48 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.3.4.tar", last modified: Thu Jul 13 10:22:53 2023, max compression
```

## Comparing `datascience_cookiecutter-0.3.3.tar` & `datascience_cookiecutter-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6837 2023-07-02 18:37:06.563119 datascience_cookiecutter-0.3.3/README.md
--rw-r--r--   0        0        0      314 2023-07-02 18:38:44.163783 datascience_cookiecutter-0.3.3/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3.3/datascience_cookiecutter/__main__.py
--rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3.3/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3703 2023-07-02 18:08:35.811440 datascience_cookiecutter-0.3.3/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0     1113 2023-07-02 18:39:48.823866 datascience_cookiecutter-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3.3/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     7722 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     6833 2023-07-13 10:22:38.605690 datascience_cookiecutter-0.3.4/README.md
+-rw-r--r--   0        0        0      314 2023-07-13 10:22:38.628656 datascience_cookiecutter-0.3.4/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3.4/datascience_cookiecutter/__main__.py
+-rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3.4/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3701 2023-07-13 10:22:38.622411 datascience_cookiecutter-0.3.4/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0     1115 2023-07-13 10:22:53.332077 datascience_cookiecutter-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3.4/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     7720 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3.4/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.3.3/README.md` & `datascience_cookiecutter-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 - Customizable for multiple programming languages (currently, the default template currently only has Python)
 - Easy project initialization with just a few command-line arguments
 
 ## ⚙️ Installation
 The Data Science Cookiecutter is on [pypi](https://pypi.org/project/datascience-cookiecutter/) and can be installed using `pip`, `poetry`, `pdm` or `conda`.
 
 ```bash
-pdm install datascience-cookiecutter
+pdm add datascience-cookiecutter
 ```
 
 # 🚀 Basic Usage
 To create a new data science project using the Data Science Cookiecutter, follow these steps:
 
 1. Open a terminal or command prompt.
 2. `cd` to the directory where you want to create the project.
```

### Comparing `datascience_cookiecutter-0.3.3/datascience_cookiecutter/__main__.py` & `datascience_cookiecutter-0.3.4/datascience_cookiecutter/__main__.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.3/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.3.4/datascience_cookiecutter/folderbuilder.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.3/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.3.4/datascience_cookiecutter/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 install:
 \tpdm install
 
 test:
 \tpdm run pytest
 
 lint:
-\tpdm run flake8 {{name}}
+\tpdm run ruff {{name}}
 \tpdm run mypy {{name}}
 
 format:
 \tpdm run isort -v {{name}}
 \tpdm run black {{name}}
 """
 
@@ -93,23 +93,23 @@
 version = "0.1.0"
 description = ""
 authors = [
 \t{name = "", email = ""},
 ]
 dependencies = [
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 readme = "README.md"
 license = {text = "MIT"}
 
 [project.optional-dependencies]
 lint = [
-\t"ruff>=0.0.275",
-\t"black>=23.3.0",
-\t"isort>=5.11.5",
+\t"ruff>=0.0.278",
+\t"black>=23.7.0",
+\t"isort>=5.12.0",
 \t"mypy>=1.4.1",
 ]
 
 [build-system]
 requires = ["pdm-backend"]
 build-backend = "pdm.backend"
 """
```

### Comparing `datascience_cookiecutter-0.3.3/pyproject.toml` & `datascience_cookiecutter-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "datascience_cookiecutter"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
-    "pydantic>=2.0",
+    "pydantic>=2.0.2",
     "loguru>=0.7.0",
-    "click>=8.1.3",
+    "click>=8.1.4",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,17 +25,17 @@
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 lint = [
     "pytest>=7.4.0",
-    "ruff>=0.0.275",
-    "black>=23.3.0",
-    "isort>=5.11.5",
+    "ruff>=0.0.278",
+    "black>=23.7.0",
+    "isort>=5.12.0",
     "mypy>=1.4.1",
 ]
 
 [project.scripts]
 cookiecutter = "datascience_cookiecutter.__main__:create_project"
 
 [project.urls]
```

### Comparing `datascience_cookiecutter-0.3.3/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.3.4/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.3/PKG-INFO` & `datascience_cookiecutter-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: datascience_cookiecutter
-Version: 0.3.3
+Version: 0.3.4
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Project-URL: Github, https://github.com/raoulg/datascience-cookiecutter
-Requires-Python: >=3.7
-Requires-Dist: pydantic>=2.0
+Requires-Python: >=3.9
+Requires-Dist: pydantic>=2.0.2
 Requires-Dist: loguru>=0.7.0
-Requires-Dist: click>=8.1.3
+Requires-Dist: click>=8.1.4
 Requires-Dist: pytest>=7.4.0; extra == "lint"
-Requires-Dist: ruff>=0.0.275; extra == "lint"
-Requires-Dist: black>=23.3.0; extra == "lint"
-Requires-Dist: isort>=5.11.5; extra == "lint"
+Requires-Dist: ruff>=0.0.278; extra == "lint"
+Requires-Dist: black>=23.7.0; extra == "lint"
+Requires-Dist: isort>=5.12.0; extra == "lint"
 Requires-Dist: mypy>=1.4.1; extra == "lint"
 Provides-Extra: lint
 Description-Content-Type: text/markdown
 
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -54,15 +54,15 @@
 - Customizable for multiple programming languages (currently, the default template currently only has Python)
 - Easy project initialization with just a few command-line arguments
 
 ## ⚙️ Installation
 The Data Science Cookiecutter is on [pypi](https://pypi.org/project/datascience-cookiecutter/) and can be installed using `pip`, `poetry`, `pdm` or `conda`.
 
 ```bash
-pdm install datascience-cookiecutter
+pdm add datascience-cookiecutter
 ```
 
 # 🚀 Basic Usage
 To create a new data science project using the Data Science Cookiecutter, follow these steps:
 
 1. Open a terminal or command prompt.
 2. `cd` to the directory where you want to create the project.
```

