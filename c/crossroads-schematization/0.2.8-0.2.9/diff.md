# Comparing `tmp/crossroads-schematization-0.2.8.tar.gz` & `tmp/crossroads-schematization-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.2.8.tar", last modified: Fri Jul  7 10:23:22 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.9.tar", last modified: Tue Jul 11 17:03:04 2023, max compression
```

## Comparing `crossroads-schematization-0.2.8.tar` & `crossroads-schematization-0.2.9.tar`

### file list

```diff
@@ -1,43 +1,58 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.8/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.8/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.843182 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1188 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.843182 crossroads-schematization-0.2.8/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-07 10:22:54.000000 crossroads-schematization-0.2.8/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     8217 2023-07-06 12:33:37.000000 crossroads-schematization-0.2.8/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    52583 2023-07-07 07:58:48.000000 crossroads-schematization-0.2.8/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    26625 2023-07-07 10:17:53.000000 crossroads-schematization-0.2.8/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.8/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.843182 crossroads-schematization-0.2.8/crschem/resources/
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/crschem/resources/400/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.8/crschem/resources/400/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.8/crschem/resources/400/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     3458 2023-07-07 10:21:11.000000 crossroads-schematization-0.2.8/crschem/resources/400/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3456 2023-07-07 10:21:17.000000 crossroads-schematization-0.2.8/crschem/resources/400/style-96.xml
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/crschem/resources/500/
--rw-r--r--   0 jm        (1000) jm        (1000)     1941 2023-07-07 10:01:36.000000 crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1932 2023-07-07 10:02:54.000000 crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1519 2023-07-07 10:06:34.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1516 2023-07-07 10:06:11.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     3458 2023-07-07 10:21:05.000000 crossroads-schematization-0.2.8/crschem/resources/500/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3457 2023-07-07 10:20:48.000000 crossroads-schematization-0.2.8/crschem/resources/500/style-96.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.8/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.8/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.8/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.347661 crossroads-schematization-0.2.9/
+-rw-r--r--   0 jm        (1000) jm        (1000)      141 2023-07-10 12:56:10.000000 crossroads-schematization-0.2.9/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-11 17:03:04.347661 crossroads-schematization-0.2.9/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.9/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.339661 crossroads-schematization-0.2.9/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-11 17:03:04.000000 crossroads-schematization-0.2.9/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1760 2023-07-11 17:03:04.000000 crossroads-schematization-0.2.9/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-11 17:03:04.000000 crossroads-schematization-0.2.9/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-11 17:03:04.000000 crossroads-schematization-0.2.9/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-11 17:03:04.000000 crossroads-schematization-0.2.9/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.339661 crossroads-schematization-0.2.9/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-11 17:02:35.000000 crossroads-schematization-0.2.9/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     8563 2023-07-10 13:13:14.000000 crossroads-schematization-0.2.9/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    27352 2023-07-11 08:41:01.000000 crossroads-schematization-0.2.9/crschem/crossroad_schematization.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.343661 crossroads-schematization-0.2.9/crschem/model/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.343661 crossroads-schematization-0.2.9/crschem/model/__pycache__/
+-rw-r--r--   0 jm        (1000) jm        (1000)    11279 2023-07-10 12:50:48.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/branch.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)    25891 2023-07-10 12:51:18.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/crossing.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     3035 2023-07-10 13:12:42.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/simple_way.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     4069 2023-07-11 09:15:45.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/straight_sidewalk.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     8607 2023-07-10 12:51:04.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/straight_way.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)    26410 2023-07-11 14:03:35.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/traffic_island.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)    22321 2023-07-11 17:00:32.000000 crossroads-schematization-0.2.9/crschem/model/__pycache__/turning_sidewalk.cpython-311.pyc
+-rw-r--r--   0 jm        (1000) jm        (1000)     6249 2023-07-10 12:50:45.000000 crossroads-schematization-0.2.9/crschem/model/branch.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    16105 2023-07-10 12:51:13.000000 crossroads-schematization-0.2.9/crschem/model/crossing.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     1573 2023-07-10 13:12:39.000000 crossroads-schematization-0.2.9/crschem/model/simple_way.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     1790 2023-07-11 09:15:36.000000 crossroads-schematization-0.2.9/crschem/model/straight_sidewalk.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     4123 2023-07-10 12:50:56.000000 crossroads-schematization-0.2.9/crschem/model/straight_way.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    13671 2023-07-11 14:03:31.000000 crossroads-schematization-0.2.9/crschem/model/traffic_island.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    12249 2023-07-11 17:00:29.000000 crossroads-schematization-0.2.9/crschem/model/turning_sidewalk.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7199 2023-07-11 08:33:31.000000 crossroads-schematization-0.2.9/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.339661 crossroads-schematization-0.2.9/crschem/resources/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.343661 crossroads-schematization-0.2.9/crschem/resources/400/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.9/crschem/resources/400/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.9/crschem/resources/400/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.9/crschem/resources/400/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.9/crschem/resources/400/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.9/crschem/resources/400/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.9/crschem/resources/400/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.9/crschem/resources/400/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.9/crschem/resources/400/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     4101 2023-07-10 14:48:21.000000 crossroads-schematization-0.2.9/crschem/resources/400/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     4100 2023-07-10 14:48:52.000000 crossroads-schematization-0.2.9/crschem/resources/400/style-96.xml
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-11 17:03:04.347661 crossroads-schematization-0.2.9/crschem/resources/500/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1941 2023-07-07 10:01:36.000000 crossroads-schematization-0.2.9/crschem/resources/500/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1932 2023-07-07 10:02:54.000000 crossroads-schematization-0.2.9/crschem/resources/500/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.9/crschem/resources/500/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1519 2023-07-07 10:06:34.000000 crossroads-schematization-0.2.9/crschem/resources/500/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.9/crschem/resources/500/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1516 2023-07-07 10:06:11.000000 crossroads-schematization-0.2.9/crschem/resources/500/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.9/crschem/resources/500/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.9/crschem/resources/500/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     4102 2023-07-10 14:49:05.000000 crossroads-schematization-0.2.9/crschem/resources/500/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     4101 2023-07-10 14:49:12.000000 crossroads-schematization-0.2.9/crschem/resources/500/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     8274 2023-07-11 09:20:13.000000 crossroads-schematization-0.2.9/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.9/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-11 17:03:04.347661 crossroads-schematization-0.2.9/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.9/setup.py
```

### Comparing `crossroads-schematization-0.2.8/PKG-INFO` & `crossroads-schematization-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.8
+Version: 0.2.9
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.8/README.md` & `crossroads-schematization-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.9/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.8
+Version: 0.2.9
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.8/crschem/cmd.py` & `crossroads-schematization-0.2.9/crschem/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 
 import argparse
 import geopandas
 import sys
 
 import crschem.crossroad_schematization as cs
