# Comparing `tmp/titan-iris-0.9.2.tar.gz` & `tmp/titan-iris-0.9.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.9.2.tar", last modified: Thu Jul 13 09:37:22 2023, max compression
+gzip compressed data, was "titan-iris-0.9.2.dev5.tar", last modified: Thu Jul 13 08:48:33 2023, max compression
```

## Comparing `titan-iris-0.9.2.tar` & `titan-iris-0.9.2.dev5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-13 09:37:09.000000 titan-iris-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 09:37:09.000000 titan-iris-0.9.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 09:37:09.000000 titan-iris-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-13 09:37:22.773489 titan-iris-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-13 09:37:09.000000 titan-iris-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 09:37:09.000000 titan-iris-0.9.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-13 09:37:09.000000 titan-iris-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 09:37:09.000000 titan-iris-0.9.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 09:37:22.777489 titan-iris-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 09:37:09.000000 titan-iris-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    26312 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-07-13 09:37:09.000000 titan-iris-0.9.2/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-13 09:37:22.000000 titan-iris-0.9.2/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-13 09:37:22.000000 titan-iris-0.9.2/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:37:22.000000 titan-iris-0.9.2/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 09:37:22.000000 titan-iris-0.9.2/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 09:37:22.000000 titan-iris-0.9.2/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 09:37:22.000000 titan-iris-0.9.2/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:37:22.773489 titan-iris-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-13 09:37:09.000000 titan-iris-0.9.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-13 09:37:09.000000 titan-iris-0.9.2/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 08:48:33.345836 titan-iris-0.9.2.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.337836 titan-iris-0.9.2.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.337836 titan-iris-0.9.2.dev5/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18417 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/tests/test_sdk.py
```

### Comparing `titan-iris-0.9.2/.gitignore` & `titan-iris-0.9.2.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/Dockerfile` & `titan-iris-0.9.2.dev5/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/PKG-INFO` & `titan-iris-0.9.2.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.9.2
+Version: 0.9.2.dev5
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.9.2/README.md` & `titan-iris-0.9.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/setup.py` & `titan-iris-0.9.2.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/config.yaml` & `titan-iris-0.9.2.dev5/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/gradio/run.py` & `titan-iris-0.9.2.dev5/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/main.py` & `titan-iris-0.9.2.dev5/src/iris/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import typer
 import yaml
 from trogon import Trogon
 from typer.main import get_group
 import iris.sdk as sdk
 
-from .sdk.utils import exception_to_json_error
+from .sdk.utils import exception_to_json_error, valid_qlora
 
 logger = getLogger(__name__)
 logger.setLevel(sdk.conf_mgr.LOG_LEVEL)
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                   sdk CLI Module                                                     #
 
@@ -455,15 +455,14 @@
                 print("Label indices must start at zero")
                 raise typer.Abort()
 
             label_names_list = [label_names_dict[i] for i in range(label_names_num)]
             flags.update({"label_names": label_names_list})
 
     elif task == "language_modelling" or task == "language_modeling":
-        task = "language_modelling"
         # sequence of task specific flags
         # if the flag shouldn't be accepted, set error_message to the error string to print.
         # if it should be, and you want to warn, print, but don't set error_message
         error_message = False
         if type == "athena":
             error_message = "Knowledge distillation is not yet supported for language modelling."
         if label_column and len(label_column):
@@ -473,19 +472,31 @@
         if num_labels is not None:
             print("num_labels is not necessary for language modelling tasks")
         if label_names is not None and len(label_names) > 0:
             print("label_names is not necessary for language modelling tasks")
         if has_negative:
             print("has_negative is not necessary for language modelling tasks")
 
+        if no_qlora and valid_qlora(model):  # If want to disable qlora, but qlora is available:
+            print(f"QLoRA manually disabled for {model}")
+            use_qlora = False
+        elif not no_qlora and not valid_qlora(model):  # If qlora isn't explicitly disabled, but is not available.
+            print(f"QLoRA not available for {model}. Proceeding without QLoRA.")
+            use_qlora = False
+        elif no_qlora and not valid_qlora(model):  # Qlora disabled, but it wasn't available anyways.
+            use_qlora = False
+        else:  # Qlora not explicitly disabled, and qlora is available.
+            print("QLoRA is available and will be used.")
+            use_qlora = True
+
         if error_message:
             print(error_message)
             raise typer.Abort()
         else:
-            flags.update({"text_fields": text_fields, "no_qlora": no_qlora})
+            flags.update({"text_fields": text_fields, "use_qlora": use_qlora})
     else:
         print(f"Unrecognised task {task}")
         raise typer.Abort()
 
     if num_epochs >= 99:
         logging.warning(
             "Woah there cowboy, that's a mighty high number of epochs you got there. "
```

### Comparing `titan-iris-0.9.2/src/iris/sdk/auth_utils.py` & `titan-iris-0.9.2.dev5/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/sdk/conf_manager.py` & `titan-iris-0.9.2.dev5/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/sdk/exception.py` & `titan-iris-0.9.2.dev5/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/sdk/iris_sdk.py` & `titan-iris-0.9.2.dev5/src/iris/sdk/iris_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 import os
 from datetime import datetime
 from importlib import util
 from pathlib import Path
 from typing import List, Optional, Union
 from urllib.parse import urljoin
 
-
-from .utils import valid_qlora
-
 # for iris infer
 import numpy as np
 
 # for iris pull
 import requests
 import tritonclient.http
 from rich import print
@@ -45,17 +42,17 @@
     print_status_dict_results,
     pull_image,
     telemetry_decorator,
     upload_from_file,
 )
 
 try:
-    from importlib import metadata as import_metadata
+    from importlib import metadata
 except ImportError:  # for Python<3.8
-    import importlib_metadata as import_metadata
+    import importlib_metadata as metadata
 
 
 # ───────────────────────────────────────────────────── imports ────────────────────────────────────────────────────── #
 
 
 # Whether to use tqdm for progress bars
 TQDM = True
@@ -125,56 +122,32 @@
         headers = {}
     endpoint = "experiment"
     # detype the flags, so we can send them
     payload = {k: str(val) if val is not None else None for k, val in flags.items()}
     logger.debug(f"Dispatching job with payload {payload}")
     url = urljoin(conf_mgr.runner_url, f"{endpoint}/")
 
-    local_family = None
     for local_artefact_field in ["model", "dataset"]:
         local_artefact = payload[local_artefact_field]
         if os.path.exists(local_artefact):
             print(
                 f"Local {local_artefact_field} found. \
                 If you intended to use a huggingface module then rename the local file."
             )  # todo
-            server_artefact = upload(
+            local_uuid = upload(
                 name=local_artefact.split("/")[-1],
                 src=local_artefact,
                 description="Experiment model",
                 internal_artefact_type=local_artefact_field,
             )  # todo add more data to the uploaded model?
-            if server_artefact:
-                payload[local_artefact_field] = server_artefact["uuid"]
-                if local_artefact_field == "model":
-                    local_family = json.loads(server_artefact["metadata"])["local_model_family"]
+            if local_uuid:
+                payload[local_artefact_field] = local_uuid
             else:
                 raise UploadOnPostError
 
-    if flags["task"] == "language_modelling":
-        if flags["no_qlora"] and valid_qlora(flags["model"], local_family):
-            # If want to disable qlora, but qlora is available:
-            print(f"QLoRA manually disabled for {flags['model']}")
-            use_qlora = False
-        elif not flags["no_qlora"] and not valid_qlora(flags["model"], local_family):
-            # If qlora isn't explicitly disabled, but is not available.
-            print(f"QLoRA not available for {flags['model']}. Proceeding without QLoRA.")
-            use_qlora = False
-        elif flags["no_qlora"] and not valid_qlora(flags["model"], local_family):
-            # Qlora disabled, but it wasn't available anyways.
-            use_qlora = False
-        else:  # Qlora not explicitly disabled, and qlora is available.
-            print("QLoRA is available and will be used.")
-            use_qlora = True
-        payload.pop("no_qlora")
-    else:
-        use_qlora = False
-    payload.update({"use_qlora": use_qlora})
-    payload.update({"local_model_family": local_family})
-
     headers.update({"Authorization": f"Bearer {conf_mgr.access_token}"})
     response = requests.post(url=url, headers=headers, data=payload)
     if not response.ok:
         raise handle_bad_response(response, endpoint)  # already returns json object
     else:
         dumped_response = dump(response)
         if json_output:
@@ -573,15 +546,15 @@
                 datetime.strptime(existing_artefact["time_created"], "%Y-%m-%dT%H:%M:%S.%fZ").strftime(
                     "%d-%m-%Y %H:%M:%S"
                 )
             )
             # Return artefact data for found/existing artefact.
             if not internal_artefact_type:
                 print(f"Artefact was already uploaded at {created_time} with ID: {existing_artefact['uuid']}")
