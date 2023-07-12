# Comparing `tmp/scope_py-0.1.0.tar.gz` & `tmp/scope_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scope_py-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "scope_py-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scope_py-0.1.0.tar` & `scope_py-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,31 @@
--rw-r--r--   0        0        0      331 2023-07-10 23:42:23.800061 scope_py-0.1.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2023-07-10 22:45:54.383697 scope_py-0.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      463 2023-07-10 23:59:43.270510 scope_py-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      468 2023-07-11 16:47:40.630107 scope_py-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-07-11 00:04:06.640954 scope_py-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      674 2023-07-11 16:47:33.318798 scope_py-0.1.0/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2023-07-10 22:45:54.384373 scope_py-0.1.0/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      372 2023-07-11 16:51:19.075525 scope_py-0.1.0/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0     1799 2023-07-10 22:45:54.384647 scope_py-0.1.0/.gitignore
--rw-r--r--   0        0        0     1540 2023-07-11 00:07:22.831682 scope_py-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-07-10 22:45:54.384818 scope_py-0.1.0/.pypirc
--rw-r--r--   0        0        0      459 2023-07-10 22:45:54.384943 scope_py-0.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      815 2023-07-10 23:16:45.587799 scope_py-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      444 2023-07-10 22:45:54.385111 scope_py-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-07-10 22:45:54.385201 scope_py-0.1.0/LICENSE
--rw-r--r--   0        0        0     3235 2023-07-11 06:05:10.298814 scope_py-0.1.0/README.md
--rw-r--r--   0        0        0     2780 2023-07-10 22:45:54.385504 scope_py-0.1.0/SECURITY.md
--rw-r--r--   0        0        0     1308 2023-07-10 22:45:54.385605 scope_py-0.1.0/SUPPORT.md
--rw-r--r--   0        0        0      634 2023-07-10 22:45:54.385738 scope_py-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     2321 2023-07-10 22:45:54.385838 scope_py-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      360 2023-07-10 22:45:54.385916 scope_py-0.1.0/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2023-07-10 22:45:54.385998 scope_py-0.1.0/docs/developer.md
--rw-r--r--   0        0        0      468 2023-07-10 22:45:54.386107 scope_py-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-07-10 22:45:54.386201 scope_py-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       48 2023-07-10 23:42:27.768049 scope_py-0.1.0/docs/modules.rst
--rw-r--r--   0        0        0      471 2023-07-10 22:45:54.386384 scope_py-0.1.0/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-07-10 22:45:54.386558 scope_py-0.1.0/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-07-10 22:45:54.386642 scope_py-0.1.0/docs/pyproject.md
--rw-r--r--   0        0        0       42 2023-07-10 22:45:54.386915 scope_py-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0      378 2023-07-11 00:04:53.617323 scope_py-0.1.0/docs/scope.rst
--rw-r--r--   0        0        0       44 2023-07-10 22:45:54.387005 scope_py-0.1.0/docs/vscode.md
--rw-r--r--   0        0        0      208 2023-07-10 22:45:54.387100 scope_py-0.1.0/docs/workflows.md
--rw-r--r--   0        0        0     6655 2023-07-11 16:53:28.144634 scope_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-07-10 22:45:54.387356 scope_py-0.1.0/src/README.md
--rw-r--r--   0        0        0    10283 2023-07-11 00:21:19.202364 scope_py-0.1.0/src/scope/__init__.py
--rw-r--r--   0        0        0      989 2023-07-10 22:45:54.387743 scope_py-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1172 2023-07-11 00:07:08.026045 scope_py-0.1.0/tests/test_methods.py
--rw-r--r--   0        0        0     5087 1970-01-01 00:00:00.000000 scope_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-07-10 23:42:23.800061 scope_py-0.1.1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2023-07-10 22:45:54.383697 scope_py-0.1.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      463 2023-07-10 23:59:43.270510 scope_py-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1371 2023-07-11 17:29:49.172918 scope_py-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      318 2023-07-10 22:45:54.384373 scope_py-0.1.1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1799 2023-07-10 22:45:54.384647 scope_py-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-07-11 00:07:22.831682 scope_py-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-07-10 22:45:54.384818 scope_py-0.1.1/.pypirc
+-rw-r--r--   0        0        0      459 2023-07-10 22:45:54.384943 scope_py-0.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0      815 2023-07-10 23:16:45.587799 scope_py-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1133 2023-07-11 17:52:53.733232 scope_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3677 2023-07-11 17:51:40.203177 scope_py-0.1.1/README.md
+-rw-r--r--   0        0        0      634 2023-07-10 22:45:54.385738 scope_py-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2023-07-10 22:45:54.385838 scope_py-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      360 2023-07-10 22:45:54.385916 scope_py-0.1.1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2023-07-10 22:45:54.385998 scope_py-0.1.1/docs/developer.md
+-rw-r--r--   0        0        0      468 2023-07-10 22:45:54.386107 scope_py-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-07-10 22:45:54.386201 scope_py-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       48 2023-07-10 23:42:27.768049 scope_py-0.1.1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2023-07-10 22:45:54.386384 scope_py-0.1.1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-07-10 22:45:54.386558 scope_py-0.1.1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-07-10 22:45:54.386642 scope_py-0.1.1/docs/pyproject.md
+-rw-r--r--   0        0        0       42 2023-07-10 22:45:54.386915 scope_py-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0      378 2023-07-11 00:04:53.617323 scope_py-0.1.1/docs/scope.rst
+-rw-r--r--   0        0        0       44 2023-07-10 22:45:54.387005 scope_py-0.1.1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2023-07-10 22:45:54.387100 scope_py-0.1.1/docs/workflows.md
+-rw-r--r--   0        0        0     6655 2023-07-11 16:53:28.144634 scope_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10283 2023-07-12 22:03:57.372601 scope_py-0.1.1/src/scope/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-10 22:45:54.387743 scope_py-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1172 2023-07-11 00:07:08.026045 scope_py-0.1.1/tests/test_methods.py
+-rw-r--r--   0        0        0     5529 1970-01-01 00:00:00.000000 scope_py-0.1.1/PKG-INFO
```

### Comparing `scope_py-0.1.0/.devcontainer/devcontainer.json` & `scope_py-0.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/.gitignore` & `scope_py-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/.pre-commit-config.yaml` & `scope_py-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/.vscode/settings.json` & `scope_py-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/LICENSE` & `scope_py-0.1.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
     MIT License
 