+from crschem.model.turning_sidewalk import TurningSidewalk
 
 def get_crossroad_schematization_command():
 
 
     # a trick to avoid the creation of files given as parameters
     class FileOpener(argparse.FileType):
         # delayed FileType;
@@ -35,20 +36,21 @@
     group_input.add_argument('--overpass', help='Use Overpass to download data instead of the OSM api', action='store_true')
     group_input.add_argument('--ignore-cache', help='Ignore local cache', action='store_true')
 
     group_preprocess = parser.add_argument_group('Preprocessing', "Parameters of the preprocesses (crseg, crdesc)")
     group_preprocess.add_argument('--c0', help='Initial intersection size (distance between boundaries and middle of the initial intersection). Default: 2.', type=float, default=2)
     group_preprocess.add_argument('--c1', help='Intersection size (aggregation by adjacency). Default: 2.', type=float, default=2)
     group_preprocess.add_argument('--c2', help='Intersection size (aggregation by cycle detection). Default: 4.', type=float, default=4)
+    group_preprocess.add_argument('--similar-direction-angle', help='Maximum angle for lanes to be considered inside the same branch (in degree). Default: 60.', type=int, default=60)
 
     group_process = parser.add_argument_group("Processing", "Parameters of the processing")
     group_process.add_argument('--keep-doubled-crossings', help='In case of double crossings (current bad configuration in OSM data with traffic lights), keep both nodes.', action='store_true')
     group_process.add_argument('--ignore-crossings-for-sidewalks', help='Do not use crossings to shape the sidewalks', action='store_true')
     group_process.add_argument('--use-fixed-width-on-branches', help='Use a fixed width on each branch (do not evaluate the width adjustment)', action='store_true')
