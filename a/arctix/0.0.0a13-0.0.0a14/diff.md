# Comparing `tmp/arctix-0.0.0a13.tar.gz` & `tmp/arctix-0.0.0a14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.0a13.tar", max compression
+gzip compressed data, was "arctix-0.0.0a14.tar", max compression
```

## Comparing `arctix-0.0.0a13.tar` & `arctix-0.0.0a14.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1501 2023-06-16 20:53:03.789659 arctix-0.0.0a13/LICENSE
--rw-r--r--   0        0        0     2019 2023-07-13 06:54:11.763536 arctix-0.0.0a13/README.md
--rw-r--r--   0        0        0     3923 2023-07-13 06:56:57.004336 arctix-0.0.0a13/pyproject.toml
--rw-r--r--   0        0        0      325 2023-07-11 00:38:48.289266 arctix-0.0.0a13/src/arctix/__init__.py
--rw-r--r--   0        0        0    16123 2023-07-13 05:08:24.349012 arctix-0.0.0a13/src/arctix/formatter.py
--rw-r--r--   0        0        0    14512 2023-07-13 06:40:57.190842 arctix-0.0.0a13/src/arctix/summarizer.py
--rw-r--r--   0        0        0        0 2023-07-09 21:11:34.623419 arctix-0.0.0a13/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0     3140 2023-07-13 05:08:24.349389 arctix-0.0.0a13/src/arctix/utils/format.py
--rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 arctix-0.0.0a13/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-13 07:01:44.098384 arctix-0.0.0a14/LICENSE
+-rw-r--r--   0        0        0     2019 2023-07-13 07:01:44.098384 arctix-0.0.0a14/README.md
+-rw-r--r--   0        0        0     3923 2023-07-13 07:01:44.098384 arctix-0.0.0a14/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/__init__.py
+-rw-r--r--   0        0        0    16123 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/formatter.py
+-rw-r--r--   0        0        0    14512 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/summarizer.py
+-rw-r--r--   0        0        0        0 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0     3140 2023-07-13 07:01:44.098384 arctix-0.0.0a14/src/arctix/utils/format.py
+-rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 arctix-0.0.0a14/PKG-INFO
```

### Comparing `arctix-0.0.0a13/LICENSE` & `arctix-0.0.0a14/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a13/README.md` & `arctix-0.0.0a14/README.md`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a13/pyproject.toml` & `arctix-0.0.0a14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.0a13"
+version = "0.0.0a14"
 description = "A library to get a text summary of nested objects"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = []
 license = "BSD-3-Clause"
```

### Comparing `arctix-0.0.0a13/src/arctix/formatter.py` & `arctix-0.0.0a14/src/arctix/formatter.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a13/src/arctix/summarizer.py` & `arctix-0.0.0a14/src/arctix/summarizer.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a13/src/arctix/utils/format.py` & `arctix-0.0.0a14/src/arctix/utils/format.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a13/PKG-INFO` & `arctix-0.0.0a14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.0a13
+Version: 0.0.0a14
 Summary: A library to get a text summary of nested objects
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.0a13 Summary: A library to get
+Metadata-Version: 2.1 Name: arctix Version: 0.0.0a14 Summary: A library to get
 a text summary of nested objects Home-page: https://github.com/durandtibo/
 arctix License: BSD-3-Clause Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

