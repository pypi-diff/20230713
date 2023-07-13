# Comparing `tmp/aitomatic-1.3.0.tar.gz` & `tmp/aitomatic-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitomatic-1.3.0.tar", last modified: Tue Jul 11 02:29:39 2023, max compression
+gzip compressed data, was "aitomatic-1.3.1.tar", last modified: Tue Jul 11 04:44:20 2023, max compression
```

## Comparing `aitomatic-1.3.0.tar` & `aitomatic-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.869127 aitomatic-1.3.0/
--rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.3.0/LICENSE
--rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.3.0/MANIFEST.in
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-07-11 02:29:39.869315 aitomatic-1.3.0/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.3.0/README.md
--rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.3.0/pyproject.toml
--rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.3.0/requirements.txt
--rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-07-11 02:29:39.870600 aitomatic-1.3.0/setup.cfg
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.822116 aitomatic-1.3.0/src/
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.848249 aitomatic-1.3.0/src/aitomatic/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/__init__.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.857881 aitomatic-1.3.0/src/aitomatic/api/
--rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/api/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)    10935 2023-07-11 02:28:42.000000 aitomatic-1.3.0/src/aitomatic/api/build.py
--rw-r--r--   0 hungvo     (501) staff       (20)     7441 2023-07-11 02:28:42.000000 aitomatic-1.3.0/src/aitomatic/api/client.py
--rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/api/exceptions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/api/model_params.py
--rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/api/tuning_utils.py
--rw-r--r--   0 hungvo     (501) staff       (20)    16606 2023-07-11 02:28:42.000000 aitomatic-1.3.0/src/aitomatic/api/web_model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.864030 aitomatic-1.3.0/src/aitomatic/dsl/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_conclusions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_features.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_handler.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.3.0/src/aitomatic/dsl/arl_rules.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.3.0/src/aitomatic/dsl/utils.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.868234 aitomatic-1.3.0/src/aitomatic/objects/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.3.0/src/aitomatic/objects/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-07-03 03:38:53.000000 aitomatic-1.3.0/src/aitomatic/objects/dataset.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.3.0/src/aitomatic/objects/model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 02:29:39.851384 aitomatic-1.3.0/src/aitomatic.egg-info/
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/SOURCES.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/dependency_links.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/requires.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-07-11 02:29:39.000000 aitomatic-1.3.0/src/aitomatic.egg-info/top_level.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-07-11 02:28:57.000000 aitomatic-1.3.0/version.txt
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.376624 aitomatic-1.3.1/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.3.1/LICENSE
+-rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.3.1/MANIFEST.in
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-07-11 04:44:20.376855 aitomatic-1.3.1/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.3.1/README.md
+-rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.3.1/pyproject.toml
+-rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.3.1/requirements.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-07-11 04:44:20.378040 aitomatic-1.3.1/setup.cfg
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.348107 aitomatic-1.3.1/src/
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.352705 aitomatic-1.3.1/src/aitomatic/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.3.1/src/aitomatic/__init__.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.367349 aitomatic-1.3.1/src/aitomatic/api/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.3.1/src/aitomatic/api/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    12366 2023-07-11 02:32:26.000000 aitomatic-1.3.1/src/aitomatic/api/build.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    11242 2023-07-11 02:32:26.000000 aitomatic-1.3.1/src/aitomatic/api/client.py
+-rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.3.1/src/aitomatic/api/exceptions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.3.1/src/aitomatic/api/model_params.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.3.1/src/aitomatic/api/tuning_utils.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    18015 2023-07-11 02:32:26.000000 aitomatic-1.3.1/src/aitomatic/api/web_model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.372539 aitomatic-1.3.1/src/aitomatic/dsl/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.3.1/src/aitomatic/dsl/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.3.1/src/aitomatic/dsl/arl_conclusions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.3.1/src/aitomatic/dsl/arl_features.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.3.1/src/aitomatic/dsl/arl_handler.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.3.1/src/aitomatic/dsl/arl_rules.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.3.1/src/aitomatic/dsl/utils.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.375804 aitomatic-1.3.1/src/aitomatic/objects/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.3.1/src/aitomatic/objects/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-07-03 03:38:53.000000 aitomatic-1.3.1/src/aitomatic/objects/dataset.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.3.1/src/aitomatic/objects/model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-07-11 04:44:20.355160 aitomatic-1.3.1/src/aitomatic.egg-info/
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-07-11 04:44:20.000000 aitomatic-1.3.1/src/aitomatic.egg-info/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-07-11 04:44:20.000000 aitomatic-1.3.1/src/aitomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-07-11 04:44:20.000000 aitomatic-1.3.1/src/aitomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-07-11 04:44:20.000000 aitomatic-1.3.1/src/aitomatic.egg-info/requires.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-07-11 04:44:20.000000 aitomatic-1.3.1/src/aitomatic.egg-info/top_level.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-07-11 04:44:09.000000 aitomatic-1.3.1/version.txt
```

### Comparing `aitomatic-1.3.0/LICENSE` & `aitomatic-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/PKG-INFO` & `aitomatic-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.3.0
+Version: 1.3.1
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.3.0/README.md` & `aitomatic-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/setup.cfg` & `aitomatic-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/api/__init__.py` & `aitomatic-1.3.1/src/aitomatic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/api/build.py` & `aitomatic-1.3.1/src/aitomatic/api/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,80 +123,83 @@
         ]
 
         return conclusion_threshold_hyperparms
 
     def update_training_job_status(self, training_jobs: dict) -> dict:
         for model_name in list(training_jobs.keys):
             status, model = self.check_model_status(model_name=model_name)
