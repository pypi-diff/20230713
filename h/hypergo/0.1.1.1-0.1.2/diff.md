# Comparing `tmp/hypergo-0.1.1.1.tar.gz` & `tmp/hypergo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.1.1.tar", last modified: Fri Jun 16 20:14:54 2023, max compression
+gzip compressed data, was "hypergo-0.1.2.tar", last modified: Thu Jul 13 18:09:05 2023, max compression
```

## Comparing `hypergo-0.1.1.1.tar` & `hypergo-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:54.866047 hypergo-0.1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:54.850046 hypergo-0.1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:54.858047 hypergo-0.1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 20:14:54.866047 hypergo-0.1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:54.862047 hypergo-0.1.1.1/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:54.866047 hypergo-0.1.1.1/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 20:14:54.000000 hypergo-0.1.1.1/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-16 20:14:54.000000 hypergo-0.1.1.1/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:14:54.000000 hypergo-0.1.1.1/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 20:14:54.000000 hypergo-0.1.1.1/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 20:14:54.000000 hypergo-0.1.1.1/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 20:14:54.866047 hypergo-0.1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:54.866047 hypergo-0.1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-16 20:14:43.000000 hypergo-0.1.1.1/tests/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.165165 hypergo-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.165165 hypergo-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 18:08:54.000000 hypergo-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-13 18:08:54.000000 hypergo-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 18:08:54.000000 hypergo-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-13 18:08:54.000000 hypergo-0.1.2/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:54.000000 hypergo-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-13 18:09:05.169165 hypergo-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 18:08:54.000000 hypergo-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-07-13 18:08:54.000000 hypergo-0.1.2/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-13 18:08:54.000000 hypergo-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 18:08:54.000000 hypergo-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 18:09:05.169165 hypergo-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_utility.py
```

### Comparing `hypergo-0.1.1.1/.github/workflows/python-publish.yml` & `hypergo-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/.gitignore` & `hypergo-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/BACKLOG.md` & `hypergo-0.1.2/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.2/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/hypergo/config.py` & `hypergo-0.1.2/hypergo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import sys
-from typing import List
+from typing import Any, Dict, List
 
 import yaml
 
 from hypergo.custom_types import TypedDictType
 
 if sys.version_info >= (3, 11):
     from typing import NotRequired
@@ -22,14 +22,15 @@
     lib_func: str
     input_keys: List[str]
     output_keys: List[str]
     input_bindings: List[str]
     output_bindings: List[str]
     input_operations: NotRequired[List[str]]
     output_operations: NotRequired[List[str]]
+    custom_properties: NotRequired[Dict[str, Any]]
 
 
 class Config:  # pylint: disable=too-many-instance-attributes
     # @staticmethod
     # def from_yaml(file_name: str) -> "Config":
     #     return Config.from_dict(Utility.yaml_read(file_name))
```

### Comparing `hypergo-0.1.1.1/hypergo/executor.py` & `hypergo-0.1.2/hypergo/executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import inspect
 import json
 import re
-from typing import Any, Callable, Generator, List, Mapping, Optional, cast
+from typing import Any, Callable, Generator, List, Mapping, Optional, Set, cast
 
 from hypergo.config import ConfigType
 from hypergo.context import ContextType
 from hypergo.local_storage import LocalStorage
 from hypergo.message import MessageType
 from hypergo.storage import Storage
 from hypergo.utility import Utility
@@ -26,17 +26,37 @@
     def __init__(self, config: ConfigType, storage: Optional[Storage] = None) -> None:
         self._config: ConfigType = config
         self._func_spec: Callable[..., Any] = Executor.func_spec(config["lib_func"])
         self._arg_spec: List[type] = Executor.arg_spec(self._func_spec)
         self._storage: Optional[Storage] = storage
 
     def get_args(self, context: ContextType) -> List[Any]:
-        args: List[Any] = []
+        def get_formatted_input_binding(input_binding: str, routing_key: str) -> str:
+            formatted_input_binding: str = input_binding
+            if "?" in input_binding:
+                # Hypergo-209 if a component includes custom_properties key in the config, find the key
+                # from custom_properties which is a subset of the routing key coming from the message
+                # and use it to massage input_binding values containing ?
+                input_message_routing_key_set: Set[str] = set(routing_key.split("."))
+                for key in self._config.get("custom_properties", {}).keys():
+                    key_set: Set[str] = set(key.split("."))
+                    # key is a proper subset of the
+                    # input_message_routing_key_set
+                    if key_set.intersection(input_message_routing_key_set) == key_set:
+                        formatted_input_binding = input_binding.replace("?", key.replace('.', '\\.'))
+                        break
+            return formatted_input_binding
 
