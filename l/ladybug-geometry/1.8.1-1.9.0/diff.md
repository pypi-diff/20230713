# Comparing `tmp/ladybug-geometry-1.8.1.tar.gz` & `tmp/ladybug-geometry-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-geometry-1.8.1.tar", last modified: Tue Nov 26 01:32:00 2019, max compression
+gzip compressed data, was "dist/ladybug-geometry-1.9.0.tar", last modified: Sat Jan 18 20:09:23 2020, max compression
```

## Comparing `ladybug-geometry-1.8.1.tar` & `ladybug-geometry-1.9.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/.github/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1746 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/.github/project-manager.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/docs/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/_templates/layout.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/docs/_build/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/docs/_build/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/_build/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/_build/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/_build/.nojekyll
--rw-rw-r--   0 travis    (2000) travis    (2000)      376 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     7123 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      489 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/modules.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)      899 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/docs/_static/custom.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     9045 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3447 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/_2d.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7767 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/line.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16470 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/pointvector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11317 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/arc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4313 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/_1d.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3826 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/ray.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13520 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/plane.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35086 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/polyface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6448 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/sphere.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22427 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/mesh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81100 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/face.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13914 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/_mesh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7524 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/intersection3d.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3243 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/_2d.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7392 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/line.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13508 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/pointvector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14546 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/arc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3094 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/_1d.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/ray.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35230 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/polygon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24727 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/mesh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8789 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/intersection2d.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/ladybug_geometry/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7715 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tox.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9045 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/ladybug_geometry.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      987 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/deploy.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 01:32:00.000000 ladybug-geometry-1.8.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18366 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/mesh2d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8071 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/pointvector2d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15696 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/plane_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8257 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/line2d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46014 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/face3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5313 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/ray2d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31054 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/polyface3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10697 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/arc2d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9316 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/pointvector3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24994 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/polygon2d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15609 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/mesh3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5150 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/sphere3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9788 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/line3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6152 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/ray3d_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11154 2019-11-26 01:31:15.000000 ladybug-geometry-1.8.1/tests/arc3d_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/.github/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1746 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/.github/project-manager.yml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/docs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/docs/_templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/_templates/layout.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/docs/_build/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/docs/_build/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/_build/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/_build/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/_build/.nojekyll
+-rw-rw-r--   0 travis    (2000) travis    (2000)      376 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7123 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      489 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/modules.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/docs/_static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      899 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/docs/_static/custom.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9045 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/_2d.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7979 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/line.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16600 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/pointvector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11700 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/arc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/_1d.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3962 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/ray.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13699 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/plane.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35454 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/polyface.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6844 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/sphere.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22801 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/mesh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81443 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/face.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14457 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/_mesh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7524 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/intersection3d.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/_2d.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7600 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/line.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13648 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/pointvector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14914 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/arc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3474 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/_1d.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2932 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/ray.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35520 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/polygon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25101 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/mesh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8789 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/intersection2d.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/ladybug_geometry/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7715 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      215 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9045 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       17 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/ladybug_geometry.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      987 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/dev-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      972 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/deploy.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 20:09:23.000000 ladybug-geometry-1.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18894 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/mesh2d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8440 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/pointvector2d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16132 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/plane_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8664 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/line2d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46600 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/face3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5695 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/ray2d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31931 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/polyface3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11076 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/arc2d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9674 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/pointvector3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25544 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/polygon2d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16158 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/mesh3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5568 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/sphere3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10204 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/line3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6551 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/ray3d_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11570 2020-01-18 20:08:42.000000 ladybug-geometry-1.9.0/tests/arc3d_test.py
```

### Comparing `ladybug-geometry-1.8.1/.github/project-manager.yml` & `ladybug-geometry-1.9.0/.github/project-manager.yml`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/docs/_templates/layout.html` & `ladybug-geometry-1.9.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/docs/conf.py` & `ladybug-geometry-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/docs/_static/custom.css` & `ladybug-geometry-1.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/PKG-INFO` & `ladybug-geometry-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-geometry
-Version: 1.8.1
+Version: 1.9.0
 Summary: Ladybug geometry is a Python library that houses all of the basic geometry computation needed for Ladybug Tools core libraries.
 Home-page: https://github.com/ladybug-tools/ladybug-geometry
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: 
         ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/_2d.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/_2d.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,121 @@
 # coding=utf-8
-"""Base class for 2D geometries in sD space (Surface3D and Mesh3D)."""
+"""Base class for 2D geometries in 2D space (Polygon2D and Mesh2D)."""
 from __future__ import division
 
-from .pointvector import Point3D
+from .pointvector import Point2D
 
 
-class Base2DIn3D(object):
-    """Base class for 2D geometries in 3D space (Surface3D and Mesh3D).
-
-    Args:
-        vertices: A list of Point3D objects representing the vertices.
+class Base2DIn2D(object):
+    """Base class for 2D geometries in 2D space (Polygon2D and Mesh2D).
 
     Properties:
         * vertices
         * min
         * max
         * center
     """
     __slots__ = ('_vertices', '_min', '_max', '_center')
 
     def __init__(self, vertices):
-        """Initilize Base2DIn3D.
+        """Initilize Base2DIn2D.
+
+        Args:
+            vertices: A list of Point2D objects representing the vertices.
         """
         self._vertices = self._check_vertices_input(vertices)
         self._min = None
         self._max = None
         self._center = None
 
     @property
     def vertices(self):
         """Tuple of all vertices in this object."""
         return self._vertices
 
     @property
     def min(self):
-        """A Point3D for the minimum bounding box vertex around this geometry."""
+        """A Point2D for the minimum bounding rectangle vertex around this geometry."""
         if self._min is None:
             self._calculate_min_max()
         return self._min
 
     @property
     def max(self):
-        """A Point3D for the maximum bounding box vertex around this geometry."""
+        """A Point2D for the maximum bounding rectangle vertex around this geometry."""
         if self._max is None:
             self._calculate_min_max()
         return self._max
 
     @property
     def center(self):
-        """A Point3D for the center of the bounding box around this geometry."""
+        """A Point2D for the center of the bounding rectangle around this geometry."""
         if self._center is None:
             min, max = self.min, self.max
-            self._center = Point3D(
-                (min.x + max.x) / 2, (min.y + max.y) / 2, (min.z + max.z) / 2)
+            self._center = Point2D((min.x + max.x) / 2, (min.y + max.y) / 2)
         return self._center
 
     def duplicate(self):
         """Get a copy of this object."""
         return self.__copy__()
 
     def _calculate_min_max(self):
-        """Calculate maximum and minimum Point3D for this object."""
-        min_pt = [self.vertices[0].x, self.vertices[0].y, self.vertices[0].z]
-        max_pt = [self.vertices[0].x, self.vertices[0].y, self.vertices[0].z]
+        """Calculate maximum and minimum Point2D for this object."""
+        min_pt = [self.vertices[0].x, self.vertices[0].y]
+        max_pt = [self.vertices[0].x, self.vertices[0].y]
 
         for v in self.vertices[1:]:
             if v.x < min_pt[0]:
                 min_pt[0] = v.x
             elif v.x > max_pt[0]:
                 max_pt[0] = v.x
             if v.y < min_pt[1]:
                 min_pt[1] = v.y
             elif v.y > max_pt[1]:
                 max_pt[1] = v.y
-            if v.z < min_pt[2]:
-                min_pt[2] = v.z
-            elif v.z > max_pt[2]:
-                max_pt[2] = v.z
 
-        self._min = Point3D(min_pt[0], min_pt[1], min_pt[2])
-        self._max = Point3D(max_pt[0], max_pt[1], max_pt[2])
+        self._min = Point2D(min_pt[0], min_pt[1])
+        self._max = Point2D(max_pt[0], max_pt[1])
 
     def _check_vertices_input(self, vertices):
         if not isinstance(vertices, tuple):
             vertices = tuple(vertices)
         assert len(vertices) >= 3, 'There must be at least 3 vertices for a {}.' \
             ' Got {}'.format(self.__class__.__name__, len(vertices))
         for vert in vertices:
-            assert isinstance(vert, Point3D), \
-                'Expected Point3D for {} vertex. Got {}.'.format(
+            assert isinstance(vert, Point2D), \
+                'Expected Point2D for {} vertex. Got {}.'.format(
                     self.__class__.__name__, type(vert))
         return vertices
 
     def __len__(self):
-        return len(self.vertices)
+        return len(self._vertices)
 
     def __getitem__(self, key):
-        return self.vertices[key]
+        return self._vertices[key]
 
     def __iter__(self):
-        return iter(self.vertices)
+        return iter(self._vertices)
 
     def __copy__(self):
-        return Base2DIn3D(self._vertices)
+        return Base2DIn2D(self._vertices)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Base2DIn2D) and self.__key() == other.__key()
+    
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
-        """Base2Din3D representation."""
-        return 'Base 2D Object (3D Space)'
+        """Base2Din2D representation."""
+        return 'Base 2D Object (2D Space)'
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/line.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,18 +208,25 @@
         return base
 
     def _u_in(self, u):
         return u >= 0.0 and u <= 1.0
 
     def __abs__(self):
         return abs(self.v)
+    
+    def __copy__(self):
+        return LineSegment3D(self.p, self.v)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.p), hash(self.v))
+
+    def __hash__(self):
+        return hash(self.__key())
 
     def __eq__(self, other):
-        if isinstance(other, LineSegment3D):
-            return self.p == other.p and self.v == other.v
-        else:
-            return False
+        return isinstance(other, LineSegment3D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'LineSegment3D (<%.2f, %.2f, %.2f> to <%.2f, %.2f, %.2f>)' % \
             (self.p.x, self.p.y, self.p.z,
              self.p.x + self.v.x, self.p.y + self.v.y, self.p.z + self.v.z)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/pointvector.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/pointvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,20 +199,25 @@
         dt = (u * x + v * y + w * z) * (1 - ct) / r2
         return Vector3D((u * dt + x * ct + (-w * y + v * z) * st),
                         (v * dt + y * ct + (w * x - u * z) * st),
                         (w * dt + z * ct + (-v * x + u * y) * st))
 
     def __copy__(self):
         return self.__class__(self.x, self.y, self.z)
+    
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (self.x, self.y, self.z)
+
+    def __hash__(self):
+        return hash(self.__key())
 
     def __eq__(self, other):
-        if isinstance(other, (Vector3D, Point3D)):
-            return self.x == other.x and self.y == other.y and self.z == other.z
-        else:
-            return False
+        return isinstance(other, (Vector3D, Point3D)) and \
+            self.__key() == other.__key()
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __nonzero__(self):
         return self.x != 0 or self.y != 0 or self.z != 0
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/arc.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/arc.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,28 @@
             v2 = pt3 - pt1
             n = v1.cross(v2)
         except Exception as e:
             raise ValueError('Incorrect Point3D input for Arc3D:\n\t{}'.format(e))
         return Plane(n, pt1)
 
     def __copy__(self):
-        return self.__class__(self.plane, self.radius, self.a1, self.a2)
+        return Arc3D(self.plane, self.radius, self.a1, self.a2)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.plane), self.radius, self.a1, self.a2)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Arc3D) and self.__key() == other.__key()
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         return 'Arc3D (center {}) (radius {}) (length {})'.format(
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/_1d.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,27 @@
     def to_dict(self):
         """Get LineSegment3D/Ray3D as a dictionary."""
         return {'p': self.p.to_array(),
                 'v': self.v.to_array()}
 
     def __copy__(self):
         return self.__class__(self.p, self.v)
+    
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.p), hash(self.v))
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Base1DIn3D) and self.__key() == other.__key()
+    
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         """Base1Din3D representation."""
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/ray.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/ray.py`

 * *Files 16% similar despite different names*

