# Comparing `tmp/garden_ai-0.5.1.tar.gz` & `tmp/garden_ai-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.5.1.tar", max compression
+gzip compressed data, was "garden_ai-0.5.2.tar", max compression
```

## Comparing `garden_ai-0.5.1.tar` & `garden_ai-0.5.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1078 2023-07-10 15:47:33.288110 garden_ai-0.5.1/LICENSE
--rw-r--r--   0        0        0      797 2023-07-10 15:47:33.288110 garden_ai-0.5.1/README.md
--rw-r--r--   0        0        0      418 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/__main__.py
--rw-r--r--   0        0        0     4454 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/_model.py
--rw-r--r--   0        0        0      180 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/app/__init__.py
--rw-r--r--   0        0        0     2855 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/app/console.py
--rw-r--r--   0        0        0    11506 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/app/main.py
--rw-r--r--   0        0        0     3895 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/app/model.py
--rw-r--r--   0        0        0    11770 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0     3493 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/backend_client.py
--rw-r--r--   0        0        0    18096 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/client.py
--rw-r--r--   0        0        0      440 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/constants.py
--rw-r--r--   0        0        0     9394 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/datacite.py
--rw-r--r--   0        0        0    14824 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2802 2023-07-10 15:47:33.288110 garden_ai-0.5.1/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1603 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      798 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7553 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/local_data.py
--rw-r--r--   0        0        0     8126 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/mlmodel.py
--rw-r--r--   0        0        0        0 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/model_file_transfer/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/model_file_transfer/upload.py
--rw-r--r--   0        0        0    19626 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/pipelines.py
--rw-r--r--   0        0        0    10745 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/steps.py
--rw-r--r--   0        0        0     2019 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     5258 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/utils/_meta.py
--rw-r--r--   0        0        0     1018 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0     8533 2023-07-10 15:47:33.292110 garden_ai-0.5.1/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2866 2023-07-10 15:47:47.140793 garden_ai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 garden_ai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-13 20:51:41.118266 garden_ai-0.5.2/LICENSE
+-rw-r--r--   0        0        0      797 2023-07-13 20:51:41.118266 garden_ai-0.5.2/README.md
+-rw-r--r--   0        0        0      418 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/__main__.py
+-rw-r--r--   0        0        0     4454 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/_model.py
+-rw-r--r--   0        0        0      180 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/console.py
+-rw-r--r--   0        0        0    11506 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/main.py
+-rw-r--r--   0        0        0     3895 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/model.py
+-rw-r--r--   0        0        0    11770 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0     4002 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    18653 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/client.py
+-rw-r--r--   0        0        0      440 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/constants.py
+-rw-r--r--   0        0        0     9394 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/datacite.py
+-rw-r--r--   0        0        0    14824 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2802 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1603 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      798 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7553 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/local_data.py
+-rw-r--r--   0        0        0     8126 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/model_file_transfer/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/model_file_transfer/upload.py
+-rw-r--r--   0        0        0    19626 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    10745 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/steps.py
+-rw-r--r--   0        0        0     2019 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     5258 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0     1018 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0     8533 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2867 2023-07-13 20:51:53.382439 garden_ai-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 garden_ai-0.5.2/PKG-INFO
```

### Comparing `garden_ai-0.5.1/LICENSE` & `garden_ai-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/README.md` & `garden_ai-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/_model.py` & `garden_ai-0.5.2/garden_ai/_model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/app/console.py` & `garden_ai-0.5.2/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/app/garden.py` & `garden_ai-0.5.2/garden_ai/app/garden.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/app/main.py` & `garden_ai-0.5.2/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/app/model.py` & `garden_ai-0.5.2/garden_ai/app/model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/app/pipeline.py` & `garden_ai-0.5.2/garden_ai/app/pipeline.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/backend_client.py` & `garden_ai-0.5.2/garden_ai/backend_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 from enum import Enum
 from dataclasses import dataclass
