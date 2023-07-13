# Comparing `tmp/crossroads-segmentation-0.1.8.tar.gz` & `tmp/crossroads-segmentation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-segmentation-0.1.8.tar", last modified: Thu Jul  7 14:33:33 2022, max compression
+gzip compressed data, was "crossroads-segmentation-0.1.9.tar", last modified: Fri Jul  8 08:55:15 2022, max compression
```

## Comparing `crossroads-segmentation-0.1.8.tar` & `crossroads-segmentation-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-07 14:33:33.923466 crossroads-segmentation-0.1.8/
--rw-r--r--   0 jm        (1000) jm        (1000)      105 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.8/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     5239 2022-07-07 14:33:33.923466 crossroads-segmentation-0.1.8/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     4655 2022-07-05 13:28:26.000000 crossroads-segmentation-0.1.8/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-07 14:33:33.915466 crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     5239 2022-07-07 14:33:33.000000 crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1350 2022-07-07 14:33:33.000000 crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2022-07-07 14:33:33.000000 crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       93 2022-07-07 14:33:33.000000 crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        6 2022-07-07 14:33:33.000000 crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-07 14:33:33.915466 crossroads-segmentation-0.1.8/crseg/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2022-07-07 14:32:53.000000 crossroads-segmentation-0.1.8/crseg/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)    11620 2022-07-07 14:32:41.000000 crossroads-segmentation-0.1.8/crseg/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    21553 2022-06-29 09:58:55.000000 crossroads-segmentation-0.1.8/crseg/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)     9070 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.8/crseg/crossroad_connections.py
--rw-r--r--   0 jm        (1000) jm        (1000)      995 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.8/crseg/lane_description.py
--rw-r--r--   0 jm        (1000) jm        (1000)     1223 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.8/crseg/link.py
--rw-r--r--   0 jm        (1000) jm        (1000)     4617 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.8/crseg/region.py
--rw-r--r--   0 jm        (1000) jm        (1000)     2746 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.8/crseg/regionfactory.py
--rw-r--r--   0 jm        (1000) jm        (1000)     6635 2022-07-07 14:18:02.000000 crossroads-segmentation-0.1.8/crseg/reliability.py
--rw-r--r--   0 jm        (1000) jm        (1000)    20716 2022-07-07 14:31:57.000000 crossroads-segmentation-0.1.8/crseg/segmentation.py
--rw-r--r--   0 jm        (1000) jm        (1000)     7490 2022-07-07 14:18:05.000000 crossroads-segmentation-0.1.8/crseg/utils.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-07 14:33:33.919466 crossroads-segmentation-0.1.8/examples/
--rw-r--r--   0 jm        (1000) jm        (1000)   147456 2022-04-19 15:03:04.000000 crossroads-segmentation-0.1.8/examples/barcelone.gpkg
--rw-r--r--   0 jm        (1000) jm        (1000)   131072 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.8/examples/champey.gpkg
--rw-r--r--   0 jm        (1000) jm        (1000)   159744 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.8/examples/conakry.gpkg
--rw-r--r--   0 jm        (1000) jm        (1000)     6232 2022-04-10 11:16:26.000000 crossroads-segmentation-0.1.8/examples/crossroads-A-all-structured.json
--rw-r--r--   0 jm        (1000) jm        (1000)     3203 2022-04-10 11:16:01.000000 crossroads-segmentation-0.1.8/examples/crossroads-A-all.json
--rw-r--r--   0 jm        (1000) jm        (1000)     4221 2022-04-10 11:16:21.000000 crossroads-segmentation-0.1.8/examples/crossroads-A-single-structured.json
--rw-r--r--   0 jm        (1000) jm        (1000)     2156 2022-04-10 11:15:53.000000 crossroads-segmentation-0.1.8/examples/crossroads-A-single.json
--rw-r--r--   0 jm        (1000) jm        (1000)     2089 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.8/examples/crossroads-by-name.json
--rw-r--r--   0 jm        (1000) jm        (1000)     4564 2022-04-10 11:09:52.000000 crossroads-segmentation-0.1.8/examples/crossroads-obelisque-1000.json
--rw-r--r--   0 jm        (1000) jm        (1000)     8949 2022-04-10 11:12:08.000000 crossroads-segmentation-0.1.8/examples/crossroads-obelisque-50-structured.json
--rw-r--r--   0 jm        (1000) jm        (1000)     4564 2022-04-10 11:10:01.000000 crossroads-segmentation-0.1.8/examples/crossroads-obelisque-50.json
--rw-r--r--   0 jm        (1000) jm        (1000)     2523 2022-04-10 11:12:18.000000 crossroads-segmentation-0.1.8/examples/crossroads-obelisque-single-structured.json
--rw-r--r--   0 jm        (1000) jm        (1000)     1288 2022-04-10 11:10:10.000000 crossroads-segmentation-0.1.8/examples/crossroads-obelisque-single.json
--rw-r--r--   0 jm        (1000) jm        (1000)   180224 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.8/examples/genoa.gpkg
--rwxr-xr-x   0 jm        (1000) jm        (1000)    11248 2022-07-07 14:32:44.000000 crossroads-segmentation-0.1.8/examples/get-crossroad-segmentation.py
--rwxr-xr-x   0 jm        (1000) jm        (1000)      647 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.8/examples/get-paris-streets.py
--rw-r--r--   0 jm        (1000) jm        (1000)   184320 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.8/examples/new-york.gpkg
--rwxr-xr-x   0 jm        (1000) jm        (1000)     3032 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.8/examples/stats-intersection-info.py
--rw-r--r--   0 jm        (1000) jm        (1000)   176128 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.8/examples/tokyo.gpkg
--rw-r--r--   0 jm        (1000) jm        (1000)   167936 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.8/examples/warsaw.gpkg
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-07 14:33:33.923466 crossroads-segmentation-0.1.8/images/
--rw-r--r--   0 jm        (1000) jm        (1000)    15584 2022-02-02 10:36:43.000000 crossroads-segmentation-0.1.8/images/POC1.png
--rw-r--r--   0 jm        (1000) jm        (1000)   241804 2022-02-02 10:36:43.000000 crossroads-segmentation-0.1.8/images/R1000.png
--rw-r--r--   0 jm        (1000) jm        (1000)    10394 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.8/images/segmentation-step1.png
--rw-r--r--   0 jm        (1000) jm        (1000)    10225 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.8/images/segmentation-step2.png
--rw-r--r--   0 jm        (1000) jm        (1000)     8460 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.8/images/segmentation-step3.png
--rw-r--r--   0 jm        (1000) jm        (1000)     7638 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.8/images/segmentation-step4.png
--rw-r--r--   0 jm        (1000) jm        (1000)     8082 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.8/images/segmentation-step5.png
--rw-r--r--   0 jm        (1000) jm        (1000)        5 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.8/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2022-07-07 14:33:33.923466 crossroads-segmentation-0.1.8/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1181 2022-04-29 14:47:30.000000 crossroads-segmentation-0.1.8/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-08 08:55:15.307381 crossroads-segmentation-0.1.9/
+-rw-r--r--   0 jm        (1000) jm        (1000)      105 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.9/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     5239 2022-07-08 08:55:15.307381 crossroads-segmentation-0.1.9/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     4655 2022-07-05 13:28:26.000000 crossroads-segmentation-0.1.9/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-08 08:55:15.303381 crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     5239 2022-07-08 08:55:15.000000 crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1350 2022-07-08 08:55:15.000000 crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2022-07-08 08:55:15.000000 crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       93 2022-07-08 08:55:15.000000 crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        6 2022-07-08 08:55:15.000000 crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-08 08:55:15.303381 crossroads-segmentation-0.1.9/crseg/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2022-07-08 08:53:41.000000 crossroads-segmentation-0.1.9/crseg/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    11360 2022-07-08 08:54:11.000000 crossroads-segmentation-0.1.9/crseg/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    21553 2022-06-29 09:58:55.000000 crossroads-segmentation-0.1.9/crseg/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     9070 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.9/crseg/crossroad_connections.py
+-rw-r--r--   0 jm        (1000) jm        (1000)      995 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.9/crseg/lane_description.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     1223 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.9/crseg/link.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     4617 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.9/crseg/region.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     2746 2022-04-20 09:42:27.000000 crossroads-segmentation-0.1.9/crseg/regionfactory.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     6635 2022-07-07 14:18:02.000000 crossroads-segmentation-0.1.9/crseg/reliability.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    20714 2022-07-08 08:53:23.000000 crossroads-segmentation-0.1.9/crseg/segmentation.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7799 2022-07-08 08:54:06.000000 crossroads-segmentation-0.1.9/crseg/utils.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-08 08:55:15.307381 crossroads-segmentation-0.1.9/examples/
+-rw-r--r--   0 jm        (1000) jm        (1000)   147456 2022-04-19 15:03:04.000000 crossroads-segmentation-0.1.9/examples/barcelone.gpkg
+-rw-r--r--   0 jm        (1000) jm        (1000)   131072 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.9/examples/champey.gpkg
+-rw-r--r--   0 jm        (1000) jm        (1000)   159744 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.9/examples/conakry.gpkg
+-rw-r--r--   0 jm        (1000) jm        (1000)     6232 2022-04-10 11:16:26.000000 crossroads-segmentation-0.1.9/examples/crossroads-A-all-structured.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     3203 2022-04-10 11:16:01.000000 crossroads-segmentation-0.1.9/examples/crossroads-A-all.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     4221 2022-04-10 11:16:21.000000 crossroads-segmentation-0.1.9/examples/crossroads-A-single-structured.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     2156 2022-04-10 11:15:53.000000 crossroads-segmentation-0.1.9/examples/crossroads-A-single.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     2089 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.9/examples/crossroads-by-name.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     4564 2022-04-10 11:09:52.000000 crossroads-segmentation-0.1.9/examples/crossroads-obelisque-1000.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     8949 2022-04-10 11:12:08.000000 crossroads-segmentation-0.1.9/examples/crossroads-obelisque-50-structured.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     4564 2022-04-10 11:10:01.000000 crossroads-segmentation-0.1.9/examples/crossroads-obelisque-50.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     2523 2022-04-10 11:12:18.000000 crossroads-segmentation-0.1.9/examples/crossroads-obelisque-single-structured.json
+-rw-r--r--   0 jm        (1000) jm        (1000)     1288 2022-04-10 11:10:10.000000 crossroads-segmentation-0.1.9/examples/crossroads-obelisque-single.json
+-rw-r--r--   0 jm        (1000) jm        (1000)   180224 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.9/examples/genoa.gpkg
+-rwxr-xr-x   0 jm        (1000) jm        (1000)    11005 2022-07-08 08:53:49.000000 crossroads-segmentation-0.1.9/examples/get-crossroad-segmentation.py
+-rwxr-xr-x   0 jm        (1000) jm        (1000)      647 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.9/examples/get-paris-streets.py
+-rw-r--r--   0 jm        (1000) jm        (1000)   184320 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.9/examples/new-york.gpkg
+-rwxr-xr-x   0 jm        (1000) jm        (1000)     3032 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.9/examples/stats-intersection-info.py
+-rw-r--r--   0 jm        (1000) jm        (1000)   176128 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.9/examples/tokyo.gpkg
+-rw-r--r--   0 jm        (1000) jm        (1000)   167936 2022-05-06 14:11:22.000000 crossroads-segmentation-0.1.9/examples/warsaw.gpkg
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-07-08 08:55:15.307381 crossroads-segmentation-0.1.9/images/
+-rw-r--r--   0 jm        (1000) jm        (1000)    15584 2022-02-02 10:36:43.000000 crossroads-segmentation-0.1.9/images/POC1.png
+-rw-r--r--   0 jm        (1000) jm        (1000)   241804 2022-02-02 10:36:43.000000 crossroads-segmentation-0.1.9/images/R1000.png
+-rw-r--r--   0 jm        (1000) jm        (1000)    10394 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.9/images/segmentation-step1.png
+-rw-r--r--   0 jm        (1000) jm        (1000)    10225 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.9/images/segmentation-step2.png
+-rw-r--r--   0 jm        (1000) jm        (1000)     8460 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.9/images/segmentation-step3.png
+-rw-r--r--   0 jm        (1000) jm        (1000)     7638 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.9/images/segmentation-step4.png
+-rw-r--r--   0 jm        (1000) jm        (1000)     8082 2022-04-20 15:41:30.000000 crossroads-segmentation-0.1.9/images/segmentation-step5.png
+-rw-r--r--   0 jm        (1000) jm        (1000)        5 2022-04-20 09:42:28.000000 crossroads-segmentation-0.1.9/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2022-07-08 08:55:15.307381 crossroads-segmentation-0.1.9/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1181 2022-04-29 14:47:30.000000 crossroads-segmentation-0.1.9/setup.py
```

### Comparing `crossroads-segmentation-0.1.8/PKG-INFO` & `crossroads-segmentation-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-segmentation
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crossroads segmentation is a python tool that produces automatic segmentations of data from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-segmentation/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `crossroads-segmentation-0.1.8/README.md` & `crossroads-segmentation-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/PKG-INFO` & `crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-segmentation
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crossroads segmentation is a python tool that produces automatic segmentations of data from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-segmentation/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `crossroads-segmentation-0.1.8/crossroads_segmentation.egg-info/SOURCES.txt` & `crossroads-segmentation-0.1.9/crossroads_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/cmd.py` & `crossroads-segmentation-0.1.9/crseg/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,14 @@
 import crseg.region as rg
 import crseg.utils as u
 import json
 
 def get_crossroad_segmentation_command():
 
 
