# Comparing `tmp/fastfuels-sdk-0.1.tar.gz` & `tmp/fastfuels-sdk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfuels-sdk-0.1.tar", last modified: Thu Jun 29 23:14:56 2023, max compression
+gzip compressed data, was "fastfuels-sdk-0.2.tar", last modified: Thu Jul 13 20:37:39 2023, max compression
```

## Comparing `fastfuels-sdk-0.1.tar` & `fastfuels-sdk-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:14:56.661435 fastfuels-sdk-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-29 23:14:56.657435 fastfuels-sdk-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:14:56.657435 fastfuels-sdk-0.1/fastfuels_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/fuelgrids.py
--rw-r--r--   0 runner    (1001) docker     (123)    23730 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/fastfuels_sdk/treelists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:14:56.657435 fastfuels-sdk-0.1/fastfuels_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-29 23:14:56.000000 fastfuels-sdk-0.1/fastfuels_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 23:14:56.000000 fastfuels-sdk-0.1/fastfuels_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:14:56.000000 fastfuels-sdk-0.1/fastfuels_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 23:14:56.000000 fastfuels-sdk-0.1/fastfuels_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 23:14:56.000000 fastfuels-sdk-0.1/fastfuels_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:14:56.661435 fastfuels-sdk-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-29 23:14:46.000000 fastfuels-sdk-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:37:39.139713 fastfuels-sdk-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-13 20:37:39.139713 fastfuels-sdk-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:37:39.139713 fastfuels-sdk-0.2/fastfuels_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/fuelgrids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23730 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/fastfuels_sdk/treelists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:37:39.139713 fastfuels-sdk-0.2/fastfuels_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-13 20:37:39.000000 fastfuels-sdk-0.2/fastfuels_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 20:37:39.000000 fastfuels-sdk-0.2/fastfuels_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:37:39.000000 fastfuels-sdk-0.2/fastfuels_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 20:37:39.000000 fastfuels-sdk-0.2/fastfuels_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 20:37:39.000000 fastfuels-sdk-0.2/fastfuels_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:37:39.139713 fastfuels-sdk-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 20:37:29.000000 fastfuels-sdk-0.2/setup.py
```

### Comparing `fastfuels-sdk-0.1/LICENSE` & `fastfuels-sdk-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/PKG-INFO` & `fastfuels-sdk-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels-sdk
-Version: 0.1
+Version: 0.2
 Summary: 3D Fuels for Next Generation Fire Models
 Home-page: https://github.com/silvxlabs/fastfuels-sdk-python
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/fastfuels-sdk-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastfuels-sdk-0.1/README.md` & `fastfuels-sdk-0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk/_base.py` & `fastfuels-sdk-0.2/fastfuels_sdk/_base.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk/api.py` & `fastfuels-sdk-0.2/fastfuels_sdk/api.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk/datasets.py` & `fastfuels-sdk-0.2/fastfuels_sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk/exports.py` & `fastfuels-sdk-0.2/fastfuels_sdk/exports.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
     surf_lines = []
     part_lines = []
     for sav in sav_classes:
         id = f"{name}_{int(sav)}"
         surf_lines.append(f"&SURF ID='surf_{id}'\n")
         surf_lines.append(f"\tSURFACE_VOLUME_RATIO={sav}\n")
         surf_lines.append(f"\tCOLOR='GREEN'\n")
-        surf_lines.append(f"\tLENGTH=0.5'\n")
+        surf_lines.append(f"\tLENGTH=0.5\n")
         surf_lines.append(f"\tMOISTURE_FRACTION=0.5\n")
         surf_lines.append(f"\tGEOMETRY='CYLINDRICAL' /\n\n")
 
         part_lines.append(f"&PART ID='part_{id}'\n")
         part_lines.append(f"\tSURF_ID='surf_{id}'\n")
         part_lines.append(f"\tDRAG_LAW='CYLINDER'\n")
         part_lines.append(f"\tSTATIC=T\n")
```

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk/fuelgrids.py` & `fastfuels-sdk-0.2/fastfuels_sdk/fuelgrids.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk/treelists.py` & `fastfuels-sdk-0.2/fastfuels_sdk/treelists.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.1/fastfuels_sdk.egg-info/PKG-INFO` & `fastfuels-sdk-0.2/fastfuels_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels-sdk
-Version: 0.1
+Version: 0.2
 Summary: 3D Fuels for Next Generation Fire Models
 Home-page: https://github.com/silvxlabs/fastfuels-sdk-python
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/fastfuels-sdk-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastfuels-sdk-0.1/setup.py` & `fastfuels-sdk-0.2/setup.py`

 * *Files identical despite different names*

