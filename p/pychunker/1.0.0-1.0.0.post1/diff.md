# Comparing `tmp/pychunker-1.0.0.tar.gz` & `tmp/pychunker-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychunker-1.0.0.tar", max compression
+gzip compressed data, was "pychunker-1.0.0.post1.tar", max compression
```

## Comparing `pychunker-1.0.0.tar` & `pychunker-1.0.0.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-07-13 20:10:18.964686 pychunker-1.0.0/LICENSE
--rw-r--r--   0        0        0       57 2023-07-13 20:37:59.612809 pychunker-1.0.0/pychunker/__init__.py
--rw-r--r--   0        0        0     2675 2023-07-13 20:28:04.083774 pychunker-1.0.0/pychunker/chunk.py
--rw-r--r--   0        0        0     5832 2023-07-13 20:46:51.143097 pychunker-1.0.0/pychunker/chunkfile.py
--rw-r--r--   0        0        0      844 2023-07-13 20:16:28.807145 pychunker-1.0.0/pychunker/functions.py
--rw-r--r--   0        0        0      253 2023-07-13 20:18:44.069709 pychunker-1.0.0/pychunker/functions.pyi
--rw-r--r--   0        0        0       47 2023-07-13 20:31:49.092363 pychunker-1.0.0/pychunker/units.py
--rw-r--r--   0        0        0      658 2023-07-13 21:07:14.557248 pychunker-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-13 20:49:34.510157 pychunker-1.0.0/README.md
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 pychunker-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-13 20:10:18.964686 pychunker-1.0.0.post1/LICENSE
+-rw-r--r--   0        0        0       57 2023-07-13 20:37:59.612809 pychunker-1.0.0.post1/pychunker/__init__.py
+-rw-r--r--   0        0        0     2675 2023-07-13 20:28:04.083774 pychunker-1.0.0.post1/pychunker/chunk.py
+-rw-r--r--   0        0        0     5832 2023-07-13 20:46:51.143097 pychunker-1.0.0.post1/pychunker/chunkfile.py
+-rw-r--r--   0        0        0      844 2023-07-13 20:16:28.807145 pychunker-1.0.0.post1/pychunker/functions.py
+-rw-r--r--   0        0        0      253 2023-07-13 20:18:44.069709 pychunker-1.0.0.post1/pychunker/functions.pyi
+-rw-r--r--   0        0        0       47 2023-07-13 20:31:49.092363 pychunker-1.0.0.post1/pychunker/units.py
+-rw-r--r--   0        0        0      664 2023-07-13 21:09:37.936118 pychunker-1.0.0.post1/pyproject.toml
+-rw-r--r--   0        0        0      498 2023-07-13 21:08:41.956516 pychunker-1.0.0.post1/README.md
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 pychunker-1.0.0.post1/PKG-INFO
```

### Comparing `pychunker-1.0.0/LICENSE` & `pychunker-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0/pychunker/chunk.py` & `pychunker-1.0.0.post1/pychunker/chunk.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0/pychunker/chunkfile.py` & `pychunker-1.0.0.post1/pychunker/chunkfile.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0/pychunker/functions.py` & `pychunker-1.0.0.post1/pychunker/functions.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.0.0/pyproject.toml` & `pychunker-1.0.0.post1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pychunker"
-version = "1.0.0"
+version = "1.0.0.post1"
 description = "Module for reading/writing chunk files."
 authors = ["Romanin <semina054@gmail.com>"]
 repository = "https://github.com/romanin-rf/Chunker"
 license = "MIT"
 readme = "README.md"
 keywords = ["pychunker", "chunker", "chunkfile", "io", "file", "chunk", "read", "write"]
 classifiers = [
```

### Comparing `pychunker-1.0.0/PKG-INFO` & `pychunker-1.0.0.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunker
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Module for reading/writing chunk files.
 Home-page: https://github.com/romanin-rf/Chunker
 License: MIT
 Keywords: pychunker,chunker,chunkfile,io,file,chunk,read,write
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -22,24 +22,24 @@
 # Chunker
 ## Description
 Module for reading/writing chunk files.
 
 ## Using
 - `exmaple.py`:
 ```python
-import chunker
+import pychunker
 
-with chunker.open("chunkfile.bin", "w") as cf:
+with pychunker.open("chunkfile.bin", "w") as cf:
     cf.create_chunk("ADAT")
     cf.create_chunk("STR_")
     
     cf["ADAT"].write(b'1234567890')
     cf["STR_"].write(b'STRING')
 
-with chunker.open("chunkfile.bin") as cf:
+with pychunker.open("chunkfile.bin") as cf:
     print(cf.chunks)
 ```
 
 - `output`:
 ```python
 >>> [Chunk(name='ADAT', mode='r', size=10), Chunk(name='STR_', mode='r', size=6)]
 ```
```

