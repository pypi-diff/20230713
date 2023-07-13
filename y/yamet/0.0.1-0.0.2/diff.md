# Comparing `tmp/yamet-0.0.1.tar.gz` & `tmp/yamet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamet-0.0.1.tar", max compression
+gzip compressed data, was "yamet-0.0.2.tar", max compression
```

## Comparing `yamet-0.0.1.tar` & `yamet-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,26 @@
--rw-r--r--   0        0        0     1073 2023-06-24 17:22:50.383877 yamet-0.0.1/LICENSE
--rw-r--r--   0        0        0     2362 2023-06-24 17:22:50.390877 yamet-0.0.1/README.md
--rw-r--r--   0        0        0     1786 2023-06-24 17:22:50.396877 yamet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       13 2023-06-24 17:22:50.430877 yamet-0.0.1/src/yamet/__init__.py
--rw-r--r--   0        0        0      200 2023-06-24 17:22:50.434877 yamet-0.0.1/src/yamet/__main__.py
--rw-r--r--   0        0        0        0 2023-06-24 17:22:50.426877 yamet-0.0.1/src/yamet/py.typed
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 yamet-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-24 17:22:50.383877 yamet-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2362 2023-06-24 17:22:50.390877 yamet-0.0.2/README.md
+-rw-r--r--   0        0        0     1786 2023-07-13 16:33:16.015258 yamet-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-24 17:22:50.430877 yamet-0.0.2/src/yamet/__init__.py
+-rw-r--r--   0        0        0      200 2023-06-24 17:22:50.434877 yamet-0.0.2/src/yamet/__main__.py
+-rw-r--r--   0        0        0       53 2023-07-11 21:20:46.711274 yamet-0.0.2/src/yamet/analysis/similarity.py
+-rw-r--r--   0        0        0      216 2023-06-26 17:14:12.049374 yamet-0.0.2/src/yamet/analysis/symmetry.py
+-rw-r--r--   0        0        0       22 2023-06-26 10:28:32.209042 yamet-0.0.2/src/yamet/chemistry/data.py
+-rw-r--r--   0        0        0     6616 2023-07-03 16:17:24.196817 yamet-0.0.2/src/yamet/chemistry/utils.py
+-rw-r--r--   0        0        0    10191 2023-07-13 16:12:40.572534 yamet-0.0.2/src/yamet/collectors/singles.py
+-rw-r--r--   0        0        0       41 2023-07-13 16:12:40.576534 yamet-0.0.2/src/yamet/collectors/trajectories.py
+-rw-r--r--   0        0        0        0 2023-06-24 18:58:13.766743 yamet-0.0.2/src/yamet/collectors/utils.py
+-rw-r--r--   0        0        0     2557 2023-07-13 16:12:40.581534 yamet-0.0.2/src/yamet/common/utils.py
+-rw-r--r--   0        0        0       27 2023-07-11 21:20:46.717274 yamet-0.0.2/src/yamet/generation/inputs.py
+-rw-r--r--   0        0        0        6 2023-07-11 21:20:46.718274 yamet-0.0.2/src/yamet/generation/mlsets.py
+-rw-r--r--   0        0        0     6821 2023-07-13 16:12:40.586534 yamet-0.0.2/src/yamet/hull/hull.py
+-rw-r--r--   0        0        0      755 2023-07-13 16:12:40.590534 yamet-0.0.2/src/yamet/machine_learning/clustering.py
+-rw-r--r--   0        0        0      170 2023-07-11 21:20:46.722274 yamet-0.0.2/src/yamet/maths/routines.cpp
+-rw-r--r--   0        0        0      126 2023-07-11 21:20:46.724274 yamet-0.0.2/src/yamet/maths/routines.hpp
+-rw-r--r--   0        0        0       21 2023-07-11 21:20:46.725274 yamet-0.0.2/src/yamet/maths/routines.py
+-rw-r--r--   0        0        0      246 2023-07-11 21:20:46.727274 yamet-0.0.2/src/yamet/plotting/routines.py
+-rw-r--r--   0        0        0        0 2023-06-24 17:22:50.426877 yamet-0.0.2/src/yamet/py.typed
+-rw-r--r--   0        0        0     1413 2023-07-11 21:20:46.730274 yamet-0.0.2/src/yamet/workflows/vasp/getters.py
+-rw-r--r--   0        0        0     1730 2023-07-11 21:20:46.732274 yamet-0.0.2/src/yamet/workflows/vasp/handlers.py
+-rw-r--r--   0        0        0     7580 2023-07-11 21:20:46.733274 yamet-0.0.2/src/yamet/workflows/vasp/high_throughput.py
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 yamet-0.0.2/PKG-INFO
```

### Comparing `yamet-0.0.1/LICENSE` & `yamet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yamet-0.0.1/README.md` & `yamet-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yamet-0.0.1/pyproject.toml` & `yamet-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yamet"
-version = "0.0.1"
+version = "0.0.2"
 description = "YAMET"
 authors = ["Benedict Saunders <benedictsaunders@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/benedictsaunders/yamet"
 repository = "https://github.com/benedictsaunders/yamet"
 documentation = "https://yamet.readthedocs.io"
```

### Comparing `yamet-0.0.1/PKG-INFO` & `yamet-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamet
-Version: 0.0.1
+Version: 0.0.2
 Summary: YAMET
 Home-page: https://github.com/benedictsaunders/yamet
 License: MIT
 Author: Benedict Saunders
 Author-email: benedictsaunders@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

