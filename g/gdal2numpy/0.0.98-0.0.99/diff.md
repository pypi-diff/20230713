# Comparing `tmp/gdal2numpy-0.0.98.tar.gz` & `tmp/gdal2numpy-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gdal2numpy-0.0.98.tar", last modified: Fri Feb  3 09:47:38 2023, max compression
+gzip compressed data, was "dist\gdal2numpy-0.0.99.tar", last modified: Fri Feb  3 10:04:05 2023, max compression
```

## Comparing `gdal2numpy-0.0.98.tar` & `gdal2numpy-0.0.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/
--rw-rw-rw-   0        0        0     1091 2021-05-17 13:24:50.000000 gdal2numpy-0.0.98/LICENSE
--rw-rw-rw-   0        0        0      441 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0       14 2021-05-17 13:24:50.000000 gdal2numpy-0.0.98/README.md
--rw-rw-rw-   0        0        0      111 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-02-03 09:47:29.000000 gdal2numpy-0.0.98/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/
-drwxrwxrwx   0        0        0        0 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy/
--rw-rw-rw-   0        0        0     1221 2022-12-31 09:23:46.000000 gdal2numpy-0.0.98/src/gdal2numpy/__init__.py
--rw-rw-rw-   0        0        0     4306 2023-01-18 17:36:07.000000 gdal2numpy-0.0.98/src/gdal2numpy/filesystem.py
--rw-rw-rw-   0        0        0     3186 2023-01-31 18:14:45.000000 gdal2numpy-0.0.98/src/gdal2numpy/gdalwarp.py
--rw-rw-rw-   0        0        0     4195 2023-02-02 16:19:25.000000 gdal2numpy-0.0.98/src/gdal2numpy/module_GDAL2Numpy.py
--rw-rw-rw-   0        0        0     6906 2022-12-31 09:55:19.000000 gdal2numpy-0.0.98/src/gdal2numpy/module_MetaData.py
--rw-rw-rw-   0        0        0     6117 2023-01-18 18:34:33.000000 gdal2numpy-0.0.98/src/gdal2numpy/module_Numpy2GTiff.py
--rw-rw-rw-   0        0        0     8524 2023-02-03 09:47:29.000000 gdal2numpy-0.0.98/src/gdal2numpy/module_features.py
--rw-rw-rw-   0        0        0    11479 2023-01-30 16:20:09.000000 gdal2numpy-0.0.98/src/gdal2numpy/module_ogr.py
--rw-rw-rw-   0        0        0     3472 2022-03-01 08:50:15.000000 gdal2numpy-0.0.98/src/gdal2numpy/rasterizelike.py
--rw-rw-rw-   0        0        0     3513 2022-11-25 15:14:07.000000 gdal2numpy-0.0.98/src/gdal2numpy/rasterlike.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy.egg-info/
--rw-rw-rw-   0        0        0      441 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-03 09:47:38.000000 gdal2numpy-0.0.98/src/gdal2numpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/
+-rw-rw-rw-   0        0        0     1091 2021-05-17 13:24:50.000000 gdal2numpy-0.0.99/LICENSE
+-rw-rw-rw-   0        0        0      441 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2021-05-17 13:24:50.000000 gdal2numpy-0.0.99/README.md
+-rw-rw-rw-   0        0        0      111 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-02-03 10:03:39.000000 gdal2numpy-0.0.99/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/
+drwxrwxrwx   0        0        0        0 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy/
+-rw-rw-rw-   0        0        0     1221 2022-12-31 09:23:46.000000 gdal2numpy-0.0.99/src/gdal2numpy/__init__.py
+-rw-rw-rw-   0        0        0     4306 2023-01-18 17:36:07.000000 gdal2numpy-0.0.99/src/gdal2numpy/filesystem.py
+-rw-rw-rw-   0        0        0     3186 2023-01-31 18:14:45.000000 gdal2numpy-0.0.99/src/gdal2numpy/gdalwarp.py
+-rw-rw-rw-   0        0        0     4195 2023-02-02 16:19:25.000000 gdal2numpy-0.0.99/src/gdal2numpy/module_GDAL2Numpy.py
+-rw-rw-rw-   0        0        0     6906 2022-12-31 09:55:19.000000 gdal2numpy-0.0.99/src/gdal2numpy/module_MetaData.py
+-rw-rw-rw-   0        0        0     6117 2023-01-18 18:34:33.000000 gdal2numpy-0.0.99/src/gdal2numpy/module_Numpy2GTiff.py
+-rw-rw-rw-   0        0        0     8596 2023-02-03 10:02:31.000000 gdal2numpy-0.0.99/src/gdal2numpy/module_features.py
+-rw-rw-rw-   0        0        0    11479 2023-01-30 16:20:09.000000 gdal2numpy-0.0.99/src/gdal2numpy/module_ogr.py
+-rw-rw-rw-   0        0        0     3472 2022-03-01 08:50:15.000000 gdal2numpy-0.0.99/src/gdal2numpy/rasterizelike.py
+-rw-rw-rw-   0        0        0     3513 2022-11-25 15:14:07.000000 gdal2numpy-0.0.99/src/gdal2numpy/rasterlike.py
+drwxrwxrwx   0        0        0        0 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy.egg-info/
+-rw-rw-rw-   0        0        0      441 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-02-03 10:04:05.000000 gdal2numpy-0.0.99/src/gdal2numpy.egg-info/top_level.txt
```

### Comparing `gdal2numpy-0.0.98/LICENSE` & `gdal2numpy-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/setup.py` & `gdal2numpy-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.0.98"
+VERSION = "0.0.99"
 PACKAGE_NAME = "gdal2numpy"
 AUTHOR = "Valerio Luzzi"
 EMAIL = "valerio.luzzi@gecosistema.com"
 GITHUB = f"https://github.com/valluzzi/{PACKAGE_NAME}.git"
 DESCRIPTION = "An utils functions package"
 
 setuptools.setup(
```

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/__init__.py` & `gdal2numpy-0.0.99/src/gdal2numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/filesystem.py` & `gdal2numpy-0.0.99/src/gdal2numpy/filesystem.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/gdalwarp.py` & `gdal2numpy-0.0.99/src/gdal2numpy/gdalwarp.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/module_GDAL2Numpy.py` & `gdal2numpy-0.0.99/src/gdal2numpy/module_GDAL2Numpy.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/module_MetaData.py` & `gdal2numpy-0.0.99/src/gdal2numpy/module_MetaData.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/module_Numpy2GTiff.py` & `gdal2numpy-0.0.99/src/gdal2numpy/module_Numpy2GTiff.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/module_features.py` & `gdal2numpy-0.0.99/src/gdal2numpy/module_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,17 +235,19 @@
         else:
             if verbose:
                 print(f"Creating a new field {fieldname}({width}:{precision})")
             layer.CreateField(newfield)
             res = True
 
         # setting the default value
-        # if res and defaultValue is not None:
-        #    for feature in layer:
-        #        feature.SetField(fieldname, defaultValue)
-        #        layer.SetFeature(feature)
+        if res and defaultValue is not None:
+            layer.StartTransaction()
+            for feature in layer:
+                feature.SetField(fieldname, defaultValue)
+                layer.SetFeature(feature)
+            layer.CommitTransaction()
         # ----
 
     ds = None if closeOnExit else ds
     return res
```

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/module_ogr.py` & `gdal2numpy-0.0.99/src/gdal2numpy/module_ogr.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/rasterizelike.py` & `gdal2numpy-0.0.99/src/gdal2numpy/rasterizelike.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy/rasterlike.py` & `gdal2numpy-0.0.99/src/gdal2numpy/rasterlike.py`

 * *Files identical despite different names*

### Comparing `gdal2numpy-0.0.98/src/gdal2numpy.egg-info/SOURCES.txt` & `gdal2numpy-0.0.99/src/gdal2numpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

