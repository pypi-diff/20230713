# Comparing `tmp/clustutils4r-0.0.2.tar.gz` & `tmp/clustutils4r-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.2.tar", last modified: Thu Jul 13 08:58:00 2023, max compression
+gzip compressed data, was "clustutils4r-0.0.3.tar", last modified: Thu Jul 13 09:03:56 2023, max compression
```

## Comparing `clustutils4r-0.0.2.tar` & `clustutils4r-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 08:58:00.502368 clustutils4r-0.0.2/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.2/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3495 2023-07-13 08:58:00.502368 clustutils4r-0.0.2/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     2863 2023-07-13 08:52:52.000000 clustutils4r-0.0.2/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-13 08:57:20.000000 clustutils4r-0.0.2/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-13 08:58:00.502368 clustutils4r-0.0.2/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-13 08:57:34.000000 clustutils4r-0.0.2/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 08:58:00.498368 clustutils4r-0.0.2/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 08:58:00.498368 clustutils4r-0.0.2/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.2/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25402 2023-07-13 08:55:31.000000 clustutils4r-0.0.2/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 08:58:00.502368 clustutils4r-0.0.2/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3495 2023-07-13 08:58:00.000000 clustutils4r-0.0.2/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-13 08:58:00.000000 clustutils4r-0.0.2/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-13 08:58:00.000000 clustutils4r-0.0.2/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-13 08:58:00.000000 clustutils4r-0.0.2/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-13 08:58:00.000000 clustutils4r-0.0.2/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.3/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3495 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     2863 2023-07-13 08:52:52.000000 clustutils4r-0.0.3/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-13 09:03:19.000000 clustutils4r-0.0.3/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-13 09:03:15.000000 clustutils4r-0.0.3/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.227658 clustutils4r-0.0.3/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.3/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25402 2023-07-13 08:55:31.000000 clustutils4r-0.0.3/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/src/clustutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3495 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.2/LICENSE` & `clustutils4r-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.2/PKG-INFO` & `clustutils4r-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clustutils4r-0.0.2/README.md` & `clustutils4r-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.2/pyproject.toml` & `clustutils4r-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.2/setup.py` & `clustutils4r-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clustutils4r", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn utilities for clustering.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clustutils4r",
     project_urls={
```

### Comparing `clustutils4r-0.0.2/src/clustutils4r/eval_clustering.py` & `clustutils4r-0.0.3/src/clustutils4r/eval_clustering.py`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.2/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-0.0.3/src/clustutils4r.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

