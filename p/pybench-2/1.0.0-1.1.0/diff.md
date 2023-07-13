# Comparing `tmp/pybench_2-1.0.0.tar.gz` & `tmp/pybench_2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybench_2-1.0.0.tar", max compression
+gzip compressed data, was "pybench_2-1.1.0.tar", max compression
```

## Comparing `pybench_2-1.0.0.tar` & `pybench_2-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-07-02 03:43:25.995297 pybench_2-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-01 23:33:15.376520 pybench_2-1.0.0/pybench/__init__.py
--rw-r--r--   0        0        0     4000 2023-07-02 06:35:20.926503 pybench_2-1.0.0/pybench/__main__.py
--rw-r--r--   0        0        0      718 2023-07-02 06:30:37.792515 pybench_2-1.0.0/pybench/base.py
--rw-r--r--   0        0        0     1079 2023-07-01 23:33:15.756962 pybench_2-1.0.0/pybench/generators.py
--rw-r--r--   0        0        0     3524 2023-07-01 23:33:15.813944 pybench_2-1.0.0/pybench/helper.py
--rw-r--r--   0        0        0      461 2023-07-02 03:42:52.874991 pybench_2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 pybench_2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-07-02 03:43:25.995297 pybench_2-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 23:33:15.376520 pybench_2-1.1.0/pybench/__init__.py
+-rw-r--r--   0        0        0     4000 2023-07-02 06:35:20.926503 pybench_2-1.1.0/pybench/__main__.py
+-rw-r--r--   0        0        0      718 2023-07-02 06:30:37.792515 pybench_2-1.1.0/pybench/base.py
+-rw-r--r--   0        0        0     1079 2023-07-01 23:33:15.756962 pybench_2-1.1.0/pybench/generators.py
+-rw-r--r--   0        0        0     3524 2023-07-01 23:33:15.813944 pybench_2-1.1.0/pybench/helper.py
+-rw-r--r--   0        0        0      461 2023-07-13 19:00:01.622647 pybench_2-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 pybench_2-1.1.0/PKG-INFO
```

### Comparing `pybench_2-1.0.0/pybench/__main__.py` & `pybench_2-1.1.0/pybench/__main__.py`

 * *Files identical despite different names*

### Comparing `pybench_2-1.0.0/pybench/base.py` & `pybench_2-1.1.0/pybench/base.py`

 * *Files identical despite different names*

### Comparing `pybench_2-1.0.0/pybench/generators.py` & `pybench_2-1.1.0/pybench/generators.py`

 * *Files identical despite different names*

### Comparing `pybench_2-1.0.0/pybench/helper.py` & `pybench_2-1.1.0/pybench/helper.py`

 * *Files identical despite different names*

### Comparing `pybench_2-1.0.0/PKG-INFO` & `pybench_2-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybench-2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Set of benchmarks of Python code
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

