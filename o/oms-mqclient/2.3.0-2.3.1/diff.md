# Comparing `tmp/oms-mqclient-2.3.0.tar.gz` & `tmp/oms-mqclient-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.3.0.tar", last modified: Tue Jul 11 22:08:25 2023, max compression
+gzip compressed data, was "oms-mqclient-2.3.1.tar", last modified: Thu Jul 13 00:03:28 2023, max compression
```

## Comparing `oms-mqclient-2.3.0.tar` & `oms-mqclient-2.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5972 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13450 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    13421 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15335 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      375 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    24216 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2731 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.073164 oms-mqclient-2.3.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    30730 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    20234 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5586 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9196 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.489489 oms-mqclient-2.3.1/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.489489 oms-mqclient-2.3.1/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    13421 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    15335 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    24455 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.489489 oms-mqclient-2.3.1/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.485489 oms-mqclient-2.3.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    35457 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5586 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.3.0/LICENSE` & `oms-mqclient-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/PKG-INFO` & `oms-mqclient-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.0
-Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
+Version: 2.3.1
+Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
 Project-URL: Source, https://github.com/Observation-Management-Service/MQClient
```

### Comparing `oms-mqclient-2.3.0/README.md` & `oms-mqclient-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/__init__.py` & `oms-mqclient-2.3.1/mqclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.3.0/mqclient/broker_client_interface.py` & `oms-mqclient-2.3.1/mqclient/broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/broker_client_manager.py` & `oms-mqclient-2.3.1/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.3.1/mqclient/broker_clients/apachepulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/broker_clients/nats.py` & `oms-mqclient-2.3.1/mqclient/broker_clients/nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.3.1/mqclient/broker_clients/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/broker_clients/utils.py` & `oms-mqclient-2.3.1/mqclient/broker_clients/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/log_msgs.py` & `oms-mqclient-2.3.1/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/mqclient/queue.py` & `oms-mqclient-2.3.1/mqclient/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,16 @@
 
     async def _create_sub_queue(self, prefetch_override: Optional[int] = None) -> Sub:
         """Wrap `self._broker_client.create_sub_queue()` with instance's
         config."""
         return await self._broker_client.create_sub_queue(
             self._address,
             self._name,
-            prefetch_override if prefetch_override else self._prefetch,
+            # 0 is okay
+            prefetch_override if prefetch_override is not None else self._prefetch,
             self._auth_token,
             self._ack_timeout,
         )
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
     @wtt.spanned(
         these=[
@@ -296,15 +297,15 @@
             "self._address",
             "self._name",
             "self._prefetch",
             "self.timeout",
         ]
     )
     async def open_sub_manual_acking(
-        self,
+        self, use_prefetch_value: bool
     ) -> AsyncGenerator["ManualQueueSubResource", None]:
         """Open a resource to receive messages from the queue as an iterator.
 
         This returns a context-manager with an iterator function `iter_messages()`.
         The iterator stops when no messages are received for `timeout` seconds.
         Multiple calls to `open_sub()` is okay, but reusing the returned
         instance is not.
@@ -314,15 +315,20 @@
         *Unlike `open_sub()`*, the caller is responsible for:
             - All acking and/or nacking
             - Any error handling
 
         **NOTE: unless you need to parallelize your message processing,
         use `open_sub()`**
 
-        NOTE: prefetching is disabled for this method
+        Arguments:
+            `use_prefetch_value` - whether to use the prefetch value; `False` uses prefetch=0
+                Prefetching may be useful for short-running tasks,
+                where the bottleneck would be network delay.
+                NOTE: rabbitmq will not deliver more messages if
+                there are N un-acked messages (N = prefetch, N > 0)
 
         Examples:
             async with queue.open_sub_manual_acking() as sub:
                 async for msg in sub.iter_messages():
                     print(msg.data)
                     sub.ack(msg)
                     # if you choose not to nack on an error,
@@ -354,21 +360,20 @@
                 for msg in pending:
                     await sub.ack(msg)
 
         Returns:
             ManualQueueSubResource -- context manager w/ iterator function
         """
         sub = await self._create_sub_queue(
-            # if prefetch=N (N>0), pika requires N acks/nacks before it gets more messages
+            # if prefetch=N (N>0), pika will not deliver more messages
+            #   if there are N un-acked messages
+            #
             #   We could implement logic that checks if this condition is met
-            #   but that would go against the intention of the "manual" usage,
-            #   e.g. a long running client with long running, parallel tasks
-            #   that finish at different times shouldn't have to wait for all
-            #   tasks to finish before getting more messages.
-            prefetch_override=0,
+            #   but that would go against the intention of the "manual" usage
+            prefetch_override=(None if use_prefetch_value else 0)
         )
 
         try:
             yield ManualQueueSubResource(
                 functools.partial(
                     sub.get_message,
                     self.timeout * 1000,
```

### Comparing `oms-mqclient-2.3.0/mqclient/telemetry.py` & `oms-mqclient-2.3.1/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.3.1/oms_mqclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.0
-Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
+Version: 2.3.1
+Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
 Project-URL: Source, https://github.com/Observation-Management-Service/MQClient
```

### Comparing `oms-mqclient-2.3.0/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.3.1/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/setup.cfg` & `oms-mqclient-2.3.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [metadata]
 name = oms-mqclient
 version = attr: mqclient.__version__
 url = https://github.com/Observation-Management-Service/MQClient
 author = WIPAC Developers
 author_email = developers@icecube.wisc.edu
-description = A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
+description = A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
 	Observation Management Service
 	Event Workflow Management Service
 	python message passing client
 	message passing
```

### Comparing `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run integration tests for given broker_client, on Queue class."""
 
 # pylint:disable=invalid-name,too-many-public-methods,redefined-outer-name,unused-import
 
 import asyncio
 import logging
 from multiprocessing.dummy import Pool as ThreadPool
-from typing import Any, List
+from typing import Any, List, Optional
 
 import asyncstdlib as asl
 import pytest
 from mqclient.queue import Queue
 
 from .utils import (
     DATA_LIST,
@@ -601,62 +601,223 @@
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     ###########################################################################
     # tests 200 - 299:
     #
-    # Tests for open_sub_manual_acking()
+    # Tests for open_sub_manual_acking(use_prefetch_value)
     ###########################################################################
 
     @pytest.mark.asyncio
-    async def test_200__ideal(self, queue_name: str, auth_token: str) -> None:
-        """Test open_sub_manual_acking() ideal scenario."""
+    @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    async def test_200__ideal(
+        self,
+        queue_name: str,
+        auth_token: str,
+        sub_queue_prefetch: Optional[int],
+        use_prefetch_value: bool,
+    ) -> None:
+        """Test open_sub_manual_acking(use_prefetch_value) ideal scenario."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
                 _log_send(d)
 
-        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        if sub_queue_prefetch is not None:
+            sub = Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+                prefetch=sub_queue_prefetch,
+            )
+        else:
+            sub = Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+            )
         sub.timeout = 1
