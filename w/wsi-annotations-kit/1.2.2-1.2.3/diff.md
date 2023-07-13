# Comparing `tmp/wsi-annotations-kit-1.2.2.tar.gz` & `tmp/wsi-annotations-kit-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.2.2.tar", last modified: Thu Jul 13 16:36:07 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.2.3.tar", last modified: Thu Jul 13 16:47:28 2023, max compression
```

## Comparing `wsi-annotations-kit-1.2.2.tar` & `wsi-annotations-kit-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:36:07.000000 wsi-annotations-kit-1.2.2/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      745 2023-07-13 16:36:07.000000 wsi-annotations-kit-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 16:36:07.000000 wsi-annotations-kit-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-07-13 16:36:00.000000 wsi-annotations-kit-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:36:06.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21949 2023-07-13 16:35:54.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:36:07.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-07-13 16:36:06.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-13 16:36:06.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:36:06.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-13 16:36:06.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-13 16:36:06.000000 wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-13 16:47:21.000000 wsi-annotations-kit-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    21953 2023-07-13 16:47:14.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-13 16:47:28.000000 wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.2.2/LICENSE` & `wsi-annotations-kit-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.2.2/PKG-INFO` & `wsi-annotations-kit-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.2
+Version: 1.2.3
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.2.2/setup.py` & `wsi-annotations-kit-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.2.2",
+    version="1.2.3",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
```

### Comparing `wsi-annotations-kit-1.2.2/wsi_annotations_kit/wsi_annotations_kit.py` & `wsi-annotations-kit-1.2.3/wsi_annotations_kit/wsi_annotations_kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         # poly = shapely polygon or other geometry
         # box_crs = upper left corner for location that this object is in 
         # structure = structure name (which structure is this in general)
         # name = shape name (individual object name)
         if structure not in self.objects:
             self.objects[structure] = [Object(poly,box_crs,structure,name,properties)]
         else:
-            self.objects[structure] = [Object(poly,box_crs,structure,name,properties)]
+            self.objects[structure].append(Object(poly,box_crs,structure,name,properties))
     
     def add_names(self,names):
         
         # Initializing 
         for n in names:
             self.objects[n] = {}
             self.structure_names.append(n)
```

### Comparing `wsi-annotations-kit-1.2.2/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.2.3/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.2
+Version: 1.2.3
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

