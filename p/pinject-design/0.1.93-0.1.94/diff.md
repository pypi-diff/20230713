# Comparing `tmp/pinject_design-0.1.93.tar.gz` & `tmp/pinject_design-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinject_design-0.1.93.tar", max compression
+gzip compressed data, was "pinject_design-0.1.94.tar", max compression
```

## Comparing `pinject_design-0.1.93.tar` & `pinject_design-0.1.94.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.93/LICENSE
--rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.93/pinject_design/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.93/pinject_design/di/__init__.py
--rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.93/pinject_design/di/app_designed.py
--rw-r--r--   0        0        0     2536 2023-07-12 07:11:32.777696 pinject_design-0.1.93/pinject_design/di/app_injected.py
--rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.93/pinject_design/di/applicative.py
--rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.93/pinject_design/di/ast.py
--rw-r--r--   0        0        0     7402 2023-07-12 06:48:32.126362 pinject_design-0.1.93/pinject_design/di/design.py
--rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.93/pinject_design/di/designed.py
--rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.93/pinject_design/di/dynamic_proxy.py
--rw-r--r--   0        0        0    29448 2023-07-12 06:36:42.176942 pinject_design-0.1.93/pinject_design/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.93/pinject_design/di/implicit_globals.py
--rw-r--r--   0        0        0    32106 2023-07-12 06:06:44.180482 pinject_design-0.1.93/pinject_design/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.93/pinject_design/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.93/pinject_design/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.93/pinject_design/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.93/pinject_design/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.93/pinject_design/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.93/pinject_design/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.93/pinject_design/di/session.py
--rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.93/pinject_design/di/sessioned.py
--rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.93/pinject_design/di/static_proxy.py
--rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.93/pinject_design/di/test_ast.py
--rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.93/pinject_design/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.93/pinject_design/di/test_graph.py
--rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.93/pinject_design/di/test_injected.py
--rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.93/pinject_design/di/test_proxiable.py
--rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.93/pinject_design/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.93/pinject_design/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.93/pinject_design/global_configs
--rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.93/pinject_design/global_configs.py
--rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.93/pinject_design/graph_inspection.py
--rw-r--r--   0        0        0     1612 2023-07-11 12:13:24.402905 pinject_design-0.1.93/pinject_design/helper_structure.py
--rw-r--r--   0        0        0     6272 2023-07-11 12:13:24.403516 pinject_design-0.1.93/pinject_design/helpers.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinject_design-0.1.93/pinject_design/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.93/pinject_design/nx_graph_util.py
--rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.93/pinject_design/pinject_design.iml
--rw-r--r--   0        0        0    20791 2023-07-11 12:13:24.404826 pinject_design-0.1.93/pinject_design/run_config_utils.py
--rw-r--r--   0        0        0     1590 2023-07-11 12:13:24.405223 pinject_design-0.1.93/pinject_design/run_config_utils_v2.py
--rw-r--r--   0        0        0      938 2023-07-11 12:13:24.405644 pinject_design-0.1.93/pinject_design/test_package/__init__.py
--rw-r--r--   0        0        0      234 2023-07-11 12:13:24.406011 pinject_design-0.1.93/pinject_design/test_package/child/__init__.py
--rw-r--r--   0        0        0      284 2023-07-11 12:13:24.406483 pinject_design-0.1.93/pinject_design/test_package/child/module1.py
--rw-r--r--   0        0        0    17998 2023-07-12 06:05:41.275007 pinject_design-0.1.93/pinject_design/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.93/pinject_design/viz/__init__.py
--rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.93/pinject_design/viz/graph.py
--rw-r--r--   0        0        0      639 2023-07-12 11:40:58.814948 pinject_design-0.1.93/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.94/LICENSE
+-rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.94/pinject_design/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.94/pinject_design/di/__init__.py
+-rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.94/pinject_design/di/app_designed.py
+-rw-r--r--   0        0        0     2536 2023-07-12 11:43:38.344272 pinject_design-0.1.94/pinject_design/di/app_injected.py
+-rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.94/pinject_design/di/applicative.py
+-rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.94/pinject_design/di/ast.py
+-rw-r--r--   0        0        0     7402 2023-07-12 11:43:38.344766 pinject_design-0.1.94/pinject_design/di/design.py
+-rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.94/pinject_design/di/designed.py
+-rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.94/pinject_design/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    29449 2023-07-13 04:36:34.812657 pinject_design-0.1.94/pinject_design/di/graph.py
+-rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.94/pinject_design/di/implicit_globals.py
+-rw-r--r--   0        0        0    32106 2023-07-12 11:43:38.345979 pinject_design-0.1.94/pinject_design/di/injected.py
+-rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.94/pinject_design/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.94/pinject_design/di/permissioned/__init__.py
+-rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.94/pinject_design/di/permissioned/blueprint.py
+-rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.94/pinject_design/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.94/pinject_design/di/provider.py
+-rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.94/pinject_design/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.94/pinject_design/di/session.py
+-rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.94/pinject_design/di/sessioned.py
+-rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.94/pinject_design/di/static_proxy.py
+-rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.94/pinject_design/di/test_ast.py
+-rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.94/pinject_design/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.94/pinject_design/di/test_graph.py
+-rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.94/pinject_design/di/test_injected.py
+-rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.94/pinject_design/di/test_proxiable.py
+-rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.94/pinject_design/di/util.py
+-rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.94/pinject_design/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.94/pinject_design/global_configs
+-rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.94/pinject_design/global_configs.py
+-rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.94/pinject_design/graph_inspection.py
+-rw-r--r--   0        0        0     1612 2023-07-13 03:15:00.373837 pinject_design-0.1.94/pinject_design/helper_structure.py
+-rw-r--r--   0        0        0     6272 2023-07-11 12:13:24.403516 pinject_design-0.1.94/pinject_design/helpers.py
+-rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinject_design-0.1.94/pinject_design/module_inspector.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.94/pinject_design/nx_graph_util.py
+-rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.94/pinject_design/pinject_design.iml
+-rw-r--r--   0        0        0    21597 2023-07-13 03:19:07.943777 pinject_design-0.1.94/pinject_design/run_config_utils.py
+-rw-r--r--   0        0        0     1590 2023-07-11 12:13:24.405223 pinject_design-0.1.94/pinject_design/run_config_utils_v2.py
+-rw-r--r--   0        0        0      938 2023-07-11 12:13:24.405644 pinject_design-0.1.94/pinject_design/test_package/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-11 12:13:24.406011 pinject_design-0.1.94/pinject_design/test_package/child/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-11 12:13:24.406483 pinject_design-0.1.94/pinject_design/test_package/child/module1.py
+-rw-r--r--   0        0        0    17998 2023-07-12 11:43:38.346496 pinject_design-0.1.94/pinject_design/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.94/pinject_design/viz/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.94/pinject_design/viz/graph.py
+-rw-r--r--   0        0        0      639 2023-07-13 04:36:49.153385 pinject_design-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.94/PKG-INFO
```

### Comparing `pinject_design-0.1.93/LICENSE` & `pinject_design-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/app_designed.py` & `pinject_design-0.1.94/pinject_design/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/app_injected.py` & `pinject_design-0.1.94/pinject_design/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/applicative.py` & `pinject_design-0.1.94/pinject_design/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/ast.py` & `pinject_design-0.1.94/pinject_design/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/design.py` & `pinject_design-0.1.94/pinject_design/di/design.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/designed.py` & `pinject_design-0.1.94/pinject_design/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/dynamic_proxy.py` & `pinject_design-0.1.94/pinject_design/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/graph.py` & `pinject_design-0.1.94/pinject_design/di/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,15 @@
     def child_session(self, overrides: "Design" = None):
         if overrides is None:
             from pinject_design import Design
             overrides = Design()
         child_scope = MChildScope(self.scope, set(overrides.keys()))
         child_graph = MyObjectGraph(None, self.design + overrides, child_scope)
         child_resolver = self.resolver.child(lambda: child_graph, overrides)