-from typing import Optional, Callable
+from typing import Optional, Callable, List
 
 import requests
 
 from garden_ai.constants import GardenConstants
 from garden_ai.gardens import Garden
 
 logger = logging.getLogger()
@@ -16,14 +16,15 @@
     """Exception raised when a backend call to generate a presigned URL fails"""
 
     pass
 
 
 @dataclass
 class PresignedUrlResponse:
+    model_name: str
     url: str
     fields: Optional[dict]  # Present for upload URLs. Absent for download URLs.
 
 
 class PresignedUrlDirection(Enum):
     Upload = "upload"
     Download = "download"
@@ -66,31 +67,46 @@
     def update_doi_on_datacite(self, payload: dict):
         self._put("/doi", payload)
 
     def publish_garden_metadata(self, garden: Garden):
         payload = json.loads(garden.expanded_json())
         self._post("/garden-search-record", payload)
 
-    def _get_presigned_url(
-        self, full_model_name: str, direction: PresignedUrlDirection
-    ) -> PresignedUrlResponse:
+    def _get_presigned_urls(
+        self, model_names: List[str], direction: PresignedUrlDirection
+    ) -> List[PresignedUrlResponse]:
         payload = {
-            "s3_path": full_model_name + "/model.zip",
             "direction": direction.value,
+            "batch": [name + "/model.zip" for name in model_names],
         }
-        response_dict = self._post("/presigned-url", payload)
-        url = response_dict.get("url", None)
-        fields = response_dict.get("fields", None)
-        if not url:
-            raise PresignedURLException(
-                "Failed to generate presigned URL for model file transfer. Response was missing url field."
-            )
-        if direction == PresignedUrlDirection.Upload and not fields:
-            message = "Failed to generate presigned URL for model file upload. Response was missing 'fields' attribute."
-            raise PresignedURLException(message)
-        return PresignedUrlResponse(url, fields)
+        responses = self._post("/presigned-url", payload)["responses"]
+        results = []
 
-    def get_model_download_url(self, full_model_name: str) -> PresignedUrlResponse:
-        return self._get_presigned_url(full_model_name, PresignedUrlDirection.Download)
+        for response in responses:
+            model_name = response.get("model_name", None)
+            url = response.get("url", None)
+            fields = response.get("fields", None)
+            if not model_name:
+                raise PresignedURLException(
+                    "Failed to generate presigned URL for model file transfer. Response was missing model_name field."
+                )
+            if not url:
+                raise PresignedURLException(
+                    "Failed to generate presigned URL for model file transfer. Response was missing url field."
+                )
+            if direction == PresignedUrlDirection.Upload and not fields:
+                message = "Failed to generate presigned URL for model file upload. Response was missing 'fields' attribute."
+                raise PresignedURLException(message)
+
+            results.append(PresignedUrlResponse(model_name, url, fields))
+
+        return results
+
+    def get_model_download_urls(
+        self, model_name_batch: List[str]
+    ) -> List[PresignedUrlResponse]:
+        return self._get_presigned_urls(
+            model_name_batch, PresignedUrlDirection.Download
+        )
 
