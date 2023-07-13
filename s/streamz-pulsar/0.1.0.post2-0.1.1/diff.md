# Comparing `tmp/streamz_pulsar-0.1.0.post2.tar.gz` & `tmp/streamz_pulsar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamz_pulsar-0.1.0.post2.tar", max compression
+gzip compressed data, was "streamz_pulsar-0.1.1.tar", max compression
```

## Comparing `streamz_pulsar-0.1.0.post2.tar` & `streamz_pulsar-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1827 2023-07-12 14:06:16.274117 streamz_pulsar-0.1.0.post2/README.md
--rw-r--r--   0        0        0     1040 2023-07-12 14:16:35.791410 streamz_pulsar-0.1.0.post2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-12 14:06:16.274510 streamz_pulsar-0.1.0.post2/streamz_pulsar/__init__.py
--rw-r--r--   0        0        0      393 2023-07-12 14:06:16.274565 streamz_pulsar-0.1.0.post2/streamz_pulsar/base.py
--rw-r--r--   0        0        0     1619 2023-07-12 14:11:53.260772 streamz_pulsar-0.1.0.post2/streamz_pulsar/sinks.py
--rw-r--r--   0        0        0       51 2023-07-12 14:06:16.274706 streamz_pulsar-0.1.0.post2/streamz_pulsar/sources/__init__.py
--rw-r--r--   0        0        0     3152 2023-07-12 14:12:39.700559 streamz_pulsar-0.1.0.post2/streamz_pulsar/sources/from_pulsar.py
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 streamz_pulsar-0.1.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     1762 2023-07-13 08:56:32.208893 streamz_pulsar-0.1.1/README.md
+-rw-r--r--   0        0        0     1034 2023-07-13 08:55:43.959094 streamz_pulsar-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-12 14:06:16.274510 streamz_pulsar-0.1.1/streamz_pulsar/__init__.py
+-rw-r--r--   0        0        0      393 2023-07-12 14:06:16.274565 streamz_pulsar-0.1.1/streamz_pulsar/base.py
+-rw-r--r--   0        0        0     1700 2023-07-13 08:55:16.220944 streamz_pulsar-0.1.1/streamz_pulsar/sinks.py
+-rw-r--r--   0        0        0       51 2023-07-12 14:06:16.274706 streamz_pulsar-0.1.1/streamz_pulsar/sources/__init__.py
+-rw-r--r--   0        0        0     3204 2023-07-13 08:55:24.863378 streamz_pulsar-0.1.1/streamz_pulsar/sources/from_pulsar.py
+-rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 streamz_pulsar-0.1.1/PKG-INFO
```

### Comparing `streamz_pulsar-0.1.0.post2/README.md` & `streamz_pulsar-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 The following example creates a consumer with the `my-sub` subscription name on the `my-topic` topic, receives incoming messages, prints the content and ID of messages that arrive, and acknowledges each message to the Pulsar broker.
 
 ```python
 import pulsar
 from streamz import Stream
 
 s = Stream.from_pulsar(
+    'pulsar://localhost:6650',
     ['my-topic'],
-    subscription_name='my-sub',
-    consumer_params={'service_url': 'pulsar://localhost:6650'}
+    subscription_name='my-sub'
     )
 
 s.map(lambda x: x.decode())
 L = s.sink_to_list()
 
 s.start()
 while True:
@@ -59,16 +59,16 @@
 The following example creates a Python producer for the `my-topic` topic and sends 10 messages on that topic:
 
 ```python
 from streamz import Stream
 
 source = Stream()
 producer_ = source.to_pulsar(
+    'pulsar://localhost:6650',
     'my-topic',
-    producer_config={'service_url': 'pulsar://localhost:6650'}
     )
 
 for i in range(3):
     source.emit(('hello-pulsar-%d' % i).encode('utf-8'))
 
 producer_.stop()
 producer_.flush()
