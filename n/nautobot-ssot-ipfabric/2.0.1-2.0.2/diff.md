# Comparing `tmp/nautobot_ssot_ipfabric-2.0.1.tar.gz` & `tmp/nautobot_ssot_ipfabric-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_ssot_ipfabric-2.0.1.tar", max compression
+gzip compressed data, was "nautobot_ssot_ipfabric-2.0.2.tar", max compression
```

## Comparing `nautobot_ssot_ipfabric-2.0.1.tar` & `nautobot_ssot_ipfabric-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      591 2023-05-26 15:57:01.327861 nautobot_ssot_ipfabric-2.0.1/LICENSE
--rw-r--r--   0        0        0    12814 2023-05-26 15:57:01.327861 nautobot_ssot_ipfabric-2.0.1/README.md
--rw-r--r--   0        0        0     1348 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/__init__.py
--rw-r--r--   0        0        0      136 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/__init__.py
--rw-r--r--   0        0        0     7485 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py
--rw-r--r--   0        0        0    10106 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py
--rw-r--r--   0        0        0      522 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapters_shared.py
--rw-r--r--   0        0        0    19626 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/diffsync_models.py
--rw-r--r--   0        0        0    10621 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/jobs.py
--rw-r--r--   0        0        0     3063 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/signals.py
--rw-r--r--   0        0        0     8451 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric.png
--rw-r--r--   0        0        0    11662 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric_logo.png
--rw-r--r--   0        0        0       52 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/__init__.py
--rw-r--r--   0        0        0      477 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1545 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json
--rw-r--r--   0        0        0      985 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json
--rw-r--r--   0        0        0     1876 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json
--rw-r--r--   0        0        0     1639 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json
--rw-r--r--   0        0        0     3964 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py
--rw-r--r--   0        0        0     2989 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_jobs.py
--rw-r--r--   0        0        0     3522 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py
--rw-r--r--   0        0        0     5458 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nbutils.py
--rw-r--r--   0        0        0      516 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/__init__.py
--rw-r--r--   0        0        0     9440 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/nbutils.py
--rw-r--r--   0        0        0      508 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/test_utils.py
--rw-r--r--   0        0        0     5361 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/workers.py
--rw-r--r--   0        0        0     3177 2023-05-26 15:57:14.003926 nautobot_ssot_ipfabric-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    13854 1970-01-01 00:00:00.000000 nautobot_ssot_ipfabric-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-07-13 15:56:43.207484 nautobot_ssot_ipfabric-2.0.2/LICENSE
+-rw-r--r--   0        0        0    12869 2023-07-13 15:56:43.207484 nautobot_ssot_ipfabric-2.0.2/README.md
+-rw-r--r--   0        0        0     1348 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/__init__.py
+-rw-r--r--   0        0        0      136 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/__init__.py
+-rw-r--r--   0        0        0     7485 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py
+-rw-r--r--   0        0        0    10106 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py
+-rw-r--r--   0        0        0      522 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/adapters_shared.py
+-rw-r--r--   0        0        0    19626 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/diffsync_models.py
+-rw-r--r--   0        0        0    10772 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/jobs.py
+-rw-r--r--   0        0        0     3063 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/signals.py
+-rw-r--r--   0        0        0     8451 2023-07-13 15:56:43.219484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric.png
+-rw-r--r--   0        0        0    11662 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric_logo.png
+-rw-r--r--   0        0        0       52 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/__init__.py
+-rw-r--r--   0        0        0      477 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1545 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json
+-rw-r--r--   0        0        0      985 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json
+-rw-r--r--   0        0        0     1876 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json
+-rw-r--r--   0        0        0     1639 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json
+-rw-r--r--   0        0        0     3964 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py
+-rw-r--r--   0        0        0     2989 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_jobs.py
+-rw-r--r--   0        0        0     3522 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py
+-rw-r--r--   0        0        0     5458 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_nbutils.py
+-rw-r--r--   0        0        0      516 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/utilities/__init__.py
+-rw-r--r--   0        0        0     9440 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/utilities/nbutils.py
+-rw-r--r--   0        0        0      508 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/utilities/test_utils.py
+-rw-r--r--   0        0        0     5361 2023-07-13 15:56:43.223484 nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/workers.py
+-rw-r--r--   0        0        0     3177 2023-07-13 15:56:56.771588 nautobot_ssot_ipfabric-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13909 1970-01-01 00:00:00.000000 nautobot_ssot_ipfabric-2.0.2/PKG-INFO
```

### Comparing `nautobot_ssot_ipfabric-2.0.1/LICENSE` & `nautobot_ssot_ipfabric-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/README.md` & `nautobot_ssot_ipfabric-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 - `ipfabric_ssl_verify`- IP Fabric API SSL verification
 - `ipfabric_timeout`- IP Fabric API timeout
 
 Example `PLUGINS_CONFIG` to be updated in `nautobot_config.py` after successful installation. The chatops configuration is optional, but if you'd like to have the
 ability to call the sync job through chatops, you will be required to configure it.
 
 ```python
+PLUGINS = ["nautobot_ssot", "nautobot_ssot_ipfabric"]
+
 PLUGINS_CONFIG = {
     "nautobot_chatops": {
         "enable_slack": True,
         "slack_api_token": os.environ.get("SLACK_API_TOKEN"),
         "slack_signing_secret": os.environ.get("SLACK_SIGNING_SECRET"),
         "session_cache_timeout": 3600,
     },
```

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/__init__.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapters_shared.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/adapters_shared.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/diffsync_models.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/diffsync/diffsync_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/jobs.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,25 +37,24 @@
     try:
         uuid.UUID(str(identifier))
         return True
     except ValueError:
         return False
 
 
