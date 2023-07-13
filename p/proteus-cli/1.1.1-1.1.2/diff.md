# Comparing `tmp/proteus_cli-1.1.1.tar.gz` & `tmp/proteus_cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-1.1.1.tar", max compression
+gzip compressed data, was "proteus_cli-1.1.2.tar", max compression
```

## Comparing `proteus_cli-1.1.1.tar` & `proteus_cli-1.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3124 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/buckets/commands.py
--rw-r--r--   0        0        0     2810 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/config.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1277 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0     6754 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0     1068 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/__init__.py
--rw-r--r--   0        0        0      789 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/case.py
--rw-r--r--   0        0        0     2381 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/common.py
--rw-r--r--   0        0        0      142 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/step.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/facilities/__init__.py
--rw-r--r--   0        0        0     1166 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/facilities/case.py
--rw-r--r--   0        0        0      825 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/facilities/common.py
--rw-r--r--   0        0        0      146 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/facilities/step.py
--rw-r--r--   0        0        0      167 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/well_model/__init__.py
--rw-r--r--   0        0        0     2762 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/well_model/case.py
--rw-r--r--   0        0        0     1415 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/well_model/common.py
--rw-r--r--   0        0        0      145 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/config/well_model/step.py
--rw-r--r--   0        0        0      673 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    12408 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     7051 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0      411 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     8822 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/sources/az.py
--rw-r--r--   0        0        0     1289 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     3895 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     6930 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/simulations/opm.py
--rw-r--r--   0        0        0        0 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/utils/__init__.py
--rw-r--r--   0        0        0     8114 2023-07-12 15:03:38.568021 proteus_cli-1.1.1/cli/utils/files.py
--rw-r--r--   0        0        0      385 2023-07-12 15:03:38.572021 proteus_cli-1.1.1/cli/utils/sssh.py
--rw-r--r--   0        0        0     1917 2023-07-12 15:03:38.572021 proteus_cli-1.1.1/cli/utils/sync.py
--rw-r--r--   0        0        0      449 2023-07-12 15:03:38.572021 proteus_cli-1.1.1/logging.ini
--rw-r--r--   0        0        0     1528 2023-07-12 15:03:38.572021 proteus_cli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 proteus_cli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3124 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2810 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/config.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1277 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0     6754 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0     1068 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/case.py
+-rw-r--r--   0        0        0     2381 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/common.py
+-rw-r--r--   0        0        0      142 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/step.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/facilities/__init__.py
+-rw-r--r--   0        0        0     1800 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/facilities/case.py
+-rw-r--r--   0        0        0      825 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/facilities/common.py
+-rw-r--r--   0        0        0      146 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/facilities/step.py
+-rw-r--r--   0        0        0      167 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/well_model/__init__.py
+-rw-r--r--   0        0        0     2762 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/well_model/case.py
+-rw-r--r--   0        0        0     1415 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/well_model/common.py
+-rw-r--r--   0        0        0      145 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/config/well_model/step.py
+-rw-r--r--   0        0        0      673 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    12408 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     7051 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0      411 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     9216 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0     1289 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     3895 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     6930 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-07-13 13:04:04.943558 proteus_cli-1.1.2/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/cli/simulations/opm.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/cli/utils/__init__.py
+-rw-r--r--   0        0        0     8114 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/cli/utils/files.py
+-rw-r--r--   0        0        0      385 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/cli/utils/sssh.py
+-rw-r--r--   0        0        0     1917 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/cli/utils/sync.py
+-rw-r--r--   0        0        0      449 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/logging.ini
+-rw-r--r--   0        0        0     1528 2023-07-13 13:04:04.947558 proteus_cli-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 proteus_cli-1.1.2/PKG-INFO
```

### Comparing `proteus_cli-1.1.1/cli/__init__.py` & `proteus_cli-1.1.2/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/api/decorators.py` & `proteus_cli-1.1.2/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/api/hooks.py` & `proteus_cli-1.1.2/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/buckets/commands.py` & `proteus_cli-1.1.2/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/config.py` & `proteus_cli-1.1.2/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/commands.py` & `proteus_cli-1.1.2/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/__init__.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/case.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/case.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/cnn_pca/common.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/cnn_pca/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/facilities/case.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/facilities/case.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import os
-from collections import defaultdict
+from pathlib import Path
 
 from preprocessing.facilities.flowline import preprocess as preprocess_flowline
 
 from cli.datasets.preprocessor.config import BaseConfig, CaseStepConfig
 from cli.utils.files import RequiredFilePath
 
 