```

### Comparing `streamz_pulsar-0.1.0.post2/pyproject.toml` & `streamz_pulsar-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "streamz_pulsar"
-version = "0.1.0.post2"
+version = "0.1.1"
 description = ""
 authors = [
     "Marek Wadinger <marekwadinger@icloud.com>",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `streamz_pulsar-0.1.0.post2/streamz_pulsar/sinks.py` & `streamz_pulsar-0.1.1/streamz_pulsar/sinks.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,32 @@
         service_url: The Pulsar service url eg: pulsar://my-broker.com:6650/
 
     Examples
     --------
     >>> from streamz import Stream
     >>> source = Stream()
     >>> producer_ = source.to_pulsar(
-    ...     'my-topic',
-    ...     producer_config={'service_url': 'pulsar://localhost:6650'}
+    ...     'pulsar://localhost:6650'
+    ...     'my-topic'
     ...     )  # doctest: +SKIP
     >>> for i in range(3):
     ...     source.emit(('hello-pulsar-%d' % i).encode('utf-8'))
     """
-    def __init__(self, upstream, topic, producer_config, **kwargs):
+    def __init__(
+            self,
+            upstream,
+            service_url,
+            topic,
+            producer_config={},
+            **kwargs):
 
         self.topic = topic
-        self.client = pulsar.Client(**producer_config)
-        self.producer = self.client.create_producer(self.topic)
+        self.client = pulsar.Client(service_url)
+        self.producer = self.client.create_producer(
+            self.topic, **producer_config)
 
         kwargs["ensure_io_loop"] = True
         super().__init__(upstream, **kwargs)
         self.stopped = False
         self.polltime = 0.2
         self.futures = []
```

### Comparing `streamz_pulsar-0.1.0.post2/streamz_pulsar/sources/from_pulsar.py` & `streamz_pulsar-0.1.1/streamz_pulsar/sources/from_pulsar.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,31 +37,33 @@
         Seconds that elapse between polling Pulsar for new messages
 
     Examples
     --------
     >>> import pulsar
     >>> from streamz import Stream
     >>> s = Stream.from_pulsar(
+    ...     'pulsar://localhost:6650',
     ...     ['my-topic'],
-    ...     subscription_name='my-sub',
-    ...     consumer_params={'service_url': 'pulsar://localhost:6650'}
+    ...     subscription_name='my-sub'
     ...     )
     >>> decoder = s.map(lambda x: x.decode())
     >>> L = decoder.sink_to_list()
     """
     def __init__(
             self,
+            service_url,
             topics,
             subscription_name,
-            consumer_params,
+            consumer_params={},
             poll_interval=0.1,
             **kwargs):
+        self.consumer = None
         self.cpars = consumer_params
+        self.service_url = service_url
         self.subscription_name = subscription_name
-        self.consumer = None
         self.topics = topics
         self.poll_interval = poll_interval
         super().__init__(**kwargs)
 
     def do_poll(self):
         if self.consumer is not None:
             try:
@@ -83,17 +85,17 @@
             if self.stopped:
                 break
         self._close_consumer()
 
     def start(self):
         if self.stopped:
             self.stopped = False
-            self.client = pulsar.Client(**self.cpars)
+            self.client = pulsar.Client(self.service_url)
             self.consumer = self.client.subscribe(
-                self.topics, self.subscription_name)
+                self.topics, self.subscription_name, **self.cpars)
             weakref.finalize(
                 self, lambda consumer=self.consumer: _close_consumer(consumer)
             )
             self.loop.add_callback(self.poll_pulsar)
 
     def _close_consumer(self):
         if self.consumer is not None:
```

### Comparing `streamz_pulsar-0.1.0.post2/PKG-INFO` & `streamz_pulsar-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamz-pulsar
-Version: 0.1.0.post2
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/MarekWadinger/streamz_pulsar
 Keywords: streamz,pulsar
 Author: Marek Wadinger
 Author-email: marekwadinger@icloud.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,17 +54,17 @@
 The following example creates a consumer with the `my-sub` subscription name on the `my-topic` topic, receives incoming messages, prints the content and ID of messages that arrive, and acknowledges each message to the Pulsar broker.
 
 ```python
 import pulsar
 from streamz import Stream
 
 s = Stream.from_pulsar(
+    'pulsar://localhost:6650',
     ['my-topic'],
-    subscription_name='my-sub',
-    consumer_params={'service_url': 'pulsar://localhost:6650'}
+    subscription_name='my-sub'
     )
 
 s.map(lambda x: x.decode())
 L = s.sink_to_list()
 
 s.start()
 while True:
@@ -81,16 +81,16 @@
 The following example creates a Python producer for the `my-topic` topic and sends 10 messages on that topic:
 
 ```python
 from streamz import Stream
 
 source = Stream()
 producer_ = source.to_pulsar(
+    'pulsar://localhost:6650',
     'my-topic',
-    producer_config={'service_url': 'pulsar://localhost:6650'}
     )
 
 for i in range(3):
     source.emit(('hello-pulsar-%d' % i).encode('utf-8'))
 
 producer_.stop()
 producer_.flush()
```