-    Copyright (c) Microsoft Corporation.
+    Copyright (c) Forest Hughes.
 
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
```

### Comparing `scope_py-0.1.0/README.md` & `scope_py-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Scope
 
 Scope is a Python library inspired by _optics_ from functional programming. The aim of Scope is to make various flavors of _optics_ natural tools for Python programmers without requiring knowledge of the underlying math. Put simply, _optics_ provide an abstraction for focusing on ("getting") and manipulating ("setting") data within larger and potentially nested structures.
 
 This library favors usability over rigor and makes some decisions which increase utility at the expense of overloading and extending established terminology. For example, _traversals_ in the standard usage, provide a means of focusing on multiple parts of a datastructure but do not provide similar setting behavior, whereas instances of the `scope.Traversal` class do provide a way to set multiple parts of a larger datastructure.
 
+## Install
+
+Install by running `pip install scope-py` or by cloning this repo and running `pip install .` in the project root directory.
+
 ## Introduction
 
 The Scope library targets manipulation of JSON-like nested structures, which in Python are built from dictionaries, and lists, but custom _optics_ are definable. Scope has a few classes you should be aware of;
 
 - `Lens`: Base class providing get and put methods. Can be composed with other lenses.
 - `ParallelLens`: Allows multiple lenses to be used in parallel.
 - `Traversal`: Provides functionality for working with sequences of data.
