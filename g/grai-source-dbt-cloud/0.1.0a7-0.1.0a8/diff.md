# Comparing `tmp/grai_source_dbt_cloud-0.1.0a7.tar.gz` & `tmp/grai_source_dbt_cloud-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.1.0a7.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.1.0a8.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.1.0a7.tar` & `grai_source_dbt_cloud-0.1.0a8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a7/README.md
--rw-r--r--   0        0        0     1125 2023-07-12 11:24:15.058831 grai_source_dbt_cloud-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0       77 2023-07-12 11:24:21.735353 grai_source_dbt_cloud-0.1.0a7/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0     1210 2023-07-12 11:08:02.586185 grai_source_dbt_cloud-0.1.0a7/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0     4833 2023-07-12 10:52:48.692538 grai_source_dbt_cloud-0.1.0a7/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a7/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a8/README.md
+-rw-r--r--   0        0        0     1126 2023-07-13 14:58:35.653851 grai_source_dbt_cloud-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-07-13 13:05:07.861271 grai_source_dbt_cloud-0.1.0a8/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     1204 2023-07-12 11:33:35.152949 grai_source_dbt_cloud-0.1.0a8/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     5409 2023-07-13 14:38:41.844838 grai_source_dbt_cloud-0.1.0a8/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a8/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a8/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.1.0a7/pyproject.toml` & `grai_source_dbt_cloud-0.1.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt_cloud"
-version = "0.1.0-alpha7"
+version = "0.1.0-alpha8"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt_cloud", from = "src" },
 ]
 readme = "README.md"
@@ -14,15 +14,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
-grai-source-dbt = {version = "^0.3.0a7", allow-prereleases = true}
+grai-source-dbt = {version = "^0.3.0a11", allow-prereleases = true}
 dbtc = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.991"
 black = "^22.12.0"
```

### Comparing `grai_source_dbt_cloud-0.1.0a7/src/grai_source_dbt_cloud/base.py` & `grai_source_dbt_cloud-0.1.0a8/src/grai_source_dbt_cloud/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,17 +6,15 @@
     GraiIntegrationImplementation,
 )
 from grai_schemas.base import SourcedEdge, SourcedNode
 from grai_schemas.v1.source import SourceV1
 from grai_source_dbt_cloud.loader import DbtCloudConnector
 
 
-class DbtCloudIntegration(
-    CombinedNodesAndEdgesMixin, EventMixin, GraiIntegrationImplementation
-):
+class DbtCloudIntegration(CombinedNodesAndEdgesMixin, EventMixin, GraiIntegrationImplementation):
     def __init__(
         self,
         api_key: str,
         source: SourceV1,
         version: Optional[str] = None,
         namespace: Optional[str] = "default",
     ):
```

### Comparing `grai_source_dbt_cloud-0.1.0a7/src/grai_source_dbt_cloud/loader.py` & `grai_source_dbt_cloud-0.1.0a8/src/grai_source_dbt_cloud/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from grai_source_dbt.adapters import adapt_to_client
 from grai_source_dbt.processor import ManifestProcessor
 
 
 class Event:
     """ """
 
-    def __init__(self, reference: str, date: str, status: str, metadata: dict, nodes: List[str]):
+    def __init__(
+        self, reference: str, date: str, status: str, metadata: dict, nodes: List[str]
+    ):
         self.reference = reference
         self.date = date
         self.status = status
         self.metadata = metadata
         self.nodes = nodes
 
 
@@ -45,15 +47,17 @@
 
     def get_nodes_and_edges(self):
         """ """
         manifest_obj = self.client.cloud.get_most_recent_run_artifact(
             account_id=self.default_account["id"], path="manifest.json"
         )
 
-        manifest = ManifestProcessor.load(manifest_obj, self.namespace, self.source.spec)
+        manifest = ManifestProcessor.load(
+            manifest_obj, self.namespace, self.source.spec
+        )
 
         return manifest.adapted_nodes, manifest.adapted_edges
 
     def get_events(self, last_event_date) -> List[Event]:
         """
 
         Args:
@@ -61,23 +65,30 @@
 
         Returns:
 
         Raises:
 
         """
 
-        runs = self.get_runs(account_id=self.default_account["id"], last_event_date=last_event_date)
+        runs = self.get_runs(
+            account_id=self.default_account["id"], last_event_date=last_event_date
+        )
 
         events = []
 
         for run in runs:
-            if last_event_date and datetime.fromisoformat(run["created_at"]) < last_event_date:
+            if (
+                last_event_date
+                and datetime.fromisoformat(run["created_at"]) < last_event_date
+            ):
                 break
 
-            nodes = self.get_run_nodes(account_id=self.default_account["id"], run_id=run["id"])
+            nodes = self.get_run_nodes(
+                account_id=self.default_account["id"], run_id=run["id"]
+            )
 
             status = "success" if run["status"] == 10 else "error"
 
             events.append(
                 Event(
                     reference=run["id"],
                     date=run["created_at"],
@@ -122,15 +133,24 @@
                     unique_id (str):
 
                 Returns:
 
                 Raises:
 
                 """
-                return adapt_to_client(manifest.loader.node_map[unique_id]).spec.name
+                try:
+                    res = adapt_to_client(
+                        manifest.loader.node_map[unique_id], self.source.spec, "v1"
+                    ).spec.name
+                except:
+                    raise Exception(
+                        f"Could not find node for {unique_id}, account_id: {account_id}, run_id: {run_id}"
+                    )
+
+                return res
 
             return inner
 
         run_results = None
 
         try:
             run_results = self.client.cloud.get_run_artifact(
@@ -148,18 +168,22 @@
             )
         except:
             print(f"Something has gone wrong, no manifest.json for run {run_id}")
 
             return []
 
         unique_ids = [
-            result["unique_id"] for result in run_results["results"] if not result["unique_id"].startswith("test.")
+            result["unique_id"]
+            for result in run_results["results"]
+            if not result["unique_id"].startswith("test.")
         ]
 
-        manifest = ManifestProcessor.load(manifest_obj, self.namespace)
+        manifest = ManifestProcessor.load(
+            manifest_obj, self.namespace, self.source.spec
+        )
 
         name_mapper = get_adapted_node_map(manifest=manifest)
 
         return [name_mapper(unique_id) for unique_id in unique_ids]
 
     def get_runs(self, account_id: str, last_event_date):
         """
@@ -187,13 +211,17 @@
             )
 
             runs.extend(result["data"])
 
             if result["extra"]["pagination"]["total_count"] <= len(runs):
                 break
 
-            if last_event_date and datetime.fromisoformat(result["data"][-1]["created_at"]) < last_event_date:
+            if (
+                last_event_date
+                and datetime.fromisoformat(result["data"][-1]["created_at"])
+                < last_event_date
+            ):
                 break
 
             offset += limit
 
         return runs
```

### Comparing `grai_source_dbt_cloud-0.1.0a7/PKG-INFO` & `grai_source_dbt_cloud-0.1.0a8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbtc (>=0.4.2,<0.5.0)
 Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
-Requires-Dist: grai-source-dbt (>=0.3.0a7,<0.4.0)
+Requires-Dist: grai-source-dbt (>=0.3.0a11,<0.4.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt-cloud
 Description-Content-Type: text/markdown
 
 # Grai dbt Cloud Integration
```

