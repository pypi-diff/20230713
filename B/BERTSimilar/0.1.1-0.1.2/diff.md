# Comparing `tmp/BERTSimilar-0.1.1.tar.gz` & `tmp/BERTSimilar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BERTSimilar-0.1.1.tar", last modified: Thu Jul 13 00:46:04 2023, max compression
+gzip compressed data, was "BERTSimilar-0.1.2.tar", last modified: Thu Jul 13 00:54:36 2023, max compression
```

## Comparing `BERTSimilar-0.1.1.tar` & `BERTSimilar-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:46:04.744695 BERTSimilar-0.1.1/
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:46:04.742816 BERTSimilar-0.1.1/BERTSimilar/
--rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.1/BERTSimilar/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:46:04.743790 BERTSimilar-0.1.1/BERTSimilar.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      228 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-13 00:46:04.000000 BERTSimilar-0.1.1/BERTSimilar.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.1/LICENSE.txt
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 00:46:04.744114 BERTSimilar-0.1.1/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.1/README.md
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-13 00:46:04.744755 BERTSimilar-0.1.1/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-13 00:45:38.000000 BERTSimilar-0.1.1/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:54:36.613987 BERTSimilar-0.1.2/
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:54:36.612343 BERTSimilar-0.1.2/BERTSimilar/
+-rw-r--r--   0 rdp        (501) staff       (20)    25463 2023-07-13 00:21:31.000000 BERTSimilar-0.1.2/BERTSimilar/BERTSimilar.py
+-rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.2/BERTSimilar/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 00:54:36.613122 BERTSimilar-0.1.2/BERTSimilar.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 00:54:36.000000 BERTSimilar-0.1.2/BERTSimilar.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-13 00:54:36.000000 BERTSimilar-0.1.2/BERTSimilar.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-13 00:54:36.000000 BERTSimilar-0.1.2/BERTSimilar.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-13 00:54:36.000000 BERTSimilar-0.1.2/BERTSimilar.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-13 00:54:36.000000 BERTSimilar-0.1.2/BERTSimilar.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.2/LICENSE.txt
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 00:54:36.613362 BERTSimilar-0.1.2/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.2/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-13 00:54:36.614035 BERTSimilar-0.1.2/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-13 00:54:22.000000 BERTSimilar-0.1.2/setup.py
```

### Comparing `BERTSimilar-0.1.1/BERTSimilar.egg-info/PKG-INFO` & `BERTSimilar-0.1.2/BERTSimilar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.1/LICENSE.txt` & `BERTSimilar-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.1/PKG-INFO` & `BERTSimilar-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.1/README.md` & `BERTSimilar-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.1/setup.py` & `BERTSimilar-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='BERTSimilar',
-    version='0.1.1',
+    version='0.1.2',
     description="Get Similar Words and Embeddings using BERT Models",
     keywords="BERT NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

