# Comparing `tmp/tictactoetools-2.0.1.tar.gz` & `tmp/tictactoetools-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactoetools-2.0.1.tar", last modified: Wed Jul 12 17:54:37 2023, max compression
+gzip compressed data, was "tictactoetools-2.1.tar", last modified: Thu Jul 13 02:35:26 2023, max compression
```

## Comparing `tictactoetools-2.0.1.tar` & `tictactoetools-2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.218325 tictactoetools-2.0.1/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-2.0.1/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     2726 2023-07-12 17:54:37.215617 tictactoetools-2.0.1/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     2381 2023-07-12 17:43:35.000000 tictactoetools-2.0.1/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-12 17:54:37.218630 tictactoetools-2.0.1/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      518 2023-07-12 17:54:20.000000 tictactoetools-2.0.1/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.202525 tictactoetools-2.0.1/tests/
--rw-r--r--   0 simon      (502) staff       (20)      110 2023-07-12 17:25:13.000000 tictactoetools-2.0.1/tests/test.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.207860 tictactoetools-2.0.1/tictactoetools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-2.0.1/tictactoetools/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-2.0.1/tictactoetools/tictac_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)    13453 2023-07-12 17:28:05.000000 tictactoetools-2.0.1/tictactoetools/tictactoetools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.213924 tictactoetools-2.0.1/tictactoetools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     2726 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      288 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-13 02:35:26.526409 tictactoetools-2.1/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-2.1/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     2724 2023-07-13 02:35:26.525185 tictactoetools-2.1/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     2381 2023-07-12 17:43:35.000000 tictactoetools-2.1/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-13 02:35:26.527059 tictactoetools-2.1/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      516 2023-07-13 02:32:20.000000 tictactoetools-2.1/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-13 02:35:26.513053 tictactoetools-2.1/tests/
+-rw-r--r--   0 simon      (502) staff       (20)       75 2023-07-12 21:50:58.000000 tictactoetools-2.1/tests/test.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-13 02:35:26.516225 tictactoetools-2.1/tictactoetools/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-2.1/tictactoetools/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-2.1/tictactoetools/tictac_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)    19443 2023-07-13 02:35:12.000000 tictactoetools-2.1/tictactoetools/tictactoetools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-13 02:35:26.523222 tictactoetools-2.1/tictactoetools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     2724 2023-07-13 02:35:26.000000 tictactoetools-2.1/tictactoetools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      288 2023-07-13 02:35:26.000000 tictactoetools-2.1/tictactoetools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-13 02:35:26.000000 tictactoetools-2.1/tictactoetools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-13 02:35:26.000000 tictactoetools-2.1/tictactoetools.egg-info/top_level.txt
```

### Comparing `tictactoetools-2.0.1/LICENSE` & `tictactoetools-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactoetools-2.0.1/PKG-INFO` & `tictactoetools-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 2.0.1
+Version: 2.1
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tictactoetools-2.0.1/README.md` & `tictactoetools-2.1/README.md`

 * *Files identical despite different names*

### Comparing `tictactoetools-2.0.1/setup.py` & `tictactoetools-2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name="tictactoetools",
-    version="2.0.1",
+    version="2.1",
     author="Simon Valentino",
     author_email="simontvalentino@gmail.com",
     url="https://github.com/SimonValentino/tictactoetools.git",
     description="Creatively build Tic-Tac-Toe matches and store their data in a database of all users.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `tictactoetools-2.0.1/tictactoetools.egg-info/PKG-INFO` & `tictactoetools-2.1/tictactoetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 2.0.1
+Version: 2.1
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