@@ -16,15 +20,15 @@
 - `ParallelCRUDLens`: Allows multiple CRUD lenses to be used in parallel.
 - `CRUDTraversal`: Extension of the CRUDLens for working with sequences of data.
 
 Importantly, a `Lens` focuses on one thing and a `Traversals` focuses on many things. A `CRUDLens` extends the get/put functionality of lenses with additional create/delete functionality.
 
 ## Usage
 
-### Basic lens composition example:
+### Basic lens composition:
 
 ```python
 import scope
 
 # create a lens that focuses on item 'b' after item 'a'
 lens = scope.id['a']['b']
 # lens = scope.compose_lenses(scope.id['a'], scope.id['b']) <-- alt. syntax
@@ -32,47 +36,55 @@
 data = {'a': {'b': 3}}
 
 # note -- lens(data) is an alias for lens.get(data)
 assert lens(data) == 3
 assert lens.put(4)(data) == {'a': {'b': 4}}
 ```
 
-### CRUDTraversal example:
+### CRUDTraversal usage:
 
 ```python
 lens = CRUDTraversal(ItemCRUDLens('a'), ItemCRUDLens('c'))
 # lens = ItemCRUDLens('a')[::]['c'] <-- alt. syntax
 
 data = {'a': [{'b': 1}, {'b': 3}]}
 
 # "{'a': [{'b': 1, 'c': 2}, {'b': 3, 'c': 4}]}"
 print(lens.create([2, 4])(data))
 ```
 
-### Custom attribute lens example:
+### Create a custom attribute lens:
 
 ```python
 # create a lens that gets/sets the attribute "my_attr" on an object
-my_attr_lens = scope.Lens(lambda data: getattr(data, 'my_attr'), lambda value: lambda data: setattr(data, 'my_attr', value))
+my_attr_lens = scope.Lens(lambda data: getattr(data, 'my_attr'),
+                          lambda value: lambda data: setattr(data, 'my_attr', value))
 ```
 
-### Parallel lens example:
+### Parallel lens usage:
 
 ```python
 x_lens, y_lens = scope.id['x'], scope.id['y']
 
 # create a lens which focuses on 'x' and 'y' in parallel
 parallel_lens = x_lens | y_lens
 # parallel_lens = scope.ParallelLens(x_lens, y_lens) <-- alt. syntax
 
 data = {'x': 2, 'y': 3}
 
 assert sum(parallel_lens(data)) == 5
 ```
 