```diff
@@ -94,20 +94,24 @@
         """Get Ray3D as a dictionary."""
         base = Base1DIn3D.to_dict(self)
         base['type'] = 'Ray3D'
         return base
 
     def _u_in(self, u):
         return u >= 0.0
+    
+    def __copy__(self):
+        return Ray3D(self.p, self.v)
 
-    def __eq__(self, other):
-        if isinstance(other, Ray3D):
-            return self.p == other.p and self.v == other.v
-        else:
-            return False
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.p), hash(self.v))
+
+    def __hash__(self):
+        return hash(self.__key())
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
+    def __eq__(self, other):
+        return isinstance(other, Ray3D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'Ray3D (point <%.2f, %.2f, %.2f>) (vector <%.2f, %.2f, %.2f>)' % \
             (self.p.x, self.p.y, self.p.z, self.v.x, self.v.y, self.v.z)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/plane.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/plane.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,21 +357,28 @@
         """Get Plane as a dictionary."""
         return {'type': 'Plane',
                 'n': self.n.to_array(),
                 'o': self.o.to_array(),
                 'x': self.x.to_array()}
 
     def __copy__(self):
-        return self.__class__(self.n, self.o)
+        return Plane(self.n, self.o, self.x)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (self.n, self.o, self.x)
+
+    def __hash__(self):
+        return hash(self.__key())
 
     def __eq__(self, other):
-        if isinstance(other, Plane):
-            return self.n == other.n and self.o == other.o and self.x == other.x
-        else:
-            return False
+        return isinstance(other, Plane) and self.__key() == other.__key()
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         return 'Plane (<%.2f, %.2f, %.2f> normal) (<%.2f, %.2f, %.2f> origin)' % \
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/polyface.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/polyface.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,21 @@
         edge_information: Optional edge information, which will speed up the
             creation of the Polyface object if it is available but should be left
             as None if it is unknown. If None, edge_information will be computed
             from the vertices and face_indices inuputs. Edge information
             should be formatted as a dictionary with two keys as follows:
 
             *   'edge_indices':
-                A list of tuple objects that each contain two integers.
+                An array objects that each contain two integers.
                 These integers correspond to indices within the vertices list and
                 each tuple represents a line sengment for an edge of the polyface.
             *   'edge_types':
-                A list of integers for each edge that parallels
-                the edge_indices list. An integer of 0 denotes a naked edge, an
-                integer of 1 denotes an internal edge. Anything higher is a
-                non-manifold edge.
+                An array of integers for each edge that parallels the edge_indices
+                list. An integer of 0 denotes a naked edge, an integer of 1
+                denotes an internal edge. Anything higher is a non-manifold edge.
 
     Properties:
         * vertices
         * faces
         * edges
         * naked_edges
         * internal_edges
@@ -803,11 +802,22 @@
             [(st_i + len_faces * 2 - 1, st_i + len_faces)]
         return verts, faces_ind, edge_indices
 
     def __copy__(self):
         _new_poly = Polyface3D(self.vertices, self.face_indices, self.edge_information)
         _new_poly._faces = self._faces
         return _new_poly
+    
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices) + \
+            tuple(hash(face) for face in self._face_indices)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Polyface3D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'Polyface3D ({} faces) ({} vertices)'.format(
             len(self.faces), len(self))
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/sphere.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/sphere.py`

 * *Files 6% similar despite different names*

