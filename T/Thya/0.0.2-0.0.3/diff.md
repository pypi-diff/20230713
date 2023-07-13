# Comparing `tmp/Thya-0.0.2.tar.gz` & `tmp/Thya-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Thya-0.0.2.tar", last modified: Tue May  9 09:12:39 2023, max compression
+gzip compressed data, was "Thya-0.0.3.tar", last modified: Thu Jul 13 14:34:57 2023, max compression
```

## Comparing `Thya-0.0.2.tar` & `Thya-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 09:12:30.000000 Thya-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 09:12:30.000000 Thya-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-09 09:12:39.668153 Thya-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-09 09:12:30.000000 Thya-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/Thya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 09:12:39.668153 Thya-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-09 09:12:30.000000 Thya-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/thya/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/thya/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/data/example.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-13 14:34:40.000000 Thya-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 14:34:40.000000 Thya-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 14:34:57.875403 Thya-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 14:34:40.000000 Thya-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.871403 Thya-0.0.3/Thya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 14:34:57.000000 Thya-0.0.3/Thya.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 14:34:57.875403 Thya-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 14:34:40.000000 Thya-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/thya/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/apis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/thya/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/boundingboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/imagelabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/convert/polygons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:34:57.875403 Thya-0.0.3/thya/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/data/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-13 14:34:40.000000 Thya-0.0.3/thya/summarize.py
```

### Comparing `Thya-0.0.2/LICENSE` & `Thya-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Thya-0.0.2/PKG-INFO` & `Thya-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thya
-Version: 0.0.2
+Version: 0.0.3
 Summary: ThyaTechnology SDK
 Home-page: https://github.com/ThyaTechnology/thya
 Author: Silvio Giancola
 Author-email: silvio@thya-technology.com
 License: GNU Affero General Public License v3.0
 Keywords: Thya,Technology,SDK,Cloud,Computer Vision,Object Detection,Instance Segmentation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Thya-0.0.2/Thya.egg-info/PKG-INFO` & `Thya-0.0.3/Thya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thya
-Version: 0.0.2
+Version: 0.0.3
 Summary: ThyaTechnology SDK
 Home-page: https://github.com/ThyaTechnology/thya
 Author: Silvio Giancola
 Author-email: silvio@thya-technology.com
 License: GNU Affero General Public License v3.0
 Keywords: Thya,Technology,SDK,Cloud,Computer Vision,Object Detection,Instance Segmentation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Thya-0.0.2/setup.py` & `Thya-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     #     'SoccerNet/data/*.json', 'SoccerNet/data/SNMOT*.txt']},
     # include_package_data=True,
     install_requires=[
         'requests',
         'tqdm',
         'xmltodict',
         # 'opencv-python',
-        'imagesize'
+        'imagesize',
+        'xlsxwriter'
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 3 - Alpha',
         # Define that your audience are developers
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

### Comparing `Thya-0.0.2/thya/apis.py` & `Thya-0.0.3/thya/apis.py`

 * *Files identical despite different names*

