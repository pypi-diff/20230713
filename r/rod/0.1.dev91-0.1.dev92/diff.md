# Comparing `tmp/rod-0.1.dev91.tar.gz` & `tmp/rod-0.1.dev92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.1.dev91.tar", last modified: Thu Jul 13 15:58:57 2023, max compression
+gzip compressed data, was "rod-0.1.dev92.tar", last modified: Thu Jul 13 16:02:18 2023, max compression
```

## Comparing `rod-0.1.dev91.tar` & `rod-0.1.dev92.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.804683 rod-0.1.dev91/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-13 15:58:42.000000 rod-0.1.dev91/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 15:58:42.000000 rod-0.1.dev91/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 15:58:42.000000 rod-0.1.dev91/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-13 15:58:42.000000 rod-0.1.dev91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 15:58:57.812683 rod-0.1.dev91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-13 15:58:42.000000 rod-0.1.dev91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 15:58:42.000000 rod-0.1.dev91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-13 15:58:57.812683 rod-0.1.dev91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:58:42.000000 rod-0.1.dev91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.804683 rod-0.1.dev91/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 15:58:42.000000 rod-0.1.dev91/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.808683 rod-0.1.dev91/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 15:58:57.000000 rod-0.1.dev91/src/rod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:57.812683 rod-0.1.dev91/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 15:58:42.000000 rod-0.1.dev91/tests/test_urdf_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 15:58:42.000000 rod-0.1.dev91/tests/utils_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.243606 rod-0.1.dev92/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.235606 rod-0.1.dev92/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.235606 rod-0.1.dev92/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-13 16:02:03.000000 rod-0.1.dev92/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 16:02:03.000000 rod-0.1.dev92/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 16:02:03.000000 rod-0.1.dev92/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-13 16:02:03.000000 rod-0.1.dev92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 16:02:18.243606 rod-0.1.dev92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-13 16:02:03.000000 rod-0.1.dev92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 16:02:03.000000 rod-0.1.dev92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-13 16:02:18.243606 rod-0.1.dev92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:02:03.000000 rod-0.1.dev92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.235606 rod-0.1.dev92/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.235606 rod-0.1.dev92/src/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/src/rod/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/builder/primitive_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/builder/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/src/rod/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/kinematics/kinematic_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/kinematics/tree_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/src/rod/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/physics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/sdf/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/src/rod/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/tree/directed_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/tree/tree_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/src/rod/urdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/urdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/urdf/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/src/rod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/utils/frame_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/utils/gazebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/utils/resolve_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 16:02:03.000000 rod-0.1.dev92/src/rod/utils/resolve_uris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.235606 rod-0.1.dev92/src/rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 16:02:18.000000 rod-0.1.dev92/src/rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-13 16:02:18.000000 rod-0.1.dev92/src/rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:02:18.000000 rod-0.1.dev92/src/rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:02:17.000000 rod-0.1.dev92/src/rod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 16:02:18.000000 rod-0.1.dev92/src/rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 16:02:18.000000 rod-0.1.dev92/src/rod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:02:18.239606 rod-0.1.dev92/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 16:02:03.000000 rod-0.1.dev92/tests/test_urdf_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 16:02:03.000000 rod-0.1.dev92/tests/utils_models.py
```

### Comparing `rod-0.1.dev91/.github/workflows/ci_cd.yml` & `rod-0.1.dev92/.github/workflows/ci_cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -165,13 +165,13 @@
       - name: Inspect dist folder
         run: ls -lah dist/
 
       - name: Publish to PyPI
         if: |
           github.repository == 'ami-iit/rod' &&
           ((github.event_name == 'push' && github.ref == 'refs/heads/main') ||
-           (github.event_name == 'release'))
+           (github.event_name == 'release' && github.event.action == 'published'))
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
           skip_existing: true
```

### Comparing `rod-0.1.dev91/.github/workflows/style.yml` & `rod-0.1.dev92/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/.gitignore` & `rod-0.1.dev92/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/LICENSE` & `rod-0.1.dev92/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/PKG-INFO` & `rod-0.1.dev92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev91
+Version: 0.1.dev92
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
```

### Comparing `rod-0.1.dev91/README.md` & `rod-0.1.dev92/README.md`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/setup.cfg` & `rod-0.1.dev92/setup.cfg`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/__init__.py` & `rod-0.1.dev92/src/rod/__init__.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/builder/primitive_builder.py` & `rod-0.1.dev92/src/rod/builder/primitive_builder.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/builder/primitives.py` & `rod-0.1.dev92/src/rod/builder/primitives.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/kinematics/kinematic_tree.py` & `rod-0.1.dev92/src/rod/kinematics/kinematic_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/kinematics/tree_transforms.py` & `rod-0.1.dev92/src/rod/kinematics/tree_transforms.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/logging.py` & `rod-0.1.dev92/src/rod/logging.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/pretty_printer.py` & `rod-0.1.dev92/src/rod/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/common.py` & `rod-0.1.dev92/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/element.py` & `rod-0.1.dev92/src/rod/sdf/element.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/geometry.py` & `rod-0.1.dev92/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/joint.py` & `rod-0.1.dev92/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/link.py` & `rod-0.1.dev92/src/rod/sdf/link.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/material.py` & `rod-0.1.dev92/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/model.py` & `rod-0.1.dev92/src/rod/sdf/model.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/physics.py` & `rod-0.1.dev92/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/scene.py` & `rod-0.1.dev92/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/sdf.py` & `rod-0.1.dev92/src/rod/sdf/sdf.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/sdf/world.py` & `rod-0.1.dev92/src/rod/sdf/world.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/tree/directed_tree.py` & `rod-0.1.dev92/src/rod/tree/directed_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/tree/tree_elements.py` & `rod-0.1.dev92/src/rod/tree/tree_elements.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/urdf/exporter.py` & `rod-0.1.dev92/src/rod/urdf/exporter.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/utils/frame_convention.py` & `rod-0.1.dev92/src/rod/utils/frame_convention.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/utils/gazebo.py` & `rod-0.1.dev92/src/rod/utils/gazebo.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/utils/resolve_frames.py` & `rod-0.1.dev92/src/rod/utils/resolve_frames.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod/utils/resolve_uris.py` & `rod-0.1.dev92/src/rod/utils/resolve_uris.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/src/rod.egg-info/PKG-INFO` & `rod-0.1.dev92/src/rod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev91
+Version: 0.1.dev92
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
```

### Comparing `rod-0.1.dev91/src/rod.egg-info/SOURCES.txt` & `rod-0.1.dev92/src/rod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/tests/test_urdf_parsing.py` & `rod-0.1.dev92/tests/test_urdf_parsing.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev91/tests/utils_models.py` & `rod-0.1.dev92/tests/utils_models.py`

 * *Files identical despite different names*

