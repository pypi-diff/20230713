# Comparing `tmp/utbot_executor-1.6.2.tar.gz` & `tmp/utbot_executor-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.6.2.tar", max compression
+gzip compressed data, was "utbot_executor-1.6.3.tar", max compression
```

## Comparing `utbot_executor-1.6.2.tar` & `utbot_executor-1.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.6.2/LICENSE
--rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.6.2/README.md
--rw-r--r--   0        0        0      401 2023-04-26 11:38:17.557316 utbot_executor-1.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.6.2/utbot_executor/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.6.2/utbot_executor/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.6.2/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.6.2/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     1469 2023-04-13 11:03:00.871191 utbot_executor-1.6.2/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     8848 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0    10451 2023-04-13 11:16:20.078217 utbot_executor-1.6.2/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0      413 2023-04-13 11:10:20.054988 utbot_executor-1.6.2/utbot_executor/deep_serialization/numpy_serialization.py
--rw-r--r--   0        0        0     5445 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     3871 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0     8066 2023-04-26 11:37:56.776595 utbot_executor-1.6.2/utbot_executor/executor.py
--rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.6.2/utbot_executor/listener.py
--rw-r--r--   0        0        0      873 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/memory_compressor.py
--rw-r--r--   0        0        0     2661 2023-04-26 11:14:16.320827 utbot_executor-1.6.2/utbot_executor/parser.py
--rw-r--r--   0        0        0     1550 2023-04-26 11:37:56.759928 utbot_executor-1.6.2/utbot_executor/ut_tracer.py
--rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.6.2/utbot_executor/utils.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 utbot_executor-1.6.2/setup.py
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 utbot_executor-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.6.3/LICENSE
+-rw-r--r--   0        0        0     3418 2023-05-18 07:35:21.976168 utbot_executor-1.6.3/README.md
+-rw-r--r--   0        0        0      401 2023-05-18 07:42:08.769026 utbot_executor-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.6.3/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     1257 2023-04-26 12:37:21.090807 utbot_executor-1.6.3/utbot_executor/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.6.3/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.6.3/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     1469 2023-04-13 11:03:00.871191 utbot_executor-1.6.3/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     8848 2023-05-18 07:38:53.848568 utbot_executor-1.6.3/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0    10451 2023-05-18 07:38:55.265258 utbot_executor-1.6.3/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0      413 2023-05-18 07:38:55.005253 utbot_executor-1.6.3/utbot_executor/deep_serialization/numpy_serialization.py
+-rw-r--r--   0        0        0     5445 2023-05-18 07:38:54.805250 utbot_executor-1.6.3/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     3871 2023-05-18 07:38:10.874392 utbot_executor-1.6.3/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0     8774 2023-04-27 11:05:06.486491 utbot_executor-1.6.3/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3292 2023-04-26 12:37:21.104140 utbot_executor-1.6.3/utbot_executor/listener.py
+-rw-r--r--   0        0        0      873 2023-05-18 07:38:53.768566 utbot_executor-1.6.3/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     2661 2023-05-03 07:53:16.368721 utbot_executor-1.6.3/utbot_executor/parser.py
+-rw-r--r--   0        0        0     1550 2023-04-26 11:40:38.450019 utbot_executor-1.6.3/utbot_executor/ut_tracer.py
+-rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.6.3/utbot_executor/utils.py
+-rw-r--r--   0        0        0     4246 1970-01-01 00:00:00.000000 utbot_executor-1.6.3/setup.py
+-rw-r--r--   0        0        0     3876 1970-01-01 00:00:00.000000 utbot_executor-1.6.3/PKG-INFO
```

### Comparing `utbot_executor-1.6.2/LICENSE` & `utbot_executor-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/__main__.py` & `utbot_executor-1.6.3/utbot_executor/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import logging
 
 from utbot_executor.listener import PythonExecuteServer
 
 
