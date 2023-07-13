# Comparing `tmp/landingai-0.1.5.tar.gz` & `tmp/landingai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.1.5.tar", max compression
+gzip compressed data, was "landingai-0.2.1.tar", max compression
```

## Comparing `landingai-0.1.5.tar` & `landingai-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-07-12 18:41:46.000441 landingai-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     6741 2023-07-12 18:41:46.000441 landingai-0.1.5/README.md
--rw-r--r--   0        0        0      354 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/__init__.py
--rw-r--r--   0        0        0     6833 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/client.py
--rw-r--r--   0        0        0    19873 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9418 2023-07-12 18:41:46.028442 landingai-0.1.5/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-12 18:41:46.036442 landingai-0.1.5/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     6843 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/io.py
--rw-r--r--   0        0        0      221 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0     5287 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     5912 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/postprocess.py
--rw-r--r--   0        0        0    25559 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/predict.py
--rw-r--r--   0        0        0     6068 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4374 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     2657 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/telemetry.py
--rw-r--r--   0        0        0     1685 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/utils.py
--rw-r--r--   0        0        0    23703 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/vision_pipeline.py
--rw-r--r--   0        0        0    13403 2023-07-12 18:41:46.040442 landingai-0.1.5/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-12 18:41:46.736454 landingai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-13 10:59:42.229296 landingai-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     6774 2023-07-13 10:59:42.229296 landingai-0.2.1/README.md
+-rw-r--r--   0        0        0      354 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/__init__.py
+-rw-r--r--   0        0        0     6833 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/data_management/client.py
+-rw-r--r--   0        0        0    19873 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9418 2023-07-13 10:59:42.269297 landingai-0.2.1/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-13 10:59:42.277297 landingai-0.2.1/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0      419 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16392 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    16998 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     5912 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/postprocess.py
+-rw-r--r--   0        0        0    25559 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/predict.py
+-rw-r--r--   0        0        0     6068 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     2657 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/telemetry.py
+-rw-r--r--   0        0        0     1685 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-13 10:59:42.281297 landingai-0.2.1/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-13 10:59:43.337311 landingai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 landingai-0.2.1/PKG-INFO
```

### Comparing `landingai-0.1.5/LICENSE.md` & `landingai-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/README.md` & `landingai-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,31 +82,32 @@
 # continue the above example
 predictions = predictor.predict(image)
 image_with_preds = overlay_predictions(predictions, image)
 image_with_preds.save("image.jpg")
 ```
 ### Create a Vision Pipeline
 
-All the modules shown above and others can be chained together using the `landingai.vision_pipeline` abstraction. At its core, a pipeline is a sequence of chained calls that operate on a `landingai.vision_pipeline.FrameSet`.
+All the modules shown above and others can be chained together using the `landingai.pipeline` abstraction. At its core, a pipeline is a sequence of chained calls that operate on a `landingai.pipeline.FrameSet`.
 
 The following example shows how the previous sections come together on a pipeline. For more details, go to the [*Vision Pipelines User Guide*](https://landing-ai.github.io/landingai-python/landingai.html#vision-pipelines) 
 ```python
-cloud_sky_model = Predictor("FILL_YOUR_INFERENCE_ENDPOINT_ID"
-                            , "FILL_YOUR_API_KEY"
-                            , "FILL_YOUR_API_SECRET") 
+from landingai.predict import Predictor
+import landingai.pipeline as pl
 
-Camera = NetworkedCamera(stream_url)
+cloud_sky_model = Predictor("FILL_YOUR_INFERENCE_ENDPOINT_ID"
+                            , api_key="FILL_YOUR_API_KEY") 
+Camera = pl.image_source.NetworkedCamera(stream_url)
 for frame in Camera:
     (
         frame.downsize(width=1024)
         .run_predict(predictor=cloud_sky_model)
         .overlay_predictions()
         .show_image()
         .save_image(filename_prefix="./capture")
-    )
+    )    
 ```
 
 ## Run Examples Locally
 
 All the examples in this repo can be run locally.
 
 To give you some guidance, here's how you can run the `rtsp-capture` example locally in a shell environment:
```

