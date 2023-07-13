# Comparing `tmp/coiled-0.8.8.dev9.tar.gz` & `tmp/coiled-0.8.9.dev1.tar.gz`

## Comparing `coiled-0.8.8.dev9.tar` & `coiled-0.8.9.dev1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/context.py
--rw-r--r--   0        0        0   102668 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/magic.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/run.py
--rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/scan.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/types.py
--rw-r--r--   0        0        0    55029 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    46115 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0    93181 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.8.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102668 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/magic.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/run.py
+-rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/types.py
+-rw-r--r--   0        0        0    55030 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    46115 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    94043 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59085 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.9.dev1/PKG-INFO
```

### Comparing `coiled-0.8.8.dev9/coiled/__init__.py` & `coiled-0.8.9.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/analytics.py` & `coiled-0.8.9.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/auth.py` & `coiled-0.8.9.dev1/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cluster.py` & `coiled-0.8.9.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/coiled.yaml` & `coiled-0.8.9.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/context.py` & `coiled-0.8.9.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/core.py` & `coiled-0.8.9.dev1/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/exceptions.py` & `coiled-0.8.9.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/magic.py` & `coiled-0.8.9.dev1/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/run.py` & `coiled-0.8.9.dev1/coiled/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,15 @@
                 client = self.cluster.get_client()
                 if self.cluster.shutdown_on_close:
                     client.register_scheduler_plugin(NoClientShutdown(keepalive=self.keepalive))
                 _clients[self._name] = client
                 return client
 
     def __call__(self, *args, **kwargs):