-            if (status != 'training'):
+            if status != "training":
                 training_jobs.pop(model_name)
         return training_jobs
 
-    
     def tune_model_with_hyperparams(
         self,
         tuning_params: List[Any],
         base_name: str,
         model_type: str,
         knowledge_name: str,
         data_name: str,
         mapping_data: Any,
         label_columns: Any,
         metadata: Any,
     ) -> pd.DataFrame:
         model_log = []
         # print(f"Creating training jobs, {tuning_params}")
-        max_training_tasks = 16
-        current_training_tasks = {}
-        num_executed_jobs = 0
-        while num_executed_jobs < max_training_tasks:
-            if len(current_training_tasks) < max_training_tasks:
-                item = tuning_params[num_executed_jobs]
-                test_params = {**item}
-                model_name = f'{base_name} {num_executed_jobs}'
-                resp = self.build_model(
-                    model_type,
-                    model_name,
-                    knowledge_name,
-                    data_name,
-                    mapping_data=mapping_data,
-                    label_columns=label_columns,
-                    metadata=metadata,
-                    **item,
-                )
-                print(f'Training model {model_name}: {resp["id"]}')
-                test_params['id'] = resp['id']
-                test_params['model_name'] = model_name
-                test_params['status'] = 'training'
-                model_log.append(test_params)
-                current_training_tasks[model_name] = 'training'
-                num_executed_jobs += 1
-            else:
-                current_training_tasks = self.update_training_job_status(current_training_tasks)
-                time.sleep(5)
-                
-        # print(f'Creating training {len(tuning_params)} jobs')
-        # for i, item in enumerate(tuning_params):
-        #     test_params = {**item}
-        #     model_name = f"{base_name} {i}"
-        #     resp = self.build_model(
-        #         model_type,
-        #         model_name,
-        #         knowledge_name,
-        #         data_name,
-        #         mapping_data=mapping_data,
-        #         label_columns=label_columns,
-        #         metadata=metadata,
-        #         **item,
-        #     )
-        #     print(f'Training model {model_name}: {resp["id"]}')
-        #     test_params["id"] = resp["id"]
-        #     print(f'Creating training job for {model_name}: {test_params}')
-        #     test_params["model_name"] = model_name
-        #     model_log.append(test_params)
+        # max_training_tasks = 16
+        # current_training_tasks = {}
+        # num_executed_jobs = 0
+        # while num_executed_jobs < max_training_tasks:
+        #     if len(
+        #         current_training_tasks
+        #     ) < max_training_tasks and num_executed_jobs < len(tuning_params):
+        #         item = tuning_params[num_executed_jobs]
+        #         test_params = {**item}
+        #         model_name = f"{base_name} {num_executed_jobs}"
+        #         resp = self.build_model(
+        #             model_type,
+        #             model_name,
+        #             knowledge_name,
+        #             data_name,
+        #             mapping_data=mapping_data,
+        #             label_columns=label_columns,
+        #             metadata=metadata,
+        #             **item,
+        #         )
+        #         print(f'Training model {model_name}: {resp["id"]}')
+        #         test_params["id"] = resp["id"]
+        #         test_params["model_name"] = model_name
+        #         test_params["status"] = "training"
+        #         model_log.append(test_params)
+        #         current_training_tasks[model_name] = "training"
+        #         num_executed_jobs += 1
+        #     else:
+        #         current_training_tasks = self.update_training_job_status(
+        #             current_training_tasks
+        #         )
+        #         time.sleep(5)
+
+        print(f"Creating training {len(tuning_params)} jobs")
+        for i, item in enumerate(tuning_params):
+            test_params = {**item}
+            model_name = f"{base_name} {i}"
+            resp = self.build_model(
+                model_type,
+                model_name,
+                knowledge_name,
+                data_name,
+                mapping_data=mapping_data,
+                label_columns=label_columns,
+                metadata=metadata,
+                **item,
+            )
+            print(f'Training model {model_name}: {resp["id"]}')
+            test_params["id"] = resp["id"]
+            print(f"Creating training job for {model_name}: {test_params}")
+            test_params["model_name"] = model_name
+            model_log.append(test_params)
         model_df = pd.DataFrame(model_log)
         model_df["status"] = "training"
         model_df["output"] = {}
 
         return model_df
 
     def check_model_status(self, model_name):