```diff
@@ -183,19 +183,33 @@
 
     def duplicate(self):
         """Get a copy of this object."""
         return self.__copy__()
 
     def to_dict(self):
         """Get Sphere as a dictionary."""
-        return {'type': 'Sphere3D', 'center': self.center.to_array(),
+        return {'type': 'Sphere3D',
+                'center': self.center.to_array(),
                 'radius': self.radius}
 
     def __copy__(self):
-        return Sphere3D(self.center, self.radius)
+        return Sphere3D(self._center, self._radius)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (self._center, self._radius)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Sphere3D) and self.__key() == other.__key()
+    
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         return 'Sphere3D (center {}) (radius {}))'.format(self.center, self.radius)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/mesh.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,10 +549,21 @@
         _new_mesh = Mesh3D(self.vertices, self.faces)
         self._transfer_properties(_new_mesh)
         _new_mesh._face_centroids = self._face_centroids
         _new_mesh._face_normals = self._face_normals
         _new_mesh._vertex_normals = self._vertex_normals
         return _new_mesh
 
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices) + \
+            tuple(hash(face) for face in self._faces)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Mesh3D) and self.__key() == other.__key()
+
     def __repr__(self):
         return 'Mesh3D ({} faces) ({} vertices)'.format(
             len(self.faces), len(self))
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry3d/face.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/face.py`

 * *Files 1% similar despite different names*