-        for arg, argtype in zip(self._config["input_bindings"], self._arg_spec):
+        args: List[Any] = []
+        input_message_routing_key: str = Utility.deep_get(context, "message.routingkey")
+        input_bindings: List[str] = [
+            get_formatted_input_binding(input_binding=input_binding, routing_key=input_message_routing_key)
+            for input_binding in self._config["input_bindings"]
+        ]
+        for arg, argtype in zip(input_bindings, self._arg_spec):
             # determine if arg binding is a literal denoted by '<literal>'
             val: Any = ((match := re.match(r"'(.*)'", arg)) and match.group(1)) or Utility.deep_get(context, arg)
 
             if argtype == inspect.Parameter.empty:  # inspect._empty:
                 args.append(val)
             else:
                 args.append(Utility.safecast(argtype, val))
@@ -80,40 +100,46 @@
         envelope: MessageType = message
         if self._storage and "pass_by_reference" in self._config.get("output_operations", []):
             envelope["storagekey"] = f"passbyreference/{Utility.hash(json.dumps(envelope))}"
             self.store(envelope["storagekey"], message)
             envelope["body"] = {}
         return envelope
 
+    def get_output_routing_key(self, input_message_routing_key: str) -> str:
+        routing_key_set: Set[str] = set(input_message_routing_key.split("."))
+        tokens: List[str] = []
+        for input_key in self._config["input_keys"]:
+            # hypergo-144 dynamic routing key only for generic components
+            # output key will contain context derived from the previous
+            # producer routing key
+            input_key_set: Set[str] = set(input_key.split("."))
+            intersection_set: Set[str] = routing_key_set.intersection(input_key_set)
+            # check if the routing key is in the input_key
+            if intersection_set == input_key_set:
+                # set difference operation to remove the subset of the routing key captured by the component
+                # from its input_key and append it to tokens
+                tokens.append(".".join(routing_key_set.difference(intersection_set)))
+        token: str = self.organize_tokens(tokens)
+        output_tokens: List[str] = [
+            re.sub(r"(?<=\.)\?(?=\.)|^\?|(?<=\.)\?$|^\?$", token, output_key)
+            for output_key in self._config["output_keys"]
+        ]
+        return self.organize_tokens(output_tokens)
+
     def execute(self, input_envelope: MessageType) -> Generator[MessageType, None, None]:
         input_message: MessageType = self.open_envelope(input_envelope)
         context: ContextType = {"message": input_message, "config": self._config}
         if self._storage:
             context["storage"] = self._storage.use_sub_path(f"component/private/{self._config['name']}")
         args: List[Any] = self.get_args(context)
         execution: Any = self._func_spec(*args)
+        output_routing_key: str = self.get_output_routing_key(input_message["routingkey"])
         return_values: List[Any] = list(execution) if inspect.isgenerator(execution) else [execution]
-        routing_key: str = input_message["routingkey"]
-        routing_key_set: set = set(routing_key.split("."))
         for return_value in return_values:
-            tokens: List[str] = []
-            for input_key in self._config["input_keys"]:
-                # hypergo-144 dynamic routing key only for generic components
-                # output key will contain context derived from the previous producer routing key 
-                input_key_set: set = set(input_key.split("."))
-                intersection_set: set = routing_key_set.intersection(input_key_set)
-                # check if the routing key is in the input_key
-                if intersection_set == input_key_set:
-                    # set difference operation to remove the subset of the routing key captured by the component
-                    # from its input_key and append it to tokens
-                    tokens.append(".".join(routing_key_set.difference(intersection_set)))
-            token: str = self.organize_tokens(tokens)
-            output_tokens: List[str] = [re.sub(r"(?<=\.)\?(?=\.)|^\?|(?<=\.)\?$|^\?$", token, output_key)
-                                        for output_key in self._config["output_keys"]]
-            output_message: MessageType = {"routingkey": self.organize_tokens(output_tokens), "body": {}}
+            output_message: MessageType = {"routingkey": output_routing_key, "body": {}}
             output_context: ContextType = {"message": output_message, "config": self._config}
 
             def handle_tuple(dst: ContextType, src: Any) -> None:
                 for binding, tuple_elem in zip(self._config["output_bindings"], src):
                     Utility.deep_set(dst, binding, tuple_elem)
 
             def handle_default(dst: ContextType, src: Any) -> None:
