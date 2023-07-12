# Comparing `tmp/stac-asset-0.1.0.tar.gz` & `tmp/stac-asset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-asset-0.1.0.tar", last modified: Wed Jul 12 18:18:22 2023, max compression
+gzip compressed data, was "stac-asset-0.1.1.tar", last modified: Wed Jul 12 22:15:23 2023, max compression
```

## Comparing `stac-asset-0.1.0.tar` & `stac-asset-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.610945 stac-asset-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 18:18:06.000000 stac-asset-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 18:18:22.610945 stac-asset-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-12 18:18:06.000000 stac-asset-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-12 18:18:06.000000 stac-asset-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:18:22.610945 stac-asset-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.598945 stac-asset-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.602945 stac-asset-0.1.0/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-12 18:18:06.000000 stac-asset-0.1.0/src/stac_asset/usgs_eros_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.606945 stac-asset-0.1.0/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 18:18:22.000000 stac-asset-0.1.0/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:18:22.610945 stac-asset-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-12 18:18:06.000000 stac-asset-0.1.0/tests/test_usgs_eros_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:23.334258 stac-asset-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 22:15:02.000000 stac-asset-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 22:15:02.000000 stac-asset-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 22:15:23.334258 stac-asset-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-12 22:15:02.000000 stac-asset-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-12 22:15:02.000000 stac-asset-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:15:23.334258 stac-asset-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:23.326258 stac-asset-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:23.330258 stac-asset-0.1.1/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-12 22:15:02.000000 stac-asset-0.1.1/src/stac_asset/usgs_eros_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:23.334258 stac-asset-0.1.1/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-12 22:15:23.000000 stac-asset-0.1.1/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-12 22:15:23.000000 stac-asset-0.1.1/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:15:23.000000 stac-asset-0.1.1/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 22:15:23.000000 stac-asset-0.1.1/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 22:15:23.000000 stac-asset-0.1.1/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 22:15:23.000000 stac-asset-0.1.1/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:23.334258 stac-asset-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-12 22:15:02.000000 stac-asset-0.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-12 22:15:02.000000 stac-asset-0.1.1/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-12 22:15:02.000000 stac-asset-0.1.1/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 22:15:02.000000 stac-asset-0.1.1/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-12 22:15:02.000000 stac-asset-0.1.1/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-12 22:15:02.000000 stac-asset-0.1.1/tests/test_usgs_eros_client.py
```

### Comparing `stac-asset-0.1.0/LICENSE` & `stac-asset-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/PKG-INFO` & `stac-asset-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.1.0
+Version: 0.1.1
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: repository, https://github.com/stac-utils/stac-asset
 Project-URL: changelog, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `stac-asset-0.1.0/README.md` & `stac-asset-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/pyproject.toml` & `stac-asset-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stac-asset"
-version = "0.1.0"
+version = "0.1.1"
 description = "Read and download STAC assets across platforms and providers"
 authors = [
     { name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }
 ]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
```

### Comparing `stac-asset-0.1.0/src/stac_asset/__init__.py` & `stac-asset-0.1.1/src/stac_asset/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/_cli.py` & `stac-asset-0.1.1/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/client.py` & `stac-asset-0.1.1/src/stac_asset/client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/earthdata_client.py` & `stac-asset-0.1.1/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/errors.py` & `stac-asset-0.1.1/src/stac_asset/errors.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/filesystem_client.py` & `stac-asset-0.1.1/src/stac_asset/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/functions.py` & `stac-asset-0.1.1/src/stac_asset/functions.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/http_client.py` & `stac-asset-0.1.1/src/stac_asset/http_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/planetary_computer_client.py` & `stac-asset-0.1.1/src/stac_asset/planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/s3_client.py` & `stac-asset-0.1.1/src/stac_asset/s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/types.py` & `stac-asset-0.1.1/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset/usgs_eros_client.py` & `stac-asset-0.1.1/src/stac_asset/usgs_eros_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/src/stac_asset.egg-info/PKG-INFO` & `stac-asset-0.1.1/src/stac_asset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.1.0
+Version: 0.1.1
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: repository, https://github.com/stac-utils/stac-asset
 Project-URL: changelog, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `stac-asset-0.1.0/src/stac_asset.egg-info/SOURCES.txt` & `stac-asset-0.1.1/src/stac_asset.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/stac_asset/__init__.py
 src/stac_asset/_cli.py
 src/stac_asset/client.py
 src/stac_asset/earthdata_client.py
 src/stac_asset/errors.py
 src/stac_asset/filesystem_client.py
 src/stac_asset/functions.py
 src/stac_asset/http_client.py
 src/stac_asset/planetary_computer_client.py
+src/stac_asset/py.typed
 src/stac_asset/s3_client.py
 src/stac_asset/strategy.py
 src/stac_asset/types.py
 src/stac_asset/usgs_eros_client.py
 src/stac_asset.egg-info/PKG-INFO
 src/stac_asset.egg-info/SOURCES.txt
 src/stac_asset.egg-info/dependency_links.txt
```

### Comparing `stac-asset-0.1.0/tests/test_cli.py` & `stac-asset-0.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/tests/test_earthdata_client.py` & `stac-asset-0.1.1/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/tests/test_filesystem_client.py` & `stac-asset-0.1.1/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/tests/test_planetary_computer_client.py` & `stac-asset-0.1.1/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/tests/test_s3_client.py` & `stac-asset-0.1.1/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.1.0/tests/test_usgs_eros_client.py` & `stac-asset-0.1.1/tests/test_usgs_eros_client.py`

 * *Files identical despite different names*