-        async with sub.open_sub_manual_acking() as gen:
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 all_recvd.append(_log_recv(msg.data))
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    async def test_202__delayed_mixed_acking_nacking(
+        self,
+        queue_name: str,
+        auth_token: str,
+        sub_queue_prefetch: Optional[int],
+        use_prefetch_value: bool,
+    ) -> None:
+        """Test open_sub_manual_acking(use_prefetch_value) fail and immediate
+        recovery with multi-tasking, with mixed acking and nacking."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        class TestException(Exception):  # pylint: disable=C0115
+            pass
+
+        if sub_queue_prefetch is not None:
+            sub = Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+                prefetch=sub_queue_prefetch,
+            )
+        else:
+            sub = Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+            )
+        sub.timeout = 1
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+            pending = []
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                try:
+                    # DO WORK!
+                    print(f"{i}: `{msg.data}`")
+                    if i % 3 == 0:  # nack every 1/3
+                        raise TestException()
+                    all_recvd.append(_log_recv(msg.data))
+                    pending.append(msg)
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                    if i % 2 == 0:  # ack every 1/2
+                        print(f"ack {i}: `{msg.data}`")
+                        await gen.ack(msg)
+                        pending.remove(msg)
+                except Exception:
+                    print(f"nack {i}: `{msg.data}`")
+                    await gen.nack(msg)
+
+            for msg in pending:  # messages with index not %2 nor %3, (1,5,7,...)
+                await gen.ack(msg)
+
+        print(all_recvd)
+        if (
+            self.broker_client == "rabbitmq"
+            and use_prefetch_value
+            and sub_queue_prefetch  # int, >0
+        ):  # acked every 1/2 before we got kicked out
+            try:
+                indexes_unacked = [
+                    x
+                    for x in range(int(len(DATA_LIST) * (3 / 2)))  # math.ceil?
+                    if not (x % 2 == 0 or x % 3 == 0)
+                ]
+                print(indexes_unacked)
+                assert i == indexes_unacked[sub_queue_prefetch - 1]  # 0-index
+            except IndexError:
+                assert i + 1 == len(DATA_LIST) * (3 / 2)
+            assert len(all_recvd) == i - (i // 3)  # len == i - # of nacks
+        else:
+            assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    async def test_204__post_ack(
+        self,
+        queue_name: str,
+        auth_token: str,
+        sub_queue_prefetch: Optional[int],
+        use_prefetch_value: bool,
+    ) -> None:
+        """Test open_sub_manual_acking(use_prefetch_value) where messages
+        aren't acked until after all have been received."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        if sub_queue_prefetch is not None:
+            sub = Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+                prefetch=sub_queue_prefetch,
+            )
+        else:
+            sub = Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+            )
+        sub.timeout = 1
+        to_ack = []
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                print(f"{i}: `{msg.data}`")
+                all_recvd.append(_log_recv(msg.data))
+                to_ack.append(msg)
+                # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+
+            for i, msg in enumerate(to_ack):
+                print(f"ack {i}: `{msg.data}`")
+                await gen.ack(msg)
+
+        print(all_recvd)
+        if (
+            self.broker_client == "rabbitmq"
+            and use_prefetch_value
+            and sub_queue_prefetch  # int, >0
+        ):  # got kicked out when prefetch was met
+            assert len(all_recvd) == min(sub_queue_prefetch, len(DATA_LIST))
+        else:
+            assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
     async def test_210__immediate_recovery(
-        self, queue_name: str, auth_token: str
+        self,
+        queue_name: str,
+        auth_token: str,
+        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking() fail and immediate recovery, with
-        nacking."""
+        """Test open_sub_manual_acking(use_prefetch_value) fail and immediate
+        recovery, with nacking."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
                 _log_send(d)
 
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         sub.timeout = 1
-        async with sub.open_sub_manual_acking() as gen:
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 try:
                     # DO WORK!
                     print(f"{i}: `{msg.data}`")
                     if i == 2:
                         raise TestException()
                     all_recvd.append(_log_recv(msg.data))
@@ -666,19 +827,23 @@
                 else:
                     await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
     async def test_220__posthoc_recovery(
-        self, queue_name: str, auth_token: str
+        self,
+        queue_name: str,
+        auth_token: str,
+        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking() fail and post-hoc recovery, with
-        nacking."""
+        """Test open_sub_manual_acking(use_prefetch_value) fail and post-hoc
+        recovery, with nacking."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -687,15 +852,15 @@
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         excepted = False
         sub.timeout = 1
         # sub.except_errors = False  # has no effect
-        async with sub.open_sub_manual_acking() as gen:
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
             try:
                 async for i, msg in asl.enumerate(gen.iter_messages()):
                     print(f"{i}: `{msg.data}`")
                     if i == 2:
                         raise TestException()
                     all_recvd.append(_log_recv(msg.data))
                     # assert msg.data == DATA_LIST[i]  # we don't guarantee order
@@ -706,30 +871,35 @@
         assert excepted
 
         logging.warning("Round 2!")
 
         # continue where we left off
         posthoc = False
         sub.timeout = 1
-        async with sub.open_sub_manual_acking() as gen:
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 posthoc = True
                 all_recvd.append(_log_recv(msg.data))
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
         assert posthoc
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
     async def test_221__posthoc_recovery__fail(
-        self, queue_name: str, auth_token: str
+        self,
+        queue_name: str,
+        auth_token: str,
+        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking() fail, post-hoc recovery, then fail.
+        """Test open_sub_manual_acking(use_prefetch_value) fail, post-hoc
+        recovery, then fail.
 
         Final fail is due to not nacking.
         """
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
@@ -741,15 +911,15 @@
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         errored_msg = None
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         excepted = False
-        async with sub.open_sub_manual_acking() as gen:
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
             try:
                 async for i, msg in asl.enumerate(gen.iter_messages()):
                     print(f"{i}: `{msg.data}`")
                     if i == 2:
                         errored_msg = msg.data
                         raise TestException()
                     all_recvd.append(_log_recv(msg.data))
@@ -761,15 +931,15 @@
         assert excepted
 
         logging.warning("Round 2!")
 
         # continue where we left off
         posthoc = False
         sub.timeout = 1
-        async with sub.open_sub_manual_acking() as gen:
+        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 posthoc = True
                 all_recvd.append(_log_recv(msg.data))
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
         assert posthoc
@@ -779,77 +949,40 @@
         # This is difficult to test -- all we can tell is if it is one of these scenarios
         print(all_recvd)
         assert all_were_received(all_recvd) or (
             all_were_received(all_recvd + [errored_msg])
         )
 
     @pytest.mark.asyncio
-    async def test_230__fail_bad_usage(self, queue_name: str, auth_token: str) -> None:
-        """Failure-test open_sub_manual_acking() with reusing a
-        'QueueSubResource' instance."""
+    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    async def test_230__fail_bad_usage(
+        self,
+        queue_name: str,
+        auth_token: str,
+        use_prefetch_value: bool,
+    ) -> None:
+        """Failure-test open_sub_manual_acking(use_prefetch_value) with reusing
+        a 'QueueSubResource' instance."""
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
                 _log_send(d)
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         sub.timeout = 1
-        recv_gen = sub.open_sub_manual_acking()
+        recv_gen = sub.open_sub_manual_acking(use_prefetch_value)
         async with recv_gen as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
 
         logging.warning("Round 2!")
 
         # continue where we left off
         with pytest.raises((AttributeError, RuntimeError)):
             # AttributeError: '_AsyncGeneratorContextManager' object has no attribute 'args'
             # RuntimeError: generator didn't yield
             async with recv_gen as gen:
                 assert 0  # we should never get here
-
-    @pytest.mark.asyncio
-    async def test_240__delayed_mixed_acking_nacking(
-        self, queue_name: str, auth_token: str
-    ) -> None:
-        """Test open_sub_manual_acking() fail and immediate recovery with
-        multi-tasking, with mixed acking and nacking."""
-        all_recvd: List[Any] = []
-
-        async with Queue(
-            self.broker_client, name=queue_name, auth_token=auth_token
-        ).open_pub() as p:
-            for d in DATA_LIST:
-                await p.send(d)
-                _log_send(d)
-
-        class TestException(Exception):  # pylint: disable=C0115
-            pass
-
-        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
-        sub.timeout = 1
-        async with sub.open_sub_manual_acking() as gen:
-            pending = []
-            async for i, msg in asl.enumerate(gen.iter_messages()):
-                try:
-                    # DO WORK!
-                    print(f"{i}: `{msg.data}`")
-                    if i % 3 == 0:  # nack every 1/3
-                        raise TestException()
-                    all_recvd.append(_log_recv(msg.data))
-                    pending.append(msg)
-                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
-                    if i % 2 == 0:  # ack every 1/2
-                        await gen.ack(msg)
-                        pending.remove(msg)
-                except Exception:
-                    await gen.nack(msg)
-
-            for msg in pending:  # messages with index not %2 nor %3, (1,5,7,...)
-                await gen.ack(msg)
-
-        print(all_recvd)
-        assert all_were_received(all_recvd)
```

### Comparing `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/integrate/conftest.py` & `oms-mqclient-2.3.1/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/integrate/test_nats.py` & `oms-mqclient-2.3.1/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/integrate/test_pulsar.py` & `oms-mqclient-2.3.1/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.3.1/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.3.1/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.0/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.3.1/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

