# Comparing `tmp/mwispy-1.0.3.tar.gz` & `tmp/mwispy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shaobo/Work/script/mwisp_package/dist/.tmp-fs0fbna2/mwispy-1.0.3.tar", last modified: Thu Jul 13 01:39:28 2023, max compression
+gzip compressed data, was "/Users/shaobo/Work/script/mwisp_package/dist/.tmp-_ye5f2f0/mwispy-1.0.4.tar", last modified: Thu Jul 13 02:05:00 2023, max compression
```

## Comparing `mwispy-1.0.3.tar` & `mwispy-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:39:28.221960 mwispy-1.0.3/
--rw-r--r--   0 shaobo     (501) staff       (20)     1054 2023-07-12 05:35:20.000000 mwispy-1.0.3/LICENSE
--rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 01:39:28.221679 mwispy-1.0.3/PKG-INFO
--rw-r--r--   0 shaobo     (501) staff       (20)     7666 2023-07-13 01:26:25.000000 mwispy-1.0.3/README.md
--rw-r--r--   0 shaobo     (501) staff       (20)      729 2023-07-13 01:39:10.000000 mwispy-1.0.3/pyproject.toml
--rw-r--r--   0 shaobo     (501) staff       (20)       38 2023-07-13 01:39:28.222050 mwispy-1.0.3/setup.cfg
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:39:28.215617 mwispy-1.0.3/src/
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:39:28.219473 mwispy-1.0.3/src/mwispy/
--rw-r--r--   0 shaobo     (501) staff       (20)      279 2023-07-12 05:27:10.000000 mwispy-1.0.3/src/mwispy/__init__.py
--rw-r--r--   0 shaobo     (501) staff       (20)     2503 2023-07-12 03:35:10.000000 mwispy-1.0.3/src/mwispy/converter.py
--rw-r--r--   0 shaobo     (501) staff       (20)    14270 2023-07-13 00:43:04.000000 mwispy-1.0.3/src/mwispy/cubemoment.py
--rw-r--r--   0 shaobo     (501) staff       (20)    42692 2023-07-13 00:44:47.000000 mwispy-1.0.3/src/mwispy/datacube.py
--rw-r--r--   0 shaobo     (501) staff       (20)    17025 2023-07-13 00:42:45.000000 mwispy-1.0.3/src/mwispy/mosaic.py
--rw-r--r--   0 shaobo     (501) staff       (20)     8870 2023-07-13 00:47:35.000000 mwispy-1.0.3/src/mwispy/pvslice.py
--rw-r--r--   0 shaobo     (501) staff       (20)     1841 2023-07-12 08:26:23.000000 mwispy-1.0.3/src/mwispy/tile.py
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:39:28.221284 mwispy-1.0.3/src/mwispy.egg-info/
--rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 01:39:28.000000 mwispy-1.0.3/src/mwispy.egg-info/PKG-INFO
--rw-r--r--   0 shaobo     (501) staff       (20)      358 2023-07-13 01:39:28.000000 mwispy-1.0.3/src/mwispy.egg-info/SOURCES.txt
--rw-r--r--   0 shaobo     (501) staff       (20)        1 2023-07-13 01:39:28.000000 mwispy-1.0.3/src/mwispy.egg-info/dependency_links.txt
--rw-r--r--   0 shaobo     (501) staff       (20)      127 2023-07-13 01:39:28.000000 mwispy-1.0.3/src/mwispy.egg-info/requires.txt
--rw-r--r--   0 shaobo     (501) staff       (20)        7 2023-07-13 01:39:28.000000 mwispy-1.0.3/src/mwispy.egg-info/top_level.txt
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 02:05:00.106781 mwispy-1.0.4/
+-rw-r--r--   0 shaobo     (501) staff       (20)     1054 2023-07-12 05:35:20.000000 mwispy-1.0.4/LICENSE
+-rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 02:05:00.106371 mwispy-1.0.4/PKG-INFO
+-rw-r--r--   0 shaobo     (501) staff       (20)     7666 2023-07-13 01:26:25.000000 mwispy-1.0.4/README.md
+-rw-r--r--   0 shaobo     (501) staff       (20)      727 2023-07-13 02:04:45.000000 mwispy-1.0.4/pyproject.toml
+-rw-r--r--   0 shaobo     (501) staff       (20)       38 2023-07-13 02:05:00.106917 mwispy-1.0.4/setup.cfg
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 02:05:00.098853 mwispy-1.0.4/src/
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 02:05:00.103600 mwispy-1.0.4/src/mwispy/
+-rw-r--r--   0 shaobo     (501) staff       (20)      279 2023-07-12 05:27:10.000000 mwispy-1.0.4/src/mwispy/__init__.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     2503 2023-07-12 03:35:10.000000 mwispy-1.0.4/src/mwispy/converter.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    14270 2023-07-13 00:43:04.000000 mwispy-1.0.4/src/mwispy/cubemoment.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    42692 2023-07-13 00:44:47.000000 mwispy-1.0.4/src/mwispy/datacube.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    17025 2023-07-13 00:42:45.000000 mwispy-1.0.4/src/mwispy/mosaic.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     8870 2023-07-13 00:47:35.000000 mwispy-1.0.4/src/mwispy/pvslice.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     1841 2023-07-12 08:26:23.000000 mwispy-1.0.4/src/mwispy/tile.py
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 02:05:00.105932 mwispy-1.0.4/src/mwispy.egg-info/
+-rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 02:05:00.000000 mwispy-1.0.4/src/mwispy.egg-info/PKG-INFO
+-rw-r--r--   0 shaobo     (501) staff       (20)      358 2023-07-13 02:05:00.000000 mwispy-1.0.4/src/mwispy.egg-info/SOURCES.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)        1 2023-07-13 02:05:00.000000 mwispy-1.0.4/src/mwispy.egg-info/dependency_links.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)      125 2023-07-13 02:05:00.000000 mwispy-1.0.4/src/mwispy.egg-info/requires.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)        7 2023-07-13 02:05:00.000000 mwispy-1.0.4/src/mwispy.egg-info/top_level.txt
```

### Comparing `mwispy-1.0.3/LICENSE` & `mwispy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/PKG-INFO` & `mwispy-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mwispy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for MWISP data reduction.
 Author-email: Shaobo Zhang <shbzhang@pmo.ac.cn>
 Project-URL: Homepage, https://github.com/shbzhang/mwispy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mwispy
 ``mwispy`` derives from the [Milky Way Imaging Scroll Painting (MWISP) project](https://ui.adsabs.harvard.edu/abs/2019ApJS..240....9S).
 
 > The MWISP project is an unbiased Galactic plane CO survey for mapping region of l=-10° to +250° and |b|<=5.°2 with the 13.7 m telescope of the Purple Mountain Observatory.
```

### Comparing `mwispy-1.0.3/README.md` & `mwispy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/pyproject.toml` & `mwispy-1.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mwispy"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Shaobo Zhang", email="shbzhang@pmo.ac.cn" },
 ]
 description = "Tools for MWISP data reduction."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy >= 1.19.0",
