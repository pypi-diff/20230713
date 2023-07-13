# Comparing `tmp/strangeworks_optimization-0.1.3.tar.gz` & `tmp/strangeworks_optimization-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.1.3.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.1.4.tar", max compression
```

## Comparing `strangeworks_optimization-0.1.3.tar` & `strangeworks_optimization-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       28 2023-06-21 09:22:09.749642 strangeworks_optimization-0.1.3/README.md
--rw-r--r--   0        0        0      993 2023-06-21 09:22:25.630510 strangeworks_optimization-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      174 2023-06-21 09:22:09.749642 strangeworks_optimization-0.1.3/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     2283 2023-06-21 09:22:09.749642 strangeworks_optimization-0.1.3/strangeworks_optimization/optimization.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      196 2023-07-13 14:28:47.827502 strangeworks_optimization-0.1.4/README.md
+-rw-r--r--   0        0        0      994 2023-07-13 14:29:02.019658 strangeworks_optimization-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-13 14:28:47.827502 strangeworks_optimization-0.1.4/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     2746 2023-07-13 14:28:47.827502 strangeworks_optimization-0.1.4/strangeworks_optimization/optimization.py
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.4/PKG-INFO
```

### Comparing `strangeworks_optimization-0.1.3/pyproject.toml` & `strangeworks_optimization-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "strangeworks-optimization"
-version = "0.1.3"
+version = "0.1.4"
 description = "This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "strangeworks_optimization"}]
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
+python = ">=3.10,<4.0"
 strangeworks = "^0.4.2"
 dimod = "^0.12.7"
 strangeworks-python-core = "^0.1.7"
 pydantic = "^1.10.9"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `strangeworks_optimization-0.1.3/PKG-INFO` & `strangeworks_optimization-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization
-Version: 0.1.3
+Version: 0.1.4
 Summary: This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dimod (>=0.12.7,<0.13.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: strangeworks (>=0.4.2,<0.5.0)
 Requires-Dist: strangeworks-python-core (>=0.1.7,<0.2.0)
 Description-Content-Type: text/markdown
 
+![Tests](https://github.com/strangeworks/strangeworks-optimization/actions/workflows/cron_test.yml/badge.svg)
+
 # strangeworks-optimization
 
+[Docs](https://docs.strangeworks.com/apps/optimization)
+
```

