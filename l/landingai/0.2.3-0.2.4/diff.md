# Comparing `tmp/landingai-0.2.3.tar.gz` & `tmp/landingai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.2.3.tar", max compression
+gzip compressed data, was "landingai-0.2.4.tar", max compression
```

## Comparing `landingai-0.2.3.tar` & `landingai-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-07-13 16:32:38.850497 landingai-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     6774 2023-07-13 16:32:38.854497 landingai-0.2.3/README.md
--rw-r--r--   0        0        0      354 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/__init__.py
--rw-r--r--   0        0        0     6833 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/data_management/client.py
--rw-r--r--   0        0        0    21135 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-07-13 16:32:38.886499 landingai-0.2.3/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0      419 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    16392 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    16998 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/postprocess.py
--rw-r--r--   0        0        0    25559 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/predict.py
--rw-r--r--   0        0        0     6068 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4340 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     2657 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/telemetry.py
--rw-r--r--   0        0        0     1685 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-07-13 16:32:38.898499 landingai-0.2.3/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-13 16:32:39.806544 landingai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 landingai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-13 17:29:25.948012 landingai-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     6774 2023-07-13 17:29:25.948012 landingai-0.2.4/README.md
+-rw-r--r--   0        0        0      354 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/__init__.py
+-rw-r--r--   0        0        0     6833 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/client.py
+-rw-r--r--   0        0        0    21135 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-13 17:29:25.996012 landingai-0.2.4/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0      419 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16392 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    16998 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/postprocess.py
+-rw-r--r--   0        0        0    25559 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/predict.py
+-rw-r--r--   0        0        0     6068 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     2657 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/telemetry.py
+-rw-r--r--   0        0        0     1685 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-13 17:29:26.924010 landingai-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 landingai-0.2.4/PKG-INFO
```

### Comparing `landingai-0.2.3/LICENSE.md` & `landingai-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/README.md` & `landingai-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/common.py` & `landingai-0.2.4/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/data_management/client.py` & `landingai-0.2.4/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/data_management/media.py` & `landingai-0.2.4/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/data_management/metadata.py` & `landingai-0.2.4/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/data_management/utils.py` & `landingai-0.2.4/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/exceptions.py` & `landingai-0.2.4/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.4/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/pipeline/frameset.py` & `landingai-0.2.4/landingai/pipeline/frameset.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/pipeline/image_source.py` & `landingai-0.2.4/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/pipeline/postprocessing.py` & `landingai-0.2.4/landingai/pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/postprocess.py` & `landingai-0.2.4/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/predict.py` & `landingai-0.2.4/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/st_utils.py` & `landingai-0.2.4/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/storage/data_access.py` & `landingai-0.2.4/landingai/storage/data_access.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/storage/snowflake.py` & `landingai-0.2.4/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/telemetry.py` & `landingai-0.2.4/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/transform.py` & `landingai-0.2.4/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/utils.py` & `landingai-0.2.4/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/landingai/visualize.py` & `landingai-0.2.4/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.3/pyproject.toml` & `landingai-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.2.3"
+version = "0.2.4"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.2.3/PKG-INFO` & `landingai-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.2.3
+Version: 0.2.4
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