-    def get_model_upload_url(self, full_model_name: str) -> PresignedUrlResponse:
-        return self._get_presigned_url(full_model_name, PresignedUrlDirection.Upload)
+    def get_model_upload_url(self, model_name: str) -> PresignedUrlResponse:
+        return self._get_presigned_urls([model_name], PresignedUrlDirection.Upload)[0]
```

### Comparing `garden_ai-0.5.1/garden_ai/client.py` & `garden_ai-0.5.2/garden_ai/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -457,19 +457,36 @@
 
         """
         garden = garden_search.get_remote_garden_by_doi(doi, self.search_client)
         self._generate_presigned_urls_for_garden(garden)
         return garden
 
     def _generate_presigned_urls_for_garden(self, garden: Garden):
+        all_model_names = [
+            model_name
+            for pipeline in garden.pipelines
+            for model_name in pipeline.model_full_names
+        ]  # flatten all model names
+        all_presigned_urls = self.backend_client.get_model_download_urls(
+            all_model_names
+        )
         for pipeline in garden.pipelines:
-            pipeline_url_json = self.generate_presigned_urls_for_pipeline(pipeline)
-            pipeline._env_vars = {GardenConstants.URL_ENV_VAR_NAME: pipeline_url_json}
+            model_name_to_url = {
+                presigned_url.model_name: presigned_url.url
+                for presigned_url in all_presigned_urls
+                if presigned_url.model_name in pipeline.model_full_names
+            }
+            pipeline._env_vars = {
+                GardenConstants.URL_ENV_VAR_NAME: json.dumps(model_name_to_url)
+            }
 
     def generate_presigned_urls_for_pipeline(
         self, pipeline: Union[RegisteredPipeline, Pipeline]
     ) -> str:
-        model_name_to_url = {}
-        for model_name in pipeline.model_full_names:
-            url = self.backend_client.get_model_download_url(model_name).url
-            model_name_to_url[model_name] = url
+        all_presigned_urls = self.backend_client.get_model_download_urls(
+            pipeline.model_full_names
+        )
+        model_name_to_url = {
+            presigned_url.model_name: presigned_url.url
+            for presigned_url in all_presigned_urls
+        }
         return json.dumps(model_name_to_url)
```

### Comparing `garden_ai-0.5.1/garden_ai/datacite.py` & `garden_ai-0.5.2/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/gardens.py` & `garden_ai-0.5.2/garden_ai/gardens.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/globus_compute/containers.py` & `garden_ai-0.5.2/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/globus_compute/login_manager.py` & `garden_ai-0.5.2/garden_ai/globus_compute/login_manager.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.5.2/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/globus_search/garden_search.py` & `garden_ai-0.5.2/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/local_data.py` & `garden_ai-0.5.2/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/mlmodel.py` & `garden_ai-0.5.2/garden_ai/mlmodel.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/model_file_transfer/upload.py` & `garden_ai-0.5.2/garden_ai/model_file_transfer/upload.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/pipelines.py` & `garden_ai-0.5.2/garden_ai/pipelines.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/steps.py` & `garden_ai-0.5.2/garden_ai/steps.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/templates/pipeline` & `garden_ai-0.5.2/garden_ai/templates/pipeline`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/utils/_meta.py` & `garden_ai-0.5.2/garden_ai/utils/_meta.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/utils/filesystem.py` & `garden_ai-0.5.2/garden_ai/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/garden_ai/utils/misc.py` & `garden_ai-0.5.2/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.1/pyproject.toml` & `garden_ai-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "0.5.1" # placeholder
+version = "v0.5.2" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -30,15 +30,15 @@
 python = "^3.8"
 requests = "^2.20.0"
 globus-sdk = "^3.12.0"
 pydantic = "^1.10.2"
 typer = { extras = ["all"], version = "^0.7.0" }
 beartype = "^0.12.0"
 jinja2 = "^3.1.2"
-mlflow = "^2.3.2"
+mlflow = "^2.4.2"
 # numba is an indirect dep of ML Flow.
 # Specifying a recent version of it helps avoid install issues on M1 Macs
 numba = "^0.56"
 boto3 = "^1.26.77"
 dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
```

### Comparing `garden_ai-0.5.1/PKG-INFO` & `garden_ai-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.5.1
+Version: 0.5.2
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
@@ -20,15 +20,15 @@
 Provides-Extra: torch
 Requires-Dist: beartype (>=0.12.0,<0.13.0)
 Requires-Dist: boto3 (>=1.26.77,<2.0.0)
 Requires-Dist: dparse[conda] (>=0.6.2,<0.7.0)
 Requires-Dist: globus-compute-sdk (>=2.2.0,<3.0.0)
 Requires-Dist: globus-sdk (>=3.12.0,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: mlflow (>=2.3.2,<3.0.0)
+Requires-Dist: mlflow (>=2.4.2,<3.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "all"
```