-def get_formatted_snapshots(client):
+def get_formatted_snapshots(client: IPFClient):
     """Get all loaded snapshots and format them for display in choice menu.
 
     Returns:
         dict: Snapshot objects as dict of tuples {snapshot_ref: (description, snapshot_id)}
     """
     formatted_snapshots = {}
     snapshot_refs = []
     if client:
-        client.update()
-        for snapshot_ref, snapshot in client.snapshots.items():
+        for snapshot_ref, snapshot in client.loaded_snapshots.items():
             description = ""
             if snapshot_ref in [LAST, PREV, LAST_LOCKED]:
                 description += f"{snapshot_ref}: "
                 snapshot_refs.append(snapshot_ref)
             if snapshot.name:
                 description += snapshot.name + " - " + snapshot.end.strftime("%d-%b-%y %H:%M:%S")
             else:
@@ -135,46 +134,53 @@
             "debug",
             "snapshot",
             "safe_delete_mode",
             "sync_ipfabric_tagged_only",
             "dry_run",
         )
 
+    @staticmethod
+    def _init_ipf_client():
+        try:
+            return IPFClient(
+                base_url=IPFABRIC_HOST,
+                token=IPFABRIC_API_TOKEN,
+                verify=IPFABRIC_SSL_VERIFY,
+                timeout=IPFABRIC_TIMEOUT,
+                unloaded=False,
+            )
+        except (RuntimeError, ConnectError) as error:
+            print(f"Got an error {error}")
+            return None
+
     @classmethod
     def _get_vars(cls):
         """Extend JobDataSource._get_vars to include some variables.
 
         This also initializes them.
         """
         got_vars = super()._get_vars()
 