+## Todo‘s
+
+- [] Clean up unused files leftover from cloned template repo
+- [] Tests to achieve 100% code coverage
+- [] Add a `filter` method to all classes which accepts a predicate function and applies it to the focus
+- [] Add tests passing and code coverage badges using Github Pages
+
 ## License
 
 This project is open-sourced under the MIT license. See [LICENSE](https://github.com/fchughes/scope/blob/main/LICENSE) for more information.
 
 ## Contact
 
 For questions or issues, please open an issue on GitHub.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scope_py-0.1.0/docs/Makefile` & `scope_py-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/docs/conf.py` & `scope_py-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/docs/make.bat` & `scope_py-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/docs/pylint.md` & `scope_py-0.1.1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/pyproject.toml` & `scope_py-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/src/scope/__init__.py` & `scope_py-0.1.1/src/scope/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 from contextlib import suppress as _suppress
 
 
 class Lens:
     def __init__(self, get, put):
         self.get = get
         self.put = put
```

### Comparing `scope_py-0.1.0/tests/conftest.py` & `scope_py-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/tests/test_methods.py` & `scope_py-0.1.1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `scope_py-0.1.0/PKG-INFO` & `scope_py-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scope-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lens library which targets usability over rigor.
 Author-email: Forest Hughes <forestchughes@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,14 +40,18 @@
 
 # Scope
 
 Scope is a Python library inspired by _optics_ from functional programming. The aim of Scope is to make various flavors of _optics_ natural tools for Python programmers without requiring knowledge of the underlying math. Put simply, _optics_ provide an abstraction for focusing on ("getting") and manipulating ("setting") data within larger and potentially nested structures.
 
 This library favors usability over rigor and makes some decisions which increase utility at the expense of overloading and extending established terminology. For example, _traversals_ in the standard usage, provide a means of focusing on multiple parts of a datastructure but do not provide similar setting behavior, whereas instances of the `scope.Traversal` class do provide a way to set multiple parts of a larger datastructure.
 
+## Install
+
+Install by running `pip install scope-py` or by cloning this repo and running `pip install .` in the project root directory.
+
 ## Introduction
 
 The Scope library targets manipulation of JSON-like nested structures, which in Python are built from dictionaries, and lists, but custom _optics_ are definable. Scope has a few classes you should be aware of;
 
 - `Lens`: Base class providing get and put methods. Can be composed with other lenses.
 - `ParallelLens`: Allows multiple lenses to be used in parallel.
 - `Traversal`: Provides functionality for working with sequences of data.
@@ -56,15 +60,15 @@
 - `ParallelCRUDLens`: Allows multiple CRUD lenses to be used in parallel.
 - `CRUDTraversal`: Extension of the CRUDLens for working with sequences of data.
 
 Importantly, a `Lens` focuses on one thing and a `Traversals` focuses on many things. A `CRUDLens` extends the get/put functionality of lenses with additional create/delete functionality.
 
 ## Usage
 
-### Basic lens composition example:
+### Basic lens composition:
 
 ```python
 import scope
 
 # create a lens that focuses on item 'b' after item 'a'
 lens = scope.id['a']['b']
 # lens = scope.compose_lenses(scope.id['a'], scope.id['b']) <-- alt. syntax
@@ -72,47 +76,55 @@
 data = {'a': {'b': 3}}
 
 # note -- lens(data) is an alias for lens.get(data)
 assert lens(data) == 3
 assert lens.put(4)(data) == {'a': {'b': 4}}
 ```
 
-### CRUDTraversal example:
+### CRUDTraversal usage:
 
 ```python
 lens = CRUDTraversal(ItemCRUDLens('a'), ItemCRUDLens('c'))
 # lens = ItemCRUDLens('a')[::]['c'] <-- alt. syntax
 
 data = {'a': [{'b': 1}, {'b': 3}]}
 
 # "{'a': [{'b': 1, 'c': 2}, {'b': 3, 'c': 4}]}"
 print(lens.create([2, 4])(data))
 ```
 
-### Custom attribute lens example:
+### Create a custom attribute lens:
 
 ```python
 # create a lens that gets/sets the attribute "my_attr" on an object
-my_attr_lens = scope.Lens(lambda data: getattr(data, 'my_attr'), lambda value: lambda data: setattr(data, 'my_attr', value))
+my_attr_lens = scope.Lens(lambda data: getattr(data, 'my_attr'),
+                          lambda value: lambda data: setattr(data, 'my_attr', value))
 ```
 
-### Parallel lens example:
+### Parallel lens usage:
 
 ```python
 x_lens, y_lens = scope.id['x'], scope.id['y']
 
 # create a lens which focuses on 'x' and 'y' in parallel
 parallel_lens = x_lens | y_lens
 # parallel_lens = scope.ParallelLens(x_lens, y_lens) <-- alt. syntax
 
 data = {'x': 2, 'y': 3}
 
 assert sum(parallel_lens(data)) == 5
 ```
 
+## Todo‘s
+
+- [] Clean up unused files leftover from cloned template repo
+- [] Tests to achieve 100% code coverage
+- [] Add a `filter` method to all classes which accepts a predicate function and applies it to the focus
+- [] Add tests passing and code coverage badges using Github Pages
+
 ## License
 
 This project is open-sourced under the MIT license. See [LICENSE](https://github.com/fchughes/scope/blob/main/LICENSE) for more information.
 
 ## Contact
 
 For questions or issues, please open an issue on GitHub.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

