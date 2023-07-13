# Comparing `tmp/singletrack-ml-card-component-0.0.1.tar.gz` & `tmp/singletrack-ml-card-component-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singletrack-ml-card-component-0.0.1.tar", last modified: Thu Jul 13 13:09:11 2023, max compression
+gzip compressed data, was "singletrack-ml-card-component-0.0.2.tar", last modified: Thu Jul 13 13:44:40 2023, max compression
```

## Comparing `singletrack-ml-card-component-0.0.1.tar` & `singletrack-ml-card-component-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.101394 singletrack-ml-card-component-0.0.1/
--rw-r--r--   0 patrickcarson   (503) staff       (20)     1063 2023-07-13 12:52:39.000000 singletrack-ml-card-component-0.0.1/LICENSE
--rw-r--r--   0 patrickcarson   (503) staff       (20)       50 2023-07-13 12:58:24.000000 singletrack-ml-card-component-0.0.1/MANIFEST.in
--rw-r--r--   0 patrickcarson   (503) staff       (20)      191 2023-07-13 13:09:11.101273 singletrack-ml-card-component-0.0.1/PKG-INFO
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.098807 singletrack-ml-card-component-0.0.1/card_component/
--rw-r--r--   0 patrickcarson   (503) staff       (20)     4676 2023-07-13 12:52:39.000000 singletrack-ml-card-component-0.0.1/card_component/__init__.py
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.098168 singletrack-ml-card-component-0.0.1/card_component/frontend/
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.099245 singletrack-ml-card-component-0.0.1/card_component/frontend/build/
--rw-r--r--   0 patrickcarson   (503) staff       (20)      218 2023-07-13 13:04:15.000000 singletrack-ml-card-component-0.0.1/card_component/frontend/build/asset-manifest.json
--rw-r--r--   0 patrickcarson   (503) staff       (20)   197459 2023-07-13 13:04:11.000000 singletrack-ml-card-component-0.0.1/card_component/frontend/build/bootstrap.min.css
--rw-r--r--   0 patrickcarson   (503) staff       (20)      491 2023-07-13 13:04:15.000000 singletrack-ml-card-component-0.0.1/card_component/frontend/build/index.html
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.098276 singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.099787 singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/
--rw-r--r--   0 patrickcarson   (503) staff       (20)   458917 2023-07-13 13:04:15.000000 singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/main.1e267dda.js
--rw-r--r--   0 patrickcarson   (503) staff       (20)     1848 2023-07-13 13:04:15.000000 singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/main.1e267dda.js.LICENSE.txt
--rw-r--r--   0 patrickcarson   (503) staff       (20)  1716324 2023-07-13 13:04:15.000000 singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/main.1e267dda.js.map
--rw-r--r--   0 patrickcarson   (503) staff       (20)       38 2023-07-13 13:09:11.101437 singletrack-ml-card-component-0.0.1/setup.cfg
--rw-r--r--   0 patrickcarson   (503) staff       (20)      423 2023-07-13 13:08:58.000000 singletrack-ml-card-component-0.0.1/setup.py
-drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:09:11.101118 singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/
--rw-r--r--   0 patrickcarson   (503) staff       (20)      191 2023-07-13 13:09:10.000000 singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/PKG-INFO
--rw-r--r--   0 patrickcarson   (503) staff       (20)      645 2023-07-13 13:09:11.000000 singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/SOURCES.txt
--rw-r--r--   0 patrickcarson   (503) staff       (20)        1 2023-07-13 13:09:10.000000 singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/dependency_links.txt
--rw-r--r--   0 patrickcarson   (503) staff       (20)       16 2023-07-13 13:09:11.000000 singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/requires.txt
--rw-r--r--   0 patrickcarson   (503) staff       (20)       15 2023-07-13 13:09:11.000000 singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/top_level.txt
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.811152 singletrack-ml-card-component-0.0.2/
+-rw-r--r--   0 patrickcarson   (503) staff       (20)     1063 2023-07-13 12:52:39.000000 singletrack-ml-card-component-0.0.2/LICENSE
+-rw-r--r--   0 patrickcarson   (503) staff       (20)       50 2023-07-13 12:58:24.000000 singletrack-ml-card-component-0.0.2/MANIFEST.in
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      191 2023-07-13 13:44:40.811033 singletrack-ml-card-component-0.0.2/PKG-INFO
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.808621 singletrack-ml-card-component-0.0.2/card_component/
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      423 2023-07-13 13:42:41.000000 singletrack-ml-card-component-0.0.2/card_component/__init__.py
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.807970 singletrack-ml-card-component-0.0.2/card_component/frontend/
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.809055 singletrack-ml-card-component-0.0.2/card_component/frontend/build/
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      218 2023-07-13 13:43:12.000000 singletrack-ml-card-component-0.0.2/card_component/frontend/build/asset-manifest.json
+-rw-r--r--   0 patrickcarson   (503) staff       (20)   197459 2023-07-13 13:43:08.000000 singletrack-ml-card-component-0.0.2/card_component/frontend/build/bootstrap.min.css
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      491 2023-07-13 13:43:12.000000 singletrack-ml-card-component-0.0.2/card_component/frontend/build/index.html
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.808076 singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.809597 singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/
+-rw-r--r--   0 patrickcarson   (503) staff       (20)   458917 2023-07-13 13:43:12.000000 singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/main.1e267dda.js
+-rw-r--r--   0 patrickcarson   (503) staff       (20)     1848 2023-07-13 13:43:12.000000 singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/main.1e267dda.js.LICENSE.txt
+-rw-r--r--   0 patrickcarson   (503) staff       (20)  1716324 2023-07-13 13:43:12.000000 singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/main.1e267dda.js.map
+-rw-r--r--   0 patrickcarson   (503) staff       (20)       38 2023-07-13 13:44:40.811192 singletrack-ml-card-component-0.0.2/setup.cfg
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      423 2023-07-13 13:43:40.000000 singletrack-ml-card-component-0.0.2/setup.py
+drwxr-xr-x   0 patrickcarson   (503) staff       (20)        0 2023-07-13 13:44:40.810873 singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      191 2023-07-13 13:44:40.000000 singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/PKG-INFO
+-rw-r--r--   0 patrickcarson   (503) staff       (20)      645 2023-07-13 13:44:40.000000 singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickcarson   (503) staff       (20)        1 2023-07-13 13:44:40.000000 singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickcarson   (503) staff       (20)       16 2023-07-13 13:44:40.000000 singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/requires.txt
+-rw-r--r--   0 patrickcarson   (503) staff       (20)       15 2023-07-13 13:44:40.000000 singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/top_level.txt
```

### Comparing `singletrack-ml-card-component-0.0.1/LICENSE` & `singletrack-ml-card-component-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `singletrack-ml-card-component-0.0.1/card_component/frontend/build/bootstrap.min.css` & `singletrack-ml-card-component-0.0.2/card_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/main.1e267dda.js` & `singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/main.1e267dda.js`

 * *Files identical despite different names*

### Comparing `singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/main.1e267dda.js.LICENSE.txt` & `singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/main.1e267dda.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `singletrack-ml-card-component-0.0.1/card_component/frontend/build/static/js/main.1e267dda.js.map` & `singletrack-ml-card-component-0.0.2/card_component/frontend/build/static/js/main.1e267dda.js.map`

 * *Files identical despite different names*

### Comparing `singletrack-ml-card-component-0.0.1/singletrack_ml_card_component.egg-info/SOURCES.txt` & `singletrack-ml-card-component-0.0.2/singletrack_ml_card_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

