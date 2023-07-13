# Comparing `tmp/ezmsg-zmq-1.1.1.tar.gz` & `tmp/ezmsg-zmq-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmsg-zmq-1.1.1.tar", last modified: Wed Mar 29 20:02:56 2023, max compression
+gzip compressed data, was "ezmsg-zmq-1.1.3.tar", last modified: Thu Jul 13 15:38:22 2023, max compression
```

## Comparing `ezmsg-zmq-1.1.1.tar` & `ezmsg-zmq-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:56.781257 ezmsg-zmq-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-29 20:02:56.781257 ezmsg-zmq-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:56.781257 ezmsg-zmq-1.1.1/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:56.781257 ezmsg-zmq-1.1.1/ezmsg/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/ezmsg/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/ezmsg/zmq/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/ezmsg/zmq/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:56.781257 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-29 20:02:56.000000 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-29 20:02:56.000000 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 20:02:56.000000 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 20:02:56.000000 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 20:02:56.000000 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 20:02:56.000000 ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-29 20:02:56.781257 ezmsg-zmq-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-29 20:02:47.000000 ezmsg-zmq-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/ezmsg/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/ezmsg/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/ezmsg/zmq/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/ezmsg/zmq/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-13 15:38:22.778459 ezmsg-zmq-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/setup.py
```

### Comparing `ezmsg-zmq-1.1.1/LICENSE.txt` & `ezmsg-zmq-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezmsg-zmq-1.1.1/PKG-INFO` & `ezmsg-zmq-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg-zmq
-Version: 1.1.1
+Version: 1.1.3
 Summary: ZeroMQ units for ezmsg
 Home-page: https://github.com/iscoe/ezmsg
 Author: Preston Peranich
 Author-email: pperanich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-zmq-1.1.1/ezmsg/zmq/units.py` & `ezmsg-zmq-1.1.3/ezmsg/zmq/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,23 +57,24 @@
         zmq_topic: The ZMQ topic being sent.
     """
 
     INPUT = ez.InputStream(ZMQMessage)
 
     SETTINGS: ZMQSenderSettings
 
-    def setup(self) -> None:
+    def initialize(self) -> None:
         self.context = zmq.asyncio.Context()
         self.socket = self.context.socket(zmq.PUB)
         self.monitor = self.socket.get_monitor_socket()
         ez.logger.debug(f"{self}:binding to {self.SETTINGS.write_addr}")
         self.socket.bind(self.SETTINGS.write_addr)
         self.has_subscribers = False
 
     def shutdown(self) -> None:
+        self.monitor.close()
         self.socket.close()
 
     @ez.task
     async def _socket_monitor(self) -> None:
         while True:
             monitor_result = await self.monitor.poll(100, zmq.POLLIN)
             if monitor_result:
@@ -133,27 +134,28 @@
             if encountered by the monitor, should signal the termination
             of this particular node's activity.
     """
 
     OUTPUT = ez.OutputStream(ZMQMessage)
     SETTINGS: ZMQPollerSettings
 
-    def setup(self) -> None:
+    def initialize(self) -> None:
         self.context = zmq.asyncio.Context()
         self.socket = self.context.socket(zmq.SUB)
         self.monitor = self.socket.get_monitor_socket()
         self.socket.connect(self.SETTINGS.read_addr)
         self.socket.subscribe(self.SETTINGS.zmq_topic)
 
         self.poller = zmq.Poller()
         self.poller.register(self.socket, zmq.POLLIN)
 
         self.socket_open = False
 
     def shutdown(self) -> None:
+        self.monitor.close()
         self.socket.close()
 
     @ez.task
     async def socket_monitor(self) -> None:
         while True:
             monitor_result = await self.monitor.poll(100, zmq.POLLIN)
             if monitor_result:
```

### Comparing `ezmsg-zmq-1.1.1/ezmsg_zmq.egg-info/PKG-INFO` & `ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg-zmq
-Version: 1.1.1
+Version: 1.1.3
 Summary: ZeroMQ units for ezmsg
 Home-page: https://github.com/iscoe/ezmsg
 Author: Preston Peranich
 Author-email: pperanich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-zmq-1.1.1/setup.cfg` & `ezmsg-zmq-1.1.3/setup.cfg`

 * *Files identical despite different names*