```diff
@@ -1726,10 +1726,20 @@
         _new_face = Face3D(self.vertices, self.plane)
         self._transfer_properties(_new_face)
         _new_face._holes = self._holes
         _new_face._polygon2d = self._polygon2d
         _new_face._mesh2d = self._mesh2d
         _new_face._mesh3d = self._mesh3d
         return _new_face
+    
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices) + (hash(self._plane),)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Face3D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'Face3D ({} vertices)'.format(len(self))
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/_mesh.py` & `ladybug-geometry-1.9.0/ladybug_geometry/_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,21 +327,38 @@
                     vertices.append(v)
                     ind.append(ver_counter)
                     ver_counter += 1
                 face_collector.append(tuple(ind))
         return vertices, face_collector
 
     def __len__(self):
-        return len(self.vertices)
+        return len(self._vertices)
 
     def __getitem__(self, key):
-        return self.vertices[key]
+        return self._vertices[key]
 
     def __iter__(self):
-        return iter(self.vertices)
+        return iter(self._vertices)
+
+    def __copy__(self):
+        return MeshBase(self._vertices, self._faces, self._colors)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices) + \
+            tuple(hash(face) for face in self._faces)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, MeshBase) and self.__key() == other.__key()
+    
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         """Base MEsh representation."""
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/intersection3d.py` & `ladybug-geometry-1.9.0/ladybug_geometry/intersection3d.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/_2d.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry3d/_2d.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,126 @@
 # coding=utf-8
-"""Base class for 2D geometries in 2D space (Polygon2D and Mesh2D)."""
+"""Base class for 2D geometries in sD space (Surface3D and Mesh3D)."""
 from __future__ import division
 
-from .pointvector import Point2D
+from .pointvector import Point3D
 
 
-class Base2DIn2D(object):
-    """Base class for 2D geometries in 2D space (Polygon2D and Mesh2D).
+class Base2DIn3D(object):
+    """Base class for 2D geometries in 3D space (Surface3D and Mesh3D).
+
+    Args:
+        vertices: A list of Point3D objects representing the vertices.
 
     Properties:
         * vertices
         * min
         * max
         * center
     """
     __slots__ = ('_vertices', '_min', '_max', '_center')
 
     def __init__(self, vertices):
-        """Initilize Base2DIn2D.
-
-        Args:
-            vertices: A list of Point2D objects representing the vertices.
+        """Initilize Base2DIn3D.
         """
         self._vertices = self._check_vertices_input(vertices)
         self._min = None
         self._max = None
         self._center = None
 
     @property
     def vertices(self):
         """Tuple of all vertices in this object."""
         return self._vertices
 
     @property
     def min(self):
-        """A Point2D for the minimum bounding rectangle vertex around this geometry."""
+        """A Point3D for the minimum bounding box vertex around this geometry."""
         if self._min is None:
             self._calculate_min_max()
         return self._min
 
     @property
     def max(self):
-        """A Point2D for the maximum bounding rectangle vertex around this geometry."""
+        """A Point3D for the maximum bounding box vertex around this geometry."""
         if self._max is None:
             self._calculate_min_max()
         return self._max
 
     @property
     def center(self):
-        """A Point2D for the center of the bounding rectangle around this geometry."""
+        """A Point3D for the center of the bounding box around this geometry."""
         if self._center is None:
             min, max = self.min, self.max
-            self._center = Point2D((min.x + max.x) / 2, (min.y + max.y) / 2)
+            self._center = Point3D(
+                (min.x + max.x) / 2, (min.y + max.y) / 2, (min.z + max.z) / 2)
         return self._center
 
     def duplicate(self):
         """Get a copy of this object."""
         return self.__copy__()
 
     def _calculate_min_max(self):
-        """Calculate maximum and minimum Point2D for this object."""
-        min_pt = [self.vertices[0].x, self.vertices[0].y]
-        max_pt = [self.vertices[0].x, self.vertices[0].y]
+        """Calculate maximum and minimum Point3D for this object."""
+        min_pt = [self.vertices[0].x, self.vertices[0].y, self.vertices[0].z]
+        max_pt = [self.vertices[0].x, self.vertices[0].y, self.vertices[0].z]
 
         for v in self.vertices[1:]:
             if v.x < min_pt[0]:
                 min_pt[0] = v.x
             elif v.x > max_pt[0]:
                 max_pt[0] = v.x
             if v.y < min_pt[1]:
                 min_pt[1] = v.y
             elif v.y > max_pt[1]:
                 max_pt[1] = v.y
+            if v.z < min_pt[2]:
+                min_pt[2] = v.z
+            elif v.z > max_pt[2]:
+                max_pt[2] = v.z
 
-        self._min = Point2D(min_pt[0], min_pt[1])
-        self._max = Point2D(max_pt[0], max_pt[1])
+        self._min = Point3D(min_pt[0], min_pt[1], min_pt[2])
+        self._max = Point3D(max_pt[0], max_pt[1], max_pt[2])
 
     def _check_vertices_input(self, vertices):
         if not isinstance(vertices, tuple):
             vertices = tuple(vertices)
         assert len(vertices) >= 3, 'There must be at least 3 vertices for a {}.' \
             ' Got {}'.format(self.__class__.__name__, len(vertices))
         for vert in vertices:
-            assert isinstance(vert, Point2D), \
-                'Expected Point2D for {} vertex. Got {}.'.format(
+            assert isinstance(vert, Point3D), \
+                'Expected Point3D for {} vertex. Got {}.'.format(
                     self.__class__.__name__, type(vert))
         return vertices
 
     def __len__(self):
-        return len(self.vertices)
+        return len(self._vertices)
 
     def __getitem__(self, key):
-        return self.vertices[key]
+        return self._vertices[key]
 
     def __iter__(self):
-        return iter(self.vertices)
+        return iter(self._vertices)
 
     def __copy__(self):
-        return Base2DIn2D(self._vertices)
+        return Base2DIn3D(self._vertices)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Base2DIn3D) and self.__key() == other.__key()
+    
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
-        """Base2Din2D representation."""
-        return 'Base 2D Object (2D Space)'
+        """Base2Din3D representation."""
+        return 'Base 2D Object (3D Space)'
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/line.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,16 +208,23 @@
 
     def _u_in(self, u):
         return u >= 0.0 and u <= 1.0
 
     def __abs__(self):
         return abs(self.v)
 
+    def __copy__(self):
+        return LineSegment2D(self.p, self.v)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.p), hash(self.v))
+
+    def __hash__(self):
+        return hash(self.__key())
+
     def __eq__(self, other):
-        if isinstance(other, LineSegment2D):
-            return self.p == other.p and self.v == other.v
-        else:
-            return False
+        return isinstance(other, LineSegment2D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'LineSegment2D (<%.2f, %.2f> to <%.2f, %.2f>)' % \
             (self.p.x, self.p.y, self.p.x + self.v.x, self.p.y + self.v.y)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/pointvector.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/pointvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,19 +183,24 @@
         """Hidden reflection method used by both Point2D and Vector2D."""
         d = 2 * (vec.x * normal.x + vec.y * normal.y)
         return Vector2D(vec.x - d * normal.x, vec.y - d * normal.y)
 
     def __copy__(self):
         return self.__class__(self.x, self.y)
 
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (self.x, self.y)
+
+    def __hash__(self):
+        return hash(self.__key())
+
     def __eq__(self, other):
-        if isinstance(other, (Vector2D, Point2D)):
-            return self.x == other.x and self.y == other.y
-        else:
-            return False
+        return isinstance(other, (Vector2D, Point2D)) and \
+            self.__key() == other.__key()
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __nonzero__(self):
         return self.x != 0 or self.y != 0
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/arc.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/arc.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,15 +393,28 @@
 
     def _cc_difference(self, angle):
         """Get counterclockwise different between an angle and the start of this arc."""
         _diff = angle - self.a1
         return _diff if not angle < self.a1 else 2 * math.pi + _diff
 
     def __copy__(self):
-        return self.__class__(self.c, self.r, self.a1, self.a2)
+        return Arc2D(self.c, self.r, self.a1, self.a2)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (self.c, self.r, self.a1, self.a2)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Arc2D) and self.__key() == other.__key()
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         return 'Arc2D (center <%.2f, %.2f>) (radius <%.2f>) (length <%.2f>)' % \
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/_1d.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/_1d.py`

 * *Files 25% similar despite different names*

