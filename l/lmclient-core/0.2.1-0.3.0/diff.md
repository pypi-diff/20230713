# Comparing `tmp/lmclient-core-0.2.1.tar.gz` & `tmp/lmclient_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmclient-core-0.2.1.tar", max compression
+gzip compressed data, was "lmclient_core-0.3.0.tar", max compression
```

## Comparing `lmclient-core-0.2.1.tar` & `lmclient_core-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient-core-0.2.1/LICENSE
--rw-r--r--   0        0        0      966 2023-05-31 07:37:53.134651 lmclient-core-0.2.1/README.md
--rw-r--r--   0        0        0      187 2023-05-31 03:47:48.079921 lmclient-core-0.2.1/lmclient/__init__.py
--rw-r--r--   0        0        0     6248 2023-05-31 08:19:14.595390 lmclient-core-0.2.1/lmclient/client.py
--rw-r--r--   0        0        0      151 2023-05-31 03:48:41.450228 lmclient-core-0.2.1/lmclient/completions/__init__.py
--rw-r--r--   0        0        0     1421 2023-05-31 06:58:04.718510 lmclient-core-0.2.1/lmclient/completions/azure.py
--rw-r--r--   0        0        0     1223 2023-05-31 06:58:20.810104 lmclient-core-0.2.1/lmclient/completions/openai.py
--rw-r--r--   0        0        0      267 2023-05-31 07:11:15.090406 lmclient-core-0.2.1/lmclient/protocols.py
--rw-r--r--   0        0        0      690 2023-05-31 08:36:13.317730 lmclient-core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 lmclient-core-0.2.1/setup.py
--rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 lmclient-core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient_core-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3448 2023-07-13 11:01:26.959807 lmclient_core-0.3.0/README.md
+-rw-r--r--   0        0        0      212 2023-07-13 10:42:16.420929 lmclient_core-0.3.0/lmclient/__init__.py
+-rw-r--r--   0        0        0     6907 2023-07-13 10:55:54.493170 lmclient_core-0.3.0/lmclient/client.py
+-rw-r--r--   0        0        0      117 2023-07-13 09:49:59.136022 lmclient_core-0.3.0/lmclient/models/__init__.py
+-rw-r--r--   0        0        0     1516 2023-07-13 10:56:26.382623 lmclient_core-0.3.0/lmclient/models/azure.py
+-rw-r--r--   0        0        0     1328 2023-07-13 11:00:57.629913 lmclient_core-0.3.0/lmclient/models/openai.py
+-rw-r--r--   0        0        0      536 2023-07-13 10:42:15.726677 lmclient_core-0.3.0/lmclient/types.py
+-rw-r--r--   0        0        0      690 2023-07-13 10:56:45.780077 lmclient_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 lmclient_core-0.3.0/PKG-INFO
```

### Comparing `lmclient-core-0.2.1/LICENSE` & `lmclient_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmclient-core-0.2.1/lmclient/client.py` & `lmclient_core-0.3.0/lmclient/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
+import hashlib
 import time
 from enum import Enum
-from typing import ClassVar, Literal
+from typing import ClassVar, Sequence
 
 import anyio
 import asyncer
 import diskcache
 import tqdm
 
-from lmclient.protocols import CompletionModel
+from lmclient.types import ChatModel, Messages
 
 
 class ErrorMode(str, Enum):
     RAISE = 'raise'
     IGNORE = 'ignore'
 
 
@@ -21,44 +22,53 @@
     AUTO = 'auto'
     ALWAYS = 'always'
     NEVER = 'never'
 
 
 class LMClient:
     NUM_SECONDS_PER_MINUTE: ClassVar[int] = 60
-    PROGRESS_BAR_THRESHOLD: ClassVar[int] = 30
+    PROGRESS_BAR_THRESHOLD: ClassVar[int] = 20
 
     def __init__(
         self,
-        completion_model: CompletionModel,
+        model: ChatModel,
         max_requests_per_minute: int = 20,
         async_capacity: int = 3,
+        timeout: int | None = 20,
         error_mode: ErrorMode | str = ErrorMode.RAISE,
         cache_dir: str | None = None,
         progress_bar: ProgressBarMode | str = ProgressBarMode.AUTO,
     ):
