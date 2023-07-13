# Comparing `tmp/rod-0.1.dev86.tar.gz` & `tmp/rod-0.1.dev91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.1.dev86.tar", last modified: Wed Jul  5 07:32:10 2023, max compression
+gzip compressed data, was "rod-0.1.dev91.tar", last modified: Thu Jul 13 15:58:57 2023, max compression
```

## Comparing `rod-0.1.dev86.tar` & `rod-0.1.dev91.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.726205 rod-0.1.dev86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.722205 rod-0.1.dev86/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.722205 rod-0.1.dev86/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-05 07:31:53.000000 rod-0.1.dev86/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 07:31:53.000000 rod-0.1.dev86/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-05 07:31:53.000000 rod-0.1.dev86/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-05 07:31:53.000000 rod-0.1.dev86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-05 07:32:10.726205 rod-0.1.dev86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-05 07:31:53.000000 rod-0.1.dev86/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-05 07:31:53.000000 rod-0.1.dev86/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-05 07:32:10.730205 rod-0.1.dev86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:31:53.000000 rod-0.1.dev86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.722205 rod-0.1.dev86/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.722205 rod-0.1.dev86/src/rod/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.722205 rod-0.1.dev86/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.726205 rod-0.1.dev86/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.726205 rod-0.1.dev86/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.726205 rod-0.1.dev86/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.726205 rod-0.1.dev86/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.726205 rod-0.1.dev86/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-05 07:31:53.000000 rod-0.1.dev86/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:32:10.722205 rod-0.1.dev86/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-05 07:32:10.000000 rod-0.1.dev86/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-05 07:32:10.000000 rod-0.1.dev86/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:32:10.000000 rod-0.1.dev86/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:32:10.000000 rod-0.1.dev86/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 07:32:10.000000 rod-0.1.dev86/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-05 07:32:10.000000 rod-0.1.dev86/src/rod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.804683 rod-0.1.dev91/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-13 15:58:42.000000 rod-0.1.dev91/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 15:58:42.000000 rod-0.1.dev91/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 15:58:42.000000 rod-0.1.dev91/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-13 15:58:42.000000 rod-0.1.dev91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 15:58:57.812683 rod-0.1.dev91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-13 15:58:42.000000 rod-0.1.dev91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 15:58:42.000000 rod-0.1.dev91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-13 15:58:57.812683 rod-0.1.dev91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:58:42.000000 rod-0.1.dev91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.804683 rod-0.1.dev91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/builder/primitive_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/builder/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/kinematics/kinematic_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/kinematics/tree_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/physics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/src/rod/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/tree/directed_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/tree/tree_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/src/rod/urdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/urdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/urdf/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/src/rod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/frame_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/gazebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/resolve_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/resolve_uris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 15:58:42.000000 rod-0.1.dev91/tests/test_urdf_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 15:58:42.000000 rod-0.1.dev91/tests/utils_models.py
```

### Comparing `rod-0.1.dev86/.github/workflows/style.yml` & `rod-0.1.dev91/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/.gitignore` & `rod-0.1.dev91/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/LICENSE` & `rod-0.1.dev91/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/PKG-INFO` & `rod-0.1.dev91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev86
+Version: 0.1.dev91
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
@@ -29,14 +29,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment :: Simulation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: style
 Provides-Extra: pptree
+Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 # RObot Description processor
 
 **The ultimate Python tool for RObot Descriptions processing.**
```

### Comparing `rod-0.1.dev86/README.md` & `rod-0.1.dev91/README.md`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/setup.cfg` & `rod-0.1.dev91/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -61,18 +61,28 @@
 
 [options.extras_require]
 style = 
 	black
 	isort
 pptree = 
 	pptree
+test = 
+	idyntree
+	pytest
+	pytest-icdiff
+	robot-descriptions
 all = 
 	%(style)s
 	%(pptree)s
+	%(test)s
 
 [options.packages.find]
 where = src
 
+[tool:pytest]
+addopts = -rsxX -v --strict-markers
+testpaths = tests
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rod-0.1.dev86/src/rod/__init__.py` & `rod-0.1.dev91/src/rod/__init__.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/builder/primitive_builder.py` & `rod-0.1.dev91/src/rod/builder/primitive_builder.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/builder/primitives.py` & `rod-0.1.dev91/src/rod/builder/primitives.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/kinematics/kinematic_tree.py` & `rod-0.1.dev91/src/rod/kinematics/kinematic_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/kinematics/tree_transforms.py` & `rod-0.1.dev91/src/rod/kinematics/tree_transforms.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/logging.py` & `rod-0.1.dev91/src/rod/logging.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/pretty_printer.py` & `rod-0.1.dev91/src/rod/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/common.py` & `rod-0.1.dev91/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/element.py` & `rod-0.1.dev91/src/rod/sdf/element.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/geometry.py` & `rod-0.1.dev91/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/joint.py` & `rod-0.1.dev91/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/link.py` & `rod-0.1.dev91/src/rod/sdf/link.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/material.py` & `rod-0.1.dev91/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/model.py` & `rod-0.1.dev91/src/rod/sdf/model.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/physics.py` & `rod-0.1.dev91/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/scene.py` & `rod-0.1.dev91/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/sdf.py` & `rod-0.1.dev91/src/rod/sdf/sdf.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/sdf/world.py` & `rod-0.1.dev91/src/rod/sdf/world.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/tree/directed_tree.py` & `rod-0.1.dev91/src/rod/tree/directed_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/tree/tree_elements.py` & `rod-0.1.dev91/src/rod/tree/tree_elements.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/urdf/exporter.py` & `rod-0.1.dev91/src/rod/urdf/exporter.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/utils/frame_convention.py` & `rod-0.1.dev91/src/rod/utils/frame_convention.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/utils/gazebo.py` & `rod-0.1.dev91/src/rod/utils/gazebo.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/utils/resolve_frames.py` & `rod-0.1.dev91/src/rod/utils/resolve_frames.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod/utils/resolve_uris.py` & `rod-0.1.dev91/src/rod/utils/resolve_uris.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev86/src/rod.egg-info/PKG-INFO` & `rod-0.1.dev91/src/rod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev86
+Version: 0.1.dev91
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
@@ -29,14 +29,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment :: Simulation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: style
 Provides-Extra: pptree
+Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 # RObot Description processor
 
 **The ultimate Python tool for RObot Descriptions processing.**
```

### Comparing `rod-0.1.dev86/src/rod.egg-info/SOURCES.txt` & `rod-0.1.dev91/src/rod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,10 @@
 src/rod/tree/tree_elements.py
 src/rod/urdf/__init__.py
 src/rod/urdf/exporter.py
 src/rod/utils/__init__.py
 src/rod/utils/frame_convention.py
 src/rod/utils/gazebo.py
 src/rod/utils/resolve_frames.py
-src/rod/utils/resolve_uris.py
+src/rod/utils/resolve_uris.py
+tests/test_urdf_parsing.py
+tests/utils_models.py
```

