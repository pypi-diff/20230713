# Comparing `tmp/lemonai-0.0.9.tar.gz` & `tmp/lemonai-0.1.0.tar.gz`

## Comparing `lemonai-0.0.9.tar` & `lemonai-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.0.9/heatmap-example.gif
--rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.0.9/heatmap-example.png
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 lemonai-0.0.9/test.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lemonai-0.0.9/.vscode/launch.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.0.9/.vscode/settings.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.0.9/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.9/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.9/LICENSE
--rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 lemonai-0.0.9/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 lemonai-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.0/heatmap-example.gif
+-rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.0/heatmap-example.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lemonai-0.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.0/docs/tools.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.0/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.0/LICENSE
+-rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 lemonai-0.1.0/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 lemonai-0.1.0/PKG-INFO
```

### Comparing `lemonai-0.0.9/heatmap-example.gif` & `lemonai-0.1.0/heatmap-example.gif`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/heatmap-example.png` & `lemonai-0.1.0/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/src/lemonai/api_wrapper.py` & `lemonai-0.1.0/src/lemonai/api_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import json
 import requests
 from requests import Request, Session
 from typing import List, Dict, Optional
 
-class APIWrapper():
+class APIWrapper:
+
+    api_base_url: str
+
+    def __init__(self, api_domain: Optional[str] = None):
+        self.api_base_url = f"{api_domain if api_domain else 'https://bfyvsp3cwepesc7dxd2yuzkyyi0nmcye.lambda-url.eu-central-1.on.aws'}/api/v0"
 
-    api_base_url: str = "http://localhost:1313/api/v0/"
 
     def _get_session(self) -> Session:
         
         session = requests.session()
         session.headers.update(
             {
                 "Accept": "application/json",
@@ -18,15 +22,15 @@
         )
 
         return session
 
     def get_tool_list(self) -> List[Dict]:
 
         session = self._get_session()
-        url = f"{self.api_base_url}tools"
+        url = f"{self.api_base_url}/tools"
         response = session.get(url)
         response.raise_for_status()
 
         return response.json()
     
     def _get_action_request(
         self, id: str, action_input: str, params: Optional[Dict]
@@ -37,15 +41,15 @@
             action_input = action_input + "\"\""
         json_obj = json.loads(action_input.replace("'", "\"").replace("None", "\"\""))
 
         data.update(json_obj)
 
         return Request(
             method="POST",
-            url=f"{self.api_base_url}tool/{id}/execute",
+            url=f"{self.api_base_url}/tool/{id}/execute",
             json=data,
         )
 
     def run(self, id: str, action_input: str, params: Optional[Dict], api_key: Optional[str], access_token: Optional[str]) -> Dict:
         
         session = self._get_session()
         request = self._get_action_request(id, action_input, params)
```

### Comparing `lemonai-0.0.9/src/lemonai/execute_workflow.py` & `lemonai-0.1.0/src/lemonai/execute_workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from loguru import logger
 from langchain.llms.base import BaseLLM
 from langchain.agents import initialize_agent, AgentType
 from lemonai.get_integrations import get_apis_from_env
 from lemonai.api_wrapper import APIWrapper
 from lemonai.toolkit import Toolkit
 from lemonai.filter_tools import filter_tools
+from typing import Optional
 
-def execute_workflow(llm: BaseLLM, prompt_string: str):
+
+def execute_workflow(llm: BaseLLM, prompt_string: str, api_domain: Optional[str] = None):
 
     logfile_path = "lemonai.log"
     logger.remove(handler_id=None)
     logger.add(logfile_path, format="{time} - {extra[session_id]} - {extra[operation_name]}")
 
     api_keys_dict, access_tokens_dict = get_apis_from_env()
     session_id = uuid.uuid4()
 
-    _wrapper = APIWrapper()
+    _wrapper = APIWrapper(api_domain)
     toolkit = Toolkit.from_api_wrapper(_wrapper, api_keys_dict, access_tokens_dict, logger, str(session_id))
     tools = toolkit.get_tools()
 
     prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Give your action input as a valid JSON object where the keys are the params and the values are the value for each input parameter. The description of the tool may provide the JSON structure of the action input using round brackets () instead of curly brackets. Follow this structure for your action input. Your final answer should give a brief conversational overview of what you did."    
     filtered_tools = filter_tools(llm=llm, task=prompt_string, tools=tools)
     
     agent = initialize_agent(
```

### Comparing `lemonai-0.0.9/src/lemonai/filter_tools.py` & `lemonai-0.1.0/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/src/lemonai/get_integrations.py` & `lemonai-0.1.0/src/lemonai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/src/lemonai/tool.py` & `lemonai-0.1.0/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/src/lemonai/toolkit.py` & `lemonai-0.1.0/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/.gitignore` & `lemonai-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.9/pyproject.toml` & `lemonai-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