```diff
@@ -97,14 +97,27 @@
         """Get LineSegment2D/Ray2D as a dictionary."""
         return {'p': self.p.to_array(),
                 'v': self.v.to_array()}
 
     def __copy__(self):
         return self.__class__(self.p, self.v)
 
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.p), hash(self.v))
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Base1DIn2D) and self.__key() == other.__key()
+    
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
     def ToString(self):
         """Overwrite .NET ToString."""
         return self.__repr__()
 
     def __repr__(self):
         """Base1Din2D representation."""
         return 'Base 1D Object (2D Space)'
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/ray.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/ray.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,19 +73,20 @@
         base = Base1DIn2D.to_dict(self)
         base['type'] = 'Ray2D'
         return base
 
     def _u_in(self, u):
         return u >= 0.0
 
-    def __eq__(self, other):
-        if isinstance(other, Ray2D):
-            return self.p == other.p and self.v == other.v
-        else:
-            return False
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return (hash(self.p), hash(self.v))
+
+    def __hash__(self):
+        return hash(self.__key())
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
+    def __eq__(self, other):
+        return isinstance(other, Ray2D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'Ray2D (point <%.2f, %.2f>) (vector <%.2f, %.2f>)' % \
             (self.p.x, self.p.y, self.v.x, self.v.y)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/polygon.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -827,12 +827,21 @@
         """
         _a = 0
         for i, pt in enumerate(vertices):
             _a += vertices[i - 1].x * pt.y - vertices[i - 1].y * pt.x
         return _a < 0
 
     def __copy__(self):
-        _new_poly = Polygon2D(self.vertices)
-        return _new_poly
+        return Polygon2D(self._vertices)
+
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Polygon2D) and self.__key() == other.__key()
 
     def __repr__(self):
         return 'Polygon2D ({} vertices)'.format(len(self))
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/geometry2d/mesh.py` & `ladybug-geometry-1.9.0/ladybug_geometry/geometry2d/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,10 +601,21 @@
     def __copy__(self):
         _new_mesh = Mesh2D(self.vertices, self.faces)
         self._transfer_properties(_new_mesh)
         _new_mesh._face_centroids = self._face_centroids
         _new_mesh._centroid = self._centroid
         return _new_mesh
 
+    def __key(self):
+        """A tuple based on the object properties, useful for hashing."""
+        return tuple(hash(pt) for pt in self._vertices) + \
+            tuple(hash(face) for face in self._faces)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    def __eq__(self, other):
+        return isinstance(other, Mesh2D) and self.__key() == other.__key()
+
     def __repr__(self):
         return 'Ladybug Mesh2D ({} faces) ({} vertices)'.format(
             len(self.faces), len(self))
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry/intersection2d.py` & `ladybug-geometry-1.9.0/ladybug_geometry/intersection2d.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/README.md` & `ladybug-geometry-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry.egg-info/PKG-INFO` & `ladybug-geometry-1.9.0/ladybug_geometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-geometry
-Version: 1.8.1
+Version: 1.9.0
 Summary: Ladybug geometry is a Python library that houses all of the basic geometry computation needed for Ladybug Tools core libraries.
 Home-page: https://github.com/ladybug-tools/ladybug-geometry
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: 
         ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
```

### Comparing `ladybug-geometry-1.8.1/ladybug_geometry.egg-info/SOURCES.txt` & `ladybug-geometry-1.9.0/ladybug_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/.travis.yml` & `ladybug-geometry-1.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/LICENSE` & `ladybug-geometry-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/setup.py` & `ladybug-geometry-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ladybug-geometry-1.8.1/tests/mesh2d_test.py` & `ladybug-geometry-1.9.0/tests/mesh2d_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,30 @@
     assert mesh.colors is None
 
     assert len(mesh.vertex_connected_faces) == 4
     for vf in mesh.vertex_connected_faces:
         assert len(vf) == 1
 
 
+def test_equality():
+    """Test the equality of Polygon2D objects."""
+    pts = (Point2D(0, 0), Point2D(0, 2), Point2D(2, 2), Point2D(2, 0))
+    pts_2 = (Point2D(0, 0), Point2D(0, 2), Point2D(2, 2), Point2D(2, 0.1))
+    mesh = Mesh2D(pts, [(0, 1, 2, 3)])
+    mesh_dup = mesh.duplicate()
+    mesh_alt = Mesh2D(pts_2, [(0, 1, 2, 3)])
+
+    assert mesh is mesh
+    assert mesh is not mesh_dup
+    assert mesh == mesh_dup
+    assert hash(mesh) == hash(mesh_dup)
+    assert mesh != mesh_alt
+    assert hash(mesh) != hash(mesh_alt)
+
+
 def test_mesh2d_to_from_dict():
     """Test the to/from dict of Mesh2D objects."""
     pts = (Point2D(0, 0), Point2D(0, 2), Point2D(2, 2), Point2D(2, 0))
     mesh = Mesh2D(pts, [(0, 1, 2, 3)])
     mesh_dict = mesh.to_dict()
     new_mesh = Mesh2D.from_dict(mesh_dict)
     assert isinstance(new_mesh, Mesh2D)
```

### Comparing `ladybug-geometry-1.8.1/tests/pointvector2d_test.py` & `ladybug-geometry-1.9.0/tests/pointvector2d_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,16 +59,30 @@
     assert pt_1.x == 0
     assert pt_1.y == 2
 
     pt_2 = Point2D(2, 2)
     assert pt_1.distance_to_point(pt_2) == 2
 
 
+def test_equality():
+    """Test the equality of Point2D objects."""
+    pt_1 = Point2D(0, 2)
+    pt_1_dup = pt_1.duplicate()
+    pt_1_alt = Point2D(0.1, 2)
+
+    assert pt_1 is pt_1
+    assert pt_1 is not pt_1_dup
+    assert pt_1 == pt_1_dup
+    assert hash(pt_1) == hash(pt_1_dup)
+    assert pt_1 != pt_1_alt
+    assert hash(pt_1) != hash(pt_1_alt)
+
+
 def test_is_equivalent():
-    """Test the is_equivalent method."""
+    """Test the is_equivalent method using tolerances."""
     pt_1 = Point2D(0, 2)
     pt_2 = Point2D(0.00001, 2)
     pt_3 = Point2D(0, 1)
 
     assert pt_1.is_equivalent(pt_2, 0.0001) is True
     assert pt_1.is_equivalent(pt_2, 0.0000001) is False
     assert pt_1.is_equivalent(pt_3, 0.0001) is False
```

### Comparing `ladybug-geometry-1.8.1/tests/plane_test.py` & `ladybug-geometry-1.9.0/tests/plane_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,30 @@
     assert plane_flip.o == Point3D(2, 0, 2)
     assert plane_flip.n == Vector3D(0, -1, 0)
     assert plane_flip.x == Vector3D(-1, 0, 0)
     assert plane_flip.y == Vector3D(0, 0, -1)
     assert plane_flip.k == 0
 
 
+def test_equality():
+    """Test the equality of Plane objects."""
+    pt = Point3D(2, 0, 2)
+    vec = Vector3D(0, 2, 0)
+    plane = Plane(vec, pt)
+    plane_dup = plane.duplicate()
+    plane_alt = Plane(vec, Point3D(2, 0.1, 2))
+
+    assert plane is plane
+    assert plane is not plane_dup
+    assert plane == plane_dup
+    assert hash(plane) == hash(plane_dup)
+    assert plane != plane_alt
+    assert hash(plane) != hash(plane_alt)
+
+
 def test_plane_to_from_dict():
     """Test the initalization of Plane objects and basic properties."""
     pt = Point3D(2, 0, 2)
     vec = Vector3D(0, 2, 0)
     plane = Plane(vec, pt)
     plane_dict = plane.to_dict()
     new_plane = Plane.from_dict(plane_dict)