@@ -234,14 +237,49 @@
             model_df.to_parquet(file_path)
             if model_df["status"].isin(["training"]).any():
                 time.sleep(sleep_time)
             else:
                 break
         return model_df
 
+    def wait_for_task_to_complete(
+        self,
+        file_path: str = "tuning.parquet",
+        sleep_time: int = 30,
+    ):
+        print("Waiting for training jobs to complete")
+        model_df = pd.read_parquet(file_path)
+        while True:
+            not_done_df: pd.DataFrame = model_df[
+                (model_df["status"] != "success") & (model_df["status"] != "error")
+            ]
+            ids = not_done_df["id"].to_list()
+
+            # call request to bulk get model info
+            status, output = self.project.get_model_status_bulk(ids)
+
+            not_done_df.loc[:, "status"] = status
+            not_done_df.loc[:, "output"] = output
+
+            model_df.update(not_done_df)
+
+            success_length = len(model_df[model_df["status"] == "success"])
+            error_length = len(model_df[model_df["status"] == "error"])
+            df_length = len(model_df)
+            print(
+                f"Waiting for training jobs to complete: [{success_length} success, {error_length} error, {df_length} total]"
+            )
+            # print(f"MODEL_DF: {model_df.to_string()}")
+            model_df.to_parquet(file_path)
+            if model_df["status"].isin(["training"]).any():
+                time.sleep(sleep_time)
+            else:
+                break
+        return model_df
+
     def get_metadata(seft, data: Dataset, mapping_column: dict):
         metadata = {}
         dataset_metadata = data.metadata
         for key, value in mapping_column.items():
             if value in dataset_metadata:
                 metadata[key] = dataset_metadata[value]
         return metadata
@@ -272,15 +310,15 @@
         C: float = 1.0,
         # penalty: str = 'l2'
     ):
         return {
             "type": "LogisticRegression",
             "hyperparams": {
                 # 'threshold': threshold,
-                'C': C,
+                "C": C,
                 # 'penalty': penalty,
             },
         }
 
     def build_random_forest_param(
         self,
         # n_estimators: int = 3,
```

### Comparing `aitomatic-1.3.0/src/aitomatic/api/model_params.py` & `aitomatic-1.3.1/src/aitomatic/api/model_params.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/api/tuning_utils.py` & `aitomatic-1.3.1/src/aitomatic/api/tuning_utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/api/web_model.py` & `aitomatic-1.3.1/src/aitomatic/api/web_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import sys
 from typing import Dict, Tuple, Union, List, Any
 from itertools import product
-from multiprocessing.pool import ThreadPool
 
 from tqdm import tqdm
 from itertools import chain
 import requests
 import json
 import pandas as pd
 import numpy as np
@@ -72,14 +71,15 @@
         self.MODELS_ENDPOINT = f"{self.MODEL_API_ROOT}/models"
         self.PREDICTION_ENDPOINT = f"{self.MODEL_API_ROOT}/inferencing"
         self.METADATA_ENDPOINT = f"{self.MODELS_ENDPOINT}/metadata"
         self.METRICS_ENDPOINT = f"{self.MODELS_ENDPOINT}/metrics"
 
         self.KNOWLEDGE_DETAIL = lambda id_: f"{self.CLIENT_API_ROOT}/knowledges/" + id_
         self.DATA_DETAIL = lambda id_: f"{self.CLIENT_API_ROOT}/data/" + id_
+        self.RUN_INFERENCES = f"{self.CLIENT_API_ROOT}/inference"
 
     def batch_predict(self, input_data: Dict) -> Dict:
         """
         Chunks data in input_data['X'] and does prediction in batches
         """
         # TODO: Make this more versatile to it slices all large data in input
         # data, not just 'X' ... maybe
@@ -97,24 +97,24 @@
             f"{chunk_max /1024} kb or {N} data points"
         )
         out = []
         sliced_data = self.slice_data(X, N)
         for Xi in tqdm(sliced_data, total=total_batches):
             pred = self.predict({self.data_key: Xi, **Xother})[self.output_key]
             out.append(pred)