-            return existing_artefact
+            return existing_artefact["uuid"]
 
     data = post_req_response.json()["artefact"]
     art_uuid = data["uuid"]
     endpoint = "artefact/link/" + art_uuid + "/upload"
     url = urljoin(conf_mgr.runner_url, f"{endpoint}")
     logger.debug(f"Getting link from {url}")
     get_link_resp = requests.get(url=url, headers=headers)
@@ -610,15 +583,15 @@
                 print(json.dumps(result, indent=4))
             else:
                 print(
                     f"Upload validated. This {art_type} can now be used in experiments \
                     by referring to it by UUID: {art_uuid}"
                 )
                 print(f"Alternatively, you can continue to use the {art_type}'s filepath.")
-            return data
+            return art_uuid
     else:
         print("Upload failed")
         for key, value in upload_response.items():
             if isinstance(value, Path):
                 upload_response[key] = str(value)
         return dump(upload_response)
 
@@ -717,18 +690,18 @@
     if failed_packages:
         print(
             "To use the safetensors convert, you must have the following packages installed: ",
             failed_packages,
         )
         print("NB: These packages do not need to be installed with gpu support.")
         return
-    if import_metadata.version("transformers") < "4.27.0":
+    if metadata.version("transformers") < "4.27.0":
         print(
             "To use makesafe you must have transformers >= 4.27.0. You currently have "
-            + import_metadata.version("transformers")
+            + metadata.version("transformers")
         )
         return
     # else
     from .safe_convert import do_convert
 
     do_convert(model)
```

### Comparing `titan-iris-0.9.2/src/iris/sdk/safe_convert.py` & `titan-iris-0.9.2.dev5/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/src/iris/sdk/utils.py` & `titan-iris-0.9.2.dev5/src/iris/sdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,33 +233,29 @@
             tarred.seek(0)
             reader_wrapper = CallbackIOWrapper(t.update, tarred, "read")
             response = requests.put(dst, data=reader_wrapper)
             response.raise_for_status()
             return response
 
 
-def valid_qlora(model_name: str, local_family: str):
+def valid_qlora(model_name: str):
     """Cleanses an input model name and then checks if QLoRA has been implemented for it.
 
     This is based on those available in Olympus.
 
     Args:
         model_name: A model name as from model_name_or_path
-        local_family: The model family if it has previously been determined (for uploaded models).
 
     Returns: (Bool) Whether QLoRa is supported for the given model.
 
     """
 
     def clean(x: str) -> str:
         return x.replace("-", "").replace("_", "").lower()
 
-    if local_family and local_family in VALID_QLORA_MODELS:
-        return True
-
     if any(ext in clean(model_name) for ext in VALID_QLORA_MODELS):
         return True
     return False
 
 
 def exception_to_json_error(e: Exception):
     """Convert an exception to a json string with the error message and type."""
```

### Comparing `titan-iris-0.9.2/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.9.2.dev5/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.9.2
+Version: 0.9.2.dev5
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.9.2/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.9.2.dev5/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/tests/test_cli.py` & `titan-iris-0.9.2.dev5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2/tests/test_sdk.py` & `titan-iris-0.9.2.dev5/tests/test_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         patch_response = mocker.Mock()
         patch_response.json = mocker.Mock(return_value={"status": "success"})
         patch_response.ok = True
         patch_mock = mocker.patch("requests.patch", return_value=patch_response)
         mocker.patch("requests.patch", patch_mock)
 
-        result = upload(json_output=True, src=temp_dir_path, name="test_name", description="test_description")["uuid"]
+        result = upload(json_output=True, src=temp_dir_path, name="test_name", description="test_description")
         try:
             json.loads(result)
         except:
             pytest.fail("upload() did not return valid JSON")
 
 
 # --------------------------------------    iris get     -------------------------------------- #
```