-    # add information about cycleways
-    othertags = ["cycleway", "cycleway:right", "cycleway:left", "psv"]
-    ox.settings.osm_xml_way_tags = ox.settings.osm_xml_way_tags + othertags
-    ox.settings.useful_tags_way = ox.settings.useful_tags_way + othertags
-
     # a trick to avoid the creation of files given as parameters
     class FileOpener(argparse.FileType):
         # delayed FileType;
         # sample use:
         # with args.input.open() as f: f.read()
         def __call__(self, string):
             # optionally test string
```

### Comparing `crossroads-segmentation-0.1.8/crseg/crossroad.py` & `crossroads-segmentation-0.1.9/crseg/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/crossroad_connections.py` & `crossroads-segmentation-0.1.9/crseg/crossroad_connections.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/lane_description.py` & `crossroads-segmentation-0.1.9/crseg/lane_description.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/link.py` & `crossroads-segmentation-0.1.9/crseg/link.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/region.py` & `crossroads-segmentation-0.1.9/crseg/region.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/regionfactory.py` & `crossroads-segmentation-0.1.9/crseg/regionfactory.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/reliability.py` & `crossroads-segmentation-0.1.9/crseg/reliability.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/crseg/segmentation.py` & `crossroads-segmentation-0.1.9/crseg/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
             return self.regions[tag].is_crossroad()
 
     ######################### Functions used to prepare the graph ########################
 
     def prepare_network(G, keep_all_components=False, remove_non_highway=True,
                         remove_parking_aisle=True,
                         remove_footways=True, remove_cycleways=True):
