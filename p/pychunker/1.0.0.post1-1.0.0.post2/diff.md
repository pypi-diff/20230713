# Comparing `tmp/pychunker-1.0.0.post1.tar.gz` & `tmp/pychunker-1.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychunker-1.0.0.post1.tar", max compression
+gzip compressed data, was "pychunker-1.0.0.post2.tar", max compression
```

## Comparing `pychunker-1.0.0.post1.tar` & `pychunker-1.0.0.post2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-07-13 20:10:18.964686 pychunker-1.0.0.post1/LICENSE
--rw-r--r--   0        0        0       57 2023-07-13 20:37:59.612809 pychunker-1.0.0.post1/pychunker/__init__.py
--rw-r--r--   0        0        0     2675 2023-07-13 20:28:04.083774 pychunker-1.0.0.post1/pychunker/chunk.py
--rw-r--r--   0        0        0     5832 2023-07-13 20:46:51.143097 pychunker-1.0.0.post1/pychunker/chunkfile.py
--rw-r--r--   0        0        0      844 2023-07-13 20:16:28.807145 pychunker-1.0.0.post1/pychunker/functions.py
--rw-r--r--   0        0        0      253 2023-07-13 20:18:44.069709 pychunker-1.0.0.post1/pychunker/functions.pyi
--rw-r--r--   0        0        0       47 2023-07-13 20:31:49.092363 pychunker-1.0.0.post1/pychunker/units.py
--rw-r--r--   0        0        0      664 2023-07-13 21:09:37.936118 pychunker-1.0.0.post1/pyproject.toml
--rw-r--r--   0        0        0      498 2023-07-13 21:08:41.956516 pychunker-1.0.0.post1/README.md
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 pychunker-1.0.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-13 20:10:18.964686 pychunker-1.0.0.post2/LICENSE
+-rw-r--r--   0        0        0       57 2023-07-13 20:37:59.612809 pychunker-1.0.0.post2/pychunker/__init__.py
+-rw-r--r--   0        0        0     2675 2023-07-13 20:28:04.083774 pychunker-1.0.0.post2/pychunker/chunk.py
+-rw-r--r--   0        0        0     5832 2023-07-13 20:46:51.143097 pychunker-1.0.0.post2/pychunker/chunkfile.py
+-rw-r--r--   0        0        0      844 2023-07-13 20:16:28.807145 pychunker-1.0.0.post2/pychunker/functions.py
+-rw-r--r--   0        0        0      253 2023-07-13 20:18:44.069709 pychunker-1.0.0.post2/pychunker/functions.pyi
+-rw-r--r--   0        0        0       47 2023-07-13 20:31:49.092363 pychunker-1.0.0.post2/pychunker/units.py
+-rw-r--r--   0        0        0      541 2023-07-13 21:10:43.834535 pychunker-1.0.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      498 2023-07-13 21:08:41.956516 pychunker-1.0.0.post2/README.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 pychunker-1.0.0.post2/PKG-INFO
```

### Comparing `pychunker-1.0.0.post1/LICENSE` & `pychunker-1.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0.post1/pychunker/chunk.py` & `pychunker-1.0.0.post2/pychunker/chunk.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0.post1/pychunker/chunkfile.py` & `pychunker-1.0.0.post2/pychunker/chunkfile.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0.post1/pychunker/functions.py` & `pychunker-1.0.0.post2/pychunker/functions.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0.post1/pyproject.toml` & `pychunker-1.0.0.post2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 [tool.poetry]
 name = "pychunker"
-version = "1.0.0.post1"
+version = "1.0.0.post2"
 description = "Module for reading/writing chunk files."
 authors = ["Romanin <semina054@gmail.com>"]
 repository = "https://github.com/romanin-rf/Chunker"
 license = "MIT"
 readme = "README.md"
 keywords = ["pychunker", "chunker", "chunkfile", "io", "file", "chunk", "read", "write"]
 classifiers = [
-    "Topic :: System :: Filesystems",
-    "Topic :: Software Development :: Build Tools",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Filesystems"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 
 [build-system]
```

### Comparing `pychunker-1.0.0.post1/PKG-INFO` & `pychunker-1.0.0.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: pychunker
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: Module for reading/writing chunk files.
 Home-page: https://github.com/romanin-rf/Chunker
 License: MIT
 Keywords: pychunker,chunker,chunkfile,io,file,chunk,read,write
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Project-URL: Repository, https://github.com/romanin-rf/Chunker
 Description-Content-Type: text/markdown
 
 # Chunker
 ## Description
 Module for reading/writing chunk files.
```

