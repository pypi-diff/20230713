# Comparing `tmp/sekoia_automation_sdk-1.3.6.tar.gz` & `tmp/sekoia_automation_sdk-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.3.6.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.7.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.3.6.tar` & `sekoia_automation_sdk-1.3.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/LICENSE
--rw-r--r--   0        0        0     8422 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/README.md
--rw-r--r--   0        0        0     2114 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11420 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/action.py
--rw-r--r--   0        0        0     5477 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/config.py
--rw-r--r--   0        0        0     6998 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      596 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    13709 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     2089 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/update_sdk_version.py
--rw-r--r--   0        0        0     6094 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/storage.py
--rw-r--r--   0        0        0    14583 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/LICENSE
+-rw-r--r--   0        0        0     8422 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/README.md
+-rw-r--r--   0        0        0     2114 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/action.py
+-rw-r--r--   0        0        0     5477 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6968 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      596 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-12 10:02:47.468511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-07-12 10:02:47.472511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    13709 2023-07-12 10:02:47.472511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     2089 2023-07-12 10:02:47.472511 sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/update_sdk_version.py
+-rw-r--r--   0        0        0     6094 2023-07-12 10:02:47.472511 sekoia_automation_sdk-1.3.7/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14583 2023-07-12 10:02:47.472511 sekoia_automation_sdk-1.3.7/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-07-12 10:02:47.472511 sekoia_automation_sdk-1.3.7/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.7/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.3.6/LICENSE` & `sekoia_automation_sdk-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/README.md` & `sekoia_automation_sdk-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/pyproject.toml` & `sekoia_automation_sdk-1.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.3.6"
+version = "1.3.7"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/cli.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/connector/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any
 from urllib.parse import urljoin
 
 import orjson
 import requests
 from pydantic import BaseModel
 from requests import Response
-from tenacity import Retrying, stop_after_attempt, wait_exponential
+from tenacity import Retrying, stop_after_delay, wait_exponential
 
 from sekoia_automation.constants import CHUNK_BYTES_MAX_SIZE, EVENT_BYTES_MAX_SIZE
 from sekoia_automation.trigger import Trigger
 
 # Connector are a kind of trigger that fetch events from remote sources.
 # We should add the content of push_events_to_intakes
 # so that we are able to send events directly from connectors
@@ -42,15 +42,15 @@
         Stop the connector
         """
         super().stop(*args, **kwargs)
         self._executor.shutdown(wait=True)
 
     def _retry(self):
         return Retrying(
-            stop=stop_after_attempt(5),
+            stop=stop_after_delay(3600),  # 1 hour without being able to send events
             wait=wait_exponential(multiplier=1, min=1, max=10),
             reraise=True,
         )
 
     @cached_property
     def __connector_user_agent(self):
         return f"sekoiaio-connector-{self.configuration.intake_key}"
@@ -70,20 +70,19 @@
                     res: Response = requests.post(
                         batch_api,
                         json=request_body,
                         headers={"User-Agent": self.__connector_user_agent},
                         timeout=30,
                     )
                     res.raise_for_status()
-            if res.status_code > 299:
-                self.log(f"Intake rejected events: {res.text}", level="error")
-                res.raise_for_status()
             collect_ids[chunk_index] = res.json().get("event_ids", [])
         except Exception as ex:
-            self.log_exception(ex, message=f"Failed to forward {len(chunk)} events")
+            message = f"Failed to forward {len(chunk)} events"
+            self.log(message=message, level="error")
+            self.log_exception(ex, message=message)
 
     def push_events_to_intakes(self, events: list[str], sync: bool = False) -> list:
         # no event to push
         if not events:
             return []
 
         # Reset the consecutive error count
```

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/sync_library.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/update_sdk_version.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/scripts/update_sdk_version.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/trigger.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.7/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.6/PKG-INFO` & `sekoia_automation_sdk-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.3.6
+Version: 1.3.7
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