-
         to_remove = []
         # remove footways and parkings
         for u, v, k, a in G.edges(data=True, keys=True):
             if remove_non_highway and not "highway" in a:
                 # remove a specific edge. If k==0, it will remove the first edge, and it might remain supplementary edge with a key != 0.
                 # To solve this issue, at the end of this function, we use a trick by transforming data to a DiGraph, then to a MutliDiGraph (the original
                 # data structure used by the program)
@@ -211,15 +210,14 @@
                     if ("highway" in a and a["highway"] in ["path", "pedestrian", "steps"]) and not ("psv" in a and a["psv"] in ["yes"]):
                         to_remove.append((u, v))
                 if remove_cycleways and "highway" in a and a["highway"] in ["cycleway"]:
                     to_remove.append((u, v))
                 if remove_parking_aisle:
                     if "service" in a and a["service"] in ["parking_aisle"]:
                         to_remove.append((u, v))
-
         G.remove_edges_from(to_remove)
         G = ox.utils_graph.remove_isolated_nodes(G)
         if not keep_all_components and len(G.nodes) != 0:
             G = ox.utils_graph.get_largest_component(G)
         # double transformation to fix keys != 0
         return nx.MultiDiGraph(nx.DiGraph(G))
```

### Comparing `crossroads-segmentation-0.1.8/crseg/utils.py` & `crossroads-segmentation-0.1.9/crseg/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,14 +184,19 @@
         return result
 
 
     def get_osm_data(latitude, longitude, radius, overpass, tmpfile = None):
         if overpass:
             G = ox.graph_from_point((latitude, longitude), dist=radius, network_type="all", retain_all=False, truncate_by_edge=True, simplify=False)
         else:
