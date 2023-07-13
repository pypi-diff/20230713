# Comparing `tmp/ShapeYModular-2.0.1.tar.gz` & `tmp/ShapeYModular-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShapeYModular-2.0.1.tar", last modified: Wed Jun 21 20:54:35 2023, max compression
+gzip compressed data, was "ShapeYModular-2.0.2.tar", last modified: Thu Jul 13 14:36:46 2023, max compression
```

## Comparing `ShapeYModular-2.0.1.tar` & `ShapeYModular-2.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1062 2023-06-21 20:35:32.000000 ShapeYModular-2.0.1/LICENSE
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2018 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/PKG-INFO
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1595 2023-06-21 20:54:22.000000 ShapeYModular-2.0.1/README.md
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.183731 ShapeYModular-2.0.1/ShapeYModular.egg-info/
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2018 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/PKG-INFO
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1556 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/SOURCES.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/dependency_links.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)      151 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/requires.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)       14 2023-06-21 20:54:35.000000 ShapeYModular-2.0.1/ShapeYModular.egg-info/top_level.txt
--rw-r--r--   0 namj      (1007) dcuser    (1001)       38 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/setup.cfg
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1144 2023-06-21 20:54:29.000000 ShapeYModular-2.0.1/setup.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/
--rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-05-23 22:20:02.000000 ShapeYModular-2.0.1/shapeymodular/__init__.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/analysis/
--rw-r--r--   0 namj      (1007) dcuser    (1001)       80 2023-06-09 17:43:22.000000 ShapeYModular-2.0.1/shapeymodular/analysis/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    26181 2023-06-13 18:09:42.000000 ShapeYModular-2.0.1/shapeymodular/analysis/nn_analysis.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    41776 2023-06-21 17:19:46.000000 ShapeYModular-2.0.1/shapeymodular/analysis/postprocess.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      723 2023-06-05 17:13:26.000000 ShapeYModular-2.0.1/shapeymodular/analysis/preprocess.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/data_classes/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      116 2023-06-06 15:58:15.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4190 2023-05-26 18:10:32.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/axis_description.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1840 2023-05-26 18:09:35.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/corrmat.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4573 2023-06-20 00:51:00.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/graph_data.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1630 2023-05-26 18:20:11.000000 ShapeYModular-2.0.1/shapeymodular/data_classes/nn_analysis_configs.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/data_loader/
--rw-r--r--   0 namj      (1007) dcuser    (1001)       69 2023-05-26 18:05:58.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      976 2023-06-02 17:07:40.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/data_loader.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4804 2023-05-26 18:11:03.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/dir_mat.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     7236 2023-06-06 18:12:07.000000 ShapeYModular-2.0.1/shapeymodular/data_loader/hdf.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/macros/
--rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-25 19:17:00.000000 ShapeYModular-2.0.1/shapeymodular/macros/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1615 2023-06-19 23:27:33.000000 ShapeYModular-2.0.1/shapeymodular/macros/compute_distance.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2307 2023-05-26 17:31:55.000000 ShapeYModular-2.0.1/shapeymodular/macros/compute_threshold.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    14772 2023-06-21 20:07:14.000000 ShapeYModular-2.0.1/shapeymodular/macros/graphing.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     9393 2023-06-21 19:56:24.000000 ShapeYModular-2.0.1/shapeymodular/macros/nn_batch.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/test/
--rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-23 22:19:39.000000 ShapeYModular-2.0.1/shapeymodular/test/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      230 2023-06-08 19:49:41.000000 ShapeYModular-2.0.1/shapeymodular/test/conftest.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.187731 ShapeYModular-2.0.1/shapeymodular/utils/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      113 2023-06-07 19:38:27.000000 ShapeYModular-2.0.1/shapeymodular/utils/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)      501 2023-05-25 21:00:16.000000 ShapeYModular-2.0.1/shapeymodular/utils/cmdtools.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2735 2023-06-21 19:30:05.000000 ShapeYModular-2.0.1/shapeymodular/utils/constants.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     3443 2023-06-13 15:27:47.000000 ShapeYModular-2.0.1/shapeymodular/utils/image_name_helper.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     3407 2023-06-09 19:12:08.000000 ShapeYModular-2.0.1/shapeymodular/utils/indexing_helper.py
-drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-06-21 20:54:35.191731 ShapeYModular-2.0.1/shapeymodular/visualization/
--rw-r--r--   0 namj      (1007) dcuser    (1001)      130 2023-06-20 20:45:00.000000 ShapeYModular-2.0.1/shapeymodular/visualization/__init__.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     5456 2023-05-26 16:58:09.000000 ShapeYModular-2.0.1/shapeymodular/visualization/correlation_fall_off.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1385 2023-06-20 18:39:52.000000 ShapeYModular-2.0.1/shapeymodular/visualization/exclusion_distance.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2987 2023-06-20 16:43:06.000000 ShapeYModular-2.0.1/shapeymodular/visualization/histogram.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     4167 2023-06-21 20:42:03.000000 ShapeYModular-2.0.1/shapeymodular/visualization/image.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)    38608 2023-05-26 16:58:09.000000 ShapeYModular-2.0.1/shapeymodular/visualization/image_panel.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     2843 2023-06-20 16:41:54.000000 ShapeYModular-2.0.1/shapeymodular/visualization/line_graph.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1076 2023-06-21 20:49:59.000000 ShapeYModular-2.0.1/shapeymodular/visualization/styles.py
--rw-r--r--   0 namj      (1007) dcuser    (1001)     1226 2023-06-20 18:51:46.000000 ShapeYModular-2.0.1/shapeymodular/visualization/tuning_curve.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.677389 ShapeYModular-2.0.2/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1062 2023-06-21 20:35:32.000000 ShapeYModular-2.0.2/LICENSE
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2018 2023-07-13 14:36:46.677389 ShapeYModular-2.0.2/PKG-INFO
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1595 2023-06-21 20:54:22.000000 ShapeYModular-2.0.2/README.md
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/ShapeYModular.egg-info/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2018 2023-07-13 14:36:46.000000 ShapeYModular-2.0.2/ShapeYModular.egg-info/PKG-INFO
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1550 2023-07-13 14:36:46.000000 ShapeYModular-2.0.2/ShapeYModular.egg-info/SOURCES.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-07-13 14:36:46.000000 ShapeYModular-2.0.2/ShapeYModular.egg-info/dependency_links.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      151 2023-07-13 14:36:46.000000 ShapeYModular-2.0.2/ShapeYModular.egg-info/requires.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       14 2023-07-13 14:36:46.000000 ShapeYModular-2.0.2/ShapeYModular.egg-info/top_level.txt
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       38 2023-07-13 14:36:46.677389 ShapeYModular-2.0.2/setup.cfg
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1144 2023-07-13 14:36:06.000000 ShapeYModular-2.0.2/setup.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/shapeymodular/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        1 2023-05-23 22:20:02.000000 ShapeYModular-2.0.2/shapeymodular/__init__.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/shapeymodular/analysis/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       80 2023-06-09 17:43:22.000000 ShapeYModular-2.0.2/shapeymodular/analysis/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    26181 2023-06-13 18:09:42.000000 ShapeYModular-2.0.2/shapeymodular/analysis/nn_analysis.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    34377 2023-07-11 14:54:12.000000 ShapeYModular-2.0.2/shapeymodular/analysis/postprocess.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      672 2023-07-11 14:44:36.000000 ShapeYModular-2.0.2/shapeymodular/analysis/preprocess.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/shapeymodular/data_classes/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      116 2023-06-06 15:58:15.000000 ShapeYModular-2.0.2/shapeymodular/data_classes/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4190 2023-05-26 18:10:32.000000 ShapeYModular-2.0.2/shapeymodular/data_classes/axis_description.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1840 2023-05-26 18:09:35.000000 ShapeYModular-2.0.2/shapeymodular/data_classes/corrmat.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4573 2023-06-20 00:51:00.000000 ShapeYModular-2.0.2/shapeymodular/data_classes/graph_data.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1630 2023-05-26 18:20:11.000000 ShapeYModular-2.0.2/shapeymodular/data_classes/nn_analysis_configs.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/shapeymodular/data_loader/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)       92 2023-06-29 17:53:35.000000 ShapeYModular-2.0.2/shapeymodular/data_loader/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      976 2023-06-02 17:07:40.000000 ShapeYModular-2.0.2/shapeymodular/data_loader/data_loader.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4917 2023-06-22 14:29:11.000000 ShapeYModular-2.0.2/shapeymodular/data_loader/dir_mat.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     7236 2023-06-06 18:12:07.000000 ShapeYModular-2.0.2/shapeymodular/data_loader/hdf.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1913 2023-06-30 14:57:09.000000 ShapeYModular-2.0.2/shapeymodular/data_loader/sampler.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/shapeymodular/macros/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-25 19:17:00.000000 ShapeYModular-2.0.2/shapeymodular/macros/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1736 2023-07-11 16:10:37.000000 ShapeYModular-2.0.2/shapeymodular/macros/compute_distance.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2496 2023-06-27 15:25:59.000000 ShapeYModular-2.0.2/shapeymodular/macros/compute_threshold.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)    16723 2023-06-30 15:48:23.000000 ShapeYModular-2.0.2/shapeymodular/macros/graphing.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     9393 2023-06-21 19:56:24.000000 ShapeYModular-2.0.2/shapeymodular/macros/nn_batch.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.673389 ShapeYModular-2.0.2/shapeymodular/test/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)        0 2023-05-23 22:19:39.000000 ShapeYModular-2.0.2/shapeymodular/test/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      230 2023-06-08 19:49:41.000000 ShapeYModular-2.0.2/shapeymodular/test/conftest.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.677389 ShapeYModular-2.0.2/shapeymodular/utils/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      113 2023-06-07 19:38:27.000000 ShapeYModular-2.0.2/shapeymodular/utils/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      501 2023-05-25 21:00:16.000000 ShapeYModular-2.0.2/shapeymodular/utils/cmdtools.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2901 2023-07-11 15:29:13.000000 ShapeYModular-2.0.2/shapeymodular/utils/constants.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     4128 2023-06-27 20:02:35.000000 ShapeYModular-2.0.2/shapeymodular/utils/image_name_helper.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     3407 2023-06-09 19:12:08.000000 ShapeYModular-2.0.2/shapeymodular/utils/indexing_helper.py
+drwxr-xr-x   0 namj      (1007) dcuser    (1001)        0 2023-07-13 14:36:46.677389 ShapeYModular-2.0.2/shapeymodular/visualization/
+-rw-r--r--   0 namj      (1007) dcuser    (1001)      130 2023-06-20 20:45:00.000000 ShapeYModular-2.0.2/shapeymodular/visualization/__init__.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     5456 2023-05-26 16:58:09.000000 ShapeYModular-2.0.2/shapeymodular/visualization/correlation_fall_off.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1385 2023-06-20 18:39:52.000000 ShapeYModular-2.0.2/shapeymodular/visualization/exclusion_distance.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2987 2023-06-20 16:43:06.000000 ShapeYModular-2.0.2/shapeymodular/visualization/histogram.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     5524 2023-07-11 00:53:37.000000 ShapeYModular-2.0.2/shapeymodular/visualization/image.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     2843 2023-06-20 16:41:54.000000 ShapeYModular-2.0.2/shapeymodular/visualization/line_graph.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1211 2023-07-10 17:59:50.000000 ShapeYModular-2.0.2/shapeymodular/visualization/styles.py
+-rw-r--r--   0 namj      (1007) dcuser    (1001)     1226 2023-06-20 18:51:46.000000 ShapeYModular-2.0.2/shapeymodular/visualization/tuning_curve.py
```

### Comparing `ShapeYModular-2.0.1/LICENSE` & `ShapeYModular-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/PKG-INFO` & `ShapeYModular-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShapeYModular
-Version: 2.0.1
+Version: 2.0.2
 Summary: Benchmark that tests shape recognition
 Home-page: https://github.com/njw0709/ShapeYV2
 Author: Jong Woo Nam
 Author-email: namj@usc.edu
 License: MIT
 Keywords: tests shape recognition capacity
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ShapeYModular-2.0.1/README.md` & `ShapeYModular-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/ShapeYModular.egg-info/PKG-INFO` & `ShapeYModular-2.0.2/ShapeYModular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShapeYModular
-Version: 2.0.1
+Version: 2.0.2
 Summary: Benchmark that tests shape recognition
 Home-page: https://github.com/njw0709/ShapeYV2
 Author: Jong Woo Nam
 Author-email: namj@usc.edu
 License: MIT
 Keywords: tests shape recognition capacity
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ShapeYModular-2.0.1/ShapeYModular.egg-info/SOURCES.txt` & `ShapeYModular-2.0.2/ShapeYModular.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 shapeymodular/data_classes/corrmat.py
 shapeymodular/data_classes/graph_data.py
 shapeymodular/data_classes/nn_analysis_configs.py
 shapeymodular/data_loader/__init__.py
 shapeymodular/data_loader/data_loader.py
 shapeymodular/data_loader/dir_mat.py
 shapeymodular/data_loader/hdf.py
+shapeymodular/data_loader/sampler.py
 shapeymodular/macros/__init__.py
 shapeymodular/macros/compute_distance.py
 shapeymodular/macros/compute_threshold.py
 shapeymodular/macros/graphing.py
 shapeymodular/macros/nn_batch.py
 shapeymodular/test/__init__.py
 shapeymodular/test/conftest.py
@@ -33,11 +34,10 @@
 shapeymodular/utils/image_name_helper.py
 shapeymodular/utils/indexing_helper.py
 shapeymodular/visualization/__init__.py
 shapeymodular/visualization/correlation_fall_off.py
 shapeymodular/visualization/exclusion_distance.py
 shapeymodular/visualization/histogram.py
 shapeymodular/visualization/image.py
-shapeymodular/visualization/image_panel.py
 shapeymodular/visualization/line_graph.py
 shapeymodular/visualization/styles.py
 shapeymodular/visualization/tuning_curve.py