+    "numpy >= 1.21.0",
     "scipy >= 1.7.0",
     "matplotlib >= 3.4.0",
-    "astropy >= 4.0",
-    "spectral_cube >= 0.6.0",
+    "astropy >= 4.3",
     "tqdm >= 4.62.0",
-    "reproject >= 0.9.1",
-    "radio-beam >= 0.3.3",
+    "spectral_cube >= 0.6.2",
+    "reproject >= 0.8",
+    "radio-beam >= 0.3.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/shbzhang/mwispy"
```

### Comparing `mwispy-1.0.3/src/mwispy/converter.py` & `mwispy-1.0.4/src/mwispy/converter.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/src/mwispy/cubemoment.py` & `mwispy-1.0.4/src/mwispy/cubemoment.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/src/mwispy/datacube.py` & `mwispy-1.0.4/src/mwispy/datacube.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/src/mwispy/mosaic.py` & `mwispy-1.0.4/src/mwispy/mosaic.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/src/mwispy/pvslice.py` & `mwispy-1.0.4/src/mwispy/pvslice.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/src/mwispy/tile.py` & `mwispy-1.0.4/src/mwispy/tile.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.3/src/mwispy.egg-info/PKG-INFO` & `mwispy-1.0.4/src/mwispy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mwispy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for MWISP data reduction.
 Author-email: Shaobo Zhang <shbzhang@pmo.ac.cn>
 Project-URL: Homepage, https://github.com/shbzhang/mwispy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mwispy
 ``mwispy`` derives from the [Milky Way Imaging Scroll Painting (MWISP) project](https://ui.adsabs.harvard.edu/abs/2019ApJS..240....9S).
 
 > The MWISP project is an unbiased Galactic plane CO survey for mapping region of l=-10° to +250° and |b|<=5.°2 with the 13.7 m telescope of the Purple Mountain Observatory.
```

