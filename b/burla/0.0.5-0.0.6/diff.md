# Comparing `tmp/burla-0.0.5.tar.gz` & `tmp/burla-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.5.tar", max compression
+gzip compressed data, was "burla-0.0.6.tar", max compression
```

## Comparing `burla-0.0.5.tar` & `burla-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      486 2023-07-04 19:11:58.812772 burla-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.5/src/burla/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.5/src/burla/_logstream.py
--rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.5/src/burla/config.py
--rw-r--r--   0        0        0     3921 2023-07-04 19:07:41.736595 burla-0.0.5/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 burla-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      486 2023-07-13 20:10:03.234590 burla-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-13 18:25:13.491110 burla-0.0.6/src/burla/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-12 19:34:52.816658 burla-0.0.6/src/burla/_logstream.py
+-rw-r--r--   0        0        0      907 2023-07-13 18:24:57.649392 burla-0.0.6/src/burla/config.py
+-rw-r--r--   0        0        0     3884 2023-07-13 19:36:19.611107 burla-0.0.6/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 burla-0.0.6/PKG-INFO
```

### Comparing `burla-0.0.5/src/burla/_logstream.py` & `burla-0.0.6/src/burla/_logstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
     last_log_printed_at = None
     is_first_log = True
     while True:
         try:
             timestamp, log_message = log_queue.get_nowait()
 
             if is_first_log:
-                sleep(6)  # should be same as remote_parallel_map.JOB_STATUS_POLL_RATE_SEC
+                sleep(6)  # remote_parallel_map.JOB_STATUS_POLL_RATE_SEC
                 is_first_log = False
 
             current_epoch = datetime.now(timezone.utc).timestamp()
 
             last_log_printed_delta = current_epoch - (last_log_printed_at or current_epoch)
             last_log_occurred_delta = timestamp - (last_log_timestamp or timestamp)
             sleep_time = max(last_log_occurred_delta - last_log_printed_delta, 0)
 
-            if last_log_occurred_delta - last_log_printed_delta < 0:
-                lateness = (last_log_occurred_delta - last_log_printed_delta) * -1
-                print(f"LATE!! Log should have printed {lateness} seconds ago!")
+            # if last_log_occurred_delta - last_log_printed_delta < 0:
+            #     lateness = (last_log_occurred_delta - last_log_printed_delta) * -1
+            #     print(f"LATE!! Log should have printed {lateness} seconds ago!")
 
             sleep(sleep_time)
             print(log_message)
             last_log_printed_at = datetime.now(timezone.utc).timestamp()
             last_log_timestamp = timestamp
         except queue.Empty:
             if stop_event.is_set():
```

### Comparing `burla-0.0.5/src/burla/config.py` & `burla-0.0.6/src/burla/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
 
 def load_api_key_from_local_config() -> Tuple[str, str]:
     if not CONFIG_PATH.exists():
         raise Exception(
             (
                 "No API key found.\n"
-                "To set an API key run: `burla config set api_key=<your API key>`\n"
+                "To set an API key run: `burla set_api_key=<your API key>`\n"
                 "To request an API key email jake@burla.dev."
             )
         )
     config = json.loads(CONFIG_PATH.read_text())
     return config["API_KEY"]
```

### Comparing `burla-0.0.5/src/burla/remote_parallel_map.py` & `burla-0.0.6/src/burla/remote_parallel_map.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 import sys
 import requests
 import threading
 import warnings
 from binascii import hexlify
-from datetime import datetime, timezone
 from typing import Callable, Optional
 from time import sleep, time
 from queue import PriorityQueue
 
 import dill
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
 BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
 JOB_ENV_REPO = "us-east4-docker.pkg.dev/burla-389321/burla-job-environments"
 
 # BURLA_SERVICE_URL = "https://127.0.0.1:5000"
 
-TZ = timezone.utc
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
 
 class JobTimeoutError(Exception):
     def __init__(self, job_id, timeout):
         super().__init__(f"Burla job with id: '{job_id}' timed out after {timeout} seconds.")
 
 