-        # TODO, priority and stuff
-        return self.client.run_on_scheduler(self.function, *args, **kwargs)
+        return self.client.submit(self.function, *args, **kwargs).result()
 
     def local(self, *args, **kwargs):
         return self.function(*args, **kwargs)
 
     def submit(self, *args, **kwargs) -> dask.distributed.Future:
         """Submit function call for asynchronous execution
 
@@ -161,13 +160,14 @@
             allow_ssh=True,
             environ=environ,
             scheduler_gpu=gpu,
             region=region,
             arm=arm,
             shutdown_on_close=shutdown_on_close,
             compute_purchase_option=compute_purchase_option,
+            extra_worker_on_scheduler=True,
             tags={"coiled-cluster-type": "run/python"},
         )
 
         return Function(func, cluster_kwargs, keepalive=keepalive)
 
     return decorator
```

### Comparing `coiled-0.8.8.dev9/coiled/scan.py` & `coiled-0.8.9.dev1/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/shutdown.py` & `coiled-0.8.9.dev1/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/software.py` & `coiled-0.8.9.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/types.py` & `coiled-0.8.9.dev1/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/utils.py` & `coiled-0.8.9.dev1/coiled/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -685,15 +685,15 @@
         from IPython.core.getipython import get_ipython
 
         ipython = get_ipython()
         if ipython and ipython.config.get("SpyderKernelApp"):
             is_spyder = True
 
     if is_spyder:
-        print("Creating Cluster. This might take a few minutes...")
+        print("Creating Cluster. This usually takes 1-2 minutes...")
         return Console(force_jupyter=False)
     return Console()
 
 
 def verify_aws_credentials(aws_access_key_id: str, aws_secret_access_key: str):
     """Verifies AWS Credentials are valid"""
     sts = boto3.client(
```

### Comparing `coiled-0.8.8.dev9/coiled/websockets.py` & `coiled-0.8.9.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/config.py` & `coiled-0.8.9.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/core.py` & `coiled-0.8.9.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/curl.py` & `coiled-0.8.9.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/env.py` & `coiled-0.8.9.dev1/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/login.py` & `coiled-0.8.9.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/package_sync.py` & `coiled-0.8.9.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/prefect.py` & `coiled-0.8.9.dev1/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/run.py` & `coiled-0.8.9.dev1/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/utils.py` & `coiled-0.8.9.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.8.9.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.8.9.dev1/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/cluster/logs.py` & `coiled-0.8.9.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/cluster/metrics.py` & `coiled-0.8.9.dev1/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.8.9.dev1/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/cluster/utils.py` & `coiled-0.8.9.dev1/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.8.9.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.8.9.dev1/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/setup/__init__.py` & `coiled-0.8.9.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/setup/amp.py` & `coiled-0.8.9.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/setup/aws.py` & `coiled-0.8.9.dev1/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/setup/entry.py` & `coiled-0.8.9.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/setup/gcp.py` & `coiled-0.8.9.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.8.9.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/extensions/prefect/runners.py` & `coiled-0.8.9.dev1/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/extensions/prefect/workers.py` & `coiled-0.8.9.dev1/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/v2/__init__.py` & `coiled-0.8.9.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/v2/cluster.py` & `coiled-0.8.9.dev1/coiled/v2/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,16 @@
     account
         Name of Coiled account to use. If not provided, will
         default to the user account for the ``cloud`` object being used.
     shutdown_on_close
         Whether or not to shut down the cluster when it finishes.
         Defaults to True, unless name points to an existing cluster.
     idle_timeout
-        Shut down the cluster after this duration if no activity has occurred.
+        Shut down the cluster after this duration if no activity has occurred. E.g. "30 minutes"
+        Default: "20 minutes"
     use_scheduler_public_ip
         Boolean value that determines if the Python client connects to the
         Dask scheduler using the scheduler machine's public IP address. The
         default behaviour when set to True is to connect to the scheduler
         using its public IP address, which means traffic will be routed over
         the public internet. When set to False, traffic will be routed over
         the local network the scheduler lives in, so make sure the scheduler
@@ -347,14 +348,15 @@
         package_sync: Union[bool, List[str]] = False,
         package_sync_strict: bool = False,
         package_sync_ignore: Optional[List[str]] = None,
         package_sync_fail_on: Literal["critical-only", "warning-or-higher", "any"] = "critical-only",
         private_to_creator: Optional[bool] = None,
         use_best_zone: bool = True,
         compute_purchase_option: Optional[Literal["on-demand", "spot", "spot_with_fallback"]] = None,
+        extra_worker_on_scheduler: Optional[bool] = None,
         # easier network config
         scheduler_port: Optional[int] = None,
         allow_ingress_from: Optional[str] = None,
         allow_ssh: Optional[bool] = None,
         jupyter: Optional[bool] = None,
         region: Optional[str] = None,
         arm: Optional[bool] = None,
@@ -466,14 +468,16 @@
 
         # Set cluster attributes from kwargs (first choice) or dask config
 
         self.private_to_creator = (
             dask.config.get("coiled.private-to-creator") if private_to_creator is None else private_to_creator
         )
 
+        self.extra_worker_on_scheduler = extra_worker_on_scheduler
+
         # FIXME what happens when no kwargs passed but coiled.software is set in dask config?
         self.software_environment = software or dask.config.get("coiled.software")
         self.software_container = container
         if not container and not software and not package_sync:
             self.package_sync = True
 
         self.worker_class = worker_class or dask.config.get("coiled.worker.class")
@@ -591,14 +595,15 @@
                 "ingress"
             ]  # type: ignore
 
         if jupyter:
             self.scheduler_options["jupyter"] = True
 
         if idle_timeout:
+            dask.utils.parse_timedelta(idle_timeout)  # fail fast if dask can't parse this timedelta
             self.scheduler_options["idle_timeout"] = idle_timeout
 
         if not self.asynchronous:
             # If we don't close the cluster, the user's ipython session gets spammed with
             # messages from distributed.
             #
             # Note that this doesn't solve all such spammy dead clusters (which is probably still
@@ -644,27 +649,15 @@
                         additional_data={
                             **self._as_json_compatible(),
                         },
                     )
             if self.start_adaptive:
                 adaptive_max = 20
                 logger.warn(
-                    f"""n_workers was not specified so turning on adaptive scaling with a min
-of {n_workers} and max of {adaptive_max}.
-
-To specify a specific cluster size:
-
-    cluster = coiled.Cluster(n_workers=100, ...)
-
-Alternatively, to control adaptive scaling:
-
-    cluster = coiled.Cluster(...)
-    cluster.adapt(minimum=0, maximum=100)
-
-For more information, see: https://docs.coiled.io/user_guide/clusters/size-and-type.html. and https://docs.coiled.io/user_guide/clusters/scale.html#adaptive-scaling.
+                    """Using adaptive scaling. To manually control the size of your cluster, use n_workers=.
 """
                 )
                 self.adapt(minimum=n_workers, maximum=adaptive_max)
 
     @property
     def details_url(self):
         return get_details_url(self.cloud.server, self.account, self.cluster_id)
