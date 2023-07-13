# Comparing `tmp/pylinac-3.9.0.tar.gz` & `tmp/pylinac-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinac-3.9.0.tar", max compression
+gzip compressed data, was "pylinac-3.9.1.tar", max compression
```

## Comparing `pylinac-3.9.0.tar` & `pylinac-3.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1075 2023-03-07 19:53:37.822356 pylinac-3.9.0/LICENSE.txt
--rw-r--r--   0        0        0     1410 2023-03-07 19:53:37.871356 pylinac-3.9.0/pylinac/__init__.py
--rw-r--r--   0        0        0    46373 2023-03-07 19:53:37.872357 pylinac-3.9.0/pylinac/acr.py
--rw-r--r--   0        0        0        0 2022-12-29 14:28:05.010518 pylinac-3.9.0/pylinac/calibration/__init__.py
--rw-r--r--   0        0        0       17 2022-12-29 14:06:46.333513 pylinac-3.9.0/pylinac/calibration/BUILD
--rw-r--r--   0        0        0    47900 2023-03-07 19:53:37.873357 pylinac-3.9.0/pylinac/calibration/tg51.py
--rw-r--r--   0        0        0    33154 2023-03-07 19:53:37.874356 pylinac-3.9.0/pylinac/calibration/trs398.py
--rw-r--r--   0        0        0    12344 2023-03-07 19:53:37.875357 pylinac-3.9.0/pylinac/cheese.py
--rw-r--r--   0        0        0        0 2022-12-29 14:28:05.003517 pylinac-3.9.0/pylinac/core/__init__.py
--rw-r--r--   0        0        0      824 2022-12-29 14:28:05.027278 pylinac-3.9.0/pylinac/core/decorators.py
--rw-r--r--   0        0        0       42 2022-12-29 14:28:05.030278 pylinac-3.9.0/pylinac/core/exceptions.py
--rw-r--r--   0        0        0    16504 2023-03-07 19:53:37.876356 pylinac-3.9.0/pylinac/core/geometry.py
--rw-r--r--   0        0        0     2507 2023-03-02 20:11:41.986099 pylinac-3.9.0/pylinac/core/hill.py
--rw-r--r--   0        0        0    58687 2023-03-09 15:24:05.285210 pylinac-3.9.0/pylinac/core/image.py
--rw-r--r--   0        0        0      511 2023-03-07 19:53:37.878357 pylinac-3.9.0/pylinac/core/image_generator/__init__.py
--rw-r--r--   0        0        0    12125 2023-03-07 19:53:37.879357 pylinac-3.9.0/pylinac/core/image_generator/layers.py
--rw-r--r--   0        0        0    11617 2022-12-29 14:28:05.056276 pylinac-3.9.0/pylinac/core/image_generator/simulators.py
--rw-r--r--   0        0        0    23632 2023-03-07 19:53:37.880357 pylinac-3.9.0/pylinac/core/image_generator/utils.py
--rw-r--r--   0        0        0     9660 2023-03-07 19:53:37.880357 pylinac-3.9.0/pylinac/core/io.py
--rw-r--r--   0        0        0      393 2022-12-29 14:28:05.034277 pylinac-3.9.0/pylinac/core/mask.py
--rw-r--r--   0        0        0     4035 2023-03-07 19:53:37.882357 pylinac-3.9.0/pylinac/core/mtf.py
--rw-r--r--   0        0        0     4122 2023-03-07 19:53:37.883356 pylinac-3.9.0/pylinac/core/pdf.py
--rw-r--r--   0        0        0    71372 2023-03-07 19:53:37.884357 pylinac-3.9.0/pylinac/core/profile.py
--rw-r--r--   0        0        0    13926 2023-03-07 19:53:37.884357 pylinac-3.9.0/pylinac/core/roi.py
--rw-r--r--   0        0        0     2784 2022-12-29 14:28:05.042275 pylinac-3.9.0/pylinac/core/scale.py
--rw-r--r--   0        0        0      137 2022-12-29 14:28:05.043276 pylinac-3.9.0/pylinac/core/typing.py
--rw-r--r--   0        0        0     5603 2023-03-09 15:24:05.287222 pylinac-3.9.0/pylinac/core/utilities.py
--rw-r--r--   0        0        0    85832 2023-03-07 19:53:37.886356 pylinac-3.9.0/pylinac/ct.py
--rw-r--r--   0        0        0     5182 2023-03-07 19:53:37.887356 pylinac-3.9.0/pylinac/dlg.py
--rw-r--r--   0        0        0    63389 2023-03-07 19:53:37.888357 pylinac-3.9.0/pylinac/field_analysis.py
--rw-r--r--   0        0        0    27173 2022-12-12 16:32:57.800320 pylinac-3.9.0/pylinac/files/Pylinac Full cropped.png
--rw-r--r--   0        0        0   106826 2023-03-07 19:53:37.889357 pylinac-3.9.0/pylinac/log_analyzer.py
--rw-r--r--   0        0        0    60533 2023-03-07 19:53:37.891356 pylinac-3.9.0/pylinac/picketfence.py
--rw-r--r--   0        0        0    98374 2023-03-07 19:53:37.892356 pylinac-3.9.0/pylinac/planar_imaging.py
--rw-r--r--   0        0        0    18484 2023-03-07 19:53:37.893356 pylinac-3.9.0/pylinac/quart.py
--rw-r--r--   0        0        0      533 2022-12-29 14:28:05.003517 pylinac-3.9.0/pylinac/settings.py
--rw-r--r--   0        0        0    27974 2023-03-07 19:53:37.894356 pylinac-3.9.0/pylinac/starshot.py
--rw-r--r--   0        0        0       23 2023-03-15 16:55:51.510520 pylinac-3.9.0/pylinac/version.py
--rw-r--r--   0        0        0    20562 2023-03-07 19:53:37.896356 pylinac-3.9.0/pylinac/vmat.py
--rw-r--r--   0        0        0    78929 2023-03-08 19:33:03.746807 pylinac-3.9.0/pylinac/winston_lutz.py
--rw-r--r--   0        0        0     1857 2023-03-15 16:55:51.510520 pylinac-3.9.0/pyproject.toml
--rw-r--r--   0        0        0    17263 2023-02-22 17:04:27.014590 pylinac-3.9.0/README.rst
--rw-r--r--   0        0        0    18280 2023-03-15 16:57:33.788275 pylinac-3.9.0/setup.py
--rw-r--r--   0        0        0    18506 2023-03-15 16:57:33.789276 pylinac-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-20 20:59:31.853054 pylinac-3.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     1410 2023-03-20 20:59:31.916056 pylinac-3.9.1/pylinac/__init__.py
+-rw-r--r--   0        0        0    46373 2023-03-20 20:59:31.917054 pylinac-3.9.1/pylinac/acr.py
+-rw-r--r--   0        0        0        0 2022-12-29 14:28:05.010518 pylinac-3.9.1/pylinac/calibration/__init__.py
+-rw-r--r--   0        0        0       17 2022-12-29 14:06:46.333513 pylinac-3.9.1/pylinac/calibration/BUILD
+-rw-r--r--   0        0        0    47900 2023-03-20 20:59:31.919054 pylinac-3.9.1/pylinac/calibration/tg51.py
+-rw-r--r--   0        0        0    33154 2023-03-20 20:59:31.920054 pylinac-3.9.1/pylinac/calibration/trs398.py
+-rw-r--r--   0        0        0    12344 2023-03-20 20:59:31.921054 pylinac-3.9.1/pylinac/cheese.py
+-rw-r--r--   0        0        0        0 2022-12-29 14:28:05.003517 pylinac-3.9.1/pylinac/core/__init__.py
+-rw-r--r--   0        0        0      824 2022-12-29 14:28:05.027278 pylinac-3.9.1/pylinac/core/decorators.py
+-rw-r--r--   0        0        0       42 2022-12-29 14:28:05.030278 pylinac-3.9.1/pylinac/core/exceptions.py
+-rw-r--r--   0        0        0    16504 2023-03-20 20:59:31.923054 pylinac-3.9.1/pylinac/core/geometry.py
+-rw-r--r--   0        0        0     2507 2023-03-02 20:11:41.986099 pylinac-3.9.1/pylinac/core/hill.py
+-rw-r--r--   0        0        0    58687 2023-03-20 20:59:31.924053 pylinac-3.9.1/pylinac/core/image.py
+-rw-r--r--   0        0        0      511 2023-03-20 20:59:31.925053 pylinac-3.9.1/pylinac/core/image_generator/__init__.py
+-rw-r--r--   0        0        0    12125 2023-03-20 20:59:31.927053 pylinac-3.9.1/pylinac/core/image_generator/layers.py
+-rw-r--r--   0        0        0    11617 2022-12-29 14:28:05.056276 pylinac-3.9.1/pylinac/core/image_generator/simulators.py
+-rw-r--r--   0        0        0    23632 2023-03-20 20:59:31.928053 pylinac-3.9.1/pylinac/core/image_generator/utils.py
+-rw-r--r--   0        0        0     9660 2023-03-20 20:59:31.929053 pylinac-3.9.1/pylinac/core/io.py
+-rw-r--r--   0        0        0      393 2022-12-29 14:28:05.034277 pylinac-3.9.1/pylinac/core/mask.py
+-rw-r--r--   0        0        0     4035 2023-03-20 20:59:31.930053 pylinac-3.9.1/pylinac/core/mtf.py
+-rw-r--r--   0        0        0     4122 2023-03-20 20:59:31.931053 pylinac-3.9.1/pylinac/core/pdf.py
+-rw-r--r--   0        0        0    71372 2023-03-20 20:59:31.932053 pylinac-3.9.1/pylinac/core/profile.py
+-rw-r--r--   0        0        0    13926 2023-03-20 20:59:31.933053 pylinac-3.9.1/pylinac/core/roi.py
+-rw-r--r--   0        0        0     2784 2022-12-29 14:28:05.042275 pylinac-3.9.1/pylinac/core/scale.py
+-rw-r--r--   0        0        0      137 2022-12-29 14:28:05.043276 pylinac-3.9.1/pylinac/core/typing.py
+-rw-r--r--   0        0        0     5603 2023-03-20 20:59:31.935053 pylinac-3.9.1/pylinac/core/utilities.py
+-rw-r--r--   0        0        0    85832 2023-03-20 20:59:31.937053 pylinac-3.9.1/pylinac/ct.py
+-rw-r--r--   0        0        0     5182 2023-03-20 20:59:31.938053 pylinac-3.9.1/pylinac/dlg.py
+-rw-r--r--   0        0        0    63389 2023-03-20 20:59:31.939052 pylinac-3.9.1/pylinac/field_analysis.py
+-rw-r--r--   0        0        0    27173 2022-12-12 16:32:57.800320 pylinac-3.9.1/pylinac/files/Pylinac Full cropped.png
+-rw-r--r--   0        0        0   107412 2023-03-20 22:07:14.075595 pylinac-3.9.1/pylinac/log_analyzer.py
+-rw-r--r--   0        0        0    60533 2023-03-20 20:59:31.942053 pylinac-3.9.1/pylinac/picketfence.py
+-rw-r--r--   0        0        0    98374 2023-03-20 20:59:31.944053 pylinac-3.9.1/pylinac/planar_imaging.py
+-rw-r--r--   0        0        0    18484 2023-03-20 20:59:31.945052 pylinac-3.9.1/pylinac/quart.py
+-rw-r--r--   0        0        0      533 2022-12-29 14:28:05.003517 pylinac-3.9.1/pylinac/settings.py
+-rw-r--r--   0        0        0    27974 2023-03-20 20:59:31.946053 pylinac-3.9.1/pylinac/starshot.py
+-rw-r--r--   0        0        0       23 2023-03-21 14:45:52.845646 pylinac-3.9.1/pylinac/version.py
+-rw-r--r--   0        0        0    20562 2023-03-20 20:59:31.948053 pylinac-3.9.1/pylinac/vmat.py
+-rw-r--r--   0        0        0    78929 2023-03-20 20:59:31.950053 pylinac-3.9.1/pylinac/winston_lutz.py
+-rw-r--r--   0        0        0     1878 2023-03-21 14:45:52.844672 pylinac-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0    17263 2023-03-20 20:59:05.518453 pylinac-3.9.1/README.rst
+-rw-r--r--   0        0        0    18308 2023-03-21 14:46:21.340668 pylinac-3.9.1/setup.py
+-rw-r--r--   0        0        0    18548 2023-03-21 14:46:21.341668 pylinac-3.9.1/PKG-INFO
```

### Comparing `pylinac-3.9.0/LICENSE.txt` & `pylinac-3.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/__init__.py` & `pylinac-3.9.1/pylinac/__init__.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/acr.py` & `pylinac-3.9.1/pylinac/acr.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/calibration/tg51.py` & `pylinac-3.9.1/pylinac/calibration/tg51.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/calibration/trs398.py` & `pylinac-3.9.1/pylinac/calibration/trs398.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/cheese.py` & `pylinac-3.9.1/pylinac/cheese.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/decorators.py` & `pylinac-3.9.1/pylinac/core/decorators.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/geometry.py` & `pylinac-3.9.1/pylinac/core/geometry.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/hill.py` & `pylinac-3.9.1/pylinac/core/hill.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/image.py` & `pylinac-3.9.1/pylinac/core/image.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/image_generator/layers.py` & `pylinac-3.9.1/pylinac/core/image_generator/layers.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/image_generator/simulators.py` & `pylinac-3.9.1/pylinac/core/image_generator/simulators.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/image_generator/utils.py` & `pylinac-3.9.1/pylinac/core/image_generator/utils.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/io.py` & `pylinac-3.9.1/pylinac/core/io.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/mtf.py` & `pylinac-3.9.1/pylinac/core/mtf.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/pdf.py` & `pylinac-3.9.1/pylinac/core/pdf.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/profile.py` & `pylinac-3.9.1/pylinac/core/profile.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/roi.py` & `pylinac-3.9.1/pylinac/core/roi.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/scale.py` & `pylinac-3.9.1/pylinac/core/scale.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/core/utilities.py` & `pylinac-3.9.1/pylinac/core/utilities.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/ct.py` & `pylinac-3.9.1/pylinac/ct.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/dlg.py` & `pylinac-3.9.1/pylinac/dlg.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/field_analysis.py` & `pylinac-3.9.1/pylinac/field_analysis.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/files/Pylinac Full cropped.png` & `pylinac-3.9.1/pylinac/files/Pylinac Full cropped.png`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/log_analyzer.py` & `pylinac-3.9.1/pylinac/log_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2474,49 +2474,70 @@
         for title, value in zip(header_titles, header_values):
             write_single_value(writer, title, value)
 
         # write axis data
         data_titles = (
             "Gantry",
             "Collimator",
+            "Jaws X1",
+            "Jaws X2",
+            "Jaws Y1",
+            "Jaws Y2",
             "Couch Lat",
             "Couch Lng",
+            "Couch Vert",
             "Couch Rtn",
             "MU",
             "Beam Hold",
             "Control Point",
             "Carriage A",
             "Carriage B",
         )
         ad = self.axis_data
         data_values = (
             ad.gantry,
             ad.collimator,
+            ad.jaws.x1,
+            ad.jaws.x2,
+            ad.jaws.y1,
+            ad.jaws.y2,
             ad.couch.latl,
             ad.couch.long,
+            ad.couch.vert,
             ad.couch.rotn,
+            ad.couch.pitch,
+            ad.couch.roll,
             ad.mu,
             ad.beam_hold,
             ad.control_point,
             ad.carriage_A,
             ad.carriage_B,
         )
         data_units = (
             "degrees",
             "degrees",
             "cm",
             "cm",
+            "cm",
+            "cm",
+            "cm",
+            "cm",
+            "cm",
+            "degrees",
+            "degrees",
             "degrees",
             "MU",
             None,
             None,
             "cm",
             "cm",
         )
         for title, value, unit in zip(data_titles, data_values, data_units):
+            # the value might not exist, such as pitch which is only for 6D couches
+            # thus, check the value exists first
             write_array(writer, title, value, unit)
 
         # write leaf data
         for leaf_num, leaf in self.axis_data.mlc.leaf_axes.items():
             write_array(writer, "Leaf " + str(leaf_num), leaf, "cm")
 
         print("CSV file written to: " + filename)
```