-def _get_job_info(job_id: str, last_timestamp: str, attempt=0):
+def _get_job_info(job_id: str, epoch: int, attempt=0):
     try:
-        response = requests.get(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}/{last_timestamp}")
+        response = requests.get(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}/{epoch}")
         response.raise_for_status()
         return response.json()
     except requests.exceptions.HTTPError as e:
         if str(response.status_code).startswith("5") and attempt != 3:
             warnings.warn(
                 (
                     f"Received {response.status_code} response from server checking status of job: "
                     f"{job_id} Retrying..."
                 )
             )
             sleep(2)
-            return _get_job_info(job_id, last_timestamp, attempt=attempt + 1)
+            return _get_job_info(job_id, epoch, attempt=attempt + 1)
         else:
             raise e
 
 
 def remote_parallel_map(
     function_: Callable,
     inputs: list,
@@ -54,62 +52,64 @@
     image: Optional[str] = None,
     api_key: Optional[str] = None,
 ):
     if not function_.__annotations__.get("return") is str:
         raise AttributeError("Please add the return type annotation 'str' to your input function.")
 
     if cpus > 100:
-        raise AttributeError("Currently unable to satisfy requests for >100 computers")
+        raise AttributeError("Currently unable to satisfy requests for > 100 computers")
 
     api_key = api_key or load_api_key_from_local_config()
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={"key": api_key})
     response.raise_for_status()
     job_id = response.json()["job_id"]
 
     user_python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
-    default_docker_image = f"{JOB_ENV_REPO}/python{user_python_version}/burla_job_env"
+    default_docker_image = f"{JOB_ENV_REPO}/python{user_python_version}/burla_job_env:latest"
 
     data = {
         "key": api_key,
         "func_pkl_hex_ascii": hexlify(dill.dumps(function_.__code__)).decode("ascii"),
         "inputs": inputs,
         "image": image or default_docker_image,
         "num_computers": cpus,
     }
+    job_started_at_epoch = int(time())
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data)
     response.raise_for_status()
 
-    job_start_time = time()
-    last_timestamp = "2023-07-01T00:00:00.000001Z"
-    epoch_time = 1688169600.000001  # same-ish as above
+    last_epoch = job_started_at_epoch
+    epoch = last_epoch
     job_is_running = True
     job_timed_out = False
 
     # Start printing logs generated by this job using a separate thread.
     print_queue = PriorityQueue()
     stop_event = threading.Event()
     log_thread = threading.Thread(
         target=print_logs_from_queue, args=(print_queue, stop_event), daemon=True
     )
     log_thread.start()
 
     # loop until job finishes, or times out
     while job_is_running and (not job_timed_out):
+        # TODO: record and subtract time so this loop always takes exactly JOB_STATUS_POLL_RATE_SEC
+        # sec to run? This might fix late logs?
         sleep(JOB_STATUS_POLL_RATE_SEC)
 
-        job = _get_job_info(job_id, last_timestamp)
+        job = _get_job_info(job_id, last_epoch)
 
         # add all logs to print queue
-        for epoch_time, log_message in job["logs"]:
-            print_queue.put((epoch_time, log_message))
+        for epoch, log_message in job["logs"]:
+            print_queue.put((epoch, log_message))
 
-        last_timestamp = datetime.fromtimestamp(epoch_time, TZ).isoformat().replace("+00:00", "Z")
+        last_epoch = epoch
         job_is_running = job["job_is_done"] == False
-        job_timed_out = (time() - job_start_time) > (TIMEOUT_MIN * 60)
+        job_timed_out = (time() - job_started_at_epoch) > (TIMEOUT_MIN * 60)
 
     stop_event.set()
     log_thread.join()
 
     if job_timed_out:
         raise JobTimeoutError(job_id=job_id, timeout=TIMEOUT_MIN)
 
-    return job["result"]
+    return job["return_values"]
```

### Comparing `burla-0.0.5/PKG-INFO` & `burla-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.5
+Version: 0.0.6
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