+            # add information about cycleways
+            othertags = ["cycleway", "cycleway:right", "cycleway:left", "psv"]
+            ox.settings.osm_xml_way_tags = ox.settings.osm_xml_way_tags + othertags
+            ox.settings.useful_tags_way = ox.settings.useful_tags_way + othertags
+
             p = Point(longitude, latitude)
             gdf_p = gp.GeoDataFrame(geometry=[p]).set_crs('EPSG:4326').to_crs('EPSG:3857')
             pb = gdf_p.buffer(distance=radius).envelope
             gdf_l = gp.GeoDataFrame(geometry=pb).to_crs('EPSG:4326')
             poly = gdf_l['geometry'][0]
             long1 = poly.exterior.coords.xy[0][0]
             long2 = poly.exterior.coords.xy[0][1]
@@ -203,9 +208,9 @@
                 print("Error from OpenStreetMap API. You should try using overpass.")
                 return None
             if tmpfile:
                 tmp = tmpfile
             else:
                 tmp = tempfile.NamedTemporaryFile(mode='w', delete=False, suffix=".xml")
             open(tmp.name, 'wb').write(r.content)
-            G = ox.graph_from_xml(tmp.name, simplify=False)
+            G = ox.graph_from_xml(tmp.name, simplify=False, retain_all=True)
         return G