-        self.completion_model = completion_model
+        self.completion_model = model
         self.async_capacity = async_capacity
         self.max_requests_per_minute = max_requests_per_minute
         self.error_mode = ErrorMode(error_mode)
         self.progress_bar_mode = ProgressBarMode(progress_bar)
         self._task_created_time_list: list[int] = []
         self.cache = diskcache.Cache(cache_dir) if cache_dir is not None else None
 
-    def run(self, prompts: list[str], **kwargs) -> list[str]:
+        if timeout is None:
+            default_kwargs = {}
+        else:
+            default_kwargs = {'request_timeout': timeout}
+        self.default_kwargs = default_kwargs
+
+    def run(self, prompts: Sequence[str | Messages], **kwargs) -> list[str]:
+        kwargs = {**self.default_kwargs, **kwargs}
         progress_bar = self._get_progress_bar(num_tasks=len(prompts))
         completions: list[str] = []
         for prompt in prompts:
             completion = self._run_single_task(prompt=prompt, progress_bar=progress_bar, **kwargs)
             completions.append(completion)
         progress_bar.close()
         return completions
 
     @asyncer.runnify
-    async def async_run(self, prompts: list[str], **kwargs) -> list[str]:
+    async def async_run(self, prompts: Sequence[str | Messages], **kwargs) -> list[str]:
+        kwargs = {**self.default_kwargs, **kwargs}
         limiter = anyio.CapacityLimiter(self.async_capacity)
         task_created_lock = anyio.Lock()
         progress_bar = self._get_progress_bar(num_tasks=len(prompts))
 
         soon_values: list[asyncer.SoonValue[str]] = []
         async with asyncer.create_task_group() as task_group:
             soon_func = task_group.soonify(self._async_run_single_task)
@@ -74,15 +84,15 @@
 
         progress_bar.close()
         values = [soon_value.value for soon_value in soon_values]
         return values
 
     async def _async_run_single_task(
         self,
-        prompt: str,
+        prompt: str | Messages,
         limiter: anyio.CapacityLimiter,
         task_created_lock: anyio.Lock,
         progress_bar: tqdm.tqdm,
         **kwargs,
     ) -> str:
         async with limiter:
             task_key = self._gen_task_key(prompt=prompt, **kwargs)
@@ -108,15 +118,15 @@
                     completion: str = f'Error: {e}'
                 else:
                     raise ValueError(f'Unknown error mode: {self.error_mode}')
 
             progress_bar.update(1)
             return completion
 
-    def _run_single_task(self, prompt: str, progress_bar: tqdm.tqdm, **kwargs) -> str:
+    def _run_single_task(self, prompt: str | Messages, progress_bar: tqdm.tqdm, **kwargs) -> str:
         task_key = self._gen_task_key(prompt=prompt, **kwargs)
         if self.cache is not None and task_key in self.cache:
             completion = self.cache[task_key]  # type: ignore
             progress_bar.update(1)
             return completion
 
         sleep_time = self._calculate_sleep_time()
@@ -149,18 +159,25 @@
         self._task_created_time_list = self._task_created_time_list[idx:]
 
         if len(self._task_created_time_list) < self.max_requests_per_minute:
             return 0
         else:
             return max(self.NUM_SECONDS_PER_MINUTE - int(current_time - self._task_created_time_list[0]) + 1, 0)
 
-    def _gen_task_key(self, prompt: str, **kwargs) -> str:
+    def _gen_task_key(self, prompt: str | Messages, **kwargs) -> str:
+        if not isinstance(prompt, str):
+            prompt = '---'.join([f'{message["role"]}={message["content"]}' for message in prompt])
         items = sorted([f'{key}={value}' for key, value in kwargs.items()])
         items = [prompt, self.completion_model.identifier] + items