### Comparing `pylinac-3.9.0/pylinac/picketfence.py` & `pylinac-3.9.1/pylinac/picketfence.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/planar_imaging.py` & `pylinac-3.9.1/pylinac/planar_imaging.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/quart.py` & `pylinac-3.9.1/pylinac/quart.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/settings.py` & `pylinac-3.9.1/pylinac/settings.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/starshot.py` & `pylinac-3.9.1/pylinac/starshot.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/vmat.py` & `pylinac-3.9.1/pylinac/vmat.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pylinac/winston_lutz.py` & `pylinac-3.9.1/pylinac/winston_lutz.py`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/pyproject.toml` & `pylinac-3.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylinac"
-version = "3.9.0"
+version = "3.9.1"
 description = "A toolkit for performing TG-142 QA-related tasks on a linear accelerator"
 authors = ["James Kerns <jkerns100@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 documentation = "https://pylinac.readthedocs.io/en/latest/"
 repository = "https://github.com/jrkerns/pylinac"
 keywords = ["medical", "physics", "image", "analysis", "TG-142"]
@@ -36,14 +36,15 @@
 Pillow = ">=4.0"
 argue = "^0.3.1"
 py-linq = "^1.3.0"
 cached-property = "~1.5.2"
 reportlab = ">=3.3"
 pydicom = ">=2.0"
 matplotlib = ">=2.0"
+tabulate = "~0.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = {version = "^7.1.2", python = ">=3.7,<4.0"}
 bump2version = "^1.0.1"
 nox = "^2022.1.7"
 pytest-xdist = "^2.5.0"
 google-cloud-storage = {version = "^2.4.0", python = ">=3.7,<4.0"}
```

### Comparing `pylinac-3.9.0/README.rst` & `pylinac-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pylinac-3.9.0/setup.py` & `pylinac-3.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,20 @@
  'matplotlib>=2.0',
  'numpy>=0.16',
  'py-linq>=1.3.0,<2.0.0',
  'pydicom>=2.0',
  'reportlab>=3.3',
  'scikit-image>=0.17.3',
  'scipy>=1.1',
+ 'tabulate>=0.9.0,<0.10.0',
  'tqdm>=3.8']
 
 setup_kwargs = {
     'name': 'pylinac',
-    'version': '3.9.0',
+    'version': '3.9.1',
     'description': 'A toolkit for performing TG-142 QA-related tasks on a linear accelerator',
     'long_description': 'Pylinac\n=======\n\n.. image:: https://storage.googleapis.com/pylinac_demo_files/Pylinac_Full_cropped.png\n    :width: 100%\n    :target: https://github.com/jrkerns/pylinac\n    :align: center\n\n|\n\n.. image:: https://img.shields.io/pypi/v/pylinac.svg\n    :target: https://pypi.python.org/pypi/pylinac\n    :alt: Latest Version\n\n.. image:: https://img.shields.io/pypi/l/pylinac.svg\n    :target: https://choosealicense.com/licenses/mit/\n    :alt: MIT\n\n.. image:: https://readthedocs.org/projects/pylinac/badge/?version=stable\n    :target: http://pylinac.readthedocs.org/en/stable/\n    :alt: Documentation Status\n\n\nPylinac provides TG-142 quality assurance (QA) tools to Python programmers in the field of\ntherapy and diagnostic medical physics.\n\nPylinac contains high-level modules for automatically analyzing images and data generated by linear accelerators, CT simulators, and other radiation oncology equipment.\nMost scripts can be utilized with less than 10 lines of code.\n\nThe library also contains lower-level `hackable modules & tools <http://pylinac.readthedocs.org/en/stable/pylinac_core_hacking.html>`_\nfor creating your own image analysis algorithms.\n\nThe major features of the entire package include:\n\n* Simple, concise image analysis API\n* Automatic analysis of imaging and performance metrics like MTF, Contrast, ROIs, etc.\n* PDF report generation for solid documentation\n* Automatic phantom registration even if you don\'t set up your phantom perfect\n* Image loading from file, ZIP archives, or URLs\n\nDocumentation\n-------------\n\nTo get started, install the package, run the demos, view the API docs, and learn the module design, visit the\n`Full Documentation <http://pylinac.readthedocs.org/>`_ on Read The Docs.\n\nInstallation\n------------\n\nInstall via ``pip``:\n\n.. code-block:: bash\n\n    $ pip install pylinac\n\nSee the `Installation page <http://pylinac.readthedocs.io/en/stable/installation.html>`_ for further details.\n\nQuick Start Guide\n-----------------\n\nBelow are the high-level tools currently available:\n\n* `TG-51 & TRS-398 Absolute Dose Calibration <http://pylinac.readthedocs.org/en/stable/calibration_docs.html>`__ -\n   Input the raw data and pylinac can calculate either individual values (kQ, PDDx, Pion, etc) or use the\n   provided classes to input all measurement data and have it calculate all factors and dose values automatically.\n\n   Example script:\n\n   .. code-block:: python\n\n            from pylinac import tg51, trs398\n\n            ENERGY = 6\n            TEMP = 22.1\n            PRESS = tg51.mmHg2kPa(755.0)\n            CHAMBER = \'30013\'  # PTW\n            P_ELEC = 1.000\n            ND_w = 5.443  # Gy/nC\n            MU = 200\n            CLINICAL_PDD = 66.5\n\n            tg51_6x = tg51.TG51Photon(\n                unit=\'TrueBeam1\',\n                chamber=CHAMBER,\n                temp=TEMP, press=PRESS,\n                n_dw=ND_w, p_elec=P_ELEC,\n                measured_pdd10=66.4, lead_foil=None,\n                clinical_pdd10=66.5, energy=ENERGY,\n                voltage_reference=-300, voltage_reduced=-150,\n                m_reference=(25.65, 25.66, 25.65),\n                m_opposite=(25.64, 25.65, 25.65),\n                m_reduced=(25.64, 25.63, 25.63),\n                mu=MU, tissue_correction=1.0\n            )\n\n            # Done!\n            print(tg51_6x.dose_mu_dmax)\n\n            # examine other parameters\n            print(tg51_6x.pddx)\n            print(tg51_6x.kq)\n            print(tg51_6x.p_ion)\n\n            # change readings if you adjust output\n            tg51_6x.m_reference_adjusted = (25.44, 25.44, 25.43)\n            # print new dose value\n            print(tg51_6x.dose_mu_dmax_adjusted)\n\n            # generate a PDF for record-keeping\n            tg51_6x.publish_pdf(\'TB1 6MV TG-51.pdf\', notes=[\'My notes\', \'I used Pylinac to do this; so easy!\'], open_file=False)\n\n            # TRS-398 is very similar and just as easy!\n\n* `Planar Phantom Analysis (Leeds TOR, StandardImaging QC-3 & QC-kV, Las Vegas, Doselab MC2 (kV & MV), SNC kV & MV, PTW EPID QC) <http://pylinac.readthedocs.org/en/stable/planar_imaging.html>`__ -\n     Features:\n\n     * **Automatic phantom localization** - Set up your phantom any way you like; automatic positioning,\n       angle, and inversion correction mean you can set up how you like, nor will setup variations give you headache.\n     * **High and low contrast determination** - Analyze both low and high contrast ROIs. Set thresholds\n       as you see fit.\n\n     Example script:\n\n     .. code-block:: python\n\n            from pylinac import LeedsTOR, StandardImagingQC3, LasVegas, DoselabMC2kV, DoselabMC2MV\n\n            leeds = LeedsTOR("my_leeds.dcm")\n            leeds.analyze()\n            leeds.plot_analyzed_image()\n            leeds.publish_pdf()\n\n            qc3 = StandardImagingQC3("my_qc3.dcm")\n            qc3.analyze()\n            qc3.plot_analyzed_image()\n            qc3.publish_pdf(\'qc3.pdf\')\n\n            lv = LasVegas("my_lv.dcm")\n            lv.analyze()\n            lv.plot_analyzed_image()\n            lv.publish_pdf(\'lv.pdf\', open_file=True)  # open the PDF after publishing\n\n            ...\n\n* `Winston-Lutz Analysis <http://pylinac.readthedocs.org/en/stable/winston_lutz.html>`_ -\n    The Winston-Lutz module analyzes EPID images taken of a small radiation field and BB to determine the 2D\n    distance from BB to field CAX. Additionally, the isocenter size of the gantry, collimator, and couch can\n    all be determined *without the BB being at isocenter*. Analysis is based on\n    `Winkler et al <http://iopscience.iop.org/article/10.1088/0031-9155/48/9/303/meta;jsessionid=269700F201744D2EAB897C14D1F4E7B3.c2.iopscience.cld.iop.org>`_\n    , `Du et al <http://scitation.aip.org/content/aapm/journal/medphys/37/5/10.1118/1.3397452>`_, and\n    `Low et al <https://aapm.onlinelibrary.wiley.com/doi/abs/10.1118/1.597475>`_.\n\n    Features:\n\n    * **Couch shift instructions** - After running a WL test, get immediate feedback on how to shift the couch.\n      Couch values can also be passed in and the new couch values will be presented so you don\'t have to do that pesky conversion.\n      "Do I subtract that number or add it?"\n    * **Automatic field & BB positioning** - When an image or directory is loaded, the field CAX and the BB\n      are automatically found, along with the vector and scalar distance between them.\n    * **Isocenter size determination** - Using backprojections of the EPID images, the 3D gantry isocenter size\n      and position can be determined *independent of the BB position*. Additionally, the 2D planar isocenter size\n      of the collimator and couch can also be determined.\n    * **Image plotting** - WL images can be plotted separately or together, each of which shows the field CAX, BB and\n      scalar distance from BB to CAX.\n    * **Axis deviation plots** - Plot the variation of the gantry, collimator, couch, and EPID in each plane\n      as well as RMS variation.\n    * **File name interpretation** - Rename DICOM filenames to include axis information for linacs that don\'t include\n      such information in the DICOM tags. E.g. "myWL_gantry45_coll0_couch315.dcm".\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import WinstonLutz\n\n        wl = WinstonLutz("wl/image/directory")  # images are analyzed upon loading\n        wl.plot_summary()\n        print(wl.results())\n        wl.publish_pdf(\'my_wl.pdf\')\n\n* `Starshot Analysis <http://pylinac.readthedocs.org/en/stable/starshot_docs.html>`_ -\n    The Starshot module analyses a starshot image made of radiation spokes, whether gantry, collimator, MLC or couch.\n    It is based on ideas from `Depuydt et al <http://iopscience.iop.org/0031-9155/57/10/2997>`_\n    and `Gonzalez et al <http://dx.doi.org/10.1118/1.1755491>`_.\n\n    Features:\n\n    * **Analyze scanned film images, single EPID images, or a set of EPID images** -\n      Any image that you can load in can be analyzed, including 1 or a set of EPID DICOM images and\n      films that have been digitally scanned.\n    * **Any image size** - Have machines with different EPIDs? Scanned your film at different resolutions? No problem.\n    * **Dose/OD can be inverted** - Whether your device/image views dose as an increase in value or a decrease, pylinac\n      will detect it and invert if necessary.\n    * **Automatic noise detection & correction** - Sometimes there\'s dirt on the scanned film; sometimes there\'s a dead pixel on the EPID.\n      Pylinac will detect these spurious noise signals and can avoid or account for them.\n    * **Accurate, FWHM star line detection** - Pylinac uses not simply the maximum value to find the center of a star line,\n      but analyzes the entire star profile to determine the center of the FWHM, ensuring small noise or maximum value bias is avoided.\n    * **Adaptive searching** - If you passed pylinac a set of parameters and a good result wasn\'t found, pylinac can recover and\n      do an adaptive search by adjusting parameters to find a "reasonable" wobble.\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import Starshot\n\n        star = Starshot("mystarshot.tif")\n        star.analyze(radius=0.75, tolerance=1.0, fwhm=True)\n        print(star.results())  # prints out wobble information\n        star.plot_analyzed_image()  # shows a matplotlib figure\n        star.publish_pdf()  # publish a PDF report\n\n* `VMAT QA <http://pylinac.readthedocs.org/en/stable/vmat_docs.html>`_ -\n    The VMAT module consists of two classes: ``DRGS`` and ``DRMLC``, which are capable of loading an EPID DICOM Open field image and MLC field image and analyzing the\n    images according to the Varian RapidArc QA tests and procedures, specifically the Dose-Rate & Gantry-Speed (DRGS) and MLC speed (MLCS) tests.\n\n    Features:\n\n    * **Do both tests** - Pylinac can handle either DRGS or DRMLC tests.\n    * **Adjust for offsets** - Older VMAT patterns were off-center. Pylinac will find the field regardless.\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import DRGS, DRMLC\n\n        drgs = DRGS(image_paths=["path/to/DRGSopen.dcm", "path/to/DRGSdmlc.dcm"])\n        drgs.analyze(tolerance=1.5)\n        print(drgs.results())  # prints out ROI information\n        drgs.plot_analyzed_image()  # shows a matplotlib figure\n        drgs.publish_pdf(\'mydrgs.pdf\')  # generate a PDF report\n\n* `CatPhan, Quart, ACR phantom QA <http://pylinac.readthedocs.org/en/stable/cbct_docs.html>`_ -\n    The CBCT module automatically analyzes DICOM images of a CatPhan 504, 503, 600, 604, Quart DVT, and ACR CT/MR acquired when doing CT, CBCT, or MR quality assurance. It can load a folder or zip file that\n    the images are in and automatically correct for phantom setup in 6 axes.\n    CatPhans analyze the HU regions and image scaling (CTP404), the high-contrast line pairs (CTP528) to calculate the modulation transfer function (MTF), and the HU\n    uniformity (CTP486) on the corresponding slice. Quart and ACR analyze similar metrics where possible.\n\n    Features:\n\n    * **Automatic phantom registration** - Your phantom can be tilted, rotated, or translated--pylinac will register the phantom.\n    * **Automatic testing of all major modules** - Major modules are automatically registered and analyzed.\n    * **Any scan protocol** - Scan your CatPhan with any protocol; or even scan it in a regular CT scanner.\n      Any field size or field extent is allowed.\n    * **Customize modules** - You can easily override settings in the event you have a custom scenario such as a partial scan.\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import CatPhan504, CatPhan503, CatPhan600, CatPhan604, QuartDVT, ACRCT, ACRMRILarge\n\n        # for this example, we\'ll use the CatPhan504\n        cbct = CatPhan504("my/cbct_image_folder")\n        cbct.analyze(hu_tolerance=40, scaling_tolerance=1, thickness_tolerance=0.2, low_contrast_threshold=1)\n        print(cbct.results())\n        cbct.plot_analyzed_image()\n        cbct.publish_pdf(\'mycbct.pdf\')\n\n* `Log Analysis <http://pylinac.readthedocs.org/en/stable/log_analyzer.html>`_ -\n    The log analyzer module reads and parses Varian linear accelerator machine logs, both Dynalogs and Trajectory logs. The module also\n    calculates actual and expected fluences as well as performing gamma evaluations. Data is structured to be easily accessible and\n    easily plottable.\n\n    Unlike most other modules of pylinac, the log analyzer module has no end goal. Data is parsed from the logs, but what is done with that\n    info, and which info is analyzed is up to the user.\n\n    Features:\n\n    * **Analyze Dynalogs or Trajectory logs** - Either platform is supported. Tlog versions 2.1 and 3.0 supported.\n    * **Save Trajectory log data to CSV** - The Trajectory log binary data format does not allow for easy export of data. Pylinac lets you do\n      that so you can use Excel or other software that you use with Dynalogs.\n    * **Plot or analyze any axis** - Every data axis can be plotted: the actual, expected, and even the difference.\n    * **View actual or expected fluences & calculate gamma** - View fluences and gamma maps for any log.\n    * **Anonymization** - Anonymize your logs so you can share them with others.\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import load_log\n\n        tlog = load_log("tlog.bin")\n        # after loading, explore any Axis of the Varian structure\n        tlog.axis_data.gantry.plot_actual()  # plot the gantry position throughout treatment\n        tlog.fluence.gamma.calc_map(doseTA=1, distTA=1, threshold=10, resolution=0.1)\n        tlog.fluence.gamma.plot_map()  # show the gamma map as a matplotlib figure\n        tlog.publish_pdf()  # publish a PDF report\n\n        dlog = load_log("dynalog.dlg")\n        ...\n\n* `Picket Fence MLC Analysis <http://pylinac.readthedocs.org/en/stable/picketfence.html>`_ -\n    The picket fence module is meant for analyzing EPID images where a "picket fence" MLC pattern has been made.\n    Physicists regularly check MLC positioning through this test. This test can be done using film and one can\n    "eyeball" it, but this is the 21st century and we have numerous ways of quantifying such data. This module\n    attains to be one of them. It will load in an EPID dicom image and determine the MLC peaks, error of each MLC\n    pair to the picket, and give a few visual indicators for passing/warning/failing.\n\n    Features:\n\n    * **Preset & customizable MLC configurations** - Standard configurations are built-in and you can create your own configuration of leaves if needed.\n    * **Easy-to-read pass/warn/fail overlay** - Analysis gives you easy-to-read tools for determining the status of an MLC pair.\n    * **Any Source-to-Image distance** - Whatever your clinic uses as the SID for picket fence, pylinac can account for it.\n    * **Account for panel translation** - Have an off-CAX setup? No problem. Translate your EPID and pylinac knows.\n    * **Account for panel sag** - If your EPID sags at certain angles, just tell pylinac and the results will be shifted.\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import PicketFence\n\n        pf = PicketFence("mypf.dcm")\n        pf.analyze(tolerance=0.5, action_tolerance=0.25)\n        print(pf.results())\n        pf.plot_analyzed_image()\n        pf.publish_pdf()\n\n* `Open Field Analysis <http://pylinac.readthedocs.org/en/stable/field_analysis.html>`_ -\n    Field analysis from a digital image such as EPID DICOM or 2D device array can easily be analyzed. The module contains built-in\n    flatness and symmetry equation definitions but is extensible to quickly create custom F&S equations.\n\n    Features:\n    * **EPID or device data** - Any EPID image or the SNC Profiler.\n    * **Built-in F&S equations** - The common Elekta, Varian, and Siemens definitions are included\n    * **Extensible equations** - Adding custom equations for image metrics are easy\n\n    Example script:\n\n    .. code-block:: python\n\n        from pylinac import FieldAnalysis, DeviceFieldAnalysis, Protocol\n\n        fa = FieldAnalysis(path="myFS.dcm")  # equivalently, DeviceFieldAnalysis\n        fa.analyze(protocol=Protocol.VARIAN)\n        # print results\n        print(fa.results())\n        # get results as a dict\n        fa.results_data()\n        # plot results\n        fa.plot_analyzed_image()\n        # publish a PDF file\n        fa.publish_pdf(filename=\'my field analysis.pdf\')\n\nDiscussion\n----------\n\nHave questions? Ask them on the `pylinac discussion forum <https://groups.google.com/forum/#!forum/pylinac>`_.\n\nContributing\n------------\n\nContributions to pylinac can be many. The most useful things a non-programmer can contribute are images to analyze and bug reports. If\nyou have VMAT images, starshot images, machine log files, CBCT DICOM files, or anything else you want analyzed, upload them privately\n`here <https://forms.gle/RBR5ubFvjogE9iC67>`_.\n',
     'author': 'James Kerns',
     'author_email': 'jkerns100@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/jrkerns/pylinac',
```

### Comparing `pylinac-3.9.0/PKG-INFO` & `pylinac-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinac
-Version: 3.9.0
+Version: 3.9.1
 Summary: A toolkit for performing TG-142 QA-related tasks on a linear accelerator
 Home-page: https://github.com/jrkerns/pylinac
 License: MIT
 Keywords: medical,physics,image,analysis,TG-142
 Author: James Kerns
 Author-email: jkerns100@gmail.com
 Requires-Python: >=3.7.20,<4.0.0
@@ -28,14 +28,15 @@
 Requires-Dist: matplotlib (>=2.0)
 Requires-Dist: numpy (>=0.16)
 Requires-Dist: py-linq (>=1.3.0,<2.0.0)
 Requires-Dist: pydicom (>=2.0)
 Requires-Dist: reportlab (>=3.3)
 Requires-Dist: scikit-image (>=0.17.3)
 Requires-Dist: scipy (>=1.1)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=3.8)
 Project-URL: Documentation, https://pylinac.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/jrkerns/pylinac
 Description-Content-Type: text/x-rst
 
 Pylinac
 =======
```