@@ -1182,23 +1175,24 @@
                     scheduler_vm_types=scheduler_vm_types_to_use,
                     worker_vm_types=worker_vm_types_to_use,
                     backend_options=self.backend_options,
                     use_scheduler_public_ip=self.use_scheduler_public_ip,
                     use_dashboard_https=self.use_dashboard_https,
                     senv_v2_id=senv_v2_id,
                     private_to_creator=self.private_to_creator,
+                    extra_worker_on_scheduler=self.extra_worker_on_scheduler,
                 )
                 cluster_created = not cluster_existed
 
             if not self.cluster_id:
                 raise RuntimeError(f"Failed to find/create cluster {self.name}")
 
             if cluster_created:
                 logger.info(
-                    f"Creating Cluster (name: {self.name}, {self.details_url} ). This might take a few minutes..."
+                    f"Creating Cluster (name: {self.name}, {self.details_url} ). This usually takes 1-2 minutes..."
                 )
             else:
                 logger.info(f"Attaching to existing cluster (name: {self.name}, {self.details_url} )")
 
             await self._attach_to_cluster(is_new_cluster=cluster_created)
             await super()._start()
 
@@ -1938,19 +1932,36 @@
         List of worker addresses to close, if any
 
         See Also
         --------
         Scheduler.workers_to_close
         """
         scheduler_comm = self._ensure_scheduler_comm()
-        ret = await scheduler_comm.workers_to_close(
+
+        target_offset = 0
+        if self.extra_worker_on_scheduler and target:
+            # ask for an extra worker we can remove, so that if worker-on-scheduler is in the list
+            # we can keep it alive and still get to target number of workers
+            target_offset = 1
+            target -= target_offset
+
+        workers = await scheduler_comm.workers_to_close(
             target=target,
             attribute="name",
         )
-        return ret  # type: ignore
+
+        if self.extra_worker_on_scheduler and workers:
+            # Never include the extra worker-on-scheduler in list of workers to kill.
+            # Because we requested an extra possible worker (so we'd still get desired number if
+            # worker-on-scheduler was in the list), we need only return the desired number (in case
+            # extra worker-on-scheduler was *not* in the list of workers to kill).
+            desired_workers = len(workers) - target_offset
+            return list(filter(lambda name: "scheduler" not in name, workers))[:desired_workers]
+
+        return workers  # type: ignore
 
     def adapt(self, Adaptive=CoiledAdaptive, **kwargs) -> Adaptive:
         """Dynamically scale the number of workers in the cluster
         based on scaling heuristics.
 
         Parameters
         ----------
```

### Comparing `coiled-0.8.8.dev9/coiled/v2/core.py` & `coiled-0.8.9.dev1/coiled/v2/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,14 +620,15 @@
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         worker_disk_throughput: Optional[int] = None,
         backend_options: Optional[Union[AWSOptions, GCPOptions, dict]] = None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         private_to_creator: Optional[bool] = None,
+        extra_worker_on_scheduler: Optional[bool] = None,
     ) -> Tuple[int, bool]:
         # TODO (Declarative): support these args, or decide not to
         # https://gitlab.com/coiled/cloud/-/issues/4305
 
         if scheduler_class is not None:
             raise ValueError("scheduler_class is not supported in beta/new Coiled yet")
 
@@ -652,14 +653,15 @@
             "scheduler_options": scheduler_options,
             "environ": environ,
             "tags": tags,
             "dask_config": dask_config,
             "private_to_creator": private_to_creator,
             "env_id": senv_v2_id,
             "env_name": software_environment,
+            "extra_worker_on_scheduler": extra_worker_on_scheduler,
             # "jupyter_on_scheduler": True,
         }
 
         backend_options = backend_options if backend_options else {}
 
         if gcp_worker_gpu_type is not None:
             # for backwards compatibility with v1 options
```

### Comparing `coiled-0.8.8.dev9/coiled/v2/cwi_log_link.py` & `coiled-0.8.9.dev1/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/v2/states.py` & `coiled-0.8.9.dev1/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/v2/widgets/__init__.py` & `coiled-0.8.9.dev1/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/v2/widgets/rich.py` & `coiled-0.8.9.dev1/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/coiled/v2/widgets/util.py` & `coiled-0.8.9.dev1/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/LICENSE` & `coiled-0.8.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/README.md` & `coiled-0.8.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/pyproject.toml` & `coiled-0.8.9.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.8.dev9/PKG-INFO` & `coiled-0.8.9.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.8.dev9
+Version: 0.8.9.dev1
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
-Metadata-Version: 2.1 Name: coiled Version: 0.8.8.dev9 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.8.9.dev1 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

