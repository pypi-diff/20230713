# Comparing `tmp/ia-sdk-0.3.8.tar.gz` & `tmp/ia-sdk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia-sdk-0.3.8.tar", last modified: Mon Jan 23 16:38:03 2023, max compression
+gzip compressed data, was "ia-sdk-0.3.9.tar", last modified: Wed Jan 25 14:59:51 2023, max compression
```

## Comparing `ia-sdk-0.3.8.tar` & `ia-sdk-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-23 16:38:03.229351 ia-sdk-0.3.8/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5213 2023-01-23 16:38:03.229351 ia-sdk-0.3.8/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4799 2022-05-26 13:05:31.000000 ia-sdk-0.3.8/README.md
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-23 16:38:03.225352 ia-sdk-0.3.8/ia/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-01-23 16:37:02.000000 ia-sdk-0.3.8/ia/__init__.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-23 16:38:03.225352 ia-sdk-0.3.8/ia/gaius/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.3.8/ia/gaius/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    46134 2023-01-19 19:30:50.000000 ia-sdk-0.3.8/ia/gaius/agent_client.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22850 2023-01-17 21:26:52.000000 ia-sdk-0.3.8/ia/gaius/back_testing.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2022-05-26 13:05:31.000000 ia-sdk-0.3.8/ia/gaius/data_language.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    20079 2023-01-20 21:16:43.000000 ia-sdk-0.3.8/ia/gaius/data_ops.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3900 2023-01-17 04:21:58.000000 ia-sdk-0.3.8/ia/gaius/genome_info.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     7923 2023-01-23 16:37:28.000000 ia-sdk-0.3.8/ia/gaius/kb_ops.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4965 2023-01-22 21:38:34.000000 ia-sdk-0.3.8/ia/gaius/prediction_models.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    49698 2023-01-22 21:03:05.000000 ia-sdk-0.3.8/ia/gaius/pvt.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-23 16:38:03.229351 ia-sdk-0.3.8/ia/gaius/tests/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.3.8/ia/gaius/tests/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2677 2022-05-26 13:05:31.000000 ia-sdk-0.3.8/ia/gaius/tests/classification.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     6907 2023-01-17 21:18:07.000000 ia-sdk-0.3.8/ia/gaius/tests/pvt_utils.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2446 2022-07-29 18:03:36.000000 ia-sdk-0.3.8/ia/gaius/tests/utility.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4832 2023-01-19 19:17:05.000000 ia-sdk-0.3.8/ia/gaius/utils.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-23 16:38:03.229351 ia-sdk-0.3.8/ia_sdk.egg-info/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5213 2023-01-23 16:38:03.000000 ia-sdk-0.3.8/ia_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      531 2023-01-23 16:38:03.000000 ia-sdk-0.3.8/ia_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-01-23 16:38:03.000000 ia-sdk-0.3.8/ia_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       48 2023-01-23 16:38:03.000000 ia-sdk-0.3.8/ia_sdk.egg-info/requires.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-01-23 16:38:03.000000 ia-sdk-0.3.8/ia_sdk.egg-info/top_level.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-01-23 16:38:03.229351 ia-sdk-0.3.8/setup.cfg
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      766 2023-01-17 21:00:37.000000 ia-sdk-0.3.8/setup.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5213 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4799 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/README.md
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.877697 ia-sdk-0.3.9/ia/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-01-25 14:59:45.000000 ia-sdk-0.3.9/ia/__init__.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/ia/gaius/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    61594 2023-01-25 14:59:45.000000 ia-sdk-0.3.9/ia/gaius/agent_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22850 2023-01-17 21:26:52.000000 ia-sdk-0.3.9/ia/gaius/back_testing.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/data_language.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    21246 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/data_ops.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3900 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/genome_info.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9382 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/kb_ops.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4965 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/prediction_models.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    52008 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/pvt.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/ia/gaius/tests/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/tests/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2677 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/tests/classification.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     6907 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/tests/pvt_utils.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2446 2022-07-29 18:03:36.000000 ia-sdk-0.3.9/ia/gaius/tests/utility.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5644 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/ia_sdk.egg-info/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5213 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      531 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       48 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/requires.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/setup.cfg
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      766 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/setup.py
```

### Comparing `ia-sdk-0.3.8/PKG-INFO` & `ia-sdk-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: SDK for Intelligent Artifact's GAIuS agents.
 Home-page: https://intelligent-artifacts.com
 Author: Intelligent Artifacts
 Author-email: support@intelligent-artifacts.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ia-sdk-0.3.8/README.md` & `ia-sdk-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/agent_client.py` & `ia-sdk-0.3.9/ia/gaius/agent_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-"""Implements the "Agent" interface."""
 import functools
 import io
 import json
 import uuid
 from typing import Dict, List, Any, Tuple, Union
 from os.path import join
 from datetime import datetime
 from copy import deepcopy
 import requests
 
 from ia.gaius.genome_info import Genome
