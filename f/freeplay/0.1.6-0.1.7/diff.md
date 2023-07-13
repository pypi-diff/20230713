# Comparing `tmp/freeplay-0.1.6.tar.gz` & `tmp/freeplay-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.6.tar", max compression
+gzip compressed data, was "freeplay-0.1.7.tar", max compression
```

## Comparing `freeplay-0.1.6.tar` & `freeplay-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.6/README.md
--rw-r--r--   0        0        0       61 2023-06-29 11:36:19.640171 freeplay-0.1.6/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.6/freeplay/api_support.py
--rw-r--r--   0        0        0      802 2023-07-05 20:48:51.495916 freeplay-0.1.6/freeplay/completions.py
--rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.6/freeplay/errors.py
--rw-r--r--   0        0        0     8833 2023-07-11 19:42:05.561871 freeplay-0.1.6/freeplay/flavors.py
--rw-r--r--   0        0        0    22477 2023-07-11 19:42:05.562783 freeplay-0.1.6/freeplay/freeplay.py
--rw-r--r--   0        0        0      828 2023-06-27 18:52:46.171090 freeplay-0.1.6/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      391 2023-07-11 19:42:28.993845 freeplay-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.1.7/README.md
+-rw-r--r--   0        0        0       61 2023-06-28 22:11:30.981007 freeplay-0.1.7/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.1.7/freeplay/api_support.py
+-rw-r--r--   0        0        0      802 2023-07-13 15:23:08.878478 freeplay-0.1.7/freeplay/completions.py
+-rw-r--r--   0        0        0      188 2023-07-11 16:57:31.087747 freeplay-0.1.7/freeplay/errors.py
+-rw-r--r--   0        0        0     8971 2023-07-13 15:23:08.879014 freeplay-0.1.7/freeplay/flavors.py
+-rw-r--r--   0        0        0    22477 2023-07-13 15:23:08.879647 freeplay-0.1.7/freeplay/freeplay.py
+-rw-r--r--   0        0        0      828 2023-07-12 17:07:23.373407 freeplay-0.1.7/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      369 2023-07-12 17:52:35.686687 freeplay-0.1.7/freeplay/utils.py
+-rw-r--r--   0        0        0      391 2023-07-13 15:23:21.748924 freeplay-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.7/PKG-INFO
```

### Comparing `freeplay-0.1.6/freeplay/api_support.py` & `freeplay-0.1.7/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.6/freeplay/completions.py` & `freeplay-0.1.7/freeplay/completions.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.6/freeplay/flavors.py` & `freeplay-0.1.7/freeplay/flavors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import anthropic  # type: ignore
 import openai
 
 from .completions import CompletionChunk, PromptTemplateWithMetadata, CompletionResponse, ChatCompletionResponse, \
     ChatMessage
 from .errors import APIKeyMissingError
 from .llm_parameters import LLMParameters
+from .utils import format_template_variables
 
 
 class Flavor(ABC):
     @property
     @abstractmethod
     def record_format_type(self) -> str:
         raise NotImplementedError()
@@ -75,15 +76,15 @@
         "model": "text-davinci-003"
     })
 
     def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
         super().__init__(openai_api_key, openai_api_base)
 
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
-        return prompt_template.content.format(**variables)
+        return format_template_variables(prompt_template.content, variables)
 
     def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
         completion = openai.Completion.create(
             prompt=formatted_prompt,
             **self.get_model_params(llm_parameters)
         )  # type: ignore
         return CompletionResponse(
@@ -117,18 +118,19 @@
 
     def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
         super().__init__(openai_api_key, openai_api_base)
 
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         # Extract messages JSON to enable formatting of individual content fields of each message. If we do not
         # extract the JSON, current variable interpolation will fail on JSON curly braces.
-        messages_as_json = json.loads(prompt_template.content)
+        messages_as_json: list[dict[str,str]] = json.loads(prompt_template.content)
         formatted_messages = [
-            {"content": message['content'].format(**variables), "role": message['role']} for message in
-            messages_as_json]
+            {
+                "content": format_template_variables(message['content'], variables), "role": message['role']
+            } for message in messages_as_json]
         return json.dumps(formatted_messages)
 
     def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
         messages = json.loads(formatted_prompt)
         completion = self.__call_openai(messages, llm_parameters, stream=False)
         return CompletionResponse(
             content=completion.choices[0].message.content,
@@ -186,15 +188,15 @@
         "max_tokens_to_sample": 100
     })
 
     def __init__(self, anthropic_api_key: str):
         self.client = anthropic.Client(anthropic_api_key)
 
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
-        interpolated_prompt = prompt_template.content.format(**variables)
+        interpolated_prompt = format_template_variables(prompt_template.content, variables)
         # Anthropic expects a specific Chat format "Human: $PROMPT_TEXT\n\nAssistant:". We add the wrapping for Text.
         chat_formatted_prompt = f"{anthropic.HUMAN_PROMPT} {interpolated_prompt} {anthropic.AI_PROMPT}"
         return chat_formatted_prompt
 
     def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
         anthropic_response = self.client.completion(
             prompt=formatted_prompt,
```

### Comparing `freeplay-0.1.6/freeplay/freeplay.py` & `freeplay-0.1.7/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.6/freeplay/llm_parameters.py` & `freeplay-0.1.7/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.6/PKG-INFO` & `freeplay-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