-        child_graph.resolver = child_resolver
+        child_graph._resolver = child_resolver
         return child_graph
 
     @property
     def design(self):
         return self.src_design
```

### Comparing `pinject_design-0.1.93/pinject_design/di/injected.py` & `pinject_design-0.1.94/pinject_design/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/injected_analysis.py` & `pinject_design-0.1.94/pinject_design/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/permissioned/blueprint.py` & `pinject_design-0.1.94/pinject_design/di/permissioned/blueprint.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/proxiable.py` & `pinject_design-0.1.94/pinject_design/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/session.py` & `pinject_design-0.1.94/pinject_design/di/session.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/sessioned.py` & `pinject_design-0.1.94/pinject_design/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/static_proxy.py` & `pinject_design-0.1.94/pinject_design/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/test_dynamic_proxy.py` & `pinject_design-0.1.94/pinject_design/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/test_graph.py` & `pinject_design-0.1.94/pinject_design/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/test_injected.py` & `pinject_design-0.1.94/pinject_design/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/test_proxiable.py` & `pinject_design-0.1.94/pinject_design/di/test_proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/di/util.py` & `pinject_design-0.1.94/pinject_design/di/util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/exceptions.py` & `pinject_design-0.1.94/pinject_design/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/graph_inspection.py` & `pinject_design-0.1.94/pinject_design/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/helper_structure.py` & `pinject_design-0.1.94/pinject_design/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/helpers.py` & `pinject_design-0.1.94/pinject_design/helpers.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/module_inspector.py` & `pinject_design-0.1.94/pinject_design/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/nx_graph_util.py` & `pinject_design-0.1.94/pinject_design/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/run_config_utils.py` & `pinject_design-0.1.94/pinject_design/run_config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 But we can use isinstance for tagging it.
 Alright.. but how do we give the optional design?
 Hmm, an easy way is to add some metadata though..
 Adding feature to an existing data structure is not recommended.
 So I guess I need to introduce a new data structure.
 """
 import asyncio
+import importlib
 import inspect
 import json
 import os
 from collections import defaultdict
 from datetime import datetime
 from pathlib import Path
 from pprint import pformat
@@ -439,22 +440,14 @@
         main_override_resolver,
         /,
         target: str,
         design_path: Optional[str] = None,
         overrides: str = None,
         show_graph: bool = False
 ) -> Optional[RunnablePair]:
-    """
-    :param main_targets:
-    :param main_design_paths:
-    :param target:
-    :param design_path:
-    :param overrides:
-    :return:
-    """
 
     tgt = main_targets[target]
     if design_path is None:
         design_path = main_design_paths[list(main_design_paths.keys())[0]]
     main_overrides = main_override_resolver(overrides)
     design = load_variable_by_module_path(design_path) + main_overrides
     pair = RunnablePair(target=tgt, design=design)
@@ -482,49 +475,76 @@
 
 def provide_design_paths(logger, module_path) -> OrderedDict[str, str]:
     design_paths = find_default_design_paths(module_path, None)
     design_paths = {design_path.split('.')[-1]: design_path for design_path in design_paths}
     logger.info(f"main design paths:{pformat(design_paths.keys())}")
     return design_paths
 
-
 @injected_function
 def main_override_resolver(query) -> Design:
     """
     :param query: can be filename with .json, .yaml.
     we can also try parsing it as json.
     :return:
     """
-    if query is None:
+    if isinstance(query,dict):
+        return instances(**query)
+    elif query is None:
         return Design()
     elif query.endswith('.json'):
         import json
+        if not Path(query).exists():
+            raise ValueError(f"cannot find {query} for configuration.")
         return instances(**json.load(open(query)))
     elif query.endswith('.yaml'):
         import yaml
+        if not Path(query).exists():
+            raise ValueError(f"cannot find {query} for configuration.")
         return instances(**yaml.load(open(query), Loader=yaml.SafeLoader))
     else:
         try:
             import json
             return instances(**json.loads(query))
         except:
             raise ValueError(f"cannot parse {query} as json")
 
 
+def load_variable_from_script(script_file: Path, varname: str):
+    spec = importlib.util.spec_from_file_location("module.name", script_file)
+    module = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+    return getattr(module, varname)
+
+
+def parse_override_path(p) -> Design:
+    if "::" in p:
+        file, varname = p.split("::")
+        return load_variable_by_module_path(Path(file), varname)
+    else:
+        load_variable_by_module_path(p)
+
+
 def run_main():
     """
     inspect the caller's frame for runnable target and design path.
     delegates its execution to fire.Fire.
 
     I want to resolve the override, but we don't know which protocol we should use.
 
     get the file this is run,
     find the runnables
     find the designs
     pass it to fire.
