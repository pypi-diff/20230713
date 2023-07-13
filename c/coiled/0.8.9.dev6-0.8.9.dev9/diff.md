# Comparing `tmp/coiled-0.8.9.dev6.tar.gz` & `tmp/coiled-0.8.9.dev9.tar.gz`

## Comparing `coiled-0.8.9.dev6.tar` & `coiled-0.8.9.dev9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/context.py
--rw-r--r--   0        0        0   102668 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/exceptions.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/magic.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/run.py
--rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/scan.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/types.py
--rw-r--r--   0        0        0    55030 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/__init__.py
--rw-r--r--   0        0        0    94043 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/cluster.py
--rw-r--r--   0        0        0    59085 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.9.dev6/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/context.py
+-rw-r--r--   0        0        0   102271 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/exceptions.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/magic.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/run.py
+-rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/scan.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/types.py
+-rw-r--r--   0        0        0    55355 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    94043 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59085 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/PKG-INFO
```

### Comparing `coiled-0.8.9.dev6/coiled/__init__.py` & `coiled-0.8.9.dev9/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/analytics.py` & `coiled-0.8.9.dev9/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/auth.py` & `coiled-0.8.9.dev9/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cluster.py` & `coiled-0.8.9.dev9/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/coiled.yaml` & `coiled-0.8.9.dev9/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/context.py` & `coiled-0.8.9.dev9/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/core.py` & `coiled-0.8.9.dev9/coiled/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     handle_credentials,
     in_async_call,
     parse_gcp_region_zone,
     parse_identifier,
     parse_requested_memory,
     rich_console,
     validate_account,
-    verify_aws_credentials,
+    verify_aws_credentials_with_retry,
 )
 from .websockets import ConfigureBackendConnector
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 console = Console()
 SUPPORTED_BACKENDS = {"aws", "gcp"}
 
@@ -2691,26 +2691,15 @@
     console = Console()
 
     if backend not in SUPPORTED_BACKENDS:
         raise UnsupportedBackendError(f"Supplied backend: {backend} not in supported types: {SUPPORTED_BACKENDS}")
 
     if aws_access_key_id and aws_secret_access_key:
         # verify that these are valid credentials
-        for turn in range(3):
-            try:
-                verify_aws_credentials(aws_access_key_id, aws_secret_access_key)
-                break
-            except Exception:
-                # this is to address InvalidClientTokenId but doesn't hurt to retry everything
-                # a few times with expo backoff
-                if turn < 2:
-                    sleep_time = 2 ** (turn + 1)
-                    time.sleep(sleep_time)
-                else:
-                    raise
+        verify_aws_credentials_with_retry(aws_access_key_id, aws_secret_access_key)
 
     parsed_gcp_credentials: Optional[Dict] = None
 
     # Parse GCP region/zones or return default region/zone
     gcp_region, gcp_zone = parse_gcp_region_zone(region=gcp_region, zone=gcp_zone)
 
     if backend == "aws":
```

### Comparing `coiled-0.8.9.dev6/coiled/exceptions.py` & `coiled-0.8.9.dev9/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/magic.py` & `coiled-0.8.9.dev9/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/run.py` & `coiled-0.8.9.dev9/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/scan.py` & `coiled-0.8.9.dev9/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/shutdown.py` & `coiled-0.8.9.dev9/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/software.py` & `coiled-0.8.9.dev9/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/types.py` & `coiled-0.8.9.dev9/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/utils.py` & `coiled-0.8.9.dev9/coiled/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -690,16 +690,21 @@
 
     if is_spyder:
         print("Creating Cluster. This usually takes 1-2 minutes...")
         return Console(force_jupyter=False)
     return Console()
 
 
+@backoff.on_exception(backoff.expo, Exception, max_time=10)
+def verify_aws_credentials_with_retry(aws_access_key_id: str, aws_secret_access_key: str):
+    verify_aws_credentials(aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key)
+
+
 def verify_aws_credentials(aws_access_key_id: str, aws_secret_access_key: str):
-    """Verifies AWS Credentials are valid"""
+    """Verify AWS Credentials are valid, raise exception so caller knows what is wrong with credentials."""
     sts = boto3.client(
         "sts",
         aws_access_key_id=aws_access_key_id,
         aws_secret_access_key=aws_secret_access_key,
     )
     sts.get_caller_identity()
```

### Comparing `coiled-0.8.9.dev6/coiled/websockets.py` & `coiled-0.8.9.dev9/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/config.py` & `coiled-0.8.9.dev9/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/core.py` & `coiled-0.8.9.dev9/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/curl.py` & `coiled-0.8.9.dev9/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/env.py` & `coiled-0.8.9.dev9/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/login.py` & `coiled-0.8.9.dev9/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/package_sync.py` & `coiled-0.8.9.dev9/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/prefect.py` & `coiled-0.8.9.dev9/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/run.py` & `coiled-0.8.9.dev9/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/utils.py` & `coiled-0.8.9.dev9/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/cluster/__init__.py` & `coiled-0.8.9.dev9/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/cluster/better_logs.py` & `coiled-0.8.9.dev9/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/cluster/logs.py` & `coiled-0.8.9.dev9/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/cluster/metrics.py` & `coiled-0.8.9.dev9/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/cluster/ssh.py` & `coiled-0.8.9.dev9/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/cluster/utils.py` & `coiled-0.8.9.dev9/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/notebook/__init__.py` & `coiled-0.8.9.dev9/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/notebook/notebook.py` & `coiled-0.8.9.dev9/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/setup/__init__.py` & `coiled-0.8.9.dev9/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/setup/amp.py` & `coiled-0.8.9.dev9/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/setup/aws.py` & `coiled-0.8.9.dev9/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/setup/entry.py` & `coiled-0.8.9.dev9/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/setup/gcp.py` & `coiled-0.8.9.dev9/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/cli/setup/prometheus.py` & `coiled-0.8.9.dev9/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/extensions/prefect/runners.py` & `coiled-0.8.9.dev9/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/extensions/prefect/workers.py` & `coiled-0.8.9.dev9/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/__init__.py` & `coiled-0.8.9.dev9/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/cluster.py` & `coiled-0.8.9.dev9/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/core.py` & `coiled-0.8.9.dev9/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/cwi_log_link.py` & `coiled-0.8.9.dev9/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/states.py` & `coiled-0.8.9.dev9/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/widgets/__init__.py` & `coiled-0.8.9.dev9/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/widgets/rich.py` & `coiled-0.8.9.dev9/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/coiled/v2/widgets/util.py` & `coiled-0.8.9.dev9/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/LICENSE` & `coiled-0.8.9.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/README.md` & `coiled-0.8.9.dev9/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/pyproject.toml` & `coiled-0.8.9.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev6/PKG-INFO` & `coiled-0.8.9.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.9.dev6
+Version: 0.8.9.dev9
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.8.9.dev6 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.8.9.dev9 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