@@ -129,18 +155,24 @@
             yield output_envelope
 
     def organize_tokens(self, keys: List[str]) -> str:
         return ".".join(sorted(set(".".join(keys).split("."))))
 
 
 def main() -> None:
-    cfg: ConfigType = {"namespace": "datalink", "name": "csvconverter", "package": "ldp-csv-to-json-converter",
-                       "lib_func": "csv_to_json_converter_appliance.__main__.csv_to_json_appliance",
-                       "input_keys": ["batch.csv"], "output_keys": ["batch.json"],
-                       "input_bindings": ["message.body.data_blob_path"], "output_bindings": ["message.body.json_data"]}
+    cfg: ConfigType = {
+        "namespace": "datalink",
+        "name": "csvconverter",
+        "package": "ldp-csv-to-json-converter",
+        "lib_func": "csv_to_json_converter_appliance.__main__.csv_to_json_appliance",
+        "input_keys": ["batch.csv"],
+        "output_keys": ["batch.json"],
+        "input_bindings": ["message.body.data_blob_path"],
+        "output_bindings": ["message.body.json_data"],
+    }
     stg: Storage = LocalStorage()
     executor = Executor(cfg, stg)
     print(executor.retrieve("hypergo/json_test_data.json"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hypergo-0.1.1.1/hypergo/graph.py` & `hypergo-0.1.2/hypergo/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 import sys
 from typing import Dict, Generator, List, Tuple, Union
 
 import graphviz
 
 
 def format_component(config: Dict[str, Union[None, str, List[str]]]) -> Tuple[str, str]:
-    component_string = f'<<table border="0" cellborder="0"><tr><td bgcolor="#0071BD">{config.get("name")}</td></tr></table>>'
+    component_string = (
+        f'<<table border="0" cellborder="0"><tr><td bgcolor="#0071BD">{config.get("name")}</td></tr></table>>'
+    )
     return (f'component_{config.get("name")}', component_string)
 
 
-def format_topic(typestr: str, config: Dict[str, Union[None, str, List[str]]]) -> Generator[Tuple[str, str], None, None]:
+def format_topic(
+    typestr: str, config: Dict[str, Union[None, str, List[str]]]
+) -> Generator[Tuple[str, str], None, None]:
     tlist = config.get(typestr) or []
     if isinstance(tlist, str):
         tlist = [tlist]
 
     for routingkey_element in tlist:
         routingkey_str = '.'.join(sorted('&#x3a;'.join(routingkey_element.split(':')).split('.')))
         yield (f'routingkey_{routingkey_str}', routingkey_str)
@@ -28,31 +32,31 @@
 
     for folder in folders:
         config_files = glob.glob(os.path.join(folder, '**/*.json'), recursive=True)
         for config_file in config_files:
             with open(config_file, 'r', encoding='utf8') as stream:
                 config_json = json.load(stream)
                 if not isinstance(config_json, list):
-                    config_json: List(any) = [config_json]
+                    config_json = [config_json]
                 for config in config_json:
                     if config and 'name' in config:
                         configs.append(config)
     return configs
 
 
 def topics(dot: graphviz.Digraph, configs: List[Dict[str, Union[None, str, List[str]]]]) -> None:
     for config in configs:
         for routing_key_element in format_topic('output_keys', config):
             create_edge(dot, format_component(config)[0], routing_key_element[0])
-            dot.node(*routing_key_element, shape='none')
+            dot.node(*routing_key_element, shape='none', fixedsize='false')
         for routing_key_element in format_topic('error_output_keys', config):
             create_edge(dot, format_component(config)[0], routing_key_element[0])
-            dot.node(*routing_key_element, shape='none')
+            dot.node(*routing_key_element, shape='none', fixedsize='false')
         for routing_key_element in format_topic('input_keys', config):
-            dot.node(*routing_key_element, shape='none')
+            dot.node(*routing_key_element, shape='none', fixedsize='false')
             create_edge(dot, routing_key_element[0], format_component(config)[0])
 
 
 def derived_edges_inner(output_key: Tuple[str, str], in_keys: List[Tuple[str, str]]) -> List[Tuple[str, str]]:
     edges: List[Tuple[str, str]] = []
     for input_key in in_keys:
         if input_key[0] == output_key[0]:
@@ -114,8 +118,8 @@
     topics(dot, configs)
     derived_topics(dot, configs)
 
     dot.render('.graph.gv', view=True)
 
 
 if __name__ == '__main__':
-    graph(sys.argv[1:])
+    graph(sys.argv[1:])
```

### Comparing `hypergo-0.1.1.1/hypergo/message.py` & `hypergo-0.1.2/hypergo/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import sys
 from typing import cast
+from urllib.parse import urlparse
 
 import azure.functions as func
 from azure.servicebus import ServiceBusMessage
 
 from hypergo.custom_types import JsonDict, TypedDictType
 
 if sys.version_info >= (3, 11):
@@ -18,19 +19,33 @@
     routingkey: str
     storagekey: NotRequired[str]
 
 
 class Message:
     @staticmethod
     def from_azure_functions_service_bus_message(message: func.ServiceBusMessage) -> MessageType:
-        return {"body": json.loads(message.get_body().decode("utf-8")), "routingkey": message.user_properties["routingkey"], "storagekey": cast(str, message.user_properties.get("storagekey"))}
+        return {
+            "body": json.loads(message.get_body().decode("utf-8")),
+            "routingkey": message.user_properties["routingkey"],
+            "storagekey": cast(str, message.user_properties.get("storagekey")),
+        }
+
+    @staticmethod
+    def from_http_request(request: func.HttpRequest) -> MessageType:
+        return {"body": request.get_json(), "routingkey": "http_request" + urlparse(request.url).path.replace("/", ".")}
 
     @staticmethod
     def to_azure_service_bus_service_bus_message(message: MessageType) -> ServiceBusMessage:
-        ret: ServiceBusMessage = ServiceBusMessage(body=json.dumps(message["body"]), application_properties={"routingkey": message["routingkey"], "storagekey": cast(str, message.get("storagekey"))})
+        ret: ServiceBusMessage = ServiceBusMessage(
+            body=json.dumps(message["body"]),
+            application_properties={
+                "routingkey": message["routingkey"],
+                "storagekey": cast(str, message.get("storagekey")),
+            },
+        )
 
         return ret
 
     # def __init__(self, message: MessageType) -> None:
     #     self._body: JsonDict = message["body"]
     #     self._routingkey: str = message["routingkey"]
     #     self._config: Config = Config(message["config"])
```

### Comparing `hypergo-0.1.1.1/hypergo/service_bus_connection.py` & `hypergo-0.1.2/hypergo/service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/hypergo/storage.py` & `hypergo-0.1.2/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/hypergo/utility.py` & `hypergo-0.1.2/hypergo/utility.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import hashlib
 import inspect
 import json
 from typing import Any, Dict, Mapping, Union, cast, get_origin
 
 import glom
+import pydash
 import yaml
 
 from hypergo.custom_types import TypedDictType
 
 
 class Utility:
     @staticmethod
     def deep_get(dic: Union[TypedDictType, Dict[str, Any]], key: str) -> Any:
-        return glom.glom(dic, key)
+        result = pydash.get(dic, key)
+        if not result:
+            raise KeyError("Spec {key} not found in the dictionary")
+        return result
 
     @staticmethod
     def deep_set(dic: Union[TypedDictType, Dict[str, Any]], key: str, val: Any) -> None:
         glom.assign(dic, key, val, missing=dict)
 
     @staticmethod
     def yaml_read(file_name: str) -> Mapping[str, Any]:
@@ -41,14 +45,29 @@
         return hashlib.md5(content.encode("utf-8")).hexdigest()
 
     @staticmethod
     def safecast(expected_type: type, provided_value: Any) -> Any:
         ret: Any = provided_value
         value_type: Any = get_origin(expected_type) or expected_type
 
-        if value_type not in [int, float, complex, bool, str, bytes, bytearray, memoryview, list, tuple, range, set, frozenset, dict]:
+        if value_type not in [
+            int,
+            float,
+            complex,
+            bool,
+            str,
+            bytes,
+            bytearray,
+            memoryview,
+            list,
+            tuple,
+            range,
+            set,
+            frozenset,
+            dict,
+        ]:
             return cast(value_type, provided_value)
 
         if value_type != inspect.Parameter.empty:
             ret = value_type(provided_value)
 
         return ret
```

### Comparing `hypergo-0.1.1.1/hypergo/version.py` & `hypergo-0.1.2/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.2/hypergo.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 README.md
 lint.sh
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/python-publish.yml
 hypergo/__init__.py
-hypergo/__main__.py
 hypergo/azure_service_bus_connection.py
 hypergo/azure_service_bus_executor.py
 hypergo/config.py
 hypergo/context.py
 hypergo/custom_types.py
 hypergo/executor.py
 hypergo/graph.py
@@ -27,10 +26,13 @@
 hypergo.egg-info/PKG-INFO
 hypergo.egg-info/SOURCES.txt
 hypergo.egg-info/dependency_links.txt
 hypergo.egg-info/requires.txt
 hypergo.egg-info/top_level.txt
 tests/test.json
 tests/test.yaml
+tests/test_dynamic_input_bindings.py
+tests/test_dynamic_routing_key.py
 tests/test_local_storage.py
+tests/test_message.py
 tests/test_storage.py
 tests/test_utility.py
```

### Comparing `hypergo-0.1.1.1/lint.sh` & `hypergo-0.1.2/lint.sh`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # if [ $? -ne 0 ]; then { printf "\e[31mFailed, aborting.\n%s\e[0m\n" "$VERSION" ; exit 1; } fi
 
 printf "\e[1mFormatting code (autopep) $mod ...\e[0m\n"
 autopep8 --in-place --aggressive --aggressive --recursive $mod
 if [ $? -ne 0 ]; then { printf "\e[31mFailed, aborting.\e[0m\n" ; exit 1; } fi
 
 printf "\e[1mFormatting code (black) $mod ...\e[0m\n"
-black -S --line-length 512 $mod
+black -S --line-length 120 $mod
 if [ $? -ne 0 ]; then { printf "\e[31mFailed, aborting.\e[0m\n" ; exit 1; } fi
 
 printf "\e[1mSorting imports (isort) $mod ...\e[0m\n"
 isort $mod/*.py
 if [ $? -ne 0 ]; then { printf "\e[31mFailed, aborting.\e[0m\n" ; exit 1; } fi
 
 printf "\e[1mLinting (pylint) $mod ...\e[0m\n"
```

### Comparing `hypergo-0.1.1.1/tests/test.json` & `hypergo-0.1.2/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/tests/test.yaml` & `hypergo-0.1.2/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/tests/test_local_storage.py` & `hypergo-0.1.2/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/tests/test_storage.py` & `hypergo-0.1.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.1.1/tests/test_utility.py` & `hypergo-0.1.2/tests/test_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,41 @@
+import os
+import sys
 import unittest
 from unittest.mock import MagicMock
 
-from typing import Any, Dict, Mapping, Union
-from hypergo.custom_types import TypedDictType
+from typing import Dict
+
+SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
+sys.path.append(os.path.dirname(SCRIPT_DIR))
+
 from hypergo.utility import Utility
 
-import glom
 import json
 import yaml
 
+
 class TestUtility(unittest.TestCase):
     def test_deep_get(self) -> None:
         # Test when key exists in dictionary
         input_dict: Dict[str, Dict[str, int]] = {"a": {"b": 1}}
         key: str = "a.b"
         expected_output: int = 1
         self.assertEqual(Utility.deep_get(input_dict, key), expected_output)
 
+        # Test for keys with . and no nested structure
+        input_dict: Dict[str, Dict[str, int]] = {"a.b": 1}
+        key: str = "a.b"
+        expected_output: int = 1
+        self.assertEqual(Utility.deep_get(input_dict, key.replace('.', '\\.')), expected_output)
+
         # Test when key does not exist in dictionary
         input_dict: Dict[str, Dict[str, int]] = {"a": {"b": 1}}
         key: str = "a.c"
-        with self.assertRaises(glom.PathAccessError):
+        with self.assertRaises(KeyError):
             Utility.deep_get(input_dict, key)
 
     def test_deep_set(self) -> None:
         # Test when key exists in dictionary
         input_dict: Dict[str, Dict[str, int]] = {"a": {"b": 1}}
         key: str = "a.b"
         val: int = 2
```