```

### Comparing `ladybug-geometry-1.8.1/tests/line2d_test.py` & `ladybug-geometry-1.9.0/tests/line2d_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     assert seg.p == Point2D(2, 0)
     assert seg.v == Vector2D(0, 2)
     assert seg.p1 == Point2D(2, 0)
     assert seg.p2 == Point2D(2, 2)
     assert seg.length == 2
 
 
-def test_linesegment2_mutability():
-    """Test the mutability and immutability of LineSegement2D objects."""
+def test_linesegment2_immutability():
+    """Test the immutability of LineSegement2D objects."""
     pt = Point2D(2, 0)
     vec = Vector2D(0, 2)
     seg = LineSegment2D(pt, vec)
 
     assert isinstance(seg, LineSegment2D)
     with pytest.raises(AttributeError):
         seg.p.x = 3
@@ -82,14 +82,30 @@
         seg.v = Vector2D(2, 2)
 
     seg_copy = seg.duplicate()
     assert seg.p == seg_copy.p
     assert seg.v == seg_copy.v
 
 
+def test_equality():
+    """Test the equality of LineSegement2D objects."""
+    pt = Point2D(2, 0)
+    vec = Vector2D(0, 2)
+    seg = LineSegment2D(pt, vec)
+    seg_dup = seg.duplicate()
+    seg_alt = LineSegment2D(Point2D(2, 0.1), vec)
+
+    assert seg is seg
+    assert seg is not seg_dup
+    assert seg == seg_dup
+    assert hash(seg) == hash(seg_dup)
+    assert seg != seg_alt
+    assert hash(seg) != hash(seg_alt)
+
+
 def test_move():
     """Test the LineSegement2D move method."""
     pt = Point2D(2, 0)
     vec = Vector2D(0, 2)
     seg = LineSegment2D(pt, vec)
 
     vec_1 = Vector2D(2, 2)
```

### Comparing `ladybug-geometry-1.8.1/tests/face3d_test.py` & `ladybug-geometry-1.9.0/tests/face3d_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,31 @@
     assert face.perimeter == 8
     assert face.is_clockwise is False
     assert face.is_convex is True
     assert face.is_self_intersecting is False
     assert face.vertices[0] == face[0]
 
 
+def test_equality():
+    """Test the equality of Face3D objects."""
+    pts = (Point3D(0, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2))
+    pts_2 = (Point3D(0.1, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2))
+    plane = Plane(Vector3D(0, 0, 1), Point3D(0, 0, 2))
+    face = Face3D(pts, plane)
+    face_dup = face.duplicate()
+    face_alt = Face3D(pts_2, plane)
+
+    assert face is face
+    assert face is not face_dup
+    assert face == face_dup
+    assert hash(face) == hash(face_dup)
+    assert face != face_alt
+    assert hash(face) != hash(face_alt)
+
+
 def test_face3d_to_from_dict():
     """Test the to/from dict of Face3D objects."""
     pts = (Point3D(0, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2))
     plane = Plane(Vector3D(0, 0, 1), Point3D(0, 0, 2))
     face = Face3D(pts, plane)
     face_dict = face.to_dict()
     new_face = Face3D.from_dict(face_dict)
```

### Comparing `ladybug-geometry-1.8.1/tests/ray2d_test.py` & `ladybug-geometry-1.9.0/tests/ray2d_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     ray = Ray2D(pt, vec)
     ray_dict = ray.to_dict()
     new_ray = Ray2D.from_dict(ray_dict)
     assert isinstance(new_ray, Ray2D)
     assert new_ray.to_dict() == ray_dict
 
 
-def test_ray2d_mutability():
-    """Test the mutability and immutability of Ray2D objects."""
+def test_ray2d_immutability():
+    """Test the immutability of Ray2D objects."""
     pt = Point2D(2, 0)
     vec = Vector2D(0, 2)
     ray = Ray2D(pt, vec)
 
     assert isinstance(ray, Ray2D)
     with pytest.raises(AttributeError):
         ray.p.x = 3
@@ -50,14 +50,30 @@
         ray.v = Vector2D(2, 2)
 
     ray_copy = ray.duplicate()
     assert ray.p == ray_copy.p
     assert ray.v == ray_copy.v
 
 
+def test_equality():
+    """Test the equality of Ray2D objects."""
+    pt = Point2D(2, 0)
+    vec = Vector2D(0, 2)
+    ray = Ray2D(pt, vec)
+    ray_dup = ray.duplicate()
+    ray_alt = Ray2D(Point2D(2, 0.1), vec)
+
+    assert ray is ray
+    assert ray is not ray_dup
+    assert ray == ray_dup
+    assert hash(ray) == hash(ray_dup)
+    assert ray != ray_alt
+    assert hash(ray) != hash(ray_alt)
+
+
 def test_move():
     """Test the Ray2D move method."""
     pt = Point2D(2, 0)
     vec = Vector2D(0, 2)
     ray = Ray2D(pt, vec)
 
     vec_1 = Vector2D(2, 2)
```

### Comparing `ladybug-geometry-1.8.1/tests/polyface3d_test.py` & `ladybug-geometry-1.9.0/tests/polyface3d_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,34 @@
     assert polyface.faces[1].normal == Vector3D(-1, 0, 0)
     assert polyface.faces[2].normal == Vector3D(0, -1, 0)
     assert polyface.faces[3].normal == Vector3D(0, 1, 0)
     assert polyface.faces[4].normal == Vector3D(1, 0, 0)
     assert polyface.faces[5].normal == Vector3D(0, 0, 1)
 
 