+
+    The protocol to override design:
+    1. python file
+    - /path/to/config.py::design_name
+    2. python module path
+    - my.package.design_name
+    3. yaml or json file
     :return:
     """
     import inspect
     import fire
     from loguru import logger
     runnable: RunnablePair = (instances(
         root_frame=inspect.currentframe().f_back,
@@ -571,14 +591,15 @@
     })
 
 
 def run_idea_conf(conf: IdeaRunConfiguration, *args, **kwargs):
     pre_args = conf.arguments[1:]
     return run_injected(*pre_args, *args, **kwargs)
 
+
 @memoize
 def get_designs_from_module(module_path: Path):
     from loguru import logger
     logger.info(f"trying to import designs from {module_path}")
 
     def accept(name, x):
         return isinstance(x, Design) and name != "__meta_design__"
```

### Comparing `pinject_design-0.1.93/pinject_design/run_config_utils_v2.py` & `pinject_design-0.1.94/pinject_design/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/test_package/__init__.py` & `pinject_design-0.1.94/pinject_design/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pinject_design/visualize_di.py` & `pinject_design-0.1.94/pinject_design/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.93/pyproject.toml` & `pinject_design-0.1.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinject-design"
-version = "0.1.93"
+version = "0.1.94"
 description = "immutable wrapper for pinject"
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 makefun = "*"
```

### Comparing `pinject_design-0.1.93/PKG-INFO` & `pinject_design-0.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinject-design
-Version: 0.1.93
+Version: 0.1.94
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