```

### Comparing `crossroads-segmentation-0.1.8/examples/barcelone.gpkg` & `crossroads-segmentation-0.1.9/examples/barcelone.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/champey.gpkg` & `crossroads-segmentation-0.1.9/examples/champey.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/conakry.gpkg` & `crossroads-segmentation-0.1.9/examples/conakry.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-A-all-structured.json` & `crossroads-segmentation-0.1.9/examples/crossroads-A-all-structured.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-A-all.json` & `crossroads-segmentation-0.1.9/examples/crossroads-A-all.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-A-single-structured.json` & `crossroads-segmentation-0.1.9/examples/crossroads-A-single-structured.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-A-single.json` & `crossroads-segmentation-0.1.9/examples/crossroads-A-single.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-by-name.json` & `crossroads-segmentation-0.1.9/examples/crossroads-by-name.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-obelisque-1000.json` & `crossroads-segmentation-0.1.9/examples/crossroads-obelisque-1000.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-obelisque-50-structured.json` & `crossroads-segmentation-0.1.9/examples/crossroads-obelisque-50-structured.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-obelisque-50.json` & `crossroads-segmentation-0.1.9/examples/crossroads-obelisque-50.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-obelisque-single-structured.json` & `crossroads-segmentation-0.1.9/examples/crossroads-obelisque-single-structured.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/crossroads-obelisque-single.json` & `crossroads-segmentation-0.1.9/examples/crossroads-obelisque-single.json`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/genoa.gpkg` & `crossroads-segmentation-0.1.9/examples/genoa.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/get-crossroad-segmentation.py` & `crossroads-segmentation-0.1.9/examples/get-crossroad-segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 #encoding: utf-8
 
 import argcomplete, argparse
 import os
 
 import networkx as nx
 import osmnx as ox
-# add information about cycleways
-othertags = ["cycleway", "cycleway:right", "cycleway:left", "psv"]
-ox.settings.osm_xml_way_tags = ox.settings.osm_xml_way_tags + othertags
-ox.settings.useful_tags_way = ox.settings.useful_tags_way + othertags
 
 # a trick to avoid the creation of files given as parameters
 class FileOpener(argparse.FileType):
     # delayed FileType;
     # sample use:
     # with args.input.open() as f: f.read()
     def __call__(self, string):
```

### Comparing `crossroads-segmentation-0.1.8/examples/get-paris-streets.py` & `crossroads-segmentation-0.1.9/examples/get-paris-streets.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/new-york.gpkg` & `crossroads-segmentation-0.1.9/examples/new-york.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/stats-intersection-info.py` & `crossroads-segmentation-0.1.9/examples/stats-intersection-info.py`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/tokyo.gpkg` & `crossroads-segmentation-0.1.9/examples/tokyo.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/examples/warsaw.gpkg` & `crossroads-segmentation-0.1.9/examples/warsaw.gpkg`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/POC1.png` & `crossroads-segmentation-0.1.9/images/POC1.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/R1000.png` & `crossroads-segmentation-0.1.9/images/R1000.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/segmentation-step1.png` & `crossroads-segmentation-0.1.9/images/segmentation-step1.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/segmentation-step2.png` & `crossroads-segmentation-0.1.9/images/segmentation-step2.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/segmentation-step3.png` & `crossroads-segmentation-0.1.9/images/segmentation-step3.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/segmentation-step4.png` & `crossroads-segmentation-0.1.9/images/segmentation-step4.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/images/segmentation-step5.png` & `crossroads-segmentation-0.1.9/images/segmentation-step5.png`

 * *Files identical despite different names*

### Comparing `crossroads-segmentation-0.1.8/setup.py` & `crossroads-segmentation-0.1.9/setup.py`

 * *Files identical despite different names*