+def test_equality():
+    """Test the equality of Polyface3D objects."""
+    pts = [Point3D(0, 0, 0), Point3D(0, 2, 0), Point3D(2, 2, 0), Point3D(2, 0, 0),
+           Point3D(0, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2)]
+    face_indices = [[(0, 1, 2, 3)], [(0, 4, 5, 1)], [(0, 3, 7, 4)],
+                    [(2, 1, 5, 6)], [(2, 3, 7, 6)], [(4, 5, 6, 7)]]
+    face_indices_2 = [[(0, 1, 2, 3)], [(0, 4, 5, 1)], [(0, 3, 7, 4)],
+                      [(2, 1, 5, 6)], [(2, 3, 7, 6)]]
+    polyface = Polyface3D(pts, face_indices)
+    polyface_dup = polyface.duplicate()
+    polyface_alt = Polyface3D(pts, face_indices_2)
+
+    assert polyface is polyface
+    assert polyface is not polyface_dup
+    assert polyface == polyface_dup
+    assert hash(polyface) == hash(polyface_dup)
+    assert polyface != polyface_alt
+    assert hash(polyface) != hash(polyface_alt)
+
+
 def test_polyface3d_init_open():
     """Test the initalization of Poyface3D and basic properties of open objects."""
     pts = [Point3D(0, 0, 0), Point3D(0, 2, 0), Point3D(2, 2, 0), Point3D(2, 0, 0),
            Point3D(0, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2)]
     face_indices = [[(0, 1, 2, 3)], [(0, 4, 5, 1)], [(0, 3, 7, 4)],
                     [(2, 1, 5, 6)], [(2, 3, 7, 6)]]
     polyface = Polyface3D(pts, face_indices)
```

### Comparing `ladybug-geometry-1.8.1/tests/arc2d_test.py` & `ladybug-geometry-1.9.0/tests/arc2d_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,14 +142,29 @@
     arc_dict = arc.to_dict()
     new_arc = Arc2D.from_dict(arc_dict)
     assert isinstance(new_arc, Arc2D)
     assert new_arc.is_circle
     assert new_arc.to_dict() == arc_dict
 
 
+def test_equality():
+    """Test the equality of Arc2D objects."""
+    pt = Point2D(2, 0)
+    arc = Arc2D(pt, 1, 0, math.pi)
+    arc_dup = arc.duplicate()
+    arc_alt = Arc2D(pt, 1, 0.1, math.pi)
+
+    assert arc is arc
+    assert arc is not arc_dup
+    assert arc == arc_dup
+    assert hash(arc) == hash(arc_dup)
+    assert arc != arc_alt
+    assert hash(arc) != hash(arc_alt)
+
+
 def test_move():
     """Test the Arc2D move method."""
     pt = Point2D(2, 0)
     arc = Arc2D(pt, 1, 0, math.pi)
 
     vec_1 = Vector2D(2, 2)
     new_arc = arc.move(vec_1)
```

### Comparing `ladybug-geometry-1.8.1/tests/pointvector3d_test.py` & `ladybug-geometry-1.9.0/tests/pointvector3d_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,28 @@
 
     norm_vec = vec.normalize()
     assert norm_vec.x == 0
     assert norm_vec.z == 0
     assert norm_vec.magnitude == 1
 
 
+def test_equality():
+    """Test the equality of Point3D objects."""
+    pt_1 = Point3D(0, 2, 1)
+    pt_1_dup = pt_1.duplicate()
+    pt_1_alt = Point3D(0.1, 2, 1)
+
+    assert pt_1 is pt_1
+    assert pt_1 is not pt_1_dup
+    assert pt_1 == pt_1_dup
+    assert hash(pt_1) == hash(pt_1_dup)
+    assert pt_1 != pt_1_alt
+    assert hash(pt_1) != hash(pt_1_alt)
+
+
 def test_vector3_to_from_dict():
     """Test the initalization of Vector3D objects and basic properties."""
     vec = Vector3D(0, 2, 0)
     vec_dict = vec.to_dict()
     new_vec = Vector3D.from_dict(vec_dict)
     assert isinstance(new_vec, Vector3D)
     assert new_vec.to_dict() == vec_dict
```

### Comparing `ladybug-geometry-1.8.1/tests/polygon2d_test.py` & `ladybug-geometry-1.9.0/tests/polygon2d_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,30 @@
     assert polygon.is_clockwise is False
     assert polygon.is_convex is True
     assert polygon.is_self_intersecting is False
 
     assert polygon.vertices[0] == polygon[0]
 
 
+def test_equality():
+    """Test the equality of Polygon2D objects."""
+    pts = (Point2D(0, 0), Point2D(2, 0), Point2D(2, 2), Point2D(0, 2))
+    pts_2 = (Point2D(0, 0), Point2D(2, 0), Point2D(2, 2), Point2D(0.1, 2))
+    polygon = Polygon2D(pts)
+    polygon_dup = polygon.duplicate()
+    polygon_alt = Polygon2D(pts_2)
+
+    assert polygon is polygon
+    assert polygon is not polygon_dup
+    assert polygon == polygon_dup
+    assert hash(polygon) == hash(polygon_dup)
+    assert polygon != polygon_alt
+    assert hash(polygon) != hash(polygon_alt)
+
+
 def test_polygon2d_to_from_dict():
     """Test the to/from dict of Polygon2D objects."""
     pts = (Point2D(0, 0), Point2D(2, 0), Point2D(2, 2), Point2D(0, 2))
     polygon = Polygon2D(pts)
     polygon_dict = polygon.to_dict()
     new_polygon = Polygon2D.from_dict(polygon_dict)
     assert isinstance(new_polygon, Polygon2D)
```

### Comparing `ladybug-geometry-1.8.1/tests/mesh3d_test.py` & `ladybug-geometry-1.9.0/tests/mesh3d_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,30 @@
     assert mesh._is_color_by_face is False
     assert mesh.colors is None
     assert len(mesh.vertex_connected_faces) == 4
     for vf in mesh.vertex_connected_faces:
         assert len(vf) == 1
 
 
+def test_equality():
+    """Test the equality of Mesh3D objects."""
+    pts = (Point3D(0, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2))
+    pts_2 = (Point3D(0.1, 0, 2), Point3D(0, 2, 2), Point3D(2, 2, 2), Point3D(2, 0, 2))
+    mesh = Mesh3D(pts, [(0, 1, 2, 3)])
+    mesh_dup = mesh.duplicate()
+    mesh_alt = Mesh3D(pts_2, [(0, 1, 2, 3)])
+
+    assert mesh is mesh
+    assert mesh is not mesh_dup
+    assert mesh == mesh_dup
+    assert hash(mesh) == hash(mesh_dup)
+    assert mesh != mesh_alt
+    assert hash(mesh) != hash(mesh_alt)
+
+
 def test_mesh3d_to_from_dict():
     """Test the to/from dict of Mesh3D objects."""
     pts = (Point3D(0, 0), Point3D(0, 2), Point3D(2, 2), Point3D(2, 0))
     mesh = Mesh3D(pts, [(0, 1, 2, 3)])
     mesh_dict = mesh.to_dict()
     new_mesh = Mesh3D.from_dict(mesh_dict)
     assert isinstance(new_mesh, Mesh3D)