-    group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: c.TurningSidewalk.TurnShape[s], choices=list(c.TurningSidewalk.TurnShape))
+    group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: TurningSidewalk.TurnShape[s], choices=list(TurningSidewalk.TurnShape))
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
     group_output.add_argument('--display-preview', help='display a preview of the crossroad schematization', action='store_true')
     group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif, shp)', type=FileOpener('w'))
     group_output.add_argument('--scale', help='Scale of the map. Default: 400 (for 1:400)', type=int, default=400, choices=[400, 500])
@@ -74,14 +76,15 @@
             print("Loading input geojson (" + input_file + ")")
             crschem = cs.CrossroadSchematization(cr_input, G_init)
         else:
             latitude = args.by_coordinates[0]
             longitude = args.by_coordinates[1]
             crschem = cs.CrossroadSchematization.build(latitude, longitude,
                                                     args.c0, args.c1, args.c2,
+                                                    similar_direction_angle = args.similar_direction_angle,
                                                     verbose = True,
                                                     ignore_crossings_for_sidewalks = args.ignore_crossings_for_sidewalks,
                                                     use_fixed_width_on_branches = args.use_fixed_width_on_branches,
                                                     turn_shape = args.turn_shape,
                                                     remove_doubled_crossings = not args.keep_doubled_crossings,
                                                     ignore_cache = args.ignore_cache,
                                                     overpass = args.overpass,
```

### Comparing `crossroads-schematization-0.2.8/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.9/crschem/crossroad_schematization.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 import sys
 from osgeo import gdal, osr
 import tempfile
 from enum import Enum
 
 from . import utils as u
 from . import processing as p
-from . import crossroad as c
-
 
+from .model.branch import Branch
+from .model.traffic_island import TrafficIsland
+from .model.turning_sidewalk import TurningSidewalk
+from .model.simple_way import SimpleWay
+from .model.straight_way import StraightWay
+from .model.crossing import Crossing
 
 class CrossroadSchematization:
 
     class Layout(Enum):
         A5_portrait = 0
         A5_landscape = 1
         A4_portrait = 2
@@ -76,15 +80,15 @@
 
     # If the OSM data has been previously loaded, do not load it again
     def __init__(self, cr_input, 
                  osm_oriented = None,
                  osm_unoriented = None,
                  ignore_crossings_for_sidewalks = False,
                  use_fixed_width_on_branches = False,
-                 turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
+                 turn_shape = TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
                  remove_doubled_crossings = True,
                  osm_buffer_size_meters = 200, 
                  distance_kerb_footway = 0.5,
                  white_space_meter = 1.5):
         self.osm_buffer_size_meters = osm_buffer_size_meters
         self.distance_kerb_footway = distance_kerb_footway
         self.white_space_meter = white_space_meter
@@ -100,17 +104,18 @@
         is_n = cr_input["type"] == "crossroads"
         self.center = cr_input[is_n]["geometry"][0]
 
 
 
     def build(latitude, longitude,
               C0, C1, C2,
+              similar_direction_angle = 60,
               ignore_crossings_for_sidewalks = False,
               use_fixed_width_on_branches = False,
-              turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
+              turn_shape = TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
               remove_doubled_crossings = True,
               verbose = True,
               ignore_cache = False,
               overpass = False,
               log_files = False):
 
         import crseg.segmentation as cseg
@@ -132,15 +137,15 @@
             print("Segmenting intersection")
         # remove sidewalks, cycleways, service ways
         G = cseg.Segmentation.prepare_network(deepcopy(G_init))
         # build an undirected version of the graph
         undirected_G = ox.utils_graph.get_undirected(G)
         
         # segment it using topology and semantic
-        seg = cseg.Segmentation(undirected_G, C0 = C0, C1 = C1, C2 = C2, max_cycle_elements = 10)
+        seg = cseg.Segmentation(undirected_G, C0 = C0, C1 = C1, C2 = C2, max_cycle_elements = 10, similar_direction_angle = similar_direction_angle)
         seg.process()
 
         tmp1 = tempfile.NamedTemporaryFile(mode='w', delete=False)
         seg.to_json(tmp1.name, longitude, latitude)
         # convert it as a model (from https://gitlab.limos.fr/jeremyk6/crossroads-description)
         print("Converting graph as a model")
 
@@ -196,15 +201,15 @@
 
         # compute for each branch two long edges *S1* and *S2* corresponding to the sidewalks:
         print("Creating sidewalks")
         self.build_sidewalks()
 
         # add pedestrian crossings
         print("Creating crossings")
-        self.crossings = c.Crossing.create_crossings(self.osm_input, self.cr_input, 
+        self.crossings = Crossing.create_crossings(self.osm_input, self.cr_input, 
                                                      self.osm_input_oriented,
                                                      self.distance_kerb_footway,
                                                      self.remove_doubled_crossings)
 
         # assemble sidewalks
         print("Assembling sidewalks")
         self.assemble_sidewalks()
@@ -295,16 +300,16 @@
                 n1 = osm_n1 if self.is_boundary_node(osm_n1) else osm_n2
                 n2 = osm_n2 if n1 == osm_n1 else osm_n1
                 e = u.Utils.get_initial_edge_tags(self.cr_input, osm_n1, osm_n2)
                 if e is not None:
                     id = e["id"]
                     bname = e["name"]
                     if not id in self.branches:
-                        self.branches[id] = c.Branch(bname, id, self.osm_input, self.cr_input, self.distance_kerb_footway)
-                    self.branches[id].add_way(c.SimpleWay(n1, n2, e, osm_n1 == n1))
+                        self.branches[id] = Branch(bname, id, self.osm_input, self.cr_input, self.distance_kerb_footway)
+                    self.branches[id].add_way(SimpleWay(n1, n2, e, osm_n1 == n1))
 
 
     def build_sidewalks(self):
         self.sidewalks = {}
         
         for bid in self.branches:
             self.sidewalks[bid] = self.branches[bid].get_sidewalks(self.use_fixed_width_on_branches)
@@ -341,15 +346,15 @@
         original_sidewalks_ids = self.get_sidewalk_ids()
         self.merged_sidewalks = []
 
         # TODO: find crossings that should be part of the sidewalks and
         # integrate them to the final shape
 
         for sid in original_sidewalks_ids:
-            self.merged_sidewalks.append(c.TurningSidewalk(sid,
+            self.merged_sidewalks.append(TurningSidewalk(sid,
                                                             self.get_sidewalks_by_id(sid), 
                                                             self.get_crossings_by_sidewalks_ids(sid),
                                                             self.osm_input, self.cr_input, self.distance_kerb_footway,
                                                             self.ignore_crossings_for_sidewalks,
                                                             self.turn_shape))
 
 
@@ -394,15 +399,15 @@
                         if not id in traffic_islands_edges:
                             traffic_islands_edges[id] = []
                         traffic_islands_edges[id].append(";".join(elem["osm_node_ids"]))
         
         # then build traffic islands
         self.traffic_islands = []
         for eid in traffic_islands_edges:
-            self.traffic_islands.append(c.TrafficIsland(eid, traffic_islands_edges[eid], self.osm_input, self.cr_input, self.crossings))
+            self.traffic_islands.append(TrafficIsland(eid, traffic_islands_edges[eid], self.osm_input, self.cr_input, self.crossings, self.distance_kerb_footway))
 
 
     def getMapnikMap(self, dirName, resolution, scale, layout, marginCM):
         widthMeter = layout.width(marginCM / 100)
         heightMeter = layout.height(marginCM / 100)
 
         width = int(m2px(widthMeter, resolution))
@@ -546,45 +551,46 @@
     def toGDFInnerRegion(self):
         d = {'type': ['inner_region'], 'geometry': [self.inner_region]}
         return geopandas.GeoDataFrame(d, crs=2154)
 
     def toGDFOuterRegion(self):
         bbox = self.inner_region.bounds
         area = affinity.scale(box(*bbox), 1.1, 1.1)
-        outer = area.difference(self.inner_region)
+        outer = area.difference(self.inner_region.buffer(0))
 
         d = {'type': ['outer_region'], 'geometry': [outer]}
         return geopandas.GeoDataFrame(d, crs=2154)
 
 
     def toGeojson(self, filename, only_reachable_islands = False, crs = "EPSG:4326"):
         df = pandas.concat([self.toGDFInnerRegion().to_crs(crs),
-                            c.TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs),
-                            c.Branch.toGDFBranches(self.branches).to_crs(crs),
-                            c.TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs),
-                            c.Crossing.toGDFCrossings(self.crossings).to_crs(crs)])
+                            TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs),
+                            Branch.toGDFBranches(self.branches).to_crs(crs),
+                            TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs),
+                            Crossing.toGDFCrossings(self.crossings).to_crs(crs)])
         
         df.to_file(filename, driver='GeoJSON')
 
 
     def toShapefiles(self, filename, only_reachable_islands = False, crs = "EPSG:4326"):
         filename, file_extension = os.path.splitext(filename)
 
         self.toGDFInnerRegion().to_crs(crs).to_file(filename + "-inner" + file_extension) # region
         self.toGDFOuterRegion().to_crs(crs).to_file(filename + "-outer" + file_extension) # region