-        if cls.snapshot is None:
-            try:
-                cls.client = IPFClient(
-                    base_url=IPFABRIC_HOST,
-                    token=IPFABRIC_API_TOKEN,
-                    verify=IPFABRIC_SSL_VERIFY,
-                    timeout=IPFABRIC_TIMEOUT,
-                )
-            except (RuntimeError, ConnectError) as error:
-                print(f"Got an error {error}")
-                cls.client = None
-
-            formatted_snapshots = get_formatted_snapshots(cls.client)
-            if formatted_snapshots:
-                default_choice = formatted_snapshots["$last"][::-1]
-            else:
-                default_choice = "$last"
+        if cls.client is None:
+            cls.client = cls._init_ipf_client()
+        else:
+            cls.client.update()
 
-            cls.snapshot = ChoiceVar(
-                description="IPFabric snapshot to sync from. Defaults to $last",
-                default=default_choice,
-                choices=[(snapshot_id, snapshot_name) for snapshot_name, snapshot_id in formatted_snapshots.values()],
-                required=False,
-            )
+        formatted_snapshots = get_formatted_snapshots(cls.client)
+        if formatted_snapshots:
+            default_choice = formatted_snapshots["$last"][::-1]
+        else:
+            default_choice = "$last"
+
+        cls.snapshot = ChoiceVar(
+            description="IPFabric snapshot to sync from. Defaults to $last",
+            default=default_choice,
+            choices=[(snapshot_id, snapshot_name) for snapshot_name, snapshot_id in formatted_snapshots.values()],
+            required=False,
+        )
 
         if hasattr(cls, "snapshot"):
             got_vars["snapshot"] = cls.snapshot
 
         return got_vars
 
     @classmethod
@@ -216,14 +222,16 @@
 
     def load_target_adapter(self):
         """Not used."""
 
     def sync_data(self):
         """Sync a device data from IP Fabric into Nautobot."""
         if self.client is None:
+            self.client = self._init_ipf_client()
+        if self.client is None:
             self.log_failure(message="IPFabric client is not ready. Check your config.")
             return
 
         self.client.snapshot_id = self.kwargs["snapshot"]
         dry_run = self.kwargs["dry_run"]
         safe_mode = self.kwargs["safe_delete_mode"]
         tagged_only = self.kwargs["sync_ipfabric_tagged_only"]
```

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/signals.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric.png` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric.png`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric_logo.png` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_jobs.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nbutils.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/tests/test_nbutils.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/__init__.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/nbutils.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/utilities/nbutils.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/workers.py` & `nautobot_ssot_ipfabric-2.0.2/nautobot_ssot_ipfabric/workers.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.1/pyproject.toml` & `nautobot_ssot_ipfabric-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-ssot-ipfabric"
-version = "v2.0.1"
+version = "v2.0.2"
 description = "Nautobot SSoT IPFabric"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode-llc/nautobot-plugin-ssot-ipfabric"
 repository = "https://github.com/networktocode-llc/nautobot-plugin-ssot-ipfabric"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `nautobot_ssot_ipfabric-2.0.1/PKG-INFO` & `nautobot_ssot_ipfabric-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-ssot-ipfabric
-Version: 2.0.1
+Version: 2.0.2
 Summary: Nautobot SSoT IPFabric
 Home-page: https://github.com/networktocode-llc/nautobot-plugin-ssot-ipfabric
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7.1,<4.0
@@ -81,14 +81,16 @@
 - `ipfabric_ssl_verify`- IP Fabric API SSL verification
 - `ipfabric_timeout`- IP Fabric API timeout
 
 Example `PLUGINS_CONFIG` to be updated in `nautobot_config.py` after successful installation. The chatops configuration is optional, but if you'd like to have the
 ability to call the sync job through chatops, you will be required to configure it.
 
 ```python
+PLUGINS = ["nautobot_ssot", "nautobot_ssot_ipfabric"]
+
 PLUGINS_CONFIG = {
     "nautobot_chatops": {
         "enable_slack": True,
         "slack_api_token": os.environ.get("SLACK_API_TOKEN"),
         "slack_signing_secret": os.environ.get("SLACK_SIGNING_SECRET"),
         "session_cache_timeout": 3600,
     },
```