-        return '---'.join(items)
+        task_string = '---'.join(items)
+        return self.md5_hash(task_string)
+
+    @staticmethod
+    def md5_hash(string: str):
+        return hashlib.md5(string.encode()).hexdigest()
 
     def _get_progress_bar(self, num_tasks: int) -> tqdm.tqdm:
         use_progress_bar = (self.progress_bar_mode is ProgressBarMode.ALWAYS) or (
             self.progress_bar_mode is ProgressBarMode.AUTO and num_tasks > self.PROGRESS_BAR_THRESHOLD
         )
         progress_bar = tqdm.tqdm(
             desc=f'{self.completion_model.__class__.__name__}', total=num_tasks, disable=not use_progress_bar
```

### Comparing `lmclient-core-0.2.1/lmclient/completions/azure.py` & `lmclient_core-0.3.0/lmclient/models/azure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
 import os
 
 import openai
 
-from lmclient.protocols import CompletionModel
+from lmclient.types import ChatModel, Message, Messages
 
 
-class AzureCompletion(CompletionModel):
+class AzureChat(ChatModel):
     def __init__(
         self,
         model: str | None = None,
         api_key: str | None = None,
         api_base: str | None = None,
         api_version: str | None = None,
     ):
         self.model = model or os.environ['AZURE_CHAT_API_ENGINE']
 
         openai.api_type = 'azure'
         openai.api_key = api_key or os.environ['AZURE_API_KEY']
         openai.api_base = api_base or os.environ['AZURE_API_BASE']
         openai.api_version = api_version or os.getenv('AZURE_API_VERSION') or '2023-05-15'
 
-    def complete(self, prompt: str, **kwargs) -> str:
-        messages = [{'role': 'user', 'content': prompt}]
-        response = openai.ChatCompletion.create(engine=self.model, messages=messages, **kwargs)
+    def complete(self, prompt: Messages | str, **kwargs) -> str:
+        if isinstance(prompt, str):
+            prompt = [Message(role='user', content=prompt)]
+
+        response = openai.ChatCompletion.create(engine=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
-    async def async_complete(self, prompt: str, **kwargs) -> str:
-        messages = [{'role': 'user', 'content': prompt}]
-        response = await openai.ChatCompletion.acreate(engine=self.model, messages=messages, **kwargs)
+    async def async_complete(self, prompt: Messages | str, **kwargs) -> str:
+        if isinstance(prompt, str):
+            prompt = [Message(role='user', content=prompt)]
+
+        response = await openai.ChatCompletion.acreate(engine=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
     @property
     def identifier(self) -> str:
         return f'{self.__class__.__name__}({self.model})'
```

### Comparing `lmclient-core-0.2.1/lmclient/completions/openai.py` & `lmclient_core-0.3.0/lmclient/models/openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from __future__ import annotations
 
 import os
 
 import openai
 
-from lmclient.protocols import CompletionModel
+from lmclient.types import ChatModel, Message, Messages
 
 
-class OpenAICompletion(CompletionModel):
+class OpenAIChat(ChatModel):
     def __init__(
         self,
-        model: str,
+        model_name: str,
         api_key: str | None = None,
     ):
-        self.model = model
+        self.model = model_name
 
         openai.api_type = 'open_ai'
         openai.api_base = 'https://api.openai.com/v1'
         openai.api_key = api_key or os.environ['OPENAI_API_KEY']
         openai.api_version = None
 
-    def complete(self, prompt: str, **kwargs) -> str:
-        messages = [{'role': 'user', 'content': prompt}]
-        response = openai.ChatCompletion.create(model=self.model, messages=messages, **kwargs)
+    def complete(self, prompt: Messages | str, **kwargs) -> str:
+        if isinstance(prompt, str):
+            prompt = [Message(role='user', content=prompt)]
+
+        response = openai.ChatCompletion.create(model=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
-    async def async_complete(self, prompt: str, **kwargs) -> str:
-        messages = [{'role': 'user', 'content': prompt}]
-        response = await openai.ChatCompletion.acreate(model=self.model, messages=messages, **kwargs)
+    async def async_complete(self, prompt: Messages | str, **kwargs) -> str:
+        if isinstance(prompt, str):
+            prompt = [Message(role='user', content=prompt)]
+
+        response = await openai.ChatCompletion.acreate(model=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
     @property
     def identifier(self) -> str:
         return f'{self.__class__.__name__}({self.model})'
```

### Comparing `lmclient-core-0.2.1/pyproject.toml` & `lmclient_core-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lmclient-core"
-version = "0.2.1"
+version = "0.3.0"
 description = "LM Async Client, openai client, azure openai client ..."
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "lmclient"}]
 repository = "https://github.com/wangyuxinwhy/lmclient"
 keywords = ["lmclient", "openai", "azure", "async"]
```

