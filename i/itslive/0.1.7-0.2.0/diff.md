# Comparing `tmp/itslive-0.1.7.tar.gz` & `tmp/itslive-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itslive-0.1.7.tar", max compression
+gzip compressed data, was "itslive-0.2.0.tar", max compression
```

## Comparing `itslive-0.1.7.tar` & `itslive-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-05-25 15:23:33.888923 itslive-0.1.7/LICENSE
--rw-r--r--   0        0        0      239 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/cli/__init__.py
--rw-r--r--   0        0        0     5300 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/cli/export.py
--rw-r--r--   0        0        0     5861 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/cli/plot.py
--rw-r--r--   0        0        0      109 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/dataviz/__init__.py
--rw-r--r--   0        0        0     2557 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/dataviz/_viz.py
--rw-r--r--   0        0        0      618 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_cubes/__init__.py
--rw-r--r--   0        0        0    14964 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_cubes/_cubes.py
--rw-r--r--   0        0        0       67 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_pairs/__init__.py
--rw-r--r--   0        0        0      115 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_pairs/_pairs.py
--rw-r--r--   0        0        0     1047 2023-05-25 15:23:33.900924 itslive-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 itslive-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-13 19:00:58.612057 itslive-0.2.0/LICENSE
+-rw-r--r--   0        0        0      282 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/cli/__init__.py
+-rw-r--r--   0        0        0     5300 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/cli/export.py
+-rw-r--r--   0        0        0     5861 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/cli/plot.py
+-rw-r--r--   0        0        0      109 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/dataviz/__init__.py
+-rw-r--r--   0        0        0     2557 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/dataviz/_viz.py
+-rw-r--r--   0        0        0      618 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/velocity_cubes/__init__.py
+-rw-r--r--   0        0        0    14964 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/velocity_cubes/_cubes.py
+-rw-r--r--   0        0        0      111 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/velocity_pairs/__init__.py
+-rw-r--r--   0        0        0     3847 2023-07-13 19:00:58.612057 itslive-0.2.0/itslive/velocity_pairs/_pairs.py
+-rw-r--r--   0        0        0     1424 2023-07-13 19:00:58.620057 itslive-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 itslive-0.2.0/PKG-INFO
```

### Comparing `itslive-0.1.7/LICENSE` & `itslive-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itslive-0.1.7/itslive/cli/export.py` & `itslive-0.2.0/itslive/cli/export.py`

 * *Files identical despite different names*

### Comparing `itslive-0.1.7/itslive/cli/plot.py` & `itslive-0.2.0/itslive/cli/plot.py`

 * *Files identical despite different names*

### Comparing `itslive-0.1.7/itslive/dataviz/_viz.py` & `itslive-0.2.0/itslive/dataviz/_viz.py`

 * *Files identical despite different names*

### Comparing `itslive-0.1.7/itslive/velocity_cubes/__init__.py` & `itslive-0.2.0/itslive/velocity_cubes/__init__.py`

 * *Files identical despite different names*

### Comparing `itslive-0.1.7/itslive/velocity_cubes/_cubes.py` & `itslive-0.2.0/itslive/velocity_cubes/_cubes.py`

 * *Files identical despite different names*

### Comparing `itslive-0.1.7/PKG-INFO` & `itslive-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: itslive
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python client for ITSLIVE gralcier velocity data
 Home-page: https://github.com/nasa-jpl/itslive-vortex
 License: GNUL V3
 Author: Luis Lopez
 Author-email: luis.lopez@nsidc.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Shapely (>=1.8)
-Requires-Dist: matplotlib (>=3.6,<4.0)
+Requires-Dist: earthaccess (>=0.5.2)
+Requires-Dist: matplotlib (>=3.6)
 Requires-Dist: pandas (==1.5.1)
 Requires-Dist: plotext (>=0)
+Requires-Dist: pqdm (>=0.2.0)
 Requires-Dist: pyproj (>=3.3)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich-click (>=1.5)
 Requires-Dist: s3fs (>=2022.3)
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: xarray (>=2022.3)
 Requires-Dist: zarr (>=2.11)
```