### Comparing `landingai-0.1.5/landingai/common.py` & `landingai-0.2.1/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/data_management/client.py` & `landingai-0.2.1/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/data_management/media.py` & `landingai-0.2.1/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/data_management/metadata.py` & `landingai-0.2.1/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/data_management/utils.py` & `landingai-0.2.1/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/exceptions.py` & `landingai-0.2.1/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.1/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/postprocess.py` & `landingai-0.2.1/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/predict.py` & `landingai-0.2.1/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/st_utils.py` & `landingai-0.2.1/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/storage/snowflake.py` & `landingai-0.2.1/landingai/storage/snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import tempfile
 from pathlib import Path
 from typing import Optional
 
 import snowflake.connector
 from pydantic import BaseSettings, Field
 
-from landingai.io import read_file
+from landingai.storage.data_access import download_file
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SnowflakeCredential(BaseSettings):
     """Snowflake API credential. It's used to connect to Snowflake.
     It supports loading from environment variables or .env files.
@@ -74,17 +74,15 @@
         credential=credential,
         connection_config=connection_config,
     )
     if local_output is None:
         local_output = Path(tempfile.mkdtemp())
     file_path = local_output / remote_filename
     file_path.parent.mkdir(parents=True, exist_ok=True)
-    with open(str(file_path), "wb") as f:
-        data_bytes = read_file(url)
-        f.write(data_bytes)
+    download_file(url, file_output_path=file_path)
     _LOGGER.info(f"Saved file {remote_filename} to {file_path}")
     return file_path
 
 
 def get_snowflake_presigned_url(
     remote_filename: str,
     stage_name: str,
```

### Comparing `landingai-0.1.5/landingai/telemetry.py` & `landingai-0.2.1/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/transform.py` & `landingai-0.2.1/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/utils.py` & `landingai-0.2.1/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/landingai/visualize.py` & `landingai-0.2.1/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.5/pyproject.toml` & `landingai-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.1.5"
+version = "0.2.1"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.1.5/PKG-INFO` & `landingai-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.1.5
+Version: 0.2.1
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -111,31 +111,32 @@
 # continue the above example
 predictions = predictor.predict(image)
 image_with_preds = overlay_predictions(predictions, image)
 image_with_preds.save("image.jpg")
 ```
 ### Create a Vision Pipeline
 
-All the modules shown above and others can be chained together using the `landingai.vision_pipeline` abstraction. At its core, a pipeline is a sequence of chained calls that operate on a `landingai.vision_pipeline.FrameSet`.
+All the modules shown above and others can be chained together using the `landingai.pipeline` abstraction. At its core, a pipeline is a sequence of chained calls that operate on a `landingai.pipeline.FrameSet`.
 
 The following example shows how the previous sections come together on a pipeline. For more details, go to the [*Vision Pipelines User Guide*](https://landing-ai.github.io/landingai-python/landingai.html#vision-pipelines) 
 ```python
-cloud_sky_model = Predictor("FILL_YOUR_INFERENCE_ENDPOINT_ID"
-                            , "FILL_YOUR_API_KEY"
-                            , "FILL_YOUR_API_SECRET") 
+from landingai.predict import Predictor
+import landingai.pipeline as pl
 
-Camera = NetworkedCamera(stream_url)
+cloud_sky_model = Predictor("FILL_YOUR_INFERENCE_ENDPOINT_ID"
+                            , api_key="FILL_YOUR_API_KEY") 
+Camera = pl.image_source.NetworkedCamera(stream_url)
 for frame in Camera:
     (
         frame.downsize(width=1024)
         .run_predict(predictor=cloud_sky_model)
         .overlay_predictions()
         .show_image()
         .save_image(filename_prefix="./capture")
-    )
+    )    
 ```
 
 ## Run Examples Locally
 
 All the examples in this repo can be run locally.
 
 To give you some guidance, here's how you can run the `rtsp-capture` example locally in a shell environment:
```

