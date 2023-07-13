# Comparing `tmp/hmatrices-0.1.1.tar.gz` & `tmp/hmatrices-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmatrices-0.1.1.tar", max compression
+gzip compressed data, was "hmatrices-0.1.2.tar", max compression
```

## Comparing `hmatrices-0.1.1.tar` & `hmatrices-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      397 2023-07-12 11:24:03.914458 hmatrices-0.1.1/README.md
--rw-r--r--   0        0        0      403 2023-07-12 13:31:48.729920 hmatrices-0.1.1/hmatrices/__init__.py
--rw-r--r--   0        0        0      294 2023-07-12 13:42:00.566896 hmatrices-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 hmatrices-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      397 2023-07-12 11:24:03.914458 hmatrices-0.1.2/README.md
+-rw-r--r--   0        0        0      362 2023-07-13 06:58:32.177825 hmatrices-0.1.2/hmatrices/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-13 06:59:01.396305 hmatrices-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 hmatrices-0.1.2/PKG-INFO
```

### Comparing `hmatrices-0.1.1/PKG-INFO` & `hmatrices-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmatrices
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Luiz M. Faria
 Author-email: maltezfaria@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: juliacall (>=0.9.13,<0.10.0)
```

