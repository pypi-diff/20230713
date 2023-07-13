# Comparing `tmp/brainchain-0.3.6.tar.gz` & `tmp/brainchain-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.3.6.tar", max compression
+gzip compressed data, was "brainchain-0.3.7.tar", max compression
```

## Comparing `brainchain-0.3.6.tar` & `brainchain-0.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.6/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.6/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.6/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.6/brainchain/__init__.py
--rw-r--r--   0        0        0     6227 2023-07-12 20:03:29.941305 brainchain-0.3.6/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.6/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.6/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.6/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.6/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.6/brainchain/sales_intel.py
--rw-r--r--   0        0        0      532 2023-07-12 19:57:30.932222 brainchain-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.7/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.7/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.7/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.7/brainchain/__init__.py
+-rw-r--r--   0        0        0     6423 2023-07-13 16:13:29.433811 brainchain-0.3.7/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.7/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.7/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.7/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.7/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.7/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      532 2023-07-13 16:08:46.031550 brainchain-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.7/PKG-INFO
```

### Comparing `brainchain-0.3.6/brainchain/.aider.chat.history.md` & `brainchain-0.3.7/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/.aider.input.history` & `brainchain-0.3.7/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/README.md` & `brainchain-0.3.7/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/brainchain.py` & `brainchain-0.3.7/brainchain/brainchain.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,17 @@
         self.sales_intel_client = SalesIntel(salesintel_api_key)
         self.environments = ["prod", "dev"]
         self.services = {
             "agent": {
                 "prod": "https://brainchain--agent.modal.run/",
                 "dev": "https://brainchain--agent-dev.modal.run/"
             },
+            "agent-service": {
+                "agent": "https://brainchain--agent-service.modal.run/agent"
+            },
             "prompt-completion-service": {
                 "prompting": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/prompting",
                 "get_pdf_title": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/get_pdf_title",
                 "get_pdf_authors": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/get_pdf_authors"
             },
             "search": {
                 "prod": "https://brainchain--search.modal.run/",
@@ -100,30 +103,31 @@
             payload["document_text"] = text_first_page
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, json=payload)
         content = response.content.decode('utf-8')
         return json.loads(content)
 
-    def summon(self, prompt, agent_type="CCR", model="gpt-4-0613", max_tokens=2048, temperature=0.18, top_p=0.15, top_k=0.0, presence_penalty=1.0, frequency_penalty=1.0):
-        endpoint = self.services["agent"][self.env]
+    def summon(self, prompt, agent_type="CCR", model="gpt-4-0613", max_tokens=2048, temperature=0.18, top_p=0.15, top_k=0.0, presence_penalty=1.0, frequency_penalty=1.0, chat_history: list = []):
+        endpoint = self.services["agent-service"]["agent"]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {
             "prompt": prompt,
             "env": self.env,
             "agent_type": agent_type,
             "model": model,
             "max_tokens": max_tokens,
             "temperature": temperature,
             "top_p": top_p,
             "top_k": top_k,
             "presence_penalty": presence_penalty,
-            "frequency_penalty": frequency_penalty
+            "frequency_penalty": frequency_penalty,
+            "chat_history": chat_history
         }
-        response = requests.get(endpoint, headers=headers, params=params)
+        response = requests.post(endpoint, headers=headers, json=params)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
     def get_company(self, **kwargs):
```

### Comparing `brainchain-0.3.6/brainchain/carnivore.py` & `brainchain-0.3.7/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/coredata.py` & `brainchain-0.3.7/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/factcheck.py` & `brainchain-0.3.7/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/requirements.txt` & `brainchain-0.3.7/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/brainchain/sales_intel.py` & `brainchain-0.3.7/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.6/pyproject.toml` & `brainchain-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.3.6"
+version = "0.3.7"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.92"
```

### Comparing `brainchain-0.3.6/PKG-INFO` & `brainchain-0.3.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.3.6
+Version: 0.3.7
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