-        
+
         # num_threads = 4
         # pools = ThreadPool(num_threads)
         # thread_results = []
         # # for Xi in tqdm(sliced_data, total=total_batches):
 
         # for i, Xi in enumerate(sliced_data):
         #     print(f"chunkId: {i}")
         #     thread_results.append(pools.apply_async(self.predict, args=({self.data_key: Xi, **Xother}, i)))
-        
+
         # print("before out")
         # out1 = [res.get() for res in thread_results]
         # print(f"after out1: {out1}")
         # # print(f"OUT1: {out1}")
         # out = [o[0][self.output_key] for o in out1]
         # print(f"Out: {out}")
 
@@ -342,14 +342,32 @@
             err = f"{resp.status_code}: {resp.content}"
             raise ConnectionError(err)
 
     def log_metrics(self, key, value):
         self.metrics[key] = value
         self._save_metrics()
 
+    def run_inference(self, model_name: list, dataset_name: str):
+        data = {
+            "model_name": model_name,
+            "dataset_name": dataset_name,
+            "project_name": self.project_name,
+        }
+
+        resp = requests.post(
+            self.RUN_INFERENCES,
+            headers={
+                "accept": "application/json",
+                "authorization": self.api_token,
+            },
+            json=data,
+        )
+
+        return resp
+
     @staticmethod
     def get_model_names(api_token=None, project_name=None):
         if project_name is None:
             project_id = os.getenv("AITOMATIC_PROJECT_ID")
         else:
             project_id = get_project_id(project_name, api_token=api_token)
 
@@ -473,10 +491,36 @@
     model_df = model.tune_with_hyperparams(tuning_params, base_name=base_name)
     try:
         model_df.to_parquet(output_model_df_path)
     except Exception as e:
         print(f"Failed to save model_df to {output_model_df_path}")
         print(e)
     if wait_for_tuning_to_complete:
-        builder.wait_for_tuning_to_complete(
-            model_df, file_path=output_model_df_path, sleep_time=10
-        )
+        # builder.wait_for_tuning_to_complete(
+        #     model_df, file_path=output_model_df_path, sleep_time=10
+        # )
+
+        builder.wait_for_task_to_complete(file_path=output_model_df_path, sleep_time=10)
+
+
+def run_inference(project_name: str, model_names: list, dataset_name: str, **kwargs):
+    project_manager = ProjectManager(project_name=project_name)
+
+    results = project_manager.run_inference(
+        model_name=model_names, dataset_name=dataset_name
+    )
+
+    inference_tasks = results.get("results", [])
+
+    df = pd.DataFrame(inference_tasks)
+
+    file_path = kwargs.get("file_path", "infer_results.parquet")
+    df.to_parquet(file_path)
+
+    if kwargs.get("wait_for_inference_to_complete", True):
+        df = project_manager.wait_for_inference_to_complete(file_path, sleep_time=10)
+
+    if kwargs.get("download_inference_results", False):
+        output_folder = kwargs.get("output_folder", "inference_results")
+        project_manager.download_inference_results(folder_path=output_folder, df=df)
+
+    return inference_tasks
```

### Comparing `aitomatic-1.3.0/src/aitomatic/dsl/arl_conclusions.py` & `aitomatic-1.3.1/src/aitomatic/dsl/arl_conclusions.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/dsl/arl_features.py` & `aitomatic-1.3.1/src/aitomatic/dsl/arl_features.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/dsl/arl_handler.py` & `aitomatic-1.3.1/src/aitomatic/dsl/arl_handler.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/dsl/arl_rules.py` & `aitomatic-1.3.1/src/aitomatic/dsl/arl_rules.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/dsl/utils.py` & `aitomatic-1.3.1/src/aitomatic/dsl/utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/objects/dataset.py` & `aitomatic-1.3.1/src/aitomatic/objects/dataset.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic/objects/model.py` & `aitomatic-1.3.1/src/aitomatic/objects/model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.3.0/src/aitomatic.egg-info/PKG-INFO` & `aitomatic-1.3.1/src/aitomatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.3.0
+Version: 1.3.1
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.3.0/src/aitomatic.egg-info/SOURCES.txt` & `aitomatic-1.3.1/src/aitomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