```

### Comparing `ShapeYModular-2.0.1/setup.py` & `ShapeYModular-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Development Status :: 4 - Beta",
 ]
 
 # calling the setup function
 # TODO: separate dev / test / deploy setup with options
 setuptools.setup(
     name="ShapeYModular",
-    version="2.0.1",
+    version="2.0.2",
     description="Benchmark that tests shape recognition",
     long_description=long_description,
     url="https://github.com/njw0709/ShapeYV2",
     author="Jong Woo Nam",
     author_email="namj@usc.edu",
     license="MIT",
     packages=setuptools.find_packages(),
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/analysis/nn_analysis.py` & `ShapeYModular-2.0.2/shapeymodular/analysis/nn_analysis.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/analysis/preprocess.py` & `ShapeYModular-2.0.2/shapeymodular/analysis/preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,11 +16,7 @@
 
     cdf = np.cumsum(histcounts, axis=1)
     total_count = np.take(cdf, -1, axis=1)
     norm_cdf = cdf / np.expand_dims(total_count, axis=1)
     threshold_idx = np.argmax(norm_cdf > activation_level, axis=1)
     threshold = bins_array[np.arange(bins_array.shape[0]), threshold_idx]
     return threshold
-
-
-def convert_nan_dist_to_zero() -> None:
-    pass
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_classes/axis_description.py` & `ShapeYModular-2.0.2/shapeymodular/data_classes/axis_description.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_classes/corrmat.py` & `ShapeYModular-2.0.2/shapeymodular/data_classes/corrmat.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_classes/graph_data.py` & `ShapeYModular-2.0.2/shapeymodular/data_classes/graph_data.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_classes/nn_analysis_configs.py` & `ShapeYModular-2.0.2/shapeymodular/data_classes/nn_analysis_configs.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_loader/data_loader.py` & `ShapeYModular-2.0.2/shapeymodular/data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_loader/dir_mat.py` & `ShapeYModular-2.0.2/shapeymodular/data_loader/dir_mat.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     def load(
         data_path: str, file_name: str, filter_key: Union[None, str] = None
     ) -> Sequence[np.ndarray]:
         with h5py.File(os.path.join(data_path, file_name), "r") as f:
             keys = list(f.keys())
             if filter_key is not None:
                 keys = [k for k in keys if filter_key in k]
+                if len(keys) == 0:
+                    raise KeyError("No key found with filter: " + filter_key)
             data = []
             for k in keys:
                 if isinstance(f[k], h5py.Dataset):
                     dataset = typing.cast(h5py.Dataset, f[k])
                     data.append(dataset[:])
                 else:
                     warnings.warn(
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/data_loader/hdf.py` & `ShapeYModular-2.0.2/shapeymodular/data_loader/hdf.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/macros/compute_distance.py` & `ShapeYModular-2.0.2/shapeymodular/macros/compute_distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,31 +8,32 @@
     os.chdir(dirname)
     cwd = os.getcwd()
 
     # Print the current working directory
     print("Current working directory: {0}".format(cwd))
 
     if os.path.exists(os.path.join(dirname, "thresholds.mat")):
-        with open("config.json") as f:
+        with open("config.json", "r") as f:
             config = json.load(f)
         assert config["featuresThresholdsFileName"] == os.path.join(
             dirname, "thresholds.mat"
         )
     else:
         raise FileNotFoundError("thresholds.mat not found")
 
     # copy imgname files
-    cmd = ["cp", utils.PATH_IMGLIST_ALL, "."]
+    print("copying features list")
+    cmd = ["cp", utils.PATH_FEATURELIST_ALL, "./imgnames_all.txt"]
     utils.execute_and_print(cmd)
-    cmd = ["cp", utils.PATH_IMGLIST_PW, "."]
+    cmd = ["cp", utils.PATH_FEATURELIST_PW, "./imgnames_pw_series.txt"]
     utils.execute_and_print(cmd)
     print("Done preparing for distance computation")
 
 
-def compute_distance(dirname: str) -> None:
+def compute_distance(dirname: str, gpunum: int = 0) -> None:
     # change working directory
     os.chdir(dirname)
     cwd = os.getcwd()
 
     # Print the current working directory
     print("Current working directory: {0}".format(cwd))
     # compute distances
@@ -40,15 +41,15 @@
     cmd = [
         "/home/dcuser/bin/imagepop_lsh",
         "-s",
         "256x256",
         "-f",
         "imgnames_all.txt",
         "-g",
-        "0",
+        "{}".format(gpunum),
         "--distance-name",
         "Jaccard",
         "--pairwise-dist-in",
         "imgnames_pw_series.txt",
         "--normalizer-name",
         "Threshold",
         "--pairwise-dist-out",
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/macros/compute_threshold.py` & `ShapeYModular-2.0.2/shapeymodular/macros/compute_threshold.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,22 +21,27 @@
     if dtype is None:
         dtype = np.uint32
     if save_dir is None:
         save_dir = features_directory
     if file_name is None:
         file_name = "thresholds.mat"
     save_file_name = os.path.join(save_dir, file_name)
+    # check if save file exists
+    if os.path.isfile(save_file_name):
+        os.rename(save_file_name, os.path.join(save_dir, "old_" + file_name))
     all_exists, feature_files = data_loader.check_all_feature_file_exists(
         features_directory
     )
     assert all_exists
     # randomly select 5000 from feature files (out of 68500)
     subsampled_feature_files = random.sample(feature_files, sample_size)
     # check dimensions of a file
-    data = data_loader.load(features_directory, subsampled_feature_files[0])
+    data = data_loader.load(
+        features_directory, subsampled_feature_files[0], filter_key=variable_name
+    )
     shape = data[0].shape
 
     # accumulate the subsampled features
     accumulators = [[]] * len(data)
     for feature_file in tqdm(subsampled_feature_files):
         data = data_loader.load(
             features_directory, feature_file, filter_key=variable_name
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/macros/graphing.py` & `ShapeYModular-2.0.2/shapeymodular/macros/graphing.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,27 +28,28 @@
     utils.execute_and_print(cmd)
     config = dc.load_config(
         os.path.join(feature_directory, "analysis_config_pw_no_cr.json")
     )
 
     analysis_hdf_path = os.path.join(feature_directory, "analysis_results.h5")
     analysis_hdf = h5py.File(analysis_hdf_path, "r")
+    analysis_sampler = dl.Sampler(data_loader, analysis_hdf, config)
     axes = typing.cast(List, config.axes)
     dict_ax_to_graph_data_group_obj = {}
     dict_ax_to_graph_data_group_cat = {}
     for ax in axes:
         # post process data for graphing
         graph_data_list_obj_error = []
         graph_data_list_cat_error = []
         for obj in tqdm(utils.SHAPEY200_OBJS):
             graph_data_obj = an.NNClassificationError.generate_top1_error_data(
-                data_loader, analysis_hdf, obj, ax, config
+                analysis_sampler, obj, ax
             )
             graph_data_cat = an.NNClassificationError.generate_top1_error_data(
-                data_loader, analysis_hdf, obj, ax, config, within_category_error=True
+                analysis_sampler, obj, ax, within_category_error=True
             )
             graph_data_list_obj_error.append(graph_data_obj)
             graph_data_list_cat_error.append(graph_data_cat)
         graph_data_group_obj_error = dc.GraphDataGroup(graph_data_list_obj_error)
         graph_data_group_cat_error = dc.GraphDataGroup(graph_data_list_cat_error)
         print("computing statistics...")
         graph_data_group_obj_error.compute_statistics()
@@ -103,52 +104,47 @@
     utils.execute_and_print(cmd)
     config = dc.load_config(
         os.path.join(feature_directory, "analysis_config_pw_no_cr.json")
     )
 
     analysis_hdf_path = os.path.join(feature_directory, "analysis_results.h5")
     analysis_hdf = h5py.File(analysis_hdf_path, "r")
+    analysis_sampler = dl.Sampler(data_loader, analysis_hdf, config)
     axes = typing.cast(List, config.axes)
 
     for ax in axes:
         # sampled one object per category
         for obj in tqdm(utils.SHAPEY200_SAMPLED_OBJS):
             # Load necessary data
             (
                 histogram_xdist_obj,
                 histogram_otherobj_obj,
             ) = an.DistanceHistogram.gather_histogram_data(
-                data_loader,
-                analysis_hdf,
+                analysis_sampler,
                 obj,
                 ax,
-                config,
                 within_category_error=False,
             )
 
             (
                 histogram_xdist_obj,
                 histogram_otherobj_obj,
             ) = an.DistanceHistogram.gather_histogram_data(
-                data_loader,
-                analysis_hdf,
+                analysis_sampler,
                 obj,
                 ax,
-                config,
                 within_category_error=True,
             )
             graph_data_obj = an.NNClassificationError.generate_top1_error_data(
-                data_loader, analysis_hdf, obj, ax, config
+                analysis_sampler, obj, ax
             )
             graph_data_cat = an.NNClassificationError.generate_top1_error_data(
-                data_loader,
-                analysis_hdf,
+                analysis_sampler,
                 obj,
                 ax,
-                config,
                 within_category_error=True,
             )
 
             fig_obj, ax_obj = plt.subplots(1, 1)
             ax2_obj = ax_obj.twinx()
             fig_cat, ax_cat = plt.subplots(1, 1)
             ax2_cat = ax_cat.twinx()
@@ -210,15 +206,14 @@
                 bbox_inches="tight",
             )
             plt.close(fig_obj)
             plt.close(fig_cat)
 
 
 def plot_error_panels(feature_directory: str) -> None:
-    data_loader = dl.HDFProcessor()
     # create figure directory
     FIG_SAVE_DIR = os.path.join(feature_directory, "figures")
     if not os.path.exists(FIG_SAVE_DIR):
         os.makedirs(FIG_SAVE_DIR)
 
     os.chdir(feature_directory)
     cwd = os.getcwd()
@@ -227,115 +222,162 @@
 
     # copy config file to feature directory
     cmd = ["cp", utils.PATH_CONFIG_PW_NO_CR, "."]
     utils.execute_and_print(cmd)
     config = dc.load_config(
         os.path.join(feature_directory, "analysis_config_pw_no_cr.json")
     )
-
     analysis_hdf_path = os.path.join(feature_directory, "analysis_results.h5")
-    analysis_hdf = h5py.File(analysis_hdf_path, "r")
     axes = typing.cast(List, config.axes)
+    distance_mat_file = os.path.join(feature_directory, "distances-Jaccard.mat")
+    input_data_descriptions = (
+        os.path.join(feature_directory, "imgnames_pw_series.txt"),
+        os.path.join(feature_directory, "imgnames_all.txt"),
+    )
+    data_loader = dl.HDFProcessor()
+    feature_data_loader = dl.FeatureDirMatProcessor()
 
+    # load threshold
+    if os.path.exists(os.path.join(feature_directory, "old_thresholds.mat")):
+        threshold = feature_data_loader.load(feature_directory, "old_thresholds.mat")
+    else:
+        threshold = feature_data_loader.load(feature_directory, "thresholds.mat")
+    if len(threshold) > 3:
+        threshold = threshold[:3]
+    threshold = [*threshold]
     for ax in axes:
         # sampled one object per category
         for obj in tqdm(utils.SHAPEY200_SAMPLED_OBJS):
-            # Load necessary data
-            (
-                incorrect_example_ref_img_shapey_idxs,
-                (
-                    incorrect_example_best_positive_match_shapey_idxs,
-                    incorrect_example_best_positive_match_dists,
-                ),
-                _,
-                (all_candidates_sorted_idxs, all_candidates_sorted_dists),
-            ) = an.ErrorDisplay.get_list_of_errors_single_obj(
-                data_loader,
-                analysis_hdf,
-                obj,
-                ax,
-                utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
-                config,
-                within_category_error=False,
-            )
-
-            graph_data_row_list_obj = an.ErrorDisplay.error_examples_to_graph_data_list(
-                incorrect_example_ref_img_shapey_idxs,
-                incorrect_example_best_positive_match_shapey_idxs,
-                incorrect_example_best_positive_match_dists,
-                all_candidates_sorted_idxs,
-                all_candidates_sorted_dists,
-                within_category_error=False,
-            )
+            # add reference image
+            graph_data_row_list_cat = an.ErrorDisplay.add_reference_images(obj, ax)
+            graph_data_row_list_obj = an.ErrorDisplay.add_reference_images(obj, ax)
+            with h5py.File(analysis_hdf_path, "r") as analysis_hdf:
+                analysis_sampler = dl.Sampler(data_loader, analysis_hdf, config)
+                # add all candidates sorted (top1 per object)
+                graph_data_row_list_cat = (
+                    an.ErrorDisplay.add_all_candidates_top_per_obj(
+                        graph_data_row_list_cat,
+                        analysis_sampler,
+                        obj,
+                        ax,
+                        utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
+                        within_category_error=True,
+                    )
+                )
+                graph_data_row_list_obj = (
+                    an.ErrorDisplay.add_all_candidates_top_per_obj(
+                        graph_data_row_list_obj,
+                        analysis_sampler,
+                        obj,
+                        ax,
+                        utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
+                        within_category_error=False,
+                    )
+                )
 
-            (
-                incorrect_example_ref_img_shapey_idxs,
-                (
-                    incorrect_example_best_positive_match_shapey_idxs,
-                    incorrect_example_best_positive_match_dists,
-                ),
-                _,
-                (all_candidates_sorted_idxs, all_candidates_sorted_dists),
-            ) = an.ErrorDisplay.get_list_of_errors_single_obj(
-                data_loader,
-                analysis_hdf,
-                obj,
-                ax,
-                utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
-                config,
-                within_category_error=True,
+                # add top1 positive match
+                graph_data_row_list_cat = (
+                    an.ErrorDisplay.add_top_positive_match_candidate(
+                        graph_data_row_list_cat,
+                        analysis_sampler,
+                        obj,
+                        ax,
+                        utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
+                        within_category_error=True,
+                    )
+                )
+                graph_data_row_list_obj = (
+                    an.ErrorDisplay.add_top_positive_match_candidate(
+                        graph_data_row_list_obj,
+                        analysis_sampler,
+                        obj,
+                        ax,
+                        utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
+                        within_category_error=False,
+                    )
+                )
+            with h5py.File(distance_mat_file, "r") as distances:
+                same_obj_corrmat_sampler = dl.CorrMatSampler(
+                    data_loader, distances, input_data_descriptions, config
+                )
+                # add closest physical image
+                graph_data_row_list_cat = an.ErrorDisplay.add_closest_physical_image(
+                    graph_data_row_list_cat,
+                    same_obj_corrmat_sampler,
+                    obj,
+                    ax,
+                    utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
+                )
+                graph_data_row_list_obj = an.ErrorDisplay.add_closest_physical_image(
+                    graph_data_row_list_obj,
+                    same_obj_corrmat_sampler,
+                    obj,
+                    ax,
+                    utils.XRADIUS_TO_PLOT_ERR_PANEL + 1,
+                )
+            # add feature activation levels
+            graph_data_row_list_cat = (
+                an.ErrorDisplay.add_feature_activation_level_annotation(
+                    graph_data_row_list_cat,
+                    feature_data_loader,
+                    feature_directory,
+                    threshold,
+                )
             )
-
-            graph_data_row_list_cat = an.ErrorDisplay.error_examples_to_graph_data_list(
-                incorrect_example_ref_img_shapey_idxs,
-                incorrect_example_best_positive_match_shapey_idxs,
-                incorrect_example_best_positive_match_dists,
-                all_candidates_sorted_idxs,
-                all_candidates_sorted_dists,
-                within_category_error=True,
+            graph_data_row_list_obj = (
+                an.ErrorDisplay.add_feature_activation_level_annotation(
+                    graph_data_row_list_obj,
+                    feature_data_loader,
+                    feature_directory,
+                    threshold,
+                )
             )
 
             # plot error panel
             num_rows = len(graph_data_row_list_obj)
-            if num_rows != 0:
-                num_cols = len(graph_data_row_list_obj[0])
-                image_panel_display = vis.ErrorPanel(num_rows, num_cols)
-                fig = image_panel_display.fill_grid(graph_data_row_list_obj)
-                fig = image_panel_display.format_panel(graph_data_row_list_obj)
-                fig = image_panel_display.set_title(
-                    "Error Panel, obj: {}, series: {} - Object error".format(
-                        utils.ImageNameHelper.shorten_objname(obj), ax
-                    )
-                )
-                fig.savefig(
-                    os.path.join(
-                        FIG_SAVE_DIR, "error_display_obj_{}_{}.png".format(obj, ax)
-                    ),
-                    bbox_inches="tight",
+            num_cols = len(graph_data_row_list_obj[0])
+            image_panel_display = vis.ErrorPanel(num_rows, num_cols)
+            fig = image_panel_display.fill_grid(graph_data_row_list_obj)
+            fig = image_panel_display.format_panel(graph_data_row_list_obj)
+            fig = image_panel_display.set_title(
+                "Error Panel, obj: {}, series: {}, exclusion radius: {} - Object error".format(
+                    utils.ImageNameHelper.shorten_objname(obj),
+                    ax,
+                    utils.XRADIUS_TO_PLOT_ERR_PANEL,
                 )
-                plt.close(fig)
+            )
+            fig.savefig(
+                os.path.join(
+                    FIG_SAVE_DIR,
+                    "error_display_obj_{}_{}.png".format(obj, ax),
+                ),
+                bbox_inches="tight",
+            )
+            plt.close(fig)
 
             num_rows = len(graph_data_row_list_cat)
-            if num_rows != 0:
-                num_cols = len(graph_data_row_list_cat[0])
-                image_panel_display = vis.ErrorPanel(num_rows, num_cols)
-                fig = image_panel_display.fill_grid(graph_data_row_list_cat)
-                fig = image_panel_display.format_panel(graph_data_row_list_cat)
-                fig = image_panel_display.set_title(
-                    "Error Panel, obj: {}, series: {} - Category error".format(
-                        utils.ImageNameHelper.shorten_objname(obj), ax
-                    )
-                )
-                fig.savefig(
-                    os.path.join(
-                        FIG_SAVE_DIR, "error_display_cat_{}_{}.png".format(obj, ax)
-                    ),
-                    bbox_inches="tight",
+            num_cols = len(graph_data_row_list_cat[0])
+            image_panel_display = vis.ErrorPanel(num_rows, num_cols)
+            fig = image_panel_display.fill_grid(graph_data_row_list_cat)
+            fig = image_panel_display.format_panel(graph_data_row_list_cat)
+            fig = image_panel_display.set_title(
+                "Error Panel, obj: {}, series: {}, exclusion radius: {} - Category error".format(
+                    utils.ImageNameHelper.shorten_objname(obj),
+                    ax,
+                    utils.XRADIUS_TO_PLOT_ERR_PANEL,
                 )
-                plt.close(fig)
+            )
+            fig.savefig(
+                os.path.join(
+                    FIG_SAVE_DIR,
+                    "error_display_cat_{}_{}.png".format(obj, ax),
+                ),
+                bbox_inches="tight",
+            )
+            plt.close(fig)
 
 
 def plot_tuning_curves(feature_directory: str) -> None:
     data_loader = dl.HDFProcessor()
     # create figure directory
     FIG_SAVE_DIR = os.path.join(feature_directory, "figures")
     if not os.path.exists(FIG_SAVE_DIR):
@@ -349,16 +391,14 @@
     # copy config file to feature directory
     cmd = ["cp", utils.PATH_CONFIG_PW_NO_CR, "."]
     utils.execute_and_print(cmd)
     config = dc.load_config(
         os.path.join(feature_directory, "analysis_config_pw_no_cr.json")
     )
 
-    analysis_hdf_path = os.path.join(feature_directory, "analysis_results.h5")
-    analysis_hdf = h5py.File(analysis_hdf_path, "r")
     axes = typing.cast(List, config.axes)
 
     distance_mat_file = os.path.join(feature_directory, "distances-Jaccard.mat")
     input_data_descriptions = (
         os.path.join(feature_directory, "imgnames_pw_series.txt"),
         os.path.join(feature_directory, "imgnames_all.txt"),
     )
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/macros/nn_batch.py` & `ShapeYModular-2.0.2/shapeymodular/macros/nn_batch.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/utils/constants.py` & `ShapeYModular-2.0.2/shapeymodular/utils/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,11 +72,14 @@
     "float32": np.float32,
     "float64": np.float64,
 }
 PATH_CONFIG_PW_NO_CR = os.path.join(CURR_FILE_DIR, "analysis_config_pw_no_cr.json")
 PATH_CONFIG_PW_CR = os.path.join(CURR_FILE_DIR, "analysis_config_pw_cr.json")
 PATH_IMGLIST_ALL = os.path.join(CURR_FILE_DIR, "imgnames_all.txt")
 PATH_IMGLIST_PW = os.path.join(CURR_FILE_DIR, "imgnames_pw_series.txt")
+PATH_FEATURELIST_ALL = os.path.join(CURR_FILE_DIR, "features_imgnames_all.txt")
+PATH_FEATURELIST_PW = os.path.join(CURR_FILE_DIR, "features_imgnames_pw_series.txt")
+
 
 XRADIUS_TO_PLOT_ERR_PANEL = (
     2  # exclusion radius, add 1 to get the actual index (exclusion distance)
 )
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/utils/image_name_helper.py` & `ShapeYModular-2.0.2/shapeymodular/utils/image_name_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Union, Dict
 from . import constants
 import re
+import random
 
 
 class ImageNameHelper:
     @staticmethod
     def generate_imgnames_from_objname(
         objname: str, axes: Union[List[str], None] = None
     ) -> List[str]:
@@ -92,7 +93,26 @@
         return {
             "imgname": imgname,
             "objname": objname,
             "series_idx": str(series_idx),
             "ax": ax,
             "obj_cat": obj_cat,
         }
+
+    @staticmethod
+    def get_closest_physical_image(ref_shapey_idx: int, exc_dist: int) -> int:
+        series_idx = ImageNameHelper.shapey_idx_to_series_idx(ref_shapey_idx)
+        choices = []
+        closest_series_idx_high = series_idx + exc_dist
+        closest_series_idx_low = series_idx - exc_dist
+        if closest_series_idx_high <= 11:
+            choices.append(exc_dist)
+
+        if closest_series_idx_low >= 1:
+            choices.append(-exc_dist)
+
+        if len(choices) == 0:
+            return -1
+        elif len(choices) == 1:
+            return choices[0] + ref_shapey_idx
+        else:
+            return ref_shapey_idx + random.choice(choices)
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/utils/indexing_helper.py` & `ShapeYModular-2.0.2/shapeymodular/utils/indexing_helper.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/correlation_fall_off.py` & `ShapeYModular-2.0.2/shapeymodular/visualization/correlation_fall_off.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/exclusion_distance.py` & `ShapeYModular-2.0.2/shapeymodular/visualization/exclusion_distance.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/histogram.py` & `ShapeYModular-2.0.2/shapeymodular/visualization/histogram.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/image_panel.py` & `ShapeYModular-2.0.2/shapeymodular/analysis/postprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,970 +1,814 @@
-from PIL import Image
-import sys
-import os
 import numpy as np
-import h5py
-from itertools import combinations
-import functools
-from typing import Tuple
-import re
-import matplotlib
-from tqdm import tqdm
-
-matplotlib.use("Agg")
-
-import matplotlib.pyplot as plt
-from matplotlib import cm
-from mpl_toolkits.axes_grid1 import ImageGrid as MplImageGrid
-from os import path
-
-PROJECT_DIR = path.dirname(__file__)
-BLANK_IMG = path.join(PROJECT_DIR, "blank.png")
-
-
-def blockPrint():
-    sys.stdout = open(os.devnull, "w")
-
-
-def enablePrint():
-    sys.stdout = sys.__stdout__
+import shapeymodular.data_loader as dl
+import shapeymodular.utils as utils
+import shapeymodular.visualization as vis
+from typing import Union, Sequence, Tuple, List, Dict
+import typing
+import shapeymodular.data_classes as dc
+from . import nn_analysis as nn
+import os
 
 
-class DataPrepImagePanels:
-    def __init__(
-        self,
-        imgdir,
-        datadir,
-        num_series=31,
-        num_img_single_series=11,
-        num_obj_per_cat=10,
-    ):
-        (
-            self.imgnames,
-            self.objnames,
-            self.obj_categories,
-        ) = self.get_image_and_obj_names(datadir)
-        self.datadir = datadir
-        self.imgdir = imgdir
-        self.num_series = num_series
-        self.num_img_single_series = num_img_single_series
-        self.num_obj_per_cat = num_obj_per_cat
-        self.axis_of_interest = self.make_axis_of_interest()
-
-    def make_axis_of_interest(self) -> list:
-        axes = ["x", "y", "p", "r", "w"]
-        axis_of_interest = []
-        for choose in range(1, 7):
-            for comb in combinations(axes, choose):
-                axis_of_interest.append(functools.reduce(lambda a, b: a + b, comb))
-        axis_of_interest.sort()
-        return axis_of_interest
-
-    def get_image_and_obj_names(self, datadir):
-        with h5py.File(datadir, "r") as hdfstore:
-            imgnames = hdfstore["/feature_output/imgname"][:].astype("U")
-            objnames = np.unique(np.array([c.split("-")[0] for c in imgnames]))
-            obj_categories = imgnames
-            obj_categories = [s.split("_")[0] for s in obj_categories]
-            obj_categories = np.unique(np.array(obj_categories))
-        return imgnames, objnames, obj_categories
-
-    def map_to_imgname(self, idx):
-        blank = np.where(idx == -1)
-        imgs = self.imgnames[idx]
-        imgs[blank] = "blank.png"
-        return imgs
-
-    def get_list_of_errors(
-        self, obj: str, ax: str, exc_dist: int, key_head: str = "original"
-    ) -> list:
-        # returns list with errors [[img1: refimg, img2: best matching other obj]]
-        with h5py.File(self.datadir, "r") as hdfstore:
-            obj_ax_key = "/{}/{}/{}".format(key_head, obj, ax)
-            top1_cvals_sameobj = hdfstore[obj_ax_key + "/top1_cvals"][:, exc_dist]
-            top1_cvals_otherobj = hdfstore[obj_ax_key + "/top1_cvals_otherobj"][:]
-            top1_idx_otherobj = hdfstore[obj_ax_key + "/top1_idx_otherobj"][:]
-        incorrect = top1_cvals_sameobj < top1_cvals_otherobj
-        incorrect[np.isnan(top1_cvals_sameobj)] = False
-        c1, c2 = self.get_coord_corrmat(obj, ax)
-        imgidxs = np.array(range(c1, c2))
-        error_refimg = self.imgnames[imgidxs[incorrect]]
-        error_cval_refimg = top1_cvals_sameobj[incorrect]
-        error_matchimg = self.imgnames[top1_idx_otherobj[incorrect]]
-        error_cval_matchimg = top1_cvals_otherobj[incorrect]
-        # randomly select sample
-        if len(error_refimg) > 3:
-            idx = np.random.choice(len(error_refimg), 3, replace=False)
-            idx.sort()
-            error_refimg = error_refimg[idx]
-            error_cval_refimg = error_cval_refimg[idx]
-            error_matchimg = error_matchimg[idx]
-            error_cval_matchimg = error_cval_matchimg[idx]
-
-        # get all candidate images
-        candidate_list = []
-        candidate_cval_list = []
-        for img in error_refimg:
-            series_name = img.split("-")[1].split(".")[0]
-            series_num = int(re.findall("\d+", series_name)[0]) - 1
-            candidates, candidate_cvals, dists = self.get_all_candidate_images_sameobj(
-                obj, ax, series_num, key_head=key_head
-            )
-            include = dists >= exc_dist
-            candidates = candidates[include]
-            candidate_cvals = candidate_cvals[include]
-            if len(candidates) > 10:
-                dists = dists[include]
-                idx_order_dist = np.argsort(dists)[:10]
-                candidates = candidates[idx_order_dist]
-                candidate_cvals = candidate_cvals[idx_order_dist]
-            candidate_list.append(candidates)
-            candidate_cval_list.append(candidate_cvals)
-
-        list_of_errors = list(
-            map(list, zip(error_refimg, error_matchimg, candidate_list))
-        )
-        error_cvals = list(
-            map(list, zip(error_cval_refimg, error_cval_matchimg, candidate_cval_list))
-        )
-        return list_of_errors, error_cvals
-
-    def get_whole_error_list(
-        self, ax: str, exc_dist: int, key_head: str = "original"
-    ) -> Tuple[list, list]:
-        first = True
-        for obj in tqdm(self.objnames):
-            if first:
-                list_of_errors, error_cvals = self.get_list_of_errors(
-                    obj, ax, exc_dist, key_head=key_head
+class NNClassificationError:
+    @staticmethod
+    def gather_info_same_obj_cat(
+        sampler: dl.Sampler,
+        obj: str,
+        ax: str,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        same_objcat_cvals = []
+        same_objcat_idxs = []
+        obj_cat = utils.ImageNameHelper.get_obj_category_from_objname(obj)
+        objs_same_cat = [
+            other_obj for other_obj in utils.SHAPEY200_OBJS if obj_cat in other_obj
+        ]
+        for other_obj in objs_same_cat:
+            if obj != other_obj:
+                other_obj_cval = sampler.load(
+                    {
+                        "data_type": "top1_cvals_same_category",
+                        "obj": obj,
+                        "ax": ax,
+                        "other_obj_in_same_cat": other_obj,
+                    },
+                    lazy=False,
+                )
+                other_obj_idx = sampler.load(
+                    {
+                        "data_type": "top1_idx_same_category",
+                        "obj": obj,
+                        "ax": ax,
+                        "other_obj_in_same_cat": other_obj,
+                    },
+                    lazy=False,
                 )
-                first = False
+                same_objcat_cvals.append(other_obj_cval)
+                same_objcat_idxs.append(other_obj_idx)
             else:
-                new_list_of_errors, new_error_cvals = self.get_list_of_errors(
-                    obj, ax, exc_dist, key_head=key_head
+                top1_sameobj_cvals = sampler.load(
+                    {"data_type": "top1_cvals", "obj": obj, "ax": ax}, lazy=False
                 )
-                list_of_errors += new_list_of_errors
-                error_cvals += new_error_cvals
-        return list_of_errors, error_cvals
+                top1_sameobj_idx = sampler.load(
+                    {"data_type": "top1_idx", "obj": obj, "ax": ax}, lazy=False
+                )
+                same_objcat_cvals.append(top1_sameobj_cvals)
+                same_objcat_idxs.append(top1_sameobj_idx)
+        return np.array(same_objcat_cvals), np.array(same_objcat_idxs)
+
+    @staticmethod
+    def compare_same_obj_with_top1_other_obj(
+        top1_excdist: np.ndarray, top1_other: np.ndarray, distance: str = "correlation"
+    ) -> np.ndarray:
+        if top1_other.ndim == 2:
+            top1_other = top1_other.flatten()  # type: ignore
+        comparison_mask = np.tile(top1_other, (11, 1)).T
+        # compare if the largest cval for same obj is larger than the top1 cval for other objs
+        if distance == "correlation":
+            correct_counts = np.greater(top1_excdist, comparison_mask)
+        else:
+            correct_counts = np.less(top1_excdist, comparison_mask)
+        return correct_counts
 
-    def get_coltf_sameobj_candidates(
-        self, obj_name: str, axis: str
+    @staticmethod
+    def mask_same_obj_cat(top_per_obj_cvals: np.ndarray, obj: str) -> np.ndarray:
+        obj_cat = utils.ImageNameHelper.get_obj_category_from_objname(obj)
+        in_same_objcat = np.array(
+            [
+                obj_cat
+                == utils.ImageNameHelper.get_obj_category_from_objname(other_obj)
+                for other_obj in utils.SHAPEY200_OBJS
+                if other_obj != obj
+            ]
+        )
+        # zero out objs in same obj category
+        same_obj_mask = np.tile(in_same_objcat, (11, 1))
+        # zero out objs in same obj category
+        top_per_obj_cvals[same_obj_mask] = np.nan
+        return top_per_obj_cvals
+
+    @staticmethod
+    def get_top1_dists_and_idx_other_obj_cat(
+        top_per_obj_cvals: np.ndarray,
+        top_per_obj_idxs: np.ndarray,
+        obj: str,
+        distance="correlation",
     ) -> Tuple[np.ndarray, np.ndarray]:
-        same_obj_tf = np.char.startswith(self.imgnames, obj_name)
-        series_names = np.array(
-            [img.split("-")[1].split(".")[0] for img in self.imgnames]
-        )
-        same_series_tf = np.array([axis in s for s in series_names])
-        col_tf = same_obj_tf & same_series_tf
-        dists = np.array([int(re.findall(r"\d+", s)[0]) for s in series_names])
-        dists = dists[col_tf]
-        return col_tf, dists
-
-    def get_all_candidate_images_sameobj(
-        self, obj_name: str, axis: str, series_idx: int, key_head: str = "original"
-    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        cval_mat = self.grab_whole_rows(obj_name, axis, key_head=key_head)
-        cval_row = cval_mat[series_idx, :]  # series index starts from 0!
-        col_tf, dists = self.get_coltf_sameobj_candidates(obj_name, axis)
-        dists = abs(dists - (series_idx + 1))
-        candidates = self.imgnames[col_tf]
-        candidate_cvals = cval_row[col_tf]
-        return candidates, candidate_cvals, dists
-
-    def get_top_matches_sameobj_with_excdist(
-        self,
-        candidates: np.ndarray,
-        candidate_cvals: np.ndarray,
-        dists: np.ndarray,
-        excdist: int,
-    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        candidates = candidates[dists >= excdist]
-        candidate_cvals = candidate_cvals[dists >= excdist]
-        dists = dists[dists >= excdist]
-        sorted_idxs = np.argsort(-1 * candidate_cvals)
-        candidates = np.take_along_axis(candidates, sorted_idxs, axis=0)
-        candidate_cvals = np.take_along_axis(candidate_cvals, sorted_idxs, axis=0)
-        dists = np.take_along_axis(dists, sorted_idxs, axis=0)
-        return candidates, candidate_cvals, dists
-
-    def get_coord_corrmat(self, obj_name, ax="all"):
-        idx = np.where(self.objnames == obj_name)[0][0]
-        if ax == "all":
-            return (
-                idx * self.num_img_single_series * self.num_series,
-                (idx + 1) * self.num_img_single_series * self.num_series,
+        top_per_obj_cvals_masked = NNClassificationError.mask_same_obj_cat(
+            top_per_obj_cvals, obj
+        )
+        if distance == "correlation":
+            top1_dists_other_obj_cat = np.nanmax(top_per_obj_cvals_masked, axis=1)
+            top1_idxs_other_obj_cat = np.nanargmax(top_per_obj_cvals_masked, axis=1)
+        else:
+            top1_dists_other_obj_cat = np.nanmin(top_per_obj_cvals_masked, axis=1)
+            top1_idxs_other_obj_cat = np.nanargmin(top_per_obj_cvals_masked, axis=1)
+        # shapey index
+        top1_idxs_other_obj_cat = top_per_obj_idxs[
+            np.arange(utils.NUMBER_OF_VIEWS_PER_AXIS), top1_idxs_other_obj_cat
+        ]
+        return top1_dists_other_obj_cat, top1_idxs_other_obj_cat
+
+    @staticmethod
+    def compare_same_obj_cat_with_top1_other_obj_cat(
+        same_objcat_cvals: np.ndarray,
+        top_per_obj_cvals: np.ndarray,
+        obj: str,
+        distance: str = "correlation",
+    ) -> np.ndarray:
+        top_per_obj_cvals_masked = NNClassificationError.mask_same_obj_cat(
+            top_per_obj_cvals, obj
+        )
+        if distance == "correlation":
+            # top 1 other object category
+            top1_other_cat_cvals = np.nanmax(top_per_obj_cvals_masked, axis=1)
+            comparison_mask = np.tile(top1_other_cat_cvals, (11, 1)).T
+            correct_counts = np.greater(same_objcat_cvals, comparison_mask)
+        else:
+            # top 1 other object category
+            top1_other_cat_cvals = np.nanmin(top_per_obj_cvals_masked, axis=1)
+            comparison_mask = np.tile(top1_other_cat_cvals, (11, 1)).T
+            correct_counts = np.less(same_objcat_cvals, comparison_mask)
+        return correct_counts
+
+    @staticmethod
+    def generate_top1_error_data(
+        sampler: dl.Sampler,
+        obj: str,
+        ax: str,
+        within_category_error=False,
+        distance: str = "correlation",
+    ) -> dc.GraphData:
+        top1_excdist = sampler.load(
+            {"data_type": "top1_cvals", "obj": obj, "ax": ax}, lazy=False
+        )  # 1st dim = list of imgs in series, 2nd dim = exclusion dists, vals = top1 cvals with exc dist
+        top1_other = sampler.load(
+            {"data_type": "top1_cvals_otherobj", "obj": obj, "ax": ax}, lazy=False
+        )  # 1st dim = list of imgs in series, vals = top1 cvals excluding the same obj
+        top1_excdist = typing.cast(np.ndarray, top1_excdist)
+        top1_other = typing.cast(np.ndarray, top1_other)
+
+        # if within_category_error = True, you consider a match to another obj in the same obj category a correct answer
+        if within_category_error:
+            same_objcat_cvals, _ = NNClassificationError.gather_info_same_obj_cat(
+                sampler, obj, ax
+            )  # 1st dim = different objs in same obj cat, 2nd dim = imgs, 3rd dim = exclusion dist in ax
+            top_per_obj_cvals = sampler.load(
+                {"data_type": "top1_per_obj_cvals", "obj": obj, "ax": ax}, lazy=False
+            )  # 1st dim = refimgs, 2nd dim = objs (199)
+            top_per_obj_cvals = typing.cast(np.ndarray, top_per_obj_cvals)
+            correct_counts = (
+                NNClassificationError.compare_same_obj_cat_with_top1_other_obj_cat(
+                    same_objcat_cvals, top_per_obj_cvals, obj, distance=distance
+                )
             )
+            # consolidate across all objects in same obj category.
+            # if any one of them is correct (above zero after summing), then it's correct.
+            correct_counts = (correct_counts.sum(axis=0)) > 0
         else:
-            ax_idx = self.axis_of_interest.index(ax)
-            return (
-                idx * self.num_img_single_series * self.num_series
-                + ax_idx * self.num_img_single_series,
-                idx * self.num_img_single_series * self.num_series
-                + (ax_idx + 1) * self.num_img_single_series,
-            )
-
-    def grab_whole_rows(self, objname, axis, key_head="original"):
-        obj_ax_key = "/" + key_head + "/" + str(objname) + "/" + axis
-        with h5py.File(self.datadir, "r") as hdfstore:
-            r1, r2 = self.get_coord_corrmat(objname, ax=axis)
-            whole_results = hdfstore["/pairwise_correlation/original"][r1:r2, :]
-        return whole_results
-
-    def map_top_per_obj_idx_to_global_idx(self, objname, top_per_obj_idx):
-        top_per_obj_idx_mapped = np.copy(top_per_obj_idx)
-        obj_idx = np.tile(
-            np.linspace(
-                0,
-                top_per_obj_idx_mapped.shape[1] - 1,
-                num=top_per_obj_idx_mapped.shape[1],
-            ),
-            (top_per_obj_idx_mapped.shape[0], 1),
-        )
-        obj_idx[:, np.where(self.objnames == objname)[0][0] :] = (
-            obj_idx[:, np.where(self.objnames == objname)[0][0] :] + 1
-        )
-        obj_idx = obj_idx * self.num_img_single_series * self.num_series
-        top_per_obj_idx_mapped = top_per_obj_idx_mapped + obj_idx
-        top_per_obj_idx_mapped = top_per_obj_idx_mapped.astype(np.int)
-        return top_per_obj_idx_mapped
-
-    def get_best_matching_same_obj_with_exclusion(
-        self, objname, axis, sample_row_idx, key_head="original"
-    ):
-        # sampled image name
-        sampled_imgname = "{}-{}{:02d}.png".format(objname, axis, sample_row_idx + 1)
-        with h5py.File(self.datadir, "r") as hdfstore:
-            obj_ax_key = "/" + key_head + "/" + str(objname) + "/" + axis
-            print("pulling {}".format(obj_ax_key))
-            top1cvals_excdist = hdfstore[obj_ax_key + "/top1_cvals"][:]
-            top1cvals_idx = hdfstore[obj_ax_key + "/top1_idx"][:]
-        # row1 best matching same obj with exclusion distances
-        invalid = np.where(top1cvals_idx == -1)
-        top1cvals_idx = (
-            top1cvals_idx
-            + np.where(self.objnames == objname)[0][0]
-            * self.num_img_single_series
-            * self.num_series
-        )
-        top1cvals_idx[invalid] = -1
-        row1_excdist_cvals = top1cvals_excdist[sample_row_idx, :]
-        row1_imgnames = np.array(list(map(self.map_to_imgname, top1cvals_idx)))[
-            sample_row_idx, :
-        ]
-        return sampled_imgname, (row1_excdist_cvals, row1_imgnames)
-
-    def get_top11_best_matching_any_other_obj(
-        self, objname, axis, sample_row_idx, key_head="original"
-    ):
-        # sampled image name
-        sampled_imgname = "{}-{}{:02d}.png".format(objname, axis, sample_row_idx + 1)
-        with h5py.File(self.datadir, "r") as hdfstore:
-            obj_ax_key = "/" + key_head + "/" + str(objname) + "/" + axis
-            print("pulling {}".format(obj_ax_key))
-            top1_cvals_otherobj = hdfstore[obj_ax_key + "/top1_cvals_otherobj"][:]
-            top1_idx_otherobj = hdfstore[obj_ax_key + "/top1_idx_otherobj"][:]
-        # row2 top 11 best matching any obj
-        whole_results = self.grab_whole_rows(objname, axis)
-        c1, c2 = self.get_coord_corrmat(objname)
-        whole_results[:, c1:c2] = 0
-        top11_allobj_idx = np.argsort(-whole_results)[:, :11]
-        top11_allobj = np.take_along_axis(whole_results, top11_allobj_idx, axis=1)
-        top11_imgnames = np.array(list(map(self.map_to_imgname, top11_allobj_idx)))
-
-        row2_top11_any_cvals = top11_allobj[sample_row_idx, :]
-        row2_imgnames = top11_imgnames[sample_row_idx, :]
-        return sampled_imgname, (row2_top11_any_cvals, row2_imgnames)
-
-    def get_top11_best_matching_per_any_other_obj(
-        self, objname, axis, sample_row_idx, key_head="original"
-    ):
-        # sampled image name
-        sampled_imgname = "{}-{}{:02d}.png".format(objname, axis, sample_row_idx + 1)
-        with h5py.File(self.datadir, "r") as hdfstore:
-            obj_ax_key = "/" + key_head + "/" + str(objname) + "/" + axis
-            print("pulling {}".format(obj_ax_key))
-            top_per_obj_cvals = hdfstore[obj_ax_key + "/top1_per_obj_cvals"][:]
-            top_per_obj_idx = hdfstore[obj_ax_key + "/top1_per_obj_idxs"][
-                :
-            ]  # top per obj index are indices within the object, thus needs to be mapped to a global index
-        # row3 top 11 best matching per object
-        row3_top_per_obj_idx = np.argsort(-top_per_obj_cvals)[:, :11]
-
-        top_per_obj_idx_mapped = self.map_top_per_obj_idx_to_global_idx(
-            objname, top_per_obj_idx
-        )
-        row3_img_idx = np.take_along_axis(
-            top_per_obj_idx_mapped, row3_top_per_obj_idx, axis=1
-        )
-
-        row3_top_per_obj_cvals = np.take_along_axis(
-            top_per_obj_cvals, row3_top_per_obj_idx, axis=1
-        )[sample_row_idx, :]
-        row3_imgnames = np.array(list(map(self.map_to_imgname, row3_img_idx)))[
-            sample_row_idx, :
-        ]
-        return sampled_imgname, (row3_top_per_obj_cvals, row3_imgnames)
+            correct_counts = NNClassificationError.compare_same_obj_with_top1_other_obj(
+                top1_excdist, top1_other, distance=distance
+            )
+        correct = correct_counts.sum(axis=0)
+        total_sample = 11 - np.isnan(top1_excdist).sum(axis=0)
+        top1_error = (total_sample - correct) / total_sample
+        if within_category_error:
+            obj_label = "category error - {}".format(
+                utils.ImageNameHelper.shorten_objname(obj)
+            )
+            y_label = "top1 category error"
+        else:
+            obj_label = "object error - {}".format(
+                utils.ImageNameHelper.shorten_objname(obj)
+            )
+            y_label = "top1 error"
+        graph_data = dc.GraphData(
+            x=np.arange(0, utils.NUMBER_OF_VIEWS_PER_AXIS),
+            y=np.array([0, 1]),
+            x_label="exclusion distance",
+            y_label=y_label,
+            data=top1_error,
+            label=obj_label,
+            supplementary_data={
+                "num correct matches": correct,
+                "total valid samples": total_sample,
+            },
+        )
+        return graph_data
+
+
+class DistanceHistogram:
+    @staticmethod
+    def gather_histogram_data(
+        sampler: dl.Sampler,
+        obj: str,
+        ax: str,
+        within_category_error=False,
+        img_idx: Union[int, None] = None,
+    ) -> Tuple[dc.GraphDataGroup, dc.GraphData]:
+        if not within_category_error:
+            top1_hists = sampler.load(
+                {"data_type": "top1_hists", "obj": obj, "ax": ax}, lazy=False
+            )
+            cval_hist_otherobj = sampler.load(
+                {"data_type": "cval_hist_otherobj", "obj": obj, "ax": ax}, lazy=False
+            )
 
-    def get_top11_best_matching_per_any_other_obj_category(
-        self, objname, axis, sample_row_idx, key_head="original", keep_sameobj_cat=False
-    ):
-        # sampled image name
-        sampled_imgname = "{}-{}{:02d}.png".format(objname, axis, sample_row_idx + 1)
-        with h5py.File(self.datadir, "r") as hdfstore:
-            obj_ax_key = "/" + key_head + "/" + str(objname) + "/" + axis
-            print("pulling {}".format(obj_ax_key))
-            top_per_obj_cvals = hdfstore[obj_ax_key + "/top1_per_obj_cvals"][:]
-            top_per_obj_idx = hdfstore[obj_ax_key + "/top1_per_obj_idxs"][:]
-        top_per_obj_idx_mapped = self.map_top_per_obj_idx_to_global_idx(
-            objname, top_per_obj_idx
-        )
-        # row4 top 11 best matching per object category
-        current_obj_cat = objname.split("_")[0]
-
-        top_per_objcat_cvals = []
-        top_per_objcat_idxs = []
-        start_idx = 0
-        for objcat in self.obj_categories:
-            if objcat == current_obj_cat:
-                end_idx = start_idx + self.num_obj_per_cat - 1
-                if keep_sameobj_cat:
-                    top_per_objcat_cvals.append(
-                        top_per_obj_cvals[:, start_idx:end_idx].max(axis=1)
-                    )
-                    idxs = top_per_obj_cvals[:, start_idx:end_idx].argmax(axis=1)
-                    top_per_objcat_idxs.append(
-                        np.take_along_axis(
-                            top_per_obj_idx_mapped[:, start_idx:end_idx],
-                            np.expand_dims(idxs, axis=1),
-                            axis=1,
-                        )
-                    )
+            if img_idx is None:
+                same_obj_hists = typing.cast(np.ndarray, top1_hists).sum(axis=0)
+                other_obj_hist = typing.cast(np.ndarray, cval_hist_otherobj).sum(axis=0)
             else:
-                end_idx = start_idx + self.num_obj_per_cat
-                top_per_objcat_cvals.append(
-                    top_per_obj_cvals[:, start_idx:end_idx].max(axis=1)
-                )
-                idxs = top_per_obj_cvals[:, start_idx:end_idx].argmax(axis=1)
-                top_per_objcat_idxs.append(
-                    np.take_along_axis(
-                        top_per_obj_idx_mapped[:, start_idx:end_idx],
-                        np.expand_dims(idxs, axis=1),
-                        axis=1,
+                # 1st dim = series index, 2nd dim = exclusion dist, 3rd dim = histogram bins
+                same_obj_hists = typing.cast(np.ndarray, top1_hists)[img_idx, :, :]
+                other_obj_hist = typing.cast(np.ndarray, cval_hist_otherobj)[
+                    img_idx, :, :
+                ]
+        else:
+            hist_cat_other_category = sampler.load(
+                {"data_type": "hist_category_other_cat_objs", "obj": obj, "ax": ax},
+                lazy=False,
+            )
+            obj_cat = utils.ImageNameHelper.get_obj_category_from_objname(obj)
+            hist_cat_same_category = []
+            for other_obj in utils.SHAPEY200_OBJS:
+                other_obj_cat = utils.ImageNameHelper.get_obj_category_from_objname(
+                    other_obj
+                )
+                if other_obj_cat == obj_cat and other_obj != obj:
+                    hist_with_exc_dist_same_category = sampler.load(
+                        {
+                            "data_type": "hist_with_exc_dist_same_category",
+                            "obj": obj,
+                            "ax": ax,
+                            "other_obj_in_same_cat": other_obj,
+                        },
+                        lazy=False,
                     )
+                    hist_cat_same_category.append(hist_with_exc_dist_same_category)
+            # sum over all other objs
+            hist_cat_same_category = np.array(hist_cat_same_category).sum(axis=0)
+            # sum over all imgs in series
+            if img_idx is None:
+                hist_cat_same_category = typing.cast(
+                    np.ndarray, hist_cat_same_category
+                ).sum(axis=0)
+                hist_cat_other_category = typing.cast(
+                    np.ndarray, hist_cat_other_category
+                ).sum(axis=0)
+            else:
+                hist_cat_same_category = typing.cast(
+                    np.ndarray, hist_cat_same_category
+                )[img_idx, :, :]
+                hist_cat_other_category = typing.cast(
+                    np.ndarray, hist_cat_other_category
+                )[img_idx, :, :]
+            same_obj_hists = hist_cat_same_category
+            other_obj_hist = hist_cat_other_category
+
+        bins = sampler.nn_analysis_config.bins
+        same_obj_hist_graph_data_list: Sequence[dc.GraphData] = []
+        for xdist in range(utils.NUMBER_OF_VIEWS_PER_AXIS):
+            same_obj_hist_graph_data_list.append(
+                dc.GraphData(
+                    x=np.array(bins),
+                    y="counts",
+                    x_label=sampler.nn_analysis_config.distance_measure,
+                    y_label="counts",
+                    data=same_obj_hists[xdist, :],
+                    label="positive match candidates counts with exclusion",
+                    supplementary_data={"exclusion distance": np.array(xdist)},
+                    hist=True,
                 )
-            start_idx = end_idx
-
-        top_per_objcat_cvals = np.array(top_per_objcat_cvals, dtype=float).T
-        top_per_objcat_idxs = np.squeeze(
-            np.array(top_per_objcat_idxs, dtype=np.int64).T, axis=0
-        )
-
-        row4_top_per_objcat_idx = np.argsort(-top_per_objcat_cvals)[:, :11]
-        row4_img_idx = np.take_along_axis(
-            top_per_objcat_idxs, row4_top_per_objcat_idx, axis=1
+            )
+        graph_data_group_sameobj_xdist = dc.GraphDataGroup(
+            same_obj_hist_graph_data_list
         )
 
-        row4_top_per_objcat_cvals = np.take_along_axis(
-            top_per_objcat_cvals, row4_top_per_objcat_idx, axis=1
-        )[sample_row_idx, :]
-        row4_imgnames = np.array(list(map(self.map_to_imgname, row4_img_idx)))[
-            sample_row_idx, :
-        ]
-        return sampled_imgname, (row4_top_per_objcat_cvals, row4_imgnames)
-
-    def get_top_per_obj_row_with_exclusion(
-        self, row_info_same_obj, row_info_top_per_obj, exclusion_dist
-    ):
-        # grab the top matching same obj with exclusion
-        best_matching_same_obj = row_info_same_obj[1][exclusion_dist]
-        best_matching_same_obj_cval = row_info_same_obj[0][exclusion_dist]
-        # append and sort
-        top_per_obj_cvals = np.append(
-            row_info_top_per_obj[0], best_matching_same_obj_cval
-        )
-        top_per_obj_imgnames = np.append(
-            row_info_top_per_obj[1], best_matching_same_obj
-        )
-        sorted = np.argsort(top_per_obj_cvals)
-        top_per_obj_cvals = np.take_along_axis(top_per_obj_cvals, sorted[::-1], axis=0)
-        top_per_obj_imgnames = np.take_along_axis(
-            top_per_obj_imgnames, sorted[::-1], axis=0
-        )
-        # check for invalid sample with exclusion
-        if np.isnan(top_per_obj_cvals[0]):
-            top_per_obj_imgnames[:] = "blank.png"
-        return (top_per_obj_cvals, top_per_obj_imgnames)
-
-    def get_top_per_objcat_with_exclusion(
-        self, row_info_top_per_obj, row_info_top_per_objcat, obj_cat
-    ):
-        same_obj_cat_tf = [obj_cat in s.split("_") for s in row_info_top_per_obj[1]]
-        same_obj_cat_cval = 0.0
-        for i, tf in enumerate(same_obj_cat_tf):
-            if tf:
-                if row_info_top_per_obj[0][i] > same_obj_cat_cval:
-                    same_obj_cat_cval = row_info_top_per_obj[0][i]
-                    same_obj_cat_imname = row_info_top_per_obj[1][i]
-        if "same_obj_cat_imname" in locals():
-            top_per_objcat_cvals = np.append(
-                row_info_top_per_objcat[0], same_obj_cat_cval
-            )
-            top_per_objcat_imgnames = np.append(
-                row_info_top_per_objcat[1], same_obj_cat_imname
+        hist_data_otherobj = dc.GraphData(
+            x=np.array(bins),
+            y="counts",
+            x_label=sampler.nn_analysis_config.distance_measure,
+            y_label="counts",
+            data=other_obj_hist,
+            label="negative match candidates counts",
+            hist=True,
+        )
+        return graph_data_group_sameobj_xdist, hist_data_otherobj
+
+
+class ErrorDisplay:
+    @staticmethod
+    def add_reference_images(obj: str, ax: str) -> List[List[dc.GraphData]]:
+        graph_data_row_list: List[List[dc.GraphData]] = []
+        ref_img_shapey_idxs = np.array(
+            utils.IndexingHelper.objname_ax_to_shapey_index(obj, ax)
+        )
+        for ref_shapey_idx in ref_img_shapey_idxs:
+            graph_data_row: List[dc.GraphData] = []
+            parsed_ref_img = utils.ImageNameHelper.parse_shapey_idx(ref_shapey_idx)
+            ref_label = utils.ImageNameHelper.shorten_objname(parsed_ref_img["objname"])
+            ref_graph_data = dc.GraphData(
+                x="img_x",
+                y="img_y",
+                x_label="reference",
+                y_label="{}{:02d}".format(
+                    parsed_ref_img["ax"], int(parsed_ref_img["series_idx"])
+                ),
+                data=parsed_ref_img["imgname"],
+                label=ref_label,
+                supplementary_data={"highlight": vis.CORRECT_MATCH_COLOR},
+            )
+            graph_data_row.append(ref_graph_data)
+            graph_data_row_list.append(graph_data_row)
+        return graph_data_row_list
+
+    @staticmethod
+    def add_all_candidates_top_per_obj(
+        graph_data_row_list: List[List[dc.GraphData]],
+        sampler: dl.Sampler,
+        obj: str,
+        ax: str,
+        exc_dist: int,
+        within_category_error: bool = False,
+        truncate_to: int = 10,
+    ) -> List[List[dc.GraphData]]:
+        base_query = {"obj": obj, "ax": ax}
+
+        # Load necessary data
+        top1_dists_sameobj = typing.cast(
+            np.ndarray,
+            sampler.load({"data_type": "top1_cvals", **base_query}, lazy=False),
+        )
+        top1_idxs_sameobj = typing.cast(
+            np.ndarray,
+            sampler.load({"data_type": "top1_idx", **base_query}, lazy=False),
+        )
+        top_per_obj_cvals = typing.cast(
+            np.ndarray,
+            sampler.load({"data_type": "top1_per_obj_cvals", **base_query}, lazy=False),
+        )  # 1st dim = refimgs, 2nd dim = objs (199)
+        top_per_obj_idxs = typing.cast(
+            np.ndarray,
+            sampler.load({"data_type": "top1_per_obj_idxs", **base_query}, lazy=False),
+        )
+
+        if not within_category_error:
+            (
+                all_candidates_sorted_dists,
+                all_candidates_sorted_idxs,
+            ) = ErrorDisplay.get_all_candidates_sorted_top_per_obj(
+                top1_dists_sameobj,
+                top1_idxs_sameobj,
+                top_per_obj_cvals,
+                top_per_obj_idxs,
+                exc_dist,
             )
         else:
-            top_per_objcat_cvals = row_info_top_per_objcat[0]
-            top_per_objcat_imgnames = row_info_top_per_objcat[1]
-
-        # remove duplicates if there is one
-        same_obj_cat_tf = np.array(
-            [obj_cat in s.split("_") for s in top_per_objcat_imgnames]
-        )
-        if same_obj_cat_tf.sum() > 1:
-            same_obj_idx = np.where(same_obj_cat_tf == True)
-            min_cval = 1.0
-            remove_idx = 0
-            for idx in same_obj_idx[0]:
-                if top_per_objcat_cvals[idx] < min_cval:
-                    min_cval = top_per_objcat_cvals[idx]
-                    remove_idx = idx
-            top_per_objcat_cvals = np.delete(top_per_objcat_cvals, remove_idx)
-            top_per_objcat_imgnames = np.delete(top_per_objcat_imgnames, remove_idx)
-
-        sorted = np.argsort(top_per_objcat_cvals)
-        top_per_objcat_cvals = np.take_along_axis(
-            top_per_objcat_cvals, sorted[::-1], axis=0
-        )
-        top_per_objcat_imgnames = np.take_along_axis(
-            top_per_objcat_imgnames, sorted[::-1], axis=0
-        )
-        return (top_per_objcat_cvals, top_per_objcat_imgnames)
-
-    def get_top_per_obj_whole_panel_with_exclusion(self, objname, axis, exclusion_dist):
-        # grab all inputs
-        blockPrint()
-        row1_infos = [
-            self.get_best_matching_same_obj_with_exclusion(objname, axis, samp_idx)
-            for samp_idx in range(0, 11)
-        ]
-        row3_infos = [
-            self.get_top11_best_matching_per_any_other_obj(objname, axis, samp_idx)
-            for samp_idx in range(0, 11)
-        ]
-        enablePrint()
-        # organize the infos
-        top_per_obj_row_infos = [
-            self.get_top_per_obj_row_with_exclusion(e[0][1], e[1][1], exclusion_dist)
-            for e in zip(row1_infos, row3_infos)
-        ]
-        sampled_imgs = [e[0] for e in row1_infos]
-        return sampled_imgs, top_per_obj_row_infos
-
-    def get_top_per_objcat_whole_panel_with_exclusion(
-        self, objname, axis, exclusion_dist
-    ):
-        # grab all inputs
-        blockPrint()
-        row1_infos = [
-            self.get_best_matching_same_obj_with_exclusion(objname, axis, samp_idx)
-            for samp_idx in range(0, 11)
-        ]
-        row3_infos = [
-            self.get_top11_best_matching_per_any_other_obj(objname, axis, samp_idx)
-            for samp_idx in range(0, 11)
-        ]
-        row4_infos = [
-            self.get_top11_best_matching_per_any_other_obj_category(
-                objname, axis, samp_idx, keep_sameobj_cat=True
-            )
-            for samp_idx in range(0, 11)
-        ]
-        enablePrint()
-        # organize the infos
-        # replace the best matching per objcat to self if larger than other category
-        for i, (samp_img, (cval, imname)) in enumerate(row1_infos):
-            if ~np.isnan(cval[exclusion_dist]):
-                row3_infos[i] = (
-                    samp_img,
-                    (
-                        np.insert(row3_infos[i][1][0], 0, cval[exclusion_dist]),
-                        np.insert(row3_infos[i][1][1], 0, imname[exclusion_dist]),
-                    ),
+            (
+                same_objcat_dists,
+                same_objcat_idxs,
+            ) = NNClassificationError.gather_info_same_obj_cat(
+                sampler, obj, ax
+            )  # 1st dim = different objs in same obj cat, 2nd dim = imgs, 3rd dim = exclusion dist in axis
+
+            # Get top candidates per object sorted
+            (
+                all_candidates_sorted_dists,
+                all_candidates_sorted_idxs,
+            ) = ErrorDisplay.get_all_candidates_sorted_category_top_per_obj(
+                same_objcat_dists,
+                same_objcat_idxs,
+                top_per_obj_cvals,
+                top_per_obj_idxs,
+                obj,
+                exc_dist,
+            )
+
+        # add top 10 candidates to graph data row
+        for i, graph_data_row in enumerate(graph_data_row_list):
+            row_all_candidate_sorted_dists = all_candidates_sorted_dists[i, :]
+            row_all_candidate_sorted_idxs = all_candidates_sorted_idxs[i, :]
+            ref_imgname = typing.cast(str, graph_data_row[0].data)
+            ref_shapey_idx = utils.ImageNameHelper.imgname_to_shapey_idx(ref_imgname)
+            parsed_ref_img = utils.ImageNameHelper.parse_shapey_idx(ref_shapey_idx)
+            for j, candidate_shapey_idx in enumerate(
+                row_all_candidate_sorted_idxs[:truncate_to]
+            ):
+                parsed_candidate_name = utils.ImageNameHelper.parse_shapey_idx(
+                    candidate_shapey_idx
                 )
-        top_per_obj_row_infos = [
-            self.get_top_per_objcat_with_exclusion(
-                e[0][1], e[1][1], obj_cat=objname.split("_")[0]
-            )
-            for e in zip(row3_infos, row4_infos)
-        ]
-        sampled_imgs = [e[0] for e in row3_infos]
-        # make nan for invalid samples
-        for i, (_, (cval, _)) in enumerate(row1_infos):
-            if np.isnan(cval[exclusion_dist]):
-                top_per_obj_row_infos[i][1][:] = "blank.png"
-        return sampled_imgs, top_per_obj_row_infos
-
-    def get_whole_panel_single_sample(self, objname, axis, sample_idx):
-        blockPrint()
-        sampled_img, row1_info = self.get_best_matching_same_obj_with_exclusion(
-            objname, axis, sample_idx
-        )
-        _, row2_info = self.get_top11_best_matching_any_other_obj(
-            objname, axis, sample_idx
-        )
-        _, row3_info = self.get_top11_best_matching_per_any_other_obj(
-            objname, axis, sample_idx
-        )
-        _, row4_info = self.get_top11_best_matching_per_any_other_obj_category(
-            objname, axis, sample_idx
-        )
-        all_row_infos = [row1_info, row2_info, row3_info, row4_info]
-        enablePrint()
-        return sampled_img, all_row_infos
-
-    def get_corr_fall_off_graph_infos_whole_panel(self, objname, axis, objcat=False):
-        objcat = objname.split("_")[0]
-        issameobjcat = np.array([objcat in obj for obj in self.objnames])
-        objnames = self.objnames[issameobjcat]
-        corr_fall_off_row_infos = []
-        for obj in objnames:
-            row = []
-            for exc_dist in range(0, 11):
-                if objcat:
-                    (
-                        sampled_imgs,
-                        top_per_obj_row_infos,
-                    ) = self.get_top_per_objcat_whole_panel_with_exclusion(
-                        obj, axis, exc_dist
+                shortened_objname = utils.ImageNameHelper.shorten_objname(
+                    parsed_candidate_name["objname"]
+                )
+
+                if within_category_error:
+                    correct_match = (
+                        parsed_ref_img["obj_cat"] == parsed_candidate_name["obj_cat"]
+                    )
+                    highlight = (
+                        vis.CORRECT_CATEGORY_MATCH_COLOR if correct_match else None
                     )
+
                 else:
-                    (
-                        sampled_imgs,
-                        top_per_obj_row_infos,
-                    ) = self.get_top_per_obj_whole_panel_with_exclusion(
-                        obj, axis, exc_dist
+                    correct_match = (
+                        parsed_ref_img["objname"] == parsed_candidate_name["objname"]
                     )
-                row.append((sampled_imgs, top_per_obj_row_infos))
-            corr_fall_off_row_infos.append(row)
-        return corr_fall_off_row_infos
-
-
-class ImageGridV2:
-    def __init__(self, row: int, col: int, axis_pad: float = 0.05):
-        self.row = row
-        self.col = col
-        self.axis_pad = axis_pad
-        self.figure = plt.figure(figsize=(1.65 * self.col, 1.65 * self.row))
-        self.grid = MplImageGrid(
-            self.figure, 111, nrows_ncols=(self.row, self.col), axes_pad=self.axis_pad
-        )
-
-    def reset_figure(self):
-        self.figure = plt.figure(figsize=(1.6 * self.col, 1.6 * self.row))
-        self.grid = MplImageGrid(
-            self.figure, 111, nrows_ncols=(self.row, self.col), axes_pad=self.axis_pad
-        )
-
-    def fill_panel(self, imnames, ylabels, annotations):
-        for i, ax in enumerate(self.grid):
-            ax.set_xticks([])
-            ax.set_yticks([])
-            r = i // self.col
-            c = i % self.col
-            im = imnames[r][c]
-            im1 = Image.open(im)
-            ax.imshow(im1)
-            if c == 0:
-                ylabel_separated = ylabels[r].split("-")
-                if len(ylabel_separated) > 1:
-                    ax.set_ylabel(
-                        "{}\n{}".format(ylabel_separated[0], ylabel_separated[1]),
-                        fontsize=7,
-                        fontweight="bold",
+                    highlight = vis.CORRECT_MATCH_COLOR if correct_match else None
+                graph_data_row.append(
+                    dc.GraphData(
+                        x="img_x",
+                        y="img_y",
+                        x_label="candidates top per obj",
+                        y_label="{}{:02d}".format(
+                            parsed_candidate_name["ax"],
+                            int(parsed_candidate_name["series_idx"]),
+                        ),
+                        data=parsed_candidate_name["imgname"],
+                        label=shortened_objname,
+                        supplementary_data={
+                            "distance": row_all_candidate_sorted_dists[j],
+                            "correct_match": correct_match,
+                            "highlight": highlight,
+                        },
                     )
-                else:
-                    ax.set_ylabel(ylabels[r], fontsize=20, fontweight="bold")
-            t = annotations[r][c]
-            ann_seperate = t.split(":")
-            top_line_text = ann_seperate[0].split("-")
-            if len(top_line_text) > 1:
-                t = "{} \n {}".format(top_line_text[0], top_line_text[1])
-            else:
-                t = top_line_text[0]
-            ax.text(
-                128,
-                5,
-                t,
-                color="yellow",
-                fontsize=7,
-                horizontalalignment="center",
-                verticalalignment="top",
-            )
-            if len(ann_seperate) > 1:
-                ax.text(
-                    128,
-                    250,
-                    ann_seperate[1],
-                    color="yellow",
-                    fontsize=10,
-                    horizontalalignment="center",
                 )
+        return graph_data_row_list
 
-
-class ImagePanelErrorDisplay(ImageGridV2):
-    def __init__(self, datadir):
-        super().__init__(10, 12)
-        self.datadir = datadir
-
-    def shorten_imgname(self, imgname):
-        obj_codes = imgname.split("_")
-        series_name = obj_codes[1].split("-")[1]
-        series_name = series_name.split(".")[0]
-        shortened_imgname = (
-            obj_codes[0] + "_" + obj_codes[1][0:4] + "-{}".format(series_name)
-        )
-        return shortened_imgname
-
-    def fill_error_panel(
-        self,
-        list_of_errors: list,
-        cval_list: list,
+    @staticmethod
+    def add_top_positive_match_candidate(
+        graph_data_row_list: List[List[dc.GraphData]],
+        sampler: dl.Sampler,
+        obj: str,
         ax: str,
         exc_dist: int,
-        annotate: bool = True,
-    ) -> None:
-        blank_img = BLANK_IMG
-        imnames = []
-        ylabels = []
-        annotations = []
-        for i, row in enumerate(list_of_errors):
-            r = [self.datadir + row[0], self.datadir + row[1]]
-            shortened_imgname = self.shorten_imgname(row[0])
-            ylabels.append(shortened_imgname)
-            ann = []
-            ann.append("")
-            if annotate:
-                imname_short = self.shorten_imgname(row[1])
-                ann.append("{}:{:.4f}".format(imname_short, cval_list[i][1]))
-            else:
-                ann.append("")
-            for c in range(10):
-                try:
-                    cand_img = self.datadir + row[2][c]
-                    cand_cval = cval_list[i][2][c]
-                    imname_short = self.shorten_imgname(row[2][c])
-                    r.append(cand_img)
-                    if annotate:
-                        ann.append("{}:{:.4f}".format(imname_short, cand_cval))
-                    else:
-                        ann.append("")
-                except:
-                    r.append(blank_img)
-                    ann.append("")
-            imnames.append(r)
-            annotations.append(ann)
-        self.fill_panel(imnames, ylabels, annotations)
-        self.figure.suptitle(
-            "Axis: {}, Exclusion Distance: {}".format(ax, exc_dist), fontsize=15, y=0.9
-        )
-
-
-class ImagePanelAllCandidates(ImageGridV2):
-    def __init__(self, imgdir: str, row_num: int):
-        ImageGridV2.__init__(self, row_num, 11)
-        self.imgdir = imgdir
-
-    def shorten_imgname(self, imgname: str) -> str:
-        obj_codes = imgname.split("_")
-        series_name = obj_codes[1].split("-")[1]
-        series_name = series_name.split(".")[0]
-        return series_name
-
-    def change_border_color(self, border_colors: list) -> None:
-        for i, ax in enumerate(self.grid):
-            r = i // self.col
-            c = i % self.col
-            ax.set_axis_on()
-            matplotlib.pyplot.setp(
-                ax.spines.values(), color=border_colors[r][c], linewidth=3
-            )
-
-    def fill_all_candidate_panel(
-        self, refimg: str, candidates: np.ndarray, candidate_cvals: np.ndarray
-    ) -> None:
-        cmap = cm.get_cmap("plasma")
-        candidates = np.reshape(candidates, (self.row, self.col))
-        candidate_imgnames = np.char.add(self.imgdir, candidates)
-        candidate_imgnames = candidate_imgnames.tolist()
-        candidates = candidates.tolist()
-
-        candidate_cvals = np.reshape(candidate_cvals, (self.row, self.col))
-        candidate_cvals = candidate_cvals.tolist()
-        annotations = []
-        ylabels = []
-        border_colors = []
-        for r, row in enumerate(candidate_cvals):
-            ann = []
-            bc = []
-            for c, cval in enumerate(row):
-                shortened_imgname = self.shorten_imgname(candidates[r][c])
-                ann.append("{}:{:.4f}".format(shortened_imgname, cval))
-                if c == 0:
-                    ylabels.append(re.findall("[a-zA-Z]+", shortened_imgname)[0])
-                if candidates[r][c] == refimg:
-                    bc.append((1.0, 0.0, 0.0, 1.0))
-                else:
-                    bc.append(cmap(cval))
-            annotations.append(ann)
-            border_colors.append(bc)
-        self.fill_panel(candidate_imgnames, ylabels, annotations)
-        self.change_border_color(border_colors)
-        obj_codes = refimg.split("_")
-        series_name = obj_codes[1].split("-")[1]
-        shortened_imgname = (
-            obj_codes[0] + "_" + obj_codes[1][0:4] + "-{}".format(series_name)
-        )
-        self.figure.suptitle(
-            "All Candidate Images for {}".format(shortened_imgname), fontsize=15, y=0.9
-        )
+        within_category_error: bool = False,
+    ) -> List[List[dc.GraphData]]:
+        base_query = {"obj": obj, "ax": ax}
+        if not within_category_error:
+            top1_dists_sameobj = typing.cast(
+                np.ndarray,
+                sampler.load({"data_type": "top1_cvals", **base_query}, lazy=False),
+            )
+            top1_idxs_sameobj = typing.cast(
+                np.ndarray,
+                sampler.load({"data_type": "top1_idx", **base_query}, lazy=False),
+            )
+        else:
+            (
+                same_objcat_dists,
+                same_objcat_idxs,
+            ) = NNClassificationError.gather_info_same_obj_cat(
+                sampler, obj, ax
+            )  # 1st dim = different objs in same obj cat, 2nd dim = imgs, 3rd dim = exclusion dist in axis
+
+            # get top1 dists and idxs for same obj category
+            (
+                top1_dists_sameobj,
+                top1_idxs_sameobj,
+            ) = ErrorDisplay.consolidate_same_obj_cat_candidates(
+                same_objcat_dists,
+                same_objcat_idxs,
+                distance=sampler.nn_analysis_config.distance_measure,
+            )
+        top1_dists_exc_dist = top1_dists_sameobj[:, exc_dist]
+        top1_idxs_exc_dist = top1_idxs_sameobj[:, exc_dist]
+
+        for i, graph_data_row in enumerate(graph_data_row_list):
+            # add best matching positive match candidate
+            parsed_best_positive_match = utils.ImageNameHelper.parse_shapey_idx(
+                top1_idxs_exc_dist[i]
+            )
+            shortened_objname = utils.ImageNameHelper.shorten_objname(
+                parsed_best_positive_match["objname"]
+            )
+            graph_data_row.append(
+                dc.GraphData(
+                    x="img_x",
+                    y="img_y",
+                    x_label="best positive match",
+                    y_label="{}{:02d}".format(
+                        parsed_best_positive_match["ax"],
+                        int(parsed_best_positive_match["series_idx"]),
+                    ),
+                    data=parsed_best_positive_match["imgname"],
+                    label=shortened_objname,
+                    supplementary_data={
+                        "distance": top1_dists_exc_dist[i],
+                        "highlight": vis.CORRECT_MATCH_COLOR,
+                    },
+                )
+            )
+        return graph_data_row_list
 
+    @staticmethod
+    def add_closest_physical_image(
+        graph_data_row_list: List[List[dc.GraphData]],
+        corrmat_sampler: dl.CorrMatSampler,
+        obj: str,
+        ax: str,
+        exc_dist: int,
+    ) -> List[List[dc.GraphData]]:
+        corrmat = corrmat_sampler.load({"data_type": "corrmat"})
+        tuning_curves = TuningCurve.get_tuning_curve(
+            obj, ax, corrmat, corrmat_sampler.nn_analysis_config
+        )
+        for i, graph_data_row in enumerate(graph_data_row_list):
+            tuning_curve = tuning_curves[i]
+            ErrorDisplay.add_closest_physical_match_to_graph_data_row(
+                graph_data_row, tuning_curve, exc_dist
+            )
+        return graph_data_row_list
+
+    @staticmethod
+    def consolidate_same_obj_cat_candidates(
+        same_objcat_dists: np.ndarray,
+        same_objcat_idxs: np.ndarray,
+        distance: str = "correlation",
+    ) -> Tuple[
+        np.ndarray, np.ndarray
+    ]:  # output: top1 dists and idxs for every candidate in same obj category with exclusion dists (11x11)
+        # same_objcat_dists: 1st dim: different objs in same obj cat, 2nd dim: imgs, 3rd dim: exclusion dist in axis
+        assert same_objcat_dists.shape == (10, 11, 11)
+        assert same_objcat_idxs.shape == (10, 11, 11)
+        if distance == "correlation":
+            same_objcat_dists_nan_to_zero = same_objcat_dists.copy()
+            same_objcat_dists_nan_to_zero[np.isnan(same_objcat_dists)] = 0
+            top1_dists_sameobj = np.nanmax(same_objcat_dists, axis=0)
+            best_positive_match_arg = np.nanargmax(
+                same_objcat_dists_nan_to_zero, axis=0
+            )
+        else:
+            data_type = same_objcat_dists.dtype
+            same_objcat_dists_nan_to_large = same_objcat_dists.copy()
+            same_objcat_dists_nan_to_large[np.isnan(same_objcat_dists)] = np.iinfo(
+                data_type
+            ).max
+            top1_dists_sameobj = np.nanmin(same_objcat_dists, axis=0)
+            best_positive_match_arg = np.nanargmin(
+                same_objcat_dists_nan_to_large, axis=0
+            )
+        best_positive_match_arg[np.isnan(top1_dists_sameobj)] = -1
+        j, k = np.indices(best_positive_match_arg.shape)
+        top1_idxs_sameobj = same_objcat_idxs[best_positive_match_arg, j, k]
+        assert top1_idxs_sameobj.shape == (11, 11)
+        assert top1_dists_sameobj.shape == (11, 11)
+        return top1_dists_sameobj, top1_idxs_sameobj
+
+    @staticmethod
+    def get_all_candidates_sorted_top_per_obj(
+        same_obj_dists: np.ndarray,
+        same_obj_idxs: np.ndarray,
+        top_per_obj_cvals: np.ndarray,
+        top_per_obj_idxs: np.ndarray,
+        exc_dist: int,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        same_obj_dists = np.expand_dims(same_obj_dists[:, exc_dist], axis=1)
+        same_obj_idxs = np.expand_dims(same_obj_idxs[:, exc_dist], axis=1)
 
-class ImagePanelSameObjBestMatchingWithExcDist(ImageGridV2):
-    def __init__(self, imgdir: str, num_cols: int):
-        ImageGridV2.__init__(self, 1, num_cols)
-        self.imgdir = imgdir
-        self.numsample = num_cols
-
-    def shorten_imgname(self, imgname: str) -> str:
-        obj_codes = imgname.split("_")
-        series_name = obj_codes[1].split("-")[1]
-        series_name = series_name.split(".")[0]
-        return series_name
-
-    def set_xlabel(self, dists: list) -> None:
-        for i, ax in enumerate(self.grid):
-            r = i // self.col
-            c = i % self.col
-            if r == 0:
-                if c == 0:
-                    ax.set_title("Reference Img", fontsize=10, fontweight="bold")
-                else:
-                    ax.set_title(
-                        "Dist = {}".format(dists[c - 1]), fontsize=10, fontweight="bold"
-                    )
+        all_candidate_dists = np.concatenate(
+            [same_obj_dists, top_per_obj_cvals], axis=1
+        )  # 11 x 200
+        all_candidate_idxs = np.concatenate([same_obj_idxs, top_per_obj_idxs], axis=1)
+        ind_sorted = np.argsort(-all_candidate_dists, axis=1)  # descending order
+        all_candidate_idxs_sorted = np.take_along_axis(
+            all_candidate_idxs, ind_sorted, axis=1
+        )
+        all_candidate_dists_sorted = np.take_along_axis(
+            all_candidate_dists, ind_sorted, axis=1
+        )
+
+        assert all_candidate_dists_sorted.shape == (11, 200)
+        return all_candidate_dists_sorted, all_candidate_idxs_sorted
+
+    @staticmethod
+    def get_all_candidates_sorted_category_top_per_obj(
+        same_objcat_dists: np.ndarray,  # 1st dim = different objs in same obj cat, 2nd dim = imgs, 3rd dim = exclusion dist in axis
+        same_objcat_idxs: np.ndarray,
+        top_per_obj_cvals: np.ndarray,
+        top_per_obj_idxs: np.ndarray,
+        obj: str,
+        exc_dist: int,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        # get sorted top1 per object for all candidates available.
+        same_objcat_candidate_dists = same_objcat_dists[:, :, exc_dist]  # 10 x 11
+        same_objcat_candidate_idxs = same_objcat_idxs[:, :, exc_dist]
+        assert same_objcat_candidate_dists.shape == (10, 11)
+        (
+            other_objcat_candidate_dists,
+            other_objcat_candidate_idxs,
+        ) = ErrorDisplay.filter_top_per_obj_other_obj_cat(
+            top_per_obj_cvals, top_per_obj_idxs, obj
+        )  # 190 x 11
+        assert other_objcat_candidate_dists.shape == (190, 11)
+        all_candidate_dists = np.concatenate(
+            [same_objcat_candidate_dists, other_objcat_candidate_dists], axis=0
+        )  # 200 x 11
+        all_candidate_idxs = np.concatenate(
+            [same_objcat_candidate_idxs, other_objcat_candidate_idxs], axis=0
+        )
+        ind_sorted = np.argsort(
+            -all_candidate_dists, axis=0
+        )  # sort in descending order
+        sorted_all_candidate_idxs = np.take_along_axis(
+            all_candidate_idxs, ind_sorted, axis=0
+        )
+        sorted_all_candidate_dists = np.take_along_axis(
+            all_candidate_dists, ind_sorted, axis=0
+        )
+
+        assert sorted_all_candidate_dists.shape == (200, 11)
+        return sorted_all_candidate_dists.T, sorted_all_candidate_idxs.T
+
+    @staticmethod
+    def filter_top_per_obj_other_obj_cat(
+        top_per_obj_cvals: np.ndarray, top_per_obj_idxs: np.ndarray, obj: str
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        obj_cat = utils.ImageNameHelper.get_obj_category_from_objname(obj)
+        other_obj_dists = []
+        other_obj_idxs = []
+        other_obj_idx = 0
+        for other_obj in utils.SHAPEY200_OBJS:
+            if other_obj != obj:
+                other_obj_cat = utils.ImageNameHelper.get_obj_category_from_objname(
+                    other_obj
+                )
+                if other_obj_cat != obj_cat:
+                    other_obj_dists.append(top_per_obj_cvals[:, other_obj_idx])
+                    other_obj_idxs.append(top_per_obj_idxs[:, other_obj_idx])
+                other_obj_idx += 1
+        return np.array(other_obj_dists), np.array(other_obj_idxs)
+
+    @staticmethod
+    def add_closest_physical_match_to_graph_data_row(
+        graph_data_row: List[dc.GraphData],
+        tuning_curve: dc.GraphData,
+        exc_dist: int,
+    ):  # exclusion distance, not radius
+        reference_img = graph_data_row[0].data
+        assert isinstance(reference_img, str)
+        ref_shapey_idx = utils.ImageNameHelper.imgname_to_shapey_idx(reference_img)
+        closest_physical_match_shapey_idx = (
+            utils.ImageNameHelper.get_closest_physical_image(ref_shapey_idx, exc_dist)
+        )
+        if closest_physical_match_shapey_idx == -1:
+            graph_data_row.append(
+                dc.GraphData(
+                    x="img_x",
+                    y="img_y",
+                    x_label="closest physical match",
+                    y_label="",
+                    data=vis.BLANK_IMG,
+                    label="",
+                    supplementary_data={"distance": 0.0},
+                )
+            )
+        else:
+            parsed_closest_physical_match = utils.ImageNameHelper.parse_shapey_idx(
+                closest_physical_match_shapey_idx
+            )
+            shortened_objname = utils.ImageNameHelper.shorten_objname(
+                parsed_closest_physical_match["objname"]
+            )
+            closest_physical_match_series_idx = int(
+                parsed_closest_physical_match["series_idx"]
+            )
+            graph_data_row.append(
+                dc.GraphData(
+                    x="img_x",
+                    y="img_y",
+                    x_label="closest physical match",
+                    y_label="{}{:02d}".format(
+                        parsed_closest_physical_match["ax"],
+                        closest_physical_match_series_idx,
+                    ),
+                    data=parsed_closest_physical_match["imgname"],
+                    label=shortened_objname,
+                    supplementary_data={
+                        "distance": tuning_curve.data[
+                            closest_physical_match_series_idx - 1
+                        ],
+                        "highlight": vis.CORRECT_MATCH_COLOR,
+                    },
+                )
+            )
+        return graph_data_row
 
-    def fill_best_matching_panel(
-        self,
-        refimg: str,
-        candidates_sorted: np.ndarray,
-        candidate_cvals_sorted: np.ndarray,
-        dists_sorted: np.ndarray,
-        excdist: int,
-        axis: str,
-    ) -> None:
-        candidate_imgnames = np.char.add(self.imgdir, candidates_sorted)
-        candidate_imgnames = candidate_imgnames.tolist()
-        candidates = candidates_sorted.tolist()
-        dists = dists_sorted.tolist()
-
-        candidate_cvals = candidate_cvals_sorted.tolist()
-        annotations = []
-        # add ref img to first
-        candidate_imgnames.insert(0, self.imgdir + refimg)
-        candidate_cvals.insert(0, 1.0)
-        candidates.insert(0, refimg)
-        ann = []
-        for c, cval in enumerate(candidate_cvals):
-            if c < self.numsample:
-                shortened_imgname = self.shorten_imgname(candidates[c])
-                ann.append("{}:{:.4f}".format(shortened_imgname, cval))
-            else:
-                break
-        annotations.append(ann)
-        ylabels = ["Sorted Matches"]
-        candidate_imgnames = [candidate_imgnames]
-        self.fill_panel(candidate_imgnames, ylabels, annotations)
-        self.figure.suptitle(
-            "Top {} matches with Exclusion Distance of {} in {}".format(
-                self.numsample - 1, excdist, axis
-            ),
-            y=1.2,
-        )
-        self.set_xlabel(dists)
-
-
-class ImagePanelSingleSample(ImageGridV2):
-    def __init__(self, imgdir):
-        ImageGridV2.__init__(self, 4, 11)
-        self.imgdir = imgdir
-
-    def set_xlabel(self):
-        for i, ax in enumerate(self.grid):
-            r = i // self.col
-            c = i % self.col
-            if r == 0:
-                ax.set_title(
-                    "Exc. Dist = {}".format(c),
-                    fontsize=10,
-                    color="red",
-                    fontweight="bold",
-                )
-                ax.spines["bottom"].set_color("red")
-                ax.spines["bottom"].set_linewidth(4)
-            if r == 1:
-                ax.spines["top"].set_color("blue")
-                ax.spines["top"].set_linewidth(4)
-            if c == 0:
-                ax.spines["right"].set_color("red")
-                ax.spines["right"].set_linewidth(6)
-
-    def set_second_xlabel(self):
-        for i, ax in enumerate(self.grid):
-            r = i // self.col
-            c = i % self.col
-            if r == 3:
-                if c == 0:
-                    text = "Reference Image"
-                else:
-                    text = "N = {}".format(c)
-                ax.set_xlabel(text, fontsize=10, color="blue", fontweight="bold")
+    @staticmethod
+    def add_feature_activation_level_annotation(
+        graph_data_row_list: List[List[dc.GraphData]],
+        data_loader: dl.FeatureDirMatProcessor,
+        feature_dir: str,
+        thresholds: List[np.ndarray],
+    ) -> List[List[dc.GraphData]]:
+        for graph_data_row in graph_data_row_list:
+            for graph_data in graph_data_row:
+                FeatureActivationLevel.augment_graph_data_with_feature_activation_level(
+                    graph_data, data_loader, feature_dir, thresholds
+                )
+        return graph_data_row_list
 
-    def set_ylabel_color(self):
-        ylabel_colors = ["red", "blue", "black", "green"]
-        for i, ax in enumerate(self.grid):
-            r = i // self.col
-            c = i % self.col
-            if c == 0:
-                ax.yaxis.label.set_color(ylabel_colors[r])
-
-    def fill_single_sample_panel(self, sampled_imgname, row_infos):
-        blank_dir = PROJECT_DIR
-        imnames = []
-        annotations = []
-        obj_codes = sampled_imgname.split("_")
-        series_name = obj_codes[1].split("-")[1]
-        shortened_imgname = (
-            obj_codes[0] + "_" + obj_codes[1][0:4] + "-{}".format(series_name)
-        )
-        for i, item in enumerate(row_infos):
-            if i == 0:
-                row = list(item[1])
-                row = [
-                    blank_dir + img if img == "blank.png" else self.imgdir + img
-                    for img in row
-                ]
-                reference_img = row[0]
-                imnames.append(row)
-                ann = []
-                for idx, img in enumerate(item[1]):
-                    if img != "blank.png":
-                        series_name = img.split("_")[1]
-                        series_name = series_name.split("-")[1]
-                        series_name = series_name.split(".")[0]
-                        ann.append("{}:{:.4f}".format(series_name, item[0][idx]))
-                    else:
-                        ann.append("")
-                ann[0] = shortened_imgname
-                annotations.append(ann)
-            else:
-                row = [self.imgdir + img for img in item[1]]
-                row.insert(0, reference_img)
-                imnames.append(row)
-                ann = []
-                for idx, img in enumerate(item[1]):
-                    objname = img.split("_")
-                    objcode = objname[0] + "_" + objname[1].split("-")[0][0:4]
-                    ann.append("{}:{:.4f}".format(objcode, item[0][idx]))
-                ann.insert(0, shortened_imgname)
-                annotations.append(ann)
-
-        ylabels = [
-            "Within Same Obj",
-            "Top 11 Any Other Obj",
-            "Top 11 Per Obj",
-            "Top 11 Per Obj Category",
-        ]
-        self.fill_panel(imnames, ylabels, annotations)
-        self.set_xlabel()
-        self.set_second_xlabel()
-        self.set_ylabel_color()
-
-
-class ImagePanelTopPer(ImageGridV2):
-    def __init__(self, imgdir):
-        super().__init__(11, 12, axis_pad=0.07)
-        self.imgdir = imgdir
-
-    def shorten_imgname(self, imgname):
-        obj_codes = imgname.split("_")
-        series_name = obj_codes[1].split("-")[1]
-        series_name = series_name.split(".")[0]
-        shortened_imgname = (
-            obj_codes[0] + "_" + obj_codes[1][0:4] + "-{}".format(series_name)
-        )
-        return shortened_imgname
-
-    def change_border_color(self, border_colors):
-        for i, ax in enumerate(self.grid):
-            r = i // self.col
-            c = i % self.col
-            ax.set_axis_on()
-            matplotlib.pyplot.setp(
-                ax.spines.values(), color=border_colors[r][c], linewidth=2
-            )
 
-    def fill_top_per_panel(
-        self, sampled_imgnames, row_infos, axis, exclusion_dist, obj_cat=False
+class TuningCurve:
+    @staticmethod
+    def get_tuning_curve(
+        obj: str,
+        ax: str,
+        sameobj_corrmat: dc.CorrMat,
+        nn_analysis_config: dc.NNAnalysisConfig,
     ):
-        blank_dir = PROJECT_DIR
-        imnames = []
-        annotations = []
-        border_colors = []
-        for i, item in enumerate(row_infos):
-            row = list(item[1])
-            row.insert(0, sampled_imgnames[i])
-            obj_ref = sampled_imgnames[i].split("-")[0]
-            if obj_cat:
-                obj_ref = obj_ref.split("_")[0]
-            # red if correct obj / objcat
-            border_color_row = ["red" if obj_ref in img else "white" for img in row]
-            not_same_obj_idx = [i for i, n in enumerate(row) if obj_ref not in n][0]
-            if row[not_same_obj_idx] != "blank.png":
-                if obj_cat:
-                    border_color_row[not_same_obj_idx] = "green"
-                else:
-                    border_color_row[not_same_obj_idx] = "blue"
-            border_colors.append(border_color_row)
-            row = [
-                blank_dir + img if img == "blank.png" else self.imgdir + img
-                for img in row
-            ]
-            imnames.append(row)
-            ann = []
-            for idx, img in enumerate(item[1]):
-                if img != "blank.png":
-                    shortened_imgname = self.shorten_imgname(img)
-                    ann.append("{}:{:.4f}".format(shortened_imgname, item[0][idx]))
-                else:
-                    ann.append("")
-            ann.insert(0, "")
-            annotations.append(ann)
-
-        ylabels = [self.shorten_imgname(imname) for imname in sampled_imgnames]
-        self.fill_panel(imnames, ylabels, annotations)
-        if not obj_cat:
-            self.figure.suptitle(
-                "Top Per Object with Exclusion Distance of {} in {}".format(
-                    exclusion_dist, axis
-                ),
-                fontsize=15,
-                y=0.9,
-            )
-        else:
-            self.figure.suptitle(
-                "Top Per Object Category with Exclusion Distance of {} in {}".format(
-                    exclusion_dist, axis
+        obj_ax_cutout_corrmat = nn.PrepData.cut_single_obj_ax_to_all_corrmat(
+            sameobj_corrmat, obj, ax
+        )
+        col_shapey_idxs = utils.IndexingHelper.objname_ax_to_shapey_index(obj, ax)
+        col_corrmat_idxs, available_shapey_idxs = obj_ax_cutout_corrmat.description[
+            1
+        ].shapey_idx_to_corrmat_idx(col_shapey_idxs)
+        col_corrmat_idxs = typing.cast(List[int], col_corrmat_idxs)
+        row_shapey_idxs = utils.IndexingHelper.objname_ax_to_shapey_index(obj, ax)
+        row_corrmat_idxs, available_shapey_idxs = obj_ax_cutout_corrmat.description[
+            0
+        ].shapey_idx_to_corrmat_idx(row_shapey_idxs)
+        row_corrmat_idxs = typing.cast(List[int], row_corrmat_idxs)
+        assert row_corrmat_idxs == list(range(utils.NUMBER_OF_VIEWS_PER_AXIS))
+        sameobj_ax_corrmat = obj_ax_cutout_corrmat.get_subset(
+            row_corrmat_idxs, col_corrmat_idxs
+        )
+        sameobj_ax_corrmat_np = sameobj_ax_corrmat.corrmat
+        assert sameobj_ax_corrmat_np.shape == (
+            utils.NUMBER_OF_VIEWS_PER_AXIS,
+            utils.NUMBER_OF_VIEWS_PER_AXIS,
+        )
+        # save out as graphdata
+        graph_data_list: List[dc.GraphData] = []
+        for r in range(11):
+            parsed_imgname = utils.ImageNameHelper.parse_shapey_idx(row_shapey_idxs[r])
+            tuning_curve = dc.GraphData(
+                x_label="series idx",
+                y_label=nn_analysis_config.distance_measure,
+                x=np.arange(1, utils.NUMBER_OF_VIEWS_PER_AXIS + 1, 1),
+                y=np.array([0, 1]),
+                data=sameobj_ax_corrmat_np[r, :],
+                label="{}-{:2d}".format(
+                    parsed_imgname["ax"], int(parsed_imgname["series_idx"])
                 ),
-                fontsize=15,
-                y=0.9,
             )
-        self.change_border_color(border_colors)
+            graph_data_list.append(tuning_curve)
+        graph_group = dc.GraphDataGroup(data=graph_data_list)
+        return graph_group
+
+
+class FeatureActivationLevel:
+    @staticmethod
+    def get_feature_activation_level(
+        thresholds: List[np.ndarray], raw_features: List[np.ndarray]
+    ) -> List[float]:
+        assert len(thresholds) == len(raw_features)
+        feature_activation_level_list = []
+        for i, th in enumerate(thresholds):
+            feature = raw_features[i]
+            feature_activation_level = np.sum(feature > th) / feature.size
+            feature_activation_level_list.append(feature_activation_level)
+        return feature_activation_level_list
+
+    @staticmethod
+    def augment_graph_data_with_feature_activation_level(
+        graph_data: dc.GraphData,
+        data_loader: dl.FeatureDirMatProcessor,
+        feature_dir: str,
+        threshold: List[np.ndarray],
+    ) -> dc.GraphData:
+        assert isinstance(graph_data.data, str)
+        if graph_data.data == vis.BLANK_IMG:
+            return graph_data
+        assert graph_data.data in utils.SHAPEY200_IMGNAMES
+        assert os.path.exists(feature_dir)
+
+        feature_file_name = "features_" + graph_data.data.split(".")[0] + ".mat"
+        features = data_loader.load(feature_dir, feature_file_name, filter_key="l2pool")
+        features = [*features]
+        feature_activation_level = FeatureActivationLevel.get_feature_activation_level(
+            threshold, features
+        )
+        if graph_data.supplementary_data is None:
+            graph_data.supplementary_data = {}
+        typing.cast(Dict, graph_data.supplementary_data)[
+            "feature_activation_level"
+        ] = feature_activation_level
+        return graph_data
+
+    @staticmethod
+    def add_feature_activation_level_imgpanel_data(
+        graph_data_row_list: List[List[dc.GraphData]],
+        data_loader: dl.FeatureDirMatProcessor,
+        feature_dir: str,
+        threshold: List[np.ndarray],
+    ):
+        graph_data_row_list_augmented = []
+        for graph_data_row in graph_data_row_list:
+            graph_data_row_augmented = []
+            for graph_data in graph_data_row:
+                graph_data = FeatureActivationLevel.augment_graph_data_with_feature_activation_level(
+                    graph_data, data_loader, feature_dir, threshold
+                )
+                graph_data_row_augmented.append(graph_data)
+            graph_data_row_list_augmented.append(graph_data_row_augmented)
+        return graph_data_row_list_augmented
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/line_graph.py` & `ShapeYModular-2.0.2/shapeymodular/visualization/line_graph.py`

 * *Files identical despite different names*

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/styles.py` & `ShapeYModular-2.0.2/shapeymodular/visualization/styles.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 BLANK_IMG = os.path.join(os.path.dirname(__file__), "blank.png")
 MARKER_STYLES = [m for m in markers.MarkerStyle.markers if m not in ["None", "none"]]
 COLORS = cm.get_cmap("tab20", 20)
 LINE_STYLES = ["-", "--", "-.", ":"]
 LABEL_FONT_SIZE = 15
 TITLE_FONT_SIZE = 17
 TICK_FONT_SIZE = 15
-SHAPEY_IMG_DIR = os.environ.get("SHAPEY_IMG_DIR", "../data/ShapeY200/dataset/")
+SHAPEY_IMG_DIR = os.environ.get(
+    "SHAPEY_IMG_DIR", "/home/namj/projects/ShapeYAnalysis/data/ShapeY200/dataset"
+)
 ANNOTATION_FONT_SIZE = 7
+TEXT_FONT_SIZE = 8
 CORRECT_MATCH_COLOR = "blue"
-CORRECT_MATCH_BORDER_WIDTH = 4
+ERROR_DISPLAY_HIGHLIGHT_BORDER_WIDTH = 4
+INCORRECT_MATCH_COLOR = "red"
+CORRECT_CATEGORY_MATCH_COLOR = "green"
 
 
 def format_xdist_graph(
     fig: mplfig.Figure, ax: mplax.Axes
 ) -> Tuple[mplfig.Figure, mplax.Axes]:
     ax.set_xticks(list(range(-1, 10)))
     ax.set_yticks([0.0, 0.2, 0.4, 0.6, 0.8, 1.0])
```

### Comparing `ShapeYModular-2.0.1/shapeymodular/visualization/tuning_curve.py` & `ShapeYModular-2.0.2/shapeymodular/visualization/tuning_curve.py`

 * *Files identical despite different names*