@@ -15,24 +14,35 @@
         Create a preprocesor for each case group
 
         Args: -
 
         Returns:
             iterator: the list of groups to preprocess
         """
-        groups = defaultdict(list)
+        groups = {}
         for c in self.cases:
-            groups[c["group"]].append(c)
+            group = c["group"]
+            if group not in groups:
+                groups[group] = {
+                    "cases": [],
+                    "output_path": Path(c["root"]).parents[0] / "flowline.h5",  # cases/{group}/flowline.h5
+                    "root": Path(c["root"]).parents[2],  # cases/{group}/SIMULATION_{case}/../../..
+                }
+
+            # old_root = os.path.join(os.path.join(os.path.split(cases[0]["root"])[0], ".."), "..")
+            input_path = Path(c["root"]) / "*.csv"  # cases/{group}/SIMULATION_{case}/*.csv
+            groups[group]["cases"].append(input_path)
 
         return tuple(
             CaseStepConfig(
-                input=tuple(RequiredFilePath(f"{os.path.split(c['root'])[1]}/*.csv") for c in cases),
-                output=(RequiredFilePath("flowline.h5"),),
+                input=(RequiredFilePath("network.csv"),)
+                + tuple(RequiredFilePath(input_path) for input_path in group["cases"]),
+                output=(RequiredFilePath(group["output_path"]),),
                 preprocessing_fn=preprocess_flowline,
-                root=os.path.split(cases[0]["root"])[0],  # "cases/{group}"
-                split=group,
+                root=str(group["root"]),  # The only path that needs to be a string for internal susbstrings processing
+                split=group_name,
                 case=None,
                 keep=True,
                 enabled=True,
             )
-            for group, cases in groups.items()
+            for group_name, group in groups.items()
         )
```

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/facilities/common.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/facilities/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/well_model/case.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/well_model/case.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/config/well_model/common.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/config/well_model/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-1.1.2/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/preprocessor/process_step.py` & `proteus_cli-1.1.2/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/sources/az.py` & `proteus_cli-1.1.2/cli/datasets/sources/az.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             self._init_container_client()
 
     def _parse_uri(self, uri):
         match = self.URI_re.match(uri.rstrip("/"))
         assert match is not None, f"{uri} must be a blob storage URI"
         container_name = match.groupdict()["container_name"]
         storage_url = f'https://{match.groupdict()["bucket_name"]}'
-        subpath = match.groupdict()["prefix"].split("?")[0].rstrip("/")
+        subpath = match.groupdict()["prefix"].split("?")[0].rstrip("/.").rstrip("/")
 
         uri_parts = iter(uri.split("?"))
 
         uri = next(uri_parts)
         url_sas_token = next(uri_parts, "")
 
         return container_name, storage_url, subpath, url_sas_token, uri
@@ -158,14 +158,20 @@
     _blob_cache = {}
 
     @classmethod
     @lru_cache(maxsize=50000)
     def _list_blobs_with_cache(cls, container_client, name_starts_with):
         items = cls._blob_cache.setdefault(container_client, {}).get(name_starts_with)
 
+        # First let's try "indicating" that we want to search in a directory
+        # Because maybe we want to search in "SIMULATION_1" but we also have "SIMULATION_10", "SIMULATION_100"...
+        if not items:
+            items = list(container_client.list_blobs(name_starts_with=name_starts_with + "/"))
+            cls._blob_cache[container_client][name_starts_with] = items
+
         if not items:
             items = list(container_client.list_blobs(name_starts_with=name_starts_with))
             cls._blob_cache[container_client][name_starts_with] = items
 
         return items
 
     def open(self, reference):
```

### Comparing `proteus_cli-1.1.1/cli/datasets/sources/common.py` & `proteus_cli-1.1.2/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/sources/local.py` & `proteus_cli-1.1.2/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/sources/s3.py` & `proteus_cli-1.1.2/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/datasets/upload.py` & `proteus_cli-1.1.2/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/debugger/commands.py` & `proteus_cli-1.1.2/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/debugger/init_keyword_check.py` & `proteus_cli-1.1.2/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/jobs/commands.py` & `proteus_cli-1.1.2/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/jobs/list.py` & `proteus_cli-1.1.2/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/simulations/commands.py` & `proteus_cli-1.1.2/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/simulations/create.py` & `proteus_cli-1.1.2/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/simulations/dependencySolver.py` & `proteus_cli-1.1.2/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/simulations/opm.py` & `proteus_cli-1.1.2/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/utils/files.py` & `proteus_cli-1.1.2/cli/utils/files.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/cli/utils/sync.py` & `proteus_cli-1.1.2/cli/utils/sync.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-1.1.1/pyproject.toml` & `proteus_cli-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "1.1.1"
+version = "1.1.2"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
 
@@ -18,15 +18,15 @@
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
 azure-storage-blob = "^12.8.1"
 readchar = "^3.0.4"
 azure-identity = "^1.12.0"
 markupsafe = "2.0.1"
 proteus-runtime = "0.3.0"
-proteus-preprocessing = "0.4.1"
+proteus-preprocessing = "0.4.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pre-commit = "^2.9.3"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
 pytest-bdd = "^5.0.0"
```

### Comparing `proteus_cli-1.1.1/PKG-INFO` & `proteus_cli-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: cryptography (>=3.3.2,<4.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: markupsafe (==2.0.1)
-Requires-Dist: proteus-preprocessing (==0.4.1)
+Requires-Dist: proteus-preprocessing (==0.4.2)
 Requires-Dist: proteus-runtime (==0.3.0)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Requires-Dist: readchar (>=3.0.4,<4.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: tqdm (>=4.61.0,<5.0.0)
```