```

### Comparing `ladybug-geometry-1.8.1/tests/sphere3d_test.py` & `ladybug-geometry-1.9.0/tests/sphere3d_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,28 @@
     assert sp.max.z == 5
     assert sp.diameter == 6
     assert isinstance(sp.circumference, float)
     assert isinstance(sp.area, float)
     assert isinstance(sp.volume, float)
 
 
+def test_equality():
+    """Test the equality of Polygon2D objects."""
+    sphere = Sphere3D(Point3D(2, 0, 2), 3)
+    sphere_dup = sphere.duplicate()
+    sphere_alt = Sphere3D(Point3D(2, 0.1, 2), 3)
+
+    assert sphere is sphere
+    assert sphere is not sphere_dup
+    assert sphere == sphere_dup
+    assert hash(sphere) == hash(sphere_dup)
+    assert sphere != sphere_alt
+    assert hash(sphere) != hash(sphere_alt)
+
+
 def test_sphere_to_from_dict():
     """Test the Sphere3D to_dict and from_dict methods."""
     sp = Sphere3D(Point3D(4, 0, 2), 3)
     d = sp.to_dict()
     sp = Sphere3D.from_dict(d)
     assert sp.center.x == pytest.approx(4, rel=1e-3)
     assert sp.center.y == pytest.approx(0, rel=1e-3)
```

### Comparing `ladybug-geometry-1.8.1/tests/line3d_test.py` & `ladybug-geometry-1.9.0/tests/line3d_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,30 @@
     assert seg.length == 2
 
     flip_seg = seg.flip()
     assert flip_seg.p == Point3D(2, 2, 2)
     assert flip_seg.v == Vector3D(0, -2, 0)
 
 
+def test_equality():
+    """Test the equality of LineSegement3D objects."""
+    pt = Point3D(2, 0, 2)
+    vec = Vector3D(0, 2, 0)
+    seg = LineSegment3D(pt, vec)
+    seg_dup = seg.duplicate()
+    seg_alt = LineSegment3D(Point3D(2, 0.1, 2), vec)
+
+    assert seg is seg
+    assert seg is not seg_dup
+    assert seg == seg_dup
+    assert hash(seg) == hash(seg_dup)
+    assert seg != seg_alt
+    assert hash(seg) != hash(seg_alt)
+
+
 def test_linesegment3_to_from_dict():
     """Test the to/from dict of LineSegment3D objects."""
     pt = Point3D(2, 0, 2)
     vec = Vector3D(0, 2, 0)
     seg = LineSegment3D(pt, vec)
     seg_dict = seg.to_dict()
     new_seg = LineSegment3D.from_dict(seg_dict)
@@ -61,16 +77,16 @@
     assert seg.p == Point3D(2, 0, 2)
     assert seg.v == Vector3D(0, 2, 0)
     assert seg.p1 == Point3D(2, 0, 2)
     assert seg.p2 == Point3D(2, 2, 2)
     assert seg.length == 2
 
 
-def test_linesegment3d_mutability():
-    """Test the mutability and immutability of LineSegment3D objects."""
+def test_linesegment3d_immutability():
+    """Test the immutability of LineSegment3D objects."""
     pt = Point3D(2, 0, 0)
     vec = Vector3D(0, 2, 0)
     seg = LineSegment3D(pt, vec)
 
     assert isinstance(seg, LineSegment3D)
     with pytest.raises(AttributeError):
         seg.p.x = 3
```

### Comparing `ladybug-geometry-1.8.1/tests/ray3d_test.py` & `ladybug-geometry-1.9.0/tests/ray3d_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,42 @@
     assert ray.v == Vector3D(0, 2, 0)
 
     flip_ray = ray.reverse()
     assert flip_ray.p == Point3D(2, 0, 2)
     assert flip_ray.v == Vector3D(0, -2, 0)
 
 
+def test_equality():
+    """Test the equality of Ray3D objects."""
+    pt = Point3D(2, 0, 2)
+    vec = Vector3D(0, 2, 0)
+    ray = Ray3D(pt, vec)
+    ray_dup = ray.duplicate()
+    ray_alt = Ray3D(Point3D(2, 0.1, 2), vec)
+
+    assert ray is ray
+    assert ray is not ray_dup
+    assert ray == ray_dup
+    assert hash(ray) == hash(ray_dup)
+    assert ray != ray_alt
+    assert hash(ray) != hash(ray_alt)
+
+
 def test_ray3_to_from_dict():
     """Test the to/from dict of Ray3D objects."""
     pt = Point3D(2, 0, 2)
     vec = Vector3D(0, 2, 0)
     ray = Ray3D(pt, vec)
     ray_dict = ray.to_dict()
     new_ray = Ray3D.from_dict(ray_dict)
     assert isinstance(new_ray, Ray3D)
     assert new_ray.to_dict() == ray_dict
 
 
-def test_linerayment2_mutability():
+def test_ray3d_immutability():
     """Test the immutability of Ray3D objects."""
     pt = Point3D(2, 0, 0)
     vec = Vector3D(0, 2, 0)
     ray = Ray3D(pt, vec)
 
     assert isinstance(ray, Ray3D)
     with pytest.raises(AttributeError):
```

### Comparing `ladybug-geometry-1.8.1/tests/arc3d_test.py` & `ladybug-geometry-1.9.0/tests/arc3d_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,29 @@
     arc_dict = arc.to_dict()
     new_arc = Arc3D.from_dict(arc_dict)
     assert isinstance(new_arc, Arc3D)
     assert new_arc.is_circle
     assert new_arc.to_dict() == arc_dict
 
 
+def test_equality():
+    """Test the equality of Arc3D objects."""
+    pt = Point3D(2, 0, 2)
+    arc = Arc3D(Plane(o=pt), 1, 0, math.pi)
+    arc_dup = arc.duplicate()
+    arc_alt = Arc3D(Plane(o=Point3D(2, 0.1, 2)), 1, 0.1, math.pi)
+
+    assert arc is arc
+    assert arc is not arc_dup
+    assert arc == arc_dup
+    assert hash(arc) == hash(arc_dup)
+    assert arc != arc_alt
+    assert hash(arc) != hash(arc_alt)
+
+
 def test_move():
     """Test the Arc3D move method."""
     pt = Point3D(2, 0, 0)
     arc = Arc3D(Plane(o=pt), 1, 0, math.pi)
 
     vec_1 = Vector3D(2, 2, 2)
     new_arc = arc.move(vec_1)
```

