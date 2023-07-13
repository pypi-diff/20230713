# Comparing `tmp/pysparkler-0.9.dev1689125747.tar.gz` & `tmp/pysparkler-0.9.dev1689188494.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.9.dev1689125747.tar", max compression
+gzip compressed data, was "pysparkler-0.9.dev1689188494.tar", max compression
```

## Comparing `pysparkler-0.9.dev1689125747.tar` & `pysparkler-0.9.dev1689188494.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    13414 2023-07-12 01:35:40.163509 pysparkler-0.9.dev1689125747/README.md
--rw-r--r--   0        0        0     1344 2023-07-12 01:35:48.111525 pysparkler-0.9.dev1689125747/pyproject.toml
--rw-r--r--   0        0        0      807 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/__init__.py
--rw-r--r--   0        0        0     5398 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/api.py
--rw-r--r--   0        0        0     7372 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/base.py
--rw-r--r--   0        0        0     7749 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     4650 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10561 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     3895 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     6404 2023-07-12 01:35:40.167509 pysparkler-0.9.dev1689125747/pysparkler/sql_21_to_33.py
--rw-r--r--   0        0        0    14399 1970-01-01 00:00:00.000000 pysparkler-0.9.dev1689125747/PKG-INFO
+-rw-r--r--   0        0        0    13414 2023-07-12 19:01:24.249738 pysparkler-0.9.dev1689188494/README.md
+-rw-r--r--   0        0        0     1344 2023-07-12 19:01:35.106322 pysparkler-0.9.dev1689188494/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5398 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/base.py
+-rw-r--r--   0        0        0     7749 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     4650 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     3895 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     6404 2023-07-12 19:01:24.253738 pysparkler-0.9.dev1689188494/pysparkler/sql_21_to_33.py
+-rw-r--r--   0        0        0    14399 1970-01-01 00:00:00.000000 pysparkler-0.9.dev1689188494/PKG-INFO
```

### Comparing `pysparkler-0.9.dev1689125747/README.md` & `pysparkler-0.9.dev1689188494/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pyproject.toml` & `pysparkler-0.9.dev1689188494/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.9.dev1689125747"
+version = "0.9.dev1689188494"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/__init__.py` & `pysparkler-0.9.dev1689188494/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/api.py` & `pysparkler-0.9.dev1689188494/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/base.py` & `pysparkler-0.9.dev1689188494/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/cli.py` & `pysparkler-0.9.dev1689188494/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.9.dev1689188494/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.9.dev1689188494/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.9.dev1689188494/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.9.dev1689188494/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.9.dev1689188494/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/pysparkler/sql_21_to_33.py` & `pysparkler-0.9.dev1689188494/pysparkler/sql_21_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1689125747/PKG-INFO` & `pysparkler-0.9.dev1689188494/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.9.dev1689125747
+Version: 0.9.dev1689188494
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