-
-
 class AgentQueryError(BaseException):
     """Raised if any query to any node returns an error."""
     pass
 
 
 class AgentConnectionError(BaseException):
     """Raised if connecting to any node returns an error."""
@@ -40,15 +37,14 @@
         if 'unique_id' in response:
             del response['unique_id']
         for value in response.values():
             if isinstance(value, dict):
                 _remove_unique_id(value)
     return response
 
-
 class AgentClient:
     """Interface for interacting with agents."""
 
     def __init__(self, bottle_info: dict, verify:bool=True):
         """
         Provide agent information in a dictionary.
         
@@ -225,15 +221,15 @@
                 .. code-block:: python
                 
                     # set summarize_for_single_node to True
                     >>> agent.set_summarize_for_single_node(value=True)
                     >>> gdf = {'strings':['hello'], 'vectors': [], 'emotives':{}}
                     >>> agent.observe(gdf)
                     'observed'
-                    
+
                     # set summarize_for_single_node to False
                     >>> agent.set_summarize_for_single_node(value=False)
                     >>> agent.observe(gdf)
                     {'P1': 'observed'}
         
         """
         self.summarize_for_single_node = value
@@ -245,16 +241,19 @@
             Args:
                 data (dict): the GDF data to be observed
                 nodes (list, optional): Nodes to observe data on, defaults to ingress nodes
             
             Example:
                 .. code-block:: python
                 
