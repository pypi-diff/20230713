# Comparing `tmp/autopack_tools-0.2.7.tar.gz` & `tmp/autopack_tools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.7.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.8.tar", max compression
```

## Comparing `autopack_tools-0.2.7.tar` & `autopack_tools-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.7/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.7/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.7/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.7/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.7/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.7/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.7/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.7/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.7/autopack/get_pack.py
--rw-r--r--   0        0        0     3804 2023-07-10 00:05:37.324848 autopack_tools-0.2.7/autopack/installation.py
--rw-r--r--   0        0        0     2976 2023-07-10 03:48:17.484061 autopack_tools-0.2.7/autopack/pack.py
--rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.7/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.7/autopack/search.py
--rw-r--r--   0        0        0     2947 2023-07-10 00:06:33.061394 autopack_tools-0.2.7/autopack/selection.py
--rw-r--r--   0        0        0     3874 2023-07-10 18:46:01.025051 autopack_tools-0.2.7/autopack/utils.py
--rw-r--r--   0        0        0      911 2023-07-11 22:39:45.294645 autopack_tools-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.8/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.8/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.8/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.8/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.8/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.8/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.8/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.8/autopack/get_pack.py
+-rw-r--r--   0        0        0     3804 2023-07-12 23:56:33.101607 autopack_tools-0.2.8/autopack/installation.py
+-rw-r--r--   0        0        0     2976 2023-07-10 03:48:17.484061 autopack_tools-0.2.8/autopack/pack.py
+-rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.8/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.8/autopack/search.py
+-rw-r--r--   0        0        0     2625 2023-07-12 23:24:57.527362 autopack_tools-0.2.8/autopack/selection.py
+-rw-r--r--   0        0        0     3874 2023-07-12 23:56:37.571529 autopack_tools-0.2.8/autopack/utils.py
+-rw-r--r--   0        0        0     1005 2023-07-12 23:57:13.494760 autopack_tools-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.8/PKG-INFO
```

### Comparing `autopack_tools-0.2.7/LICENSE` & `autopack_tools-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/README.md` & `autopack_tools-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/api.py` & `autopack_tools-0.2.8/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/cli.py` & `autopack_tools-0.2.8/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/get_pack.py` & `autopack_tools-0.2.8/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/installation.py` & `autopack_tools-0.2.8/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/pack.py` & `autopack_tools-0.2.8/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/pack_response.py` & `autopack_tools-0.2.8/autopack/pack_response.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/autopack/selection.py` & `autopack_tools-0.2.8/autopack/selection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 import json
 
 from langchain.chat_models.base import BaseChatModel
-from langchain.schema import SystemMessage
+from langchain.schema import SystemMessage, BaseMessage
 
 from autopack.api import pack_search
 
-TOOL_SELECTION_PROMPT_TEMPLATE = """You are an autonomous AI Assistant named AutoPack. AutoPack works on behalf of another AI Assistant who will be completing tasks. AutoPack is excellent at choosing the right tools for the task. Keeping a small tool set is important, so AutoPack aims to include only the tools that are required. AutoPack has access to the following tools:
---- TOOLS ---
+TOOL_SELECTION_PROMPT_TEMPLATE = """Given the task and the tool list provided below, please return a JSON object identifying which tools would be most suitable for completing the task, along with reasons for each choice. The response should only include the JSON object, without any additional explanatory text.
+
+Please provide the recommended tools in the following format:
+{{"tools": [{{"tool_id": tool_id, "reason": reason_for_recommending }}]}}
+
+Task: {user_input}
+
+Tools List (in JSON format):
 {tools_string}
---- END TOOLS ---
-Respond with the following JSON structure:
---- FORMAT INSTRUCTIONS ---
-```json
-{{"tools": [{{ "tool_id": tool_id, "reason": reason_for_recommending }}] }}
-```
-For example, if you think tool #1234 might be necessary:
-```json
-{{'tools': [{{ "tool_id": 1234, "reason": "The breathe tool might be necessary because the user needs oxygen"}}]}}
-```
---- END FORMAT INSTRUCTIONS ---
----- TASK ----
-{user_input}
---- END TASK ---
-Given the TASK, return all of the tools that are necessary to complete the task.
-Begin!"""
+"""
 
 
 def select_packs(task_description: str, llm: BaseChatModel) -> list[str]:
     """Given a user input describing the task they wish to accomplish, return a list of Pack IDs that the given LLM
     thinks will be suitable for this task.
 
     This is good for a "pre-processing" step after receiving the task but before trying to solve it. This allows you
@@ -40,40 +31,40 @@
         llm (BaseChatModel): An LLM which will be used to evaluate the selection
 
     Returns:
         list[str]: A list of selected Pack IDs
     """
 
     packs = pack_search("")
-    pack_summaries = ""
+    pack_summaries = []
     for i, pack in enumerate(packs):
         # Use a number instead of a tool ID because the AI can mismatch tool names and repos
         pseudo_id = i + 1
-        pack_summaries += f"""--- TOOL #{pseudo_id} ---
-tool_id: {pseudo_id}
-name: "{pack.name}"
-description: "{pack.description}"
-arguments: "{pack.run_args}"
-"""
+        pack_summaries.append(
+            {"tool_id": pseudo_id, "name": pack.name, "description": pack.description, "arguments": pack.run_args}
+        )
 
-    prompt = TOOL_SELECTION_PROMPT_TEMPLATE.format(user_input=task_description, tools_string=pack_summaries)
+    prompt = TOOL_SELECTION_PROMPT_TEMPLATE.format(user_input=task_description, tools_string=json.dumps(pack_summaries))
 
     response = ask_llm(prompt, llm)
 
-    tools = json.loads(response.content)
     # TODO Handle json errors, perhaps a retry
+    try:
+        tools = json.loads(response.content)
+    except json.JSONDecodeError as e:
+        return []
 
     selected_packs = []
     for selected_tool in tools.get("tools"):
-        tool_index = selected_tool.get("tool_id")
+        tool_index = int(selected_tool.get("tool_id"))
         selected_packs.append(packs[tool_index - 1].pack_id)
 
     return selected_packs
 
 
-def ask_llm(prompt: str, llm: BaseChatModel) -> list[str]:
+def ask_llm(prompt: str, llm: BaseChatModel) -> BaseMessage:
     """Encapsulate the OpenAI specific stuff to easier support other frameworks in the future"""
     message = SystemMessage(content=prompt)
 
     response = llm(messages=[message])
 
     return response
```

### Comparing `autopack_tools-0.2.7/autopack/utils.py` & `autopack_tools-0.2.8/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.7/pyproject.toml` & `autopack_tools-0.2.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.2.7"
+version = "0.2.8"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
@@ -33,7 +33,16 @@
 types-psycopg2 = "^2.9.21.10"
 pipreqs = "^0.4.13"
 gitpython = "^3.1.31"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+line-length = 120
+
+[tool.black]
+line-length = 120
+
+[flake8]
+max-line-length = 120
```

### Comparing `autopack_tools-0.2.7/PKG-INFO` & `autopack_tools-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.7
+Version: 0.2.8
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