-        c.TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs).to_file(filename + "-sidewalks" + file_extension) # lines
-        c.Branch.toGDFBranches(self.branches).to_crs(crs).to_file(filename + "-branches" + file_extension) # lines
+        TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs).to_file(filename + "-sidewalks" + file_extension) # lines
+        Branch.toGDFBranches(self.branches).to_crs(crs).to_file(filename + "-branches" + file_extension) # lines
         
-        # islands can be points and lines
-        islands = c.TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs)
-        islands[islands.geometry.type == 'LineString'].to_file(filename + "-islands-lines" + file_extension)
+        # islands can be points, lines or polygons
+        islands = TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs)
         islands[islands.geometry.type == 'Point'].to_file(filename + "-islands-points" + file_extension)
+        islands[islands.geometry.type == 'LineString'].to_file(filename + "-islands-lines" + file_extension)
+        islands[islands.geometry.type == 'Polygon'].to_file(filename + "-islands-polygons" + file_extension)
 
         # points
-        c.Crossing.toGDFCrossings(self.crossings).to_crs(crs).to_file(filename + "-crossings" + file_extension)
+        Crossing.toGDFCrossings(self.crossings).to_crs(crs).to_file(filename + "-crossings" + file_extension)
 
 
     def show(self, 
              osm_graph = False,
              branches = False,
              simple_sidewalks = False,
              merged_sidewalks = True,
@@ -642,20 +648,23 @@
                 y = [e[1] for e in xy]
                 plt.plot(x, y, color = "black", linewidth=2)
                 plt.plot(x[1], y[1], "ok")
 
         if islands:
             for sw in self.traffic_islands:
                 if sw.is_reachable or not only_reachable_islands:
-                    if len(sw.extremities) == 0:
+                    if sw.generalization == TrafficIsland.Geometry.point:
                         x, y = sw.center
                         plt.plot(x, y, "ok", markersize=12, linewidth=12)
-                    else:
+                    elif sw.generalization == TrafficIsland.Geometry.lines:
                         for e in sw.extremities:
                             x = [sw.center[0], e[0]]
                             y = [sw.center[1], e[1]]
                             plt.plot(x, y, color="black", solid_capstyle='round', markersize=12, linewidth=12)
+                    elif sw.generalization == TrafficIsland.Geometry.polygon:
+                        x, y = sw.inner_polygon.exterior.xy
+                        plt.plot(x, y, color = "black", linewidth=1)
 
                     
 
 
         plt.show()
```

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-300.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-96.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/island-300-white.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/island-300.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/island-96-white.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/island-96.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/point-300.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/point-96.svg` & `crossroads-schematization-0.2.9/crschem/resources/400/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/style-300.xml` & `crossroads-schematization-0.2.9/crschem/resources/500/style-96.xml`

 * *Files 19% similar despite different names*

#### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/style-300.xml` & `crossroads-schematization-0.2.9/crschem/resources/500/style-96.xml`

```diff
@@ -1,52 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- 300 DPI correspond à 118,11 pixels par centimètre.
-  On va donc utiliser l'approximation: 1mm = 12 pixels
+<!-- 96 DPI correspond à 37,8 pixels par centimètre.
+  On va donc utiliser l'approximation: 1mm = 3,78 ~= 4 pixels
  -->
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
-      <PolygonPatternSymbolizer file="point-300.svg"/>
+      <PolygonPatternSymbolizer file="point-96.svg"/>
     </Rule>
   </Style>
   <Style name="outer">
     <Rule>
       <PolygonSymbolizer fill="#fff"/>
     </Rule>
   </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
-      <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
+      <LineSymbolizer stroke="#fff" stroke-width="16" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="sidewalks">
     <Rule>
-      <LineSymbolizer stroke="#000" stroke-width="12" stroke-linejoin="round" stroke-linecap="round"/>
+      <LineSymbolizer stroke="#000" stroke-width="4" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="islands-space">
     <Rule>
-      <LineSymbolizer stroke="#fff" stroke-width="144" stroke-linejoin="round" stroke-linecap="round"/>
-      <PointSymbolizer file="island-300-white.svg" allow-overlap="yes"/>
+      <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
+      <PointSymbolizer file="island-96-white.svg" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Style name="islands">
     <Rule>
-      <LineSymbolizer stroke="#000" stroke-width="96" stroke-linejoin="round" stroke-linecap="round"/>
-      <PointSymbolizer file="island-300.svg" allow-overlap="yes"/>
+      <LineSymbolizer stroke="#000" stroke-width="32" stroke-linejoin="round" stroke-linecap="round"/>
+      <PointSymbolizer file="island-96.svg" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Style name="crossings">
     <Rule>
       <Filter>[type] = crossing</Filter>
       <!-- TODO: add images for streets with a different width -->
       <!-- 3 meter street -->
-      <PointSymbolizer file="crossing-3-300.svg" transform="rotate(180 + (-[orientatio] / 3.14) * 180)" allow-overlap="yes"/>
+      <PointSymbolizer file="crossing-3-96.svg" transform="rotate(180 + (-[orientatio] / 3.14) * 180)" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Layer>
     <StyleName>inner</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-inner.shp</Parameter>
       <Parameter name="type">shape</Parameter>
@@ -70,35 +70,56 @@
     <StyleName>sidewalks-space</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks-space</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
     <StyleName>outer</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-outer.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>islands</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-islands-lines.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/style-96.xml` & `crossroads-schematization-0.2.9/crschem/resources/400/style-96.xml`

 * *Files 18% similar despite different names*

#### Comparing `crossroads-schematization-0.2.8/crschem/resources/400/style-96.xml` & `crossroads-schematization-0.2.9/crschem/resources/400/style-96.xml`

```diff
@@ -70,35 +70,56 @@
     <StyleName>sidewalks-space</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks-space</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
     <StyleName>outer</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-outer.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>islands</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-islands-lines.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-300.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-96.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/island-300-white.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/island-300.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/island-96-white.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/island-96.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/point-300.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/point-96.svg` & `crossroads-schematization-0.2.9/crschem/resources/500/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/style-300.xml` & `crossroads-schematization-0.2.9/crschem/resources/400/style-300.xml`

 * *Files 22% similar despite different names*

#### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/style-300.xml` & `crossroads-schematization-0.2.9/crschem/resources/400/style-300.xml`

```diff
@@ -70,35 +70,56 @@
     <StyleName>sidewalks-space</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks-space</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
     <StyleName>outer</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-outer.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>islands</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-islands-lines.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/style-96.xml` & `crossroads-schematization-0.2.9/crschem/resources/500/style-300.xml`

 * *Files 22% similar despite different names*

#### Comparing `crossroads-schematization-0.2.8/crschem/resources/500/style-96.xml` & `crossroads-schematization-0.2.9/crschem/resources/500/style-300.xml`

```diff
@@ -1,52 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- 96 DPI correspond à 37,8 pixels par centimètre.
-  On va donc utiliser l'approximation: 1mm = 3,78 ~= 4 pixels
+<!-- 300 DPI correspond à 118,11 pixels par centimètre.
+  On va donc utiliser l'approximation: 1mm = 12 pixels
  -->
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
-      <PolygonPatternSymbolizer file="point-96.svg"/>
+      <PolygonPatternSymbolizer file="point-300.svg"/>
     </Rule>
   </Style>
   <Style name="outer">
     <Rule>
       <PolygonSymbolizer fill="#fff"/>
     </Rule>
   </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
-      <LineSymbolizer stroke="#fff" stroke-width="16" stroke-linejoin="round" stroke-linecap="round"/>
+      <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="sidewalks">
     <Rule>
-      <LineSymbolizer stroke="#000" stroke-width="4" stroke-linejoin="round" stroke-linecap="round"/>
+      <LineSymbolizer stroke="#000" stroke-width="12" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="islands-space">
     <Rule>
-      <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
-      <PointSymbolizer file="island-96-white.svg" allow-overlap="yes"/>
+      <LineSymbolizer stroke="#fff" stroke-width="144" stroke-linejoin="round" stroke-linecap="round"/>
+      <PointSymbolizer file="island-300-white.svg" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Style name="islands">
     <Rule>
-      <LineSymbolizer stroke="#000" stroke-width="32" stroke-linejoin="round" stroke-linecap="round"/>
-      <PointSymbolizer file="island-96.svg" allow-overlap="yes"/>
+      <LineSymbolizer stroke="#000" stroke-width="96" stroke-linejoin="round" stroke-linecap="round"/>
+      <PointSymbolizer file="island-300.svg" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Style name="crossings">
     <Rule>
       <Filter>[type] = crossing</Filter>
       <!-- TODO: add images for streets with a different width -->
       <!-- 3 meter street -->
-      <PointSymbolizer file="crossing-3-96.svg" transform="rotate(180 + (-[orientatio] / 3.14) * 180)" allow-overlap="yes"/>
+      <PointSymbolizer file="crossing-3-300.svg" transform="rotate(180 + (-[orientatio] / 3.14) * 180)" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Layer>
     <StyleName>inner</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-inner.shp</Parameter>
       <Parameter name="type">shape</Parameter>
@@ -70,35 +70,56 @@
     <StyleName>sidewalks-space</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks-space</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
     <StyleName>outer</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-outer.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>sidewalks</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-islands-polygons.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>islands</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-islands-lines.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.8/crschem/utils.py` & `crossroads-schematization-0.2.9/crschem/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,7 +246,19 @@
 
 
     def pathid_to_pathcoords(path, osm):
         return [(osm.nodes[n]["x"], osm.nodes[n]["y"]) for n in path]
     
     def edge_in_osm(n1, n2, osm):
         return n1 in osm and n2 in osm[n1]
+
+    def extends_edge(coords, length = 200):
+        edgecoords = np.asarray(coords)
+        x = [a[0] for a in edgecoords]
+        y = [a[1] for a in edgecoords]
+        center = Point(sum(x) / len(x), sum(y) / len(y))
+        start = edgecoords[0]
+        end = edgecoords[1]
+        v = [center.x - start[0], center.y - start[1]]
+        v = v / linalg.norm(v)
+        return LineString([start - v * length, end + v * length])
+
```

### Comparing `crossroads-schematization-0.2.8/setup.py` & `crossroads-schematization-0.2.9/setup.py`

 * *Files identical despite different names*