-                    gdf = {"strings":["hello"], "vectors": [], "emotives":{}, "metadata":{}}
-                    agent.observe(data=gdf, nodes=["P1"])
+                    from ia.gaius.utils import create_gdf
+                    >>> gdf = create_gdf(strings=['hello'])
+                    >>> agent.observe(data=gdf, nodes=["P1"])
+                    'observed'
+                    
         """
         if nodes is None:
             nodes = self.ingress_nodes
         return self._query(self.session.post, 'observe', data=data, nodes=nodes)
 
     def _observe_event(self, data: Dict, unique_id: str = None) -> Tuple[dict, str]:
         """Exclusively uses the 'observe' call."""
@@ -301,15 +300,16 @@
 
     def learn(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return the learn results.
         
         Example:
             .. code-block:: python
             
-                model_name = agent.learn(nodes=["P1"])
+                >>> agent.learn(nodes=["P1"])
+                'MODEL|004da01b0ef40d7c3e0965a6b4fd0f413672fbff'
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'learn', nodes=nodes)
 
     def get_wm(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return information about Working Memory.
@@ -356,15 +356,16 @@
     def clear_all_memory(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Clear both the Working Memory and persisted memory.
         Equivalent to re-initializing the nodes specified
         
         Example:
             .. code-block:: python
             
-                agent.clear_all_memory(nodes=["P1"])
+                >>> agent.clear_all_memory(nodes=["P1"])
+                'all-cleared'
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'clear-all-memory', nodes=nodes)
 
     def get_percept_data(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return percept data.
@@ -385,14 +386,20 @@
             .. code-block:: python
             
                 cog_data = agent.get_cognition_data(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.query_nodes
         return self._query(self.session.get, 'cognition-data', nodes=nodes, unique_id=unique_id)
+    
+    def get_all_genes(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+        """Return cognition data."""
+        if nodes is None:
+            nodes = self.query_nodes
+        return self._query(self.session.get, 'all-genes', nodes=nodes)
 
     def get_all_genes(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return all genes for nodes.
         
         Example:
             .. code-block:: python
             
@@ -633,14 +640,298 @@
                 
                     >>> agent.get_time(nodes=['P1'])
                     '1'
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.get, 'time', nodes=nodes)
+    
+    @_ensure_connected
+    def get_models_with_symbols(self, symbols_list : List = None, nodes: List = None) -> Union[dict, Any]:
+        '''
+            Function which search the kbs on the nodes for models with certain symbols.
+            All symbols must be present in model.sequence, or the model will not be returned
+        '''
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.post(
+                f"{self._url}{node['id']}/get-models-with-symbols",
+                verify=self._verify,
+                headers=self._headers,
+                json={'data': symbols_list},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result
+    
+    @_ensure_connected
+    def get_models_with_patterns(self, symbols_list : List = None, nodes: List = None) -> Union[dict, Any]:
+        '''
+            Function which search the kbs on the nodes for models with certain regex patterns.
+            All regex patterns must be present in model.sequence, or the model will not be returned
+        '''
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.post(
+                f"{self._url}{node['id']}/get-models-with-patterns",
+                verify=self._verify,
+                headers=self._headers,
+                json={'data': symbols_list},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result
+    
+    @_ensure_connected
+    def add_model(self, sequence : List, vector : List = None, frequency : int = 1, emotives : Dict = {}, nodes: List = None) -> Union[dict, Any]:
+        '''
+            Function to explicitely add a model with the given sequence of symbols, frequency, and emotives.
+            Returns the hash of the generated function
+        '''
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.put(
+                f"{self._url}{node['id']}/add-model",
+                verify=self._verify,
+                headers=self._headers,
+                json={'sequence': sequence,
+                      'vector': vector,
+                     'frequency' : frequency,
+                     'emotives' : emotives},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result
+    
+    @_ensure_connected
+    def remove_symbols_from_system(self, symbols_list : List, nodes: List = None) -> Union[dict, Any]:
+        """Function which search the kbs on the nodes for models with certain symbols.
+            Symbols are removed, and the symbols are blacklisted, thus making it impossible fo them to
+            be in the working memory in the future.
+
+        Args:
+            symbols_list (List): list of symbols to remove. Defaults to None.
+            nodes (List, optional): list of nodes to remove symbols from. Defaults to None (all nodes).
+
+        Raises:
+            AgentQueryError: Error in Cognitive Processor handling
+
+        Returns:
+            Union[dict, Any]: dict showing old model hash -> new model hash (or 'deleted') pairs
+        """
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.delete(
+                f"{self._url}{node['id']}/symbols/remove",
+                verify=self._verify,
+                headers=self._headers,
+                json={'data': symbols_list},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result
+    
+    @_ensure_connected
+    def remove_patterns_from_system(self, symbols_list : List, nodes: List = None) -> Union[dict, Any]:
+        """Function which search the kbs on the nodes for models with certain regex patterns.
+            Removed symbols that matches patterns, but does not blacklist them. So patterns may show
+            up in the future.
+
+        Args:
+            symbols_list (List): list of regex symbol patterns to remove.
+            nodes (List, optional): list of nodes to remove symbols on. Defaults to None (all nodes).
+
+        Raises:
+            AgentQueryError: Error in Cognitive Processor handling
+
+        Returns:
+            Union[dict, Any]: dict showing old model hash -> new model hash (or 'deleted') pairs
+        """
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.delete(
+                f"{self._url}{node['id']}/patterns/remove",
+                verify=self._verify,
+                headers=self._headers,
+                json={'data': symbols_list},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result
+
+    def add_blacklisted_symbols(self, symbols_list: List, nodes: List = None):
+        """Add a symbol to the blacklist manually. 
+        List all symbols currently in the blacklist using :func:`list_blacklisted_symbols`.
+        Symbols may be removed from this list by using :func:`remove_blacklisted_symbols`.
+
+        Args:
+            symbols_list (List): list of symbols to add to the 
+            nodes (List, optional): list of nodes to add blacklisted symbols on. Defaults to None (all nodes).
+
+        Raises:
+            AgentQueryError: Error in Cognitive Processor handling
+
+        Returns:
+            dict or str: Depicting result of adding blacklisted symbols to each CP in nodes
+        """
+        
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.post(
+                f"{self._url}{node['id']}/blacklisted-symbols/add",
+                verify=self._verify,
+                headers=self._headers,
+                json={'data': symbols_list},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result   
+
+    def list_blacklisted_symbols(self, nodes: List = None):
+        """Display a list of all symbols currently 'blacklisted' on each node in *nodes*. 
+        Symbols enter this list by being removed from a Cognitive Processor via :func:`remove_symbols_from_system` or :func:`remove_patterns_from_system`.
+        Symbols may be removed from this list by using :func:`remove_blacklisted_symbols`.
+
+        Args:
+            nodes (List, optional): list of nodes to show blacklisted symbols on. Defaults to None (all nodes).
+        """
+        
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.get(
+                f"{self._url}{node['id']}/list-blacklisted-symbols",
+                verify=self._verify,
+                headers=self._headers,
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result   
+
+    
+    def remove_blacklisted_symbols(self, symbols_to_remove: List, nodes: List = None):
+        """Remove symbols from blacklist on each Cognitive Processor in *nodes*
+
+        Args:
+            symbols_to_remove (List): list of symbols to remove from blacklisted symbols
+            nodes (List, optional): list of nodes to remove blacklisted symbols on. Defaults to None (all nodes).
+
+        Raises:
+            AgentQueryError: Error in Cognitive Processor handling
+
+        Returns:
+            _type_: _description_
+        """
+        
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.delete(
+                f"{self._url}{node['id']}/blacklisted-symbols/remove",
+                verify=self._verify,
+                headers=self._headers,
+                json={'data': symbols_to_remove},
+            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+        return result    
 
     @_ensure_connected
     def get_vector(self, vector_name: str, nodes: List = None) -> Union[dict, Dict[Any, Dict[str, Any]]]:
         """Return the vector with *vector_name* on *nodes* (it will be present on at most one).
         
             Example:
                 .. code-block:: python
