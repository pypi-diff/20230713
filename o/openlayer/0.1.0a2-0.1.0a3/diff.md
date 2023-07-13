# Comparing `tmp/openlayer-0.1.0a2.tar.gz` & `tmp/openlayer-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlayer-0.1.0a2.tar", last modified: Thu Jun 29 21:23:33 2023, max compression
+gzip compressed data, was "openlayer-0.1.0a3.tar", last modified: Thu Jul 13 18:08:06 2023, max compression
```

## Comparing `openlayer-0.1.0a2.tar` & `openlayer-0.1.0a3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-29 21:23:33.678828 openlayer-0.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer/
--rw-r--r--   0 runner    (1001) docker     (123)    55482 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer/prediction_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/prediction_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/prediction_jobs/classification_prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/prediction_jobs/regression_prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/base_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/baseline_model_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/commit_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/dataset_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/model_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/project_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-29 21:23:33.678828 openlayer-0.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/tests/test_openlayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/openlayer/
+-rw-r--r--   0 runner    (1001) docker     (123)    55482 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/openlayer/prediction_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/prediction_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/prediction_jobs/classification_prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/prediction_jobs/regression_prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/openlayer/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/baseline_model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25445 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/commit_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/dataset_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/validators/project_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/openlayer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/openlayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-13 18:08:06.000000 openlayer-0.1.0a3/openlayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-13 18:08:06.000000 openlayer-0.1.0a3/openlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:08:06.000000 openlayer-0.1.0a3/openlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:08:06.000000 openlayer-0.1.0a3/openlayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 18:08:06.000000 openlayer-0.1.0a3/openlayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 18:08:06.000000 openlayer-0.1.0a3/openlayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:06.296269 openlayer-0.1.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 18:07:25.000000 openlayer-0.1.0a3/tests/test_openlayer.py
```

### Comparing `openlayer-0.1.0a2/LICENSE` & `openlayer-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/PKG-INFO` & `openlayer-0.1.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.1.0a2/README.md` & `openlayer-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/__init__.py` & `openlayer-0.1.0a3/openlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/api.py` & `openlayer-0.1.0a3/openlayer/api.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/datasets.py` & `openlayer-0.1.0a3/openlayer/datasets.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/exceptions.py` & `openlayer-0.1.0a3/openlayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/models.py` & `openlayer-0.1.0a3/openlayer/models.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/prediction_jobs/classification_prediction_job.py` & `openlayer-0.1.0a3/openlayer/prediction_jobs/classification_prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/prediction_jobs/regression_prediction_job.py` & `openlayer-0.1.0a3/openlayer/prediction_jobs/regression_prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/project_versions.py` & `openlayer-0.1.0a3/openlayer/project_versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,16 +95,20 @@
             indefinitely.
 
         Returns
         -------
         ProjectVersion
             The project version object.
         """
+        self.print_status_report()
         while self.status not in [TaskStatus.COMPLETED, TaskStatus.FAILED]:
+            prev_status_msg = self.status_message
             self.refresh()
+            if self.status_message != prev_status_msg:
+                self.print_status_report()
             time.sleep(1)
             if timeout:
                 timeout -= 1
                 if timeout <= 0:
                     print(
                         "Timeout exceeded. Visit the Openlayer dashboard to"
                         " check the status of the project version."
@@ -116,14 +120,18 @@
             print("Project version processed successfully.")
 
     def refresh(self):
         """Refreshes the project version object with the latest
         information from the server."""
         self._json = self.client.load_project_version(self.id).to_dict()
 
+    def print_status_report(self):
+        """Prints the status report along with its status message."""
+        print("Status:", self.status.value, "(" + f"{self.status_message}" + ")")
+
     def print_goal_report(self):
         """Prints the goal results of the project version."""
         if self.status != TaskStatus.COMPLETED:
             print("Project version is not complete. Nothing to print.")
             return
         print(
             tabulate.tabulate(
```

### Comparing `openlayer-0.1.0a2/openlayer/projects.py` & `openlayer-0.1.0a3/openlayer/projects.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/schemas.py` & `openlayer-0.1.0a3/openlayer/schemas.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/tasks.py` & `openlayer-0.1.0a3/openlayer/tasks.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/utils.py` & `openlayer-0.1.0a3/openlayer/utils.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/validators/base_validator.py` & `openlayer-0.1.0a3/openlayer/validators/base_validator.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/validators/baseline_model_validators.py` & `openlayer-0.1.0a3/openlayer/validators/baseline_model_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/validators/commit_validators.py` & `openlayer-0.1.0a3/openlayer/validators/commit_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         # Use data from the validation as test data
         sample_data = None
         validation_dataset_df = utils.load_dataset_from_bundle(
             bundle_path=self.bundle_path, label="validation"
         )
         if validation_dataset_df is not None:
             sample_data = validation_dataset_df[
-                self.validation_dataset_config["textColumnName"]
+                [self.validation_dataset_config["textColumnName"]]
             ].head()
 
         return sample_data
 
     def _validate_input_consistency(self):
         """Currently, there are no input consistency checks for text
         bundles."""
```

### Comparing `openlayer-0.1.0a2/openlayer/validators/dataset_validators.py` & `openlayer-0.1.0a3/openlayer/validators/dataset_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/validators/model_validators.py` & `openlayer-0.1.0a3/openlayer/validators/model_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/validators/project_validators.py` & `openlayer-0.1.0a3/openlayer/validators/project_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/openlayer/version.py` & `openlayer-0.1.0a3/openlayer/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,8 +18,8 @@
          headers=headers,
          params=params,
          json=body,
          files=files,
          data=data,
       )
 """
-__version__ = "0.1.0a2"
+__version__ = "0.1.0a3"
```

### Comparing `openlayer-0.1.0a2/openlayer.egg-info/PKG-INFO` & `openlayer-0.1.0a3/openlayer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.1.0a2/openlayer.egg-info/SOURCES.txt` & `openlayer-0.1.0a3/openlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a2/setup.cfg` & `openlayer-0.1.0a3/setup.cfg`

 * *Files identical despite different names*