-def main(hostname: str, port: int):
-    server = PythonExecuteServer(hostname, port)
+def main(hostname: str, port: int, coverage_hostname: str, coverage_port: str):
+    server = PythonExecuteServer(hostname, port, coverage_hostname, coverage_port)
     server.run()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(
         prog='UtBot Python Executor',
         description='Listen socket stream and execute function value',
@@ -18,17 +18,19 @@
     parser.add_argument('port', type=int)
     parser.add_argument('--logfile', default=None)
     parser.add_argument(
             '--loglevel',
             choices=["DEBUG", "INFO", "ERROR"],
             default="ERROR",
             )
+    parser.add_argument('coverage_hostname')
+    parser.add_argument('coverage_port', type=int)
     args = parser.parse_args()
 
     loglevel = {"DEBUG": logging.DEBUG, "INFO": logging.INFO, "ERROR": logging.ERROR}[args.loglevel]
     logging.basicConfig(
             filename=args.logfile,
             format='%(asctime)s | %(levelname)s | %(funcName)s - %(message)s',
             datefmt='%m/%d/%Y %H:%M:%S',
             level=loglevel,
             )
-    main(args.hostname, args.port)
+    main(args.hostname, args.port, args.coverage_hostname, args.coverage_port)
```

### Comparing `utbot_executor-1.6.2/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.6.3/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.6.3/utbot_executor/deep_serialization/example.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.6.3/utbot_executor/deep_serialization/json_converter.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.6.3/utbot_executor/deep_serialization/memory_objects.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/deep_serialization/test_json.json` & `utbot_executor-1.6.3/utbot_executor/deep_serialization/test_json.json`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.6.3/utbot_executor/deep_serialization/utils.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/executor.py` & `utbot_executor-1.6.3/utbot_executor/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Python code executor for UnitTestBot"""
 import copy
 import inspect
 import importlib
 import logging
 import pathlib
+import socket
 import sys
-import trace
 import traceback
+import typing
 from typing import Any, Callable, Dict, Iterable, List, Tuple
 
 from utbot_executor.deep_serialization.deep_serialization import serialize_objects, serialize_memory_dump, \
     serialize_objects_dump
 from utbot_executor.deep_serialization.json_converter import DumpLoader, deserialize_memory_objects
 from utbot_executor.deep_serialization.memory_objects import MemoryDump, ReduceMemoryObject, PythonSerializer
 from utbot_executor.deep_serialization.utils import PythonId, getattr_by_path
@@ -34,14 +35,18 @@
     serializer.clear_visited()
     for obj in objs:
         serializer.write_object_to_memory(obj)
     return serializer.memory
 
 
 class PythonExecutor:
+    def __init__(self, coverage_hostname: str, coverage_port: int):
+        self.coverage_hostname = coverage_hostname
+        self.coverage_port = coverage_port
+
     @staticmethod
     def add_syspaths(syspaths: Iterable[str]):
         for path in syspaths:
             if path not in sys.path:
                 sys.path.insert(0, path)
 
     @staticmethod
@@ -98,20 +103,29 @@
             return ExecutionFailResponse("fail", traceback.format_exc())
         logging.debug("Arguments have been created")
 
         try:
             state_before_memory = _load_objects(args + list(kwargs.values()))
             init_state_before = _update_states(loader.reload_id(), state_before_memory)
             serialized_state_init = serialize_memory_dump(init_state_before)
+
+            def _coverage_sender(info: typing.Tuple[str, int]):
+                sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+                logging.debug("Coverage message: %s:%d", request.coverage_id, info[1])
+                message = bytes(f'{request.coverage_id}:{info[1]}', encoding='utf-8')
+                sock.sendto(message, (self.coverage_hostname, self.coverage_port))
+                logging.debug("ID: %s, Coverage: %s", request.coverage_id, info)
+
             value = _run_calculate_function_value(
                     function,
                     args,
                     kwargs,
                     request.filepath,
-                    serialized_state_init
+                    serialized_state_init,
+                    tracer=UtTracer(_coverage_sender)
                     )
         except Exception as _:
             logging.debug("Error \n%s", traceback.format_exc())
             return ExecutionFailResponse("fail", traceback.format_exc())
         logging.debug("Value have been calculated: %s", value)
         return value
```

### Comparing `utbot_executor-1.6.2/utbot_executor/listener.py` & `utbot_executor-1.6.3/utbot_executor/listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 
 
 class PythonExecuteServer:
     def __init__(
             self,
             hostname: str,
             port: int,
+            coverage_hostname: str,
+            coverage_port: str,
             ):
         logging.info('PythonExecutor is creating...')
         self.clientsocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.clientsocket.connect((hostname, port))
-        self.executor = PythonExecutor()
+        self.executor = PythonExecutor(coverage_hostname, coverage_port)
 
     def run(self) -> None:
         logging.info('PythonExecutor is ready...')
         try:
             self.handler()
         finally:
             self.clientsocket.close()
```

### Comparing `utbot_executor-1.6.2/utbot_executor/memory_compressor.py` & `utbot_executor-1.6.3/utbot_executor/memory_compressor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/parser.py` & `utbot_executor-1.6.3/utbot_executor/parser.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.2/utbot_executor/ut_tracer.py` & `utbot_executor-1.6.3/utbot_executor/ut_tracer.py`

 * *Files identical despite different names*

