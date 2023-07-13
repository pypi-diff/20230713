# Comparing `tmp/PathGenMap-0.0.1.tar.gz` & `tmp/pathgenmap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PathGenMap-0.0.1.tar", last modified: Thu Jul 13 13:27:16 2023, max compression
+gzip compressed data, was "pathgenmap-0.0.2.tar", last modified: Thu Jul 13 13:52:13 2023, max compression
```

## Comparing `PathGenMap-0.0.1.tar` & `pathgenmap-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 13:27:16.540366 PathGenMap-0.0.1/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 PathGenMap-0.0.1/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 13:27:16.539168 PathGenMap-0.0.1/PKG-INFO
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 13:27:16.526650 PathGenMap-0.0.1/PathGenMap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 13:27:16.000000 PathGenMap-0.0.1/PathGenMap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      348 2023-07-13 13:27:16.000000 PathGenMap-0.0.1/PathGenMap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-13 13:27:16.000000 PathGenMap-0.0.1/PathGenMap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-13 13:27:16.000000 PathGenMap-0.0.1/PathGenMap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-13 13:27:16.000000 PathGenMap-0.0.1/PathGenMap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)     1349 2023-07-13 13:08:57.000000 PathGenMap-0.0.1/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 13:27:16.538109 PathGenMap-0.0.1/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 PathGenMap-0.0.1/pathgenmap/EggAnnot.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 PathGenMap-0.0.1/pathgenmap/Integration.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 PathGenMap-0.0.1/pathgenmap/PathAnalys.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1139 2023-07-13 13:17:10.000000 PathGenMap-0.0.1/pathgenmap/PathGenMap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 PathGenMap-0.0.1/pathgenmap/SpeciesAbundance.py
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 PathGenMap-0.0.1/pathgenmap/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-13 13:27:16.541207 PathGenMap-0.0.1/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      605 2023-07-13 13:26:21.000000 PathGenMap-0.0.1/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 13:52:13.514314 pathgenmap-0.0.2/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.2/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 13:52:13.511211 pathgenmap-0.0.2/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1349 2023-07-13 13:08:57.000000 pathgenmap-0.0.2/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 13:52:13.502704 pathgenmap-0.0.2/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.2/pathgenmap/EggAnnot.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 pathgenmap-0.0.2/pathgenmap/Integration.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.2/pathgenmap/PathAnalys.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1139 2023-07-13 13:17:10.000000 pathgenmap-0.0.2/pathgenmap/PathGenMap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.2/pathgenmap/SpeciesAbundance.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.2/pathgenmap/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 13:52:13.509910 pathgenmap-0.0.2/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 13:52:13.000000 pathgenmap-0.0.2/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      348 2023-07-13 13:52:13.000000 pathgenmap-0.0.2/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-13 13:52:13.000000 pathgenmap-0.0.2/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-13 13:52:13.000000 pathgenmap-0.0.2/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-13 13:52:13.000000 pathgenmap-0.0.2/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-13 13:52:13.514683 pathgenmap-0.0.2/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      605 2023-07-13 13:49:23.000000 pathgenmap-0.0.2/setup.py
```

### Comparing `PathGenMap-0.0.1/LICENSE` & `pathgenmap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/README.md` & `pathgenmap-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/pathgenmap/EggAnnot.py` & `pathgenmap-0.0.2/pathgenmap/EggAnnot.py`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/pathgenmap/Integration.py` & `pathgenmap-0.0.2/pathgenmap/Integration.py`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/pathgenmap/PathAnalys.py` & `pathgenmap-0.0.2/pathgenmap/PathAnalys.py`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/pathgenmap/PathGenMap.py` & `pathgenmap-0.0.2/pathgenmap/PathGenMap.py`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/pathgenmap/SpeciesAbundance.py` & `pathgenmap-0.0.2/pathgenmap/SpeciesAbundance.py`

 * *Files identical despite different names*

### Comparing `PathGenMap-0.0.1/setup.py` & `pathgenmap-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="PathGenMap",
-    version="0.0.1",
+    name="pathgenmap",
+    version="0.0.2",
     packages=find_packages(),
     scripts=["PathGenMap.py"],
 
     install_requires=["pandas>=1.1.0", "tqdm>=4.48.0"],
 
     # metadata for upload to PyPI
     author="Marcos Paulo Alves de Sousa",
```