@@ -764,14 +1055,42 @@
 
                 # will disable prediction generation on node P1
                 agent.stop_predicting(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'predicting/stop', nodes=nodes)
+    
+    def start_autolearning(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+        """Tells *nodes* to start predicting.
+
+            Example:
+                .. code-block:: python
+
+                    # will enable prediction generation on node P1
+                    agent.start_predicting(nodes=["P1"])
+        """
+        if nodes is None:
+            nodes = self.all_nodes
+        return self._query(self.session.post, 'autolearning/start', nodes=nodes)
+
+    def stop_autolearning(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+        """Tells *nodes* to stop predicting.
+
+        Useful for faster training, but abstracted nodes will not learn.
+        
+        Example:
+            .. code-block:: python
+
+                # will disable prediction generation on node P1
+                agent.stop_predicting(nodes=["P1"])
+        """
+        if nodes is None:
+            nodes = self.all_nodes
+        return self._query(self.session.post, 'autolearning/stop', nodes=nodes)
 
     @_ensure_connected
     def ping(self, nodes: List = None) -> Union[dict, Any]:
         """Ping a node to ensure it's up.
         
             Example:
             
@@ -1003,17 +1322,35 @@
         if nodes is None:
             nodes = self.query_nodes
         return self._query(self.session.post, 'clear-target-class', nodes=nodes)
 
     @_ensure_connected
     def tf_attach(self, name, config):
         return self.session.post(f'{self._url}/thinkflux/{name}/attach', data={'config' : config})
-        
+    
+    @_ensure_connected    
+    def tf_remove(self, name):
+        return self.session.delete(f'{self._url}/thinkflux/{name}/remove')
+    
     @_ensure_connected
-    def investigate_record(self, node, record):
+    def tf_list(self):
+        return self.session.get(f'{self._url}/thinkflux/list')
+    
+    @_ensure_connected
+    def investigate_record(self, node, record: str) -> dict:
+        """Function for drilling down on a model recursively in a multi-node agent. Will retrieve all data "under"
+        the abstracted model, giving a complete representation of the abstracted model
+
+        Args:
+            node (list or str): the node to start at/containing the model provided in `record`: e.g. ['P4'] or 'P4'
+            record (str): the model to search for
+
+        Returns:
+            dict: recursive structure containing a complete representation of the abstracted model
+        """
         data = {}
         try: 
             if isinstance(node, list):
                 node = node[0]
             try:
                 # if the node passed is a primitive_id, get the name (P1, P2, etc.) of the node
                 node = self.genome.primitives[node]['name']
@@ -1023,15 +1360,31 @@
             return self.__get_model_details(model=record, node=[node], topLevel=True)
 
         except Exception as e:
             print(str(e))
         return data
 
     @_ensure_connected
-    def investigate(self, record):
+    def investigate(self, record: str) -> dict:
+        """Higher level implementation of :func:`investigate_record` that does not require a node to be entered.
+        Operates on abstracted symbols, models, etc. Useful when applying in a programatic manner, where the node
+        a symbol comes from is unknown. May throw exception if unable to identify a starting point.
+        
+        Args:
+            record (str): the symbol to look for
+
+        Returns:
+            dict: recursive structure containing a complete representation of the abstracted model
+            
+        Example:
+            .. code-block:: python
+            
+                record = 'PRIMITIVE|p124b23f9|004da01b0ef40d7c3e0965a6b4fd0f413672fbff|matches|KEY|VALUE'
+                traceback = agent.investigate(record=record)
+        """
         try:
 
             split_record = str(record).split('|')
             if split_record[0] == 'PRIMITIVE':
                 if len(split_record) < 3:
                     raise Exception(f'Investigate does not know what to do with symbol: {record}')
                     
@@ -1159,10 +1512,8 @@
                     unique_subitems.append(subitem)
             
             record_data["subitems"] = tuple(unique_subitems)
         else:
             record_data['bottomLevel'] = True
 
         
-        return record_data
-    
-__all__ = ("AgentConnectionError", "AgentClient", "AgentQueryError")
+        return record_data
```

### Comparing `ia-sdk-0.3.8/ia/gaius/back_testing.py` & `ia-sdk-0.3.9/ia/gaius/back_testing.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/data_language.py` & `ia-sdk-0.3.9/ia/gaius/data_language.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/data_ops.py` & `ia-sdk-0.3.9/ia/gaius/data_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,21 @@
         self._mongo_dataset_details['files'] = [item for item in dataset['dataset']['files']]
         
         
         self.train_sequences = []
         self.test_sequences = []
 
     def prep(self, percent_of_dataset_chosen:float, percent_reserved_for_training:float, shuffle:bool=False):
+        """Prepare the dataset
+
+        Args:
+            percent_of_dataset_chosen (float): The percent of the dataset to utilize
+            percent_reserved_for_training (float): The training/testing split for the dataset (e.g. set to 80 for 80/20 trianing/testing split)
+            shuffle (bool, optional): Whether to shuffle the data. Defaults to False.
+        """
         data = [MongoDataRecords(deepcopy(self._mongo_dataset_details['files']), percent_of_dataset_chosen, percent_reserved_for_training, shuffle)]
 
         self.train_sequences = []
         self.test_sequences = []
         for d in data:
             self.train_sequences += d.train_sequences
             self.test_sequences += d.test_sequences
@@ -299,14 +306,22 @@
             lines = io.StringIO(record.decode('utf-8'))
             sequence = (tuple([json.loads(line.strip()) for line in lines]))
             return sequence
         except Exception as e:
             print(f'failed to retrieve record as StringIO: {e}')
         
     def getSequence(self, record):
+        """Wrapper function to retrieve a record from MongoDB and convert it into a sequence
+
+        Args:
+            record (ObjectId): The MongoDB ObjectId of the data record to retrieve
+
+        Returns:
+            list: GDF sequence retrieved from MongoDB
+        """
         return self.convertBinaryStringtoSequence(self.retrieveDataRecord(record))
     
     def setIterMode(self, mode:str):
         """Set mode to be used for iterating across dataset
 
         Args:
             mode (str): set to "training" or "testing" depending on what set of sequences is to be iterated across
@@ -391,14 +406,23 @@
         """
         self.result_obj.update({'testing_logs': [],
                                 'training_logs': [],
                                 'start_time_utc' : str(datetime.datetime.utcnow())})
         return
     
     def addLogRecord(self, type:str, record:dict):
+        """Called during the testing loop to insert a pvt status record into MongoDB
+
+        Args:
+            type (str): Whether the record should be appended to the training or testing logs
+            record (dict): the record to insert
+
+        Raises:
+            Exception: Thrown if the type provided is not supported
+        """
         
         record_id = self.log_collection.insert_one(record).inserted_id
         if type == 'training':
             self.result_obj['training_logs'].append(record_id)
         elif type == 'testing':
             self.result_obj['testing_logs'].append(record_id)
         else:
@@ -425,14 +449,19 @@
         self.result_obj['final_results'] = final_results
         print(f'{self.result_obj = }')
         result_id = self.result_collection.insert_one(self.result_obj).inserted_id
         print(f'saved test results in {self.result_collection_name} as id: {result_id}')
         return str(result_id)
     
     def deleteResults(self):
+        """Function used to remediate database in the event of a failed/aborted test
+
+        Returns:
+            dict: dict showing the deleted result record, if any
+        """
         try:
             delete_result = self.result_collection.find_one_and_delete({'user_id': self.result_obj['user_id'],
                                                             'dataset_id': self.result_obj['dataset_id'],
                                                             'test_id': self.result_obj['test_id'],
                                                             'start_time_utc': self.result_obj['start_time_utc']
                                                             }, {'_id': False})
             # print(f'deleted_count = {delete_result}')
```

### Comparing `ia-sdk-0.3.8/ia/gaius/genome_info.py` & `ia-sdk-0.3.9/ia/gaius/genome_info.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/kb_ops.py` & `ia-sdk-0.3.9/ia/gaius/kb_ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -77,49 +77,90 @@
         print(f'Error in list_symbols: {e}')
         raise e
     finally:    
         agent.set_summarize_for_single_node(prev_summarize_state)
     
     return symbols_dict
 
-# def identify_models_with_symbol(agent: AgentClient, symbol:str, nodes=None):
-#     """Return a list of models containing `symbol` from each node in `nodes`. Store as a dict of {node_name : list}
+def get_models_containing_symbol(agent: AgentClient, symbol_set:set, nodes=None):
+    """Checks for presence of symbols from `symbol_set` in each model on `nodes`, adding to return dict if a symbol is found.
+    
+    Args:
+        agent (AgentClient): GAIuS Agent
+        symbol (str): the symbol to search for
+        nodes (_type_, optional): nodes to search. Defaults to searching all nodes
+    """
 
-#     Args:
-#         agent (AgentClient): GAIuS Agent
-#         symbol (str): the symbol to search for
-#         nodes (_type_, optional): _description_. Defaults to None.
-#     """
-
-#     if not agent._connected:
-#         agent.connect()
-    
-#     sym_dict = {}
-#     prev_summarize_state = agent.summarize_for_single_node
-#     try:
-#         agent.set_summarize_for_single_node(False)
-#         kb = agent.get_kbs_as_json(nodes=nodes, ids=False, obj=True)
+    if not agent._connected:
+        agent.connect()
+    
+    sym_dict = {}
+    prev_summarize_state = agent.summarize_for_single_node
+    try:
+        agent.set_summarize_for_single_node(False)
+        kb = agent.get_kbs_as_json(nodes=nodes, ids=False, obj=True)
         
-#         for node, node_kb in kb.items():
-#             sym_dict[node] = []
-#             for model in node_kb['models_kb']:
-#                 unique_symbols_in_model = set()
-#                 for event in node_kb[node]["models_kb"][model]['sequence']:
-#                     for sym in event:
-#                         unique_symbols_in_model.add(sym)
-#                 if symbol in unique_symbols_in_model:
-#                     sym_dict[node].append(node_kb[node]["models_kb"][model]['name'])
+        for node, node_kb in kb.items():
+            sym_dict[node] = set()
+            if 'models_kb' not in node_kb:
+                continue
+            for model_name, model in node_kb['models_kb'].values():
+                for event in model['sequence']:
+                    for sym in event:
+                        if sym in symbol_set:
+                            sym_dict[node].add(model_name)
+            
+    except Exception as e:
+        print(f'Error in identify_models_with_symbol: {e}')
+        raise e
+    finally:    
+        agent.set_summarize_for_single_node(prev_summarize_state)
+    
+    return sym_dict
+
+def get_models_containing_symbol_strict(agent: AgentClient, symbol_set:set, nodes=None):
+    """Checks for presence of symbols from `symbol_set` in each model on `nodes`. 
+    Only adds model to return dict if all symbols in model are from symbol set
+    Store as a dict of {node_name : list}
+    
+    Args:
+        agent (AgentClient): GAIuS Agent
+        symbol (str): the symbol to search for
+        nodes (_type_, optional): nodes to search. Defaults to searching all nodes
+    """
+
+    if not agent._connected:
+        agent.connect()
+    
+    sym_dict = {}
+    prev_summarize_state = agent.summarize_for_single_node
+    try:
+        agent.set_summarize_for_single_node(False)
+        kb = agent.get_kbs_as_json(nodes=nodes, ids=False, obj=True)
         
-#     except Exception as e:
-#         print(f'Error in identify_models_with_symbol: {e}')
-#         raise e
-#     finally:    
-#         agent.set_summarize_for_single_node(prev_summarize_state)
+        for node, node_kb in kb.items():
+            sym_dict[node] = set()
+            if 'models_kb' not in node_kb:
+                continue
+            for model_name, model in node_kb['models_kb'].values():
+                unique_symbols_in_model = set()
+                for event in model['sequence']:
+                    for sym in event:
+                        unique_symbols_in_model.add(sym)
+                        
+                if all([sym in symbol_set for sym in unique_symbols_in_model]):
+                    sym_dict[node].add(model_name)
+            
+    except Exception as e:
+        print(f'Error in identify_models_with_symbol: {e}')
+        raise e
+    finally:    
+        agent.set_summarize_for_single_node(prev_summarize_state)
     
-#     return 
+    return sym_dict
 
 def get_kb_subset(agent: AgentClient, model_dict: dict):
     """Retrieve a subset of a Knowledgebase based on the provided model_dict. 
     Will only provide used symbols and vectors, all others will be trimmed.
 
     Args:
         agent (AgentClient): GAIuS Agent
```

### Comparing `ia-sdk-0.3.8/ia/gaius/prediction_models.py` & `ia-sdk-0.3.9/ia/gaius/prediction_models.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/pvt.py` & `ia-sdk-0.3.9/ia/gaius/pvt.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,28 +176,41 @@
             self.prepare_datasets()
             
             if self.sio:
                 self.sio.emit('pvt_status', 
                               PVTMessage(status='training', current_record=0, total_record_count=len(self.dataset.train_sequences), 
                                        metrics={}, cur_test_num=self.test_num, total_test_num=self.num_of_tests, 
                                        test_id=self.test_id, user_id=self.user_id, test_type=self.test_type).toJSON(), to=self.user_id)
-            self.train_agent()
-            
-            self.testing_log.append([])
+            try:
+                
+                self.train_agent()
+                
+                self.testing_log.append([])
 
-            self.test_agent()
+                self.test_agent()
+                
+                for k, labels in self.labels_set.items():
+                    self.labels_set[k] = set([label.rsplit('|', maxsplit=1)[-1] for label in labels])
+                print('Getting Classification Metrics...')
+                self.get_classification_metrics()
+                print('Saving results to pvt_results...')
+                self.pvt_results[f'test_num_{test_num}_metrics'] = self.class_metrics_data_structures
+                self.pvt_results[f'test_num_{test_num}_metrics'] = self.update_test_results_w_hive_classification_metrics(self.pvt_results[f'test_num_{test_num}_metrics'])
             
-            for k, labels in self.labels_set.items():
-                self.labels_set[k] = set([label.rsplit('|', maxsplit=1)[-1] for label in labels])
-            print('Getting Classification Metrics...')
-            self.get_classification_metrics()
-            print('Saving results to pvt_results...')
-            self.pvt_results[f'test_num_{test_num}_metrics'] = self.class_metrics_data_structures
-            self.pvt_results[f'test_num_{test_num}_metrics'] = self.update_test_results_w_hive_classification_metrics(self.pvt_results[f'test_num_{test_num}_metrics'])
+            except Exception as e:
+                print(f'error during training/testing phase of test, remediating database for failed test, then raising error')
+                if self.mongo_results:
+                    print(f'about to remediate database')
+                    self.mongo_results.deleteResults()
+                    print(f'remediated database')
+                
+                print(f'raising error {str(e)}')
+                raise e
 
+                
             try:
                 print('Plotting Results...')
                 plot_confusion_matrix(test_num=test_num, class_metrics_data_structures=self.class_metrics_data_structures)
             except Exception as e:
                 print(f'error plotting results from classification pvt: {e}')
                 pass
                 
@@ -602,21 +615,48 @@
         if 'running_accuracy' not in test_step_info:
             test_step_info['running_accuracy'] = {}
             for k in test_step_info['predicted'].keys():
                 if test_step_info['predicted'][k] in test_step_info['actual']:
                     test_step_info['running_accuracy'][k] = 1.0
                 else:
                     test_step_info['running_accuracy'][k] = 0.0
+            
+            test_step_info['response_percentage'] = {}
+            test_step_info['response_counts'] = {}
+            test_step_info['running_precisions'] = {}
+            for k in test_step_info['predicted'].keys():
+                if test_step_info['predicted'][k] != 'i_dont_know':
+                    test_step_info['response_percentage'][k] = 1.0
+                    test_step_info['response_counts'][k] = 1
+                    test_step_info['running_precisions'][k] = test_step_info['running_accuracy'][k]
+                else:
+                    test_step_info['response_percentage'][k] = 0.0
+                    test_step_info['running_precisions'][k] = 1.0
+                    test_step_info['response_counts'][k] = 0
+                    
+                
         else:
             # print(f'{test_step_info["running_accuracy"]=}, {idx=}')
             for k in test_step_info['predicted'].keys():
+                if test_step_info['predicted'][k] != 'i_dont_know':
+                    test_step_info['response_counts'][k] += 1
+                    test_step_info['response_percentage'][k] = (test_step_info['response_percentage'][k]*(idx) + 1 )/(idx+1)
+                else:
+                    test_step_info['response_percentage'][k] = (test_step_info['response_percentage'][k]*(idx))/(idx+1)
+                
+                # TODO: Add precision calculation in here
+                
                 if test_step_info['predicted'][k] in test_step_info['actual']:
                     test_step_info['running_accuracy'][k] = (test_step_info['running_accuracy'][k]*(idx) + 1)/(idx+1)
                 else:
                     test_step_info['running_accuracy'][k] = (test_step_info['running_accuracy'][k]*(idx))/(idx+1)
+                
+                    test_step_info['running_precisions'][k] = (test_step_info['running_accuracy'][k] * idx+1) / test_step_info['response_counts'][k]
+                
+                
         return test_step_info
     
     def get_emotives_value_metrics(self):
         """
         Builds emotives value data structures for each node
         """                         
         # Build an emotives Metric Data Structure
@@ -780,45 +820,52 @@
         pvt_test_result['hive'] = hive_metrics
         
         pvt_test_result['hive']['labels'] = hive_label_set_lst
 
 
         # get predictions to get hive classification of all nodes
         for i in range(0, len(self.predictions)):
-            pvt_test_result['hive']['predictions'].append(hive_model_classification(ensembles=self.predictions[i]))
+            pred = hive_model_classification(ensembles=self.predictions[i])
+            if pred is None:
+                pred = 'i_dont_know'
+            pvt_test_result['hive']['predictions'].append(deepcopy(pred))
 
         # get actuals of test   
         for i in range(0, len(self.actuals)):
             pvt_test_result['hive']['actuals'].append(self.actuals[i][0])
 
+
         # get hive accuracy of test
         for node_name, test_data in pvt_test_result.items(): 
             if node_name == 'hive':
                 try:
-                    hive_accuracy = round(accuracy_score(test_data['actuals'],test_data['predictions']),2)*100
+                    # print(f'{test_data["actuals"]=}, {test_data["predictions"]=}')
+                    # print(f'{copy_hive_preds=}')
+                    hive_accuracy = round(accuracy_score(test_data['actuals'],test_data["predictions"]),2)*100
                 except ZeroDivisionError:
                     hive_accuracy = 0.0
         pvt_test_result['hive']['metrics']['accuracy'] = hive_accuracy
 
         # get hive precision of test            
-        for node_name, test_data in pvt_test_result.items(): 
+        for node_name, test_data in pvt_test_result.items():                     
             if node_name == 'hive':
-                prec_predictions       = [p for p, a in zip(test_data['predictions'], test_data['actuals']) if p != 'i_dont_know']
-                prec_answers           = [a for p, a in zip(test_data['predictions'], test_data['actuals']) if p != 'i_dont_know']
+                
+                prec_predictions       = [p for p, a in zip(test_data["predictions"], test_data['actuals']) if p != 'i_dont_know']
+                prec_answers           = [a for p, a in zip(test_data["predictions"], test_data['actuals']) if p != 'i_dont_know']
                 try:
                     hive_precision = round(accuracy_score(prec_answers,prec_predictions),2)*100
                 except ZeroDivisionError:
                     hive_precision = 0.0
         pvt_test_result['hive']['metrics']['precision'] = hive_precision
 
         # get hive response rate percentage of test
         for node_name, test_data in pvt_test_result.items(): 
             if node_name == 'hive':
                 total_amount_of_questions            = len(test_data['actuals'])
-                updated_pred_length                  = len([p for p in test_data['predictions'] if p != 'i_dont_know'])
+                updated_pred_length                  = len([p for p in test_data["predictions"] if p != 'i_dont_know'])
                 try:
                     hive_resp_pc = np.round(updated_pred_length/total_amount_of_questions, 2)*100
                 except ZeroDivisionError:
                     hive_resp_pc = 0.0
         pvt_test_result['hive']['metrics']['resp_pc'] = hive_resp_pc
 
         # self.pvt_test_result
```

### Comparing `ia-sdk-0.3.8/ia/gaius/tests/classification.py` & `ia-sdk-0.3.9/ia/gaius/tests/classification.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/tests/pvt_utils.py` & `ia-sdk-0.3.9/ia/gaius/tests/pvt_utils.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/tests/utility.py` & `ia-sdk-0.3.9/ia/gaius/tests/utility.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/ia/gaius/utils.py` & `ia-sdk-0.3.9/ia/gaius/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -99,36 +99,60 @@
         progress.bar_style = 'success'
         progress.value = index
         label.value = "{name}: {index}".format(
             name=name,
             index=str(index or '?')
         )
 
-def abstract_names(ensemble):
+def abstract_names(ensemble: list) -> list:
+    """Get a set of model names from a prediction ensemble
+
+    Args:
+        ensemble (list): a prediction ensemble
+
+    Returns:
+        list: list of models from predictions in the prediction ensemble
+        
+    Example:
+    
+        .. code-block:: python
+        
+            from ia.gaius.agent_client import AgentClient
+            from ia.gaius.utils import abstract_names
+            ...
+            agent = AgentClient(agent_info)
+            agent.connect()
+            ...
+            ensemble = agent.get_predictions(nodes=['P1'])
+            models = abstract_names(ensemble)
+            
+    """
     return list(set([pred['name'] for pred in ensemble]))
 
-def write_gdf_to_file(directory_name, filename, sequence):
+def write_gdf_to_file(directory_name : str, filename: str, sequence: list) -> str:
     """Write a GDF sequence to a file
     
     Args:
         directory_name (str, required): directory to save GDFs to
         filename (str, required): filename to save to
         sequence (list, required): list of individual GDF events, making up a sequence
         
     Example:
         .. code-block:: python
 
             from ia.gaius.utils import write_gdf_to_file, create_gdf
-            
             sequence = [create_gdf(strings=["hello"]), create_gdf(strings=["world"])]
             filename = 'hello_world'
             directory_name = '/example/dir'
-            
             write_gdf_to_file(directory_name, filename, sequence)
     
+    .. warning::
+        Will overwrite the file at ``<directory_name>/<filename>``. Please ensure it is acceptable to do so.
+        No safety checks are performed in this function
+    
     """
     gdf_file_path = os.path.join(directory_name, filename) 
     with open(gdf_file_path, 'w') as f:
         for event_idx, event in enumerate(sequence):
             json.dump(event,f)
             if event_idx != len(sequence) - 1:
                 f.write('\n')
```

### Comparing `ia-sdk-0.3.8/ia_sdk.egg-info/PKG-INFO` & `ia-sdk-0.3.9/ia_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: SDK for Intelligent Artifact's GAIuS agents.
 Home-page: https://intelligent-artifacts.com
 Author: Intelligent Artifacts
 Author-email: support@intelligent-artifacts.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ia-sdk-0.3.8/ia_sdk.egg-info/SOURCES.txt` & `ia-sdk-0.3.9/ia_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.8/setup.py` & `ia-sdk-0.3.9/setup.py`

 * *Files identical despite different names*

