# Comparing `tmp/w3bstream_client_python-0.4.6.tar.gz` & `tmp/w3bstream_client_python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.4.6.tar", last modified: Wed Jul 12 19:38:36 2023, max compression
+gzip compressed data, was "w3bstream_client_python-1.0.0.tar", last modified: Thu Jul 13 17:37:01 2023, max compression
```

## Comparing `w3bstream_client_python-0.4.6.tar` & `w3bstream_client_python-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-30 05:29:14.000000 w3bstream_client_python-0.4.6/.gitignore
--rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-30 05:29:14.000000 w3bstream_client_python-0.4.6/LICENSE
--rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      709 2023-07-11 18:41:55.000000 w3bstream_client_python-0.4.6/README.md
--rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-11 18:41:55.000000 w3bstream_client_python-0.4.6/pyproject.toml
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/setup.cfg
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/src/
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/src/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-10 18:18:02.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3833 2023-07-12 03:25:37.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/requires.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.583950 w3bstream_client_python-1.0.0/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-30 05:29:14.000000 w3bstream_client_python-1.0.0/.gitignore
+-rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-30 05:29:14.000000 w3bstream_client_python-1.0.0/LICENSE
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      709 2023-07-11 18:41:55.000000 w3bstream_client_python-1.0.0/README.md
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-13 17:36:42.000000 w3bstream_client_python-1.0.0/pyproject.toml
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-13 17:37:01.583950 w3bstream_client_python-1.0.0/setup.cfg
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/src/
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/src/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-10 18:18:02.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3773 2023-07-13 17:36:42.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/requires.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-0.4.6/.gitignore` & `w3bstream_client_python-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.6/LICENSE` & `w3bstream_client_python-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.6/PKG-INFO` & `w3bstream_client_python-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3bstream_client_python
-Version: 0.4.6
+Version: 1.0.0
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
```

### Comparing `w3bstream_client_python-0.4.6/README.md` & `w3bstream_client_python-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.6/src/w3bstream_client_python/client.py` & `w3bstream_client_python-1.0.0/src/w3bstream_client_python/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import datetime
 import queue
 import threading
 import time
 import sys
+import json
+import datetime
 
 import requests
 from typeguard import typechecked
 
 
 @typechecked
 class Header:
     def __init__(self, device_id: str, event_type: str = 'DEFAULT', timestamp: datetime.datetime = datetime.datetime.utcnow()):
         self.event_type = event_type
         self.device_id = device_id
         self.timestamp = timestamp
 
 
 PUBLISH_INTERVAL = 5
-_PUBLISH_BATCH_SIZE = 1
+PUBLISH_BATCH_SIZE = 10
+_DATA_PUSH_EVENT_TYPE = "$DATA#PUSH"
 
 
 @typechecked
 class Client:
     def __init__(self, url: str, api_key: str, queue_size: int = 0):
         self.url = url
         self.api_key = api_key
@@ -52,15 +55,15 @@
             True if the event was successfully added to the queue, False otherwise.
         """
         try:
             self.queue.put_nowait((header, payload))
             return True
         except queue.Full:
             sys.stderr.write(
-                "The queue is full when publishing the data to W3bstream")
+                "the queue is full when publishing the data to W3bstream")
             return False
 
     def _worker(self):
         while True:
             # fetch events
             events = []
             for header, payload in self._fetch_event_batch():
@@ -71,42 +74,38 @@
                     'timestamp':  int(round(header.timestamp.timestamp())),
                 })
             # publish events
             resp = self._publish_event(events)
             if resp.status_code >= 400:
                 # TODO: Support retry mechanism when failed to publish
                 sys.stderr.write(
-                    "An error occurred when publishing the data to W3bstream: status_code %d, body: %s" % (resp.status_code, resp.text))
+                    "an error occurred when publishing the data to W3bstream: status_code %d, body: %s" % (resp.status_code, resp.text))
             # sleep interval
             time.sleep(PUBLISH_INTERVAL)
 
     def _fetch_event_batch(self):
         """
         Fetches a batch of events from the queue.
 
-        Fetches up to _PUBLISH_BATCH_SIZE events from the queue.
+        Fetches up to PUBLISH_BATCH_SIZE events from the queue.
         It will block until at least one event is available.
         """
         count = 0
-        while count < _PUBLISH_BATCH_SIZE:
+        while count < PUBLISH_BATCH_SIZE:
             try:
                 if count == 0:
                     yield self.queue.get()
                 else:
                     yield self.queue.get_nowait()
                 count += 1
             except queue.Empty:
                 break
 
     def _publish_event(self, events: list) -> requests.Response:
-        meta_data = events[0]
         headers = {
             'Authorization': 'Bearer ' + self.api_key,
             'Content-Type': 'application/octet-stream',
         }
-
-        device_id = meta_data["device_id"]
-        event_type = meta_data["event_type"]
-        timestamp = meta_data["timestamp"]
-        url = f"{self.url}?device_id={device_id}&eventType={event_type}&timestamp={timestamp}"
-        data_bytes = meta_data["payload"].encode('utf-8')
+        timestamp = int(round(datetime.datetime.now().timestamp()))
+        url = f"{self.url}?eventType={_DATA_PUSH_EVENT_TYPE}&timestamp={timestamp}"
+        data_bytes = json.dumps(events)
         return requests.post(url, data=data_bytes,  headers=headers)
```

### Comparing `w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/PKG-INFO` & `w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3bstream-client-python
-Version: 0.4.6
+Version: 1.0.0
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
```

