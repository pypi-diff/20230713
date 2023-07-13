# Comparing `tmp/reliableGPT-0.2.983.tar.gz` & `tmp/reliableGPT-0.2.984.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.983.tar", last modified: Wed Jul 12 21:29:17 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.984.tar", last modified: Thu Jul 13 00:52:03 2023, max compression
```

## Comparing `reliableGPT-0.2.983.tar` & `reliableGPT-0.2.984.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:29:17.454407 reliableGPT-0.2.983/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.983/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:29:17.454288 reliableGPT-0.2.983/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.983/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.983/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:29:17.452586 reliableGPT-0.2.983/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:29:17.454078 reliableGPT-0.2.983/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.983/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    19026 2023-07-12 21:23:16.000000 reliableGPT-0.2.983/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.983/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.983/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5272 2023-07-12 21:28:58.000000 reliableGPT-0.2.983/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-12 21:29:17.454450 reliableGPT-0.2.983/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-12 21:29:14.000000 reliableGPT-0.2.983/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 00:52:03.829091 reliableGPT-0.2.984/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.984/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 00:52:03.828971 reliableGPT-0.2.984/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.984/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.984/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 00:52:03.828194 reliableGPT-0.2.984/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 00:52:03.000000 reliableGPT-0.2.984/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 00:52:03.000000 reliableGPT-0.2.984/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 00:52:03.000000 reliableGPT-0.2.984/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 00:52:03.000000 reliableGPT-0.2.984/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 00:52:03.000000 reliableGPT-0.2.984/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 00:52:03.828805 reliableGPT-0.2.984/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.984/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    21692 2023-07-13 00:50:09.000000 reliableGPT-0.2.984/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.984/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.984/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5288 2023-07-13 00:42:18.000000 reliableGPT-0.2.984/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 00:52:03.829143 reliableGPT-0.2.984/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 00:51:58.000000 reliableGPT-0.2.984/setup.py
```

### Comparing `reliableGPT-0.2.983/LICENSE` & `reliableGPT-0.2.984/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.983/README.md` & `reliableGPT-0.2.984/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.983/reliablegpt/Alerting.py` & `reliableGPT-0.2.984/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.983/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.984/reliablegpt/IndividualRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from uuid import uuid4
 from waitress import serve
 from flask import Flask, request
 from uuid import uuid4
 import traceback
 from threading import active_count
 import random 
+import time 
+import asyncio 
+import signal
 
 ## for testing
 class CustomError(Exception):
     def __init__(self, error):
         self.error = error
 
 
@@ -53,24 +56,94 @@
     self._test = _test
     self.print_verbose(f"INIT fallback strategy {self.fallback_strategy}")
     self.caching = caching
     self.max_threads = max_threads
     self.print_verbose(f"INIT with threads {self.max_threads} {self.caching} {max_threads}")
     self.alerting = alerting
     self.azure_fallback_strategy = azure_fallback_strategy
+    self.backup_model = None
+    self.set_cooldown = False
+    self.cooldown_start_time = time.time()
 
   def handle_unhandled_exception(self, e):
     self.print_verbose(colored("UNHANDLED EXCEPTION OCCURRED", "red"))
     if self.alerting:
       self.alerting.add_error(error_type="Unhandled Exception", error_description=traceback.format_exc())
 
   def print_verbose(self, print_statement):
     if self.verbose:
       print(colored("Individual Request: " + print_statement, "blue"))
 
+  def start_cooldown(self):
+    self.set_cooldown = True
+    self.cooldown_start_time = time.time()
+
+  def call_model(self, args, kwargs):
+    try: 
+      if self._test: # private function for testing package
+        error = {"type": "RandomError"}
+        raise CustomError(error)
+      if self.set_cooldown:
+        if time.time() - self.cooldown_start_time > 900: # endpoint is being cooled down for 15 minutes
+          error = {"type": "ErrorCooldown"}
+          raise(CustomError(error=error))
+        else:
+          self.set_cooldown = False
+      result = self.model_function(*args, **kwargs)
+      if "messages" in kwargs:
+        if "engine" in kwargs:
+          self.curr_azure_model = kwargs["engine"]
+        if self.caching:
+          print(kwargs["messages"])
+          input_prompt = "\n".join(message["content"]
+                                  for message in kwargs["messages"])
+          extracted_result = result['choices'][0]['message']['content']
+          self.print_verbose(f'This is extracted result {extracted_result}')
+          self.add_cache(
+            input_prompt, extracted_result
+          )  # [TODO] turn this into a threaded call, reduce latency.
+        self.print_verbose(f"This is the result: {str(result)[:500]}")
+      return result
+    except Exception as e:
+      self.print_verbose("catches the error")
+      self.start_cooldown()
+      return self.handle_exception(args, kwargs, e)
+    
+  async def async_call_model(self, args, kwargs):
+    try: 
+      if self._test: # private function for testing package
+        error = {"type": "RandomError in async function"}
+        raise CustomError(error)
+      if self.set_cooldown:
+        if time.time() - self.cooldown_start_time > 900: # endpoint is being cooled down for 15 minutes
+          error = {"type": "ErrorCooldown"}
+          raise(CustomError(error=error))
+        else:
+          self.set_cooldown = False
+      result = await self.model_function(*args, **kwargs)
+      if "messages" in kwargs:
+        if "engine" in kwargs:
+          self.curr_azure_model = kwargs["engine"]
+        if self.caching:
+          print(kwargs["messages"])
+          input_prompt = "\n".join(message["content"]
+                                  for message in kwargs["messages"])
+          extracted_result = result['choices'][0]['message']['content']
+          self.print_verbose(f'This is extracted result {extracted_result}')
+          self.add_cache(
+            input_prompt, extracted_result
+          )  # [TODO] turn this into a threaded call, reduce latency.
+        self.print_verbose(f"This is the result: {str(result)[:500]}")
+      return result
+    except Exception as e:
+      self.print_verbose("catches the error")
+      self.start_cooldown()
+      return self.handle_exception(args, kwargs, e)
+
+
   ## Code that handles / wraps openai calls
   def __call__(self, *args, **kwargs):
     try:
       self.print_verbose(f"calling model function: {self.model_function}")
       self.print_verbose(f"these are the kwargs: {kwargs}")
       self.print_verbose(f"this is the openai api base: {openai.api_base}")
       self.print_verbose(f"testing enabled: {self._test}")
@@ -81,17 +154,14 @@
           user_email=self.user_email,
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.request',
         )
       except:
         print("ReliableGPT error occured during saving request")
       self.print_verbose(f"max threads: {self.max_threads}, caching: {self.caching}")
-      if self._test:
-        error = {"type": "RandomError"}
-        raise CustomError(error)
       if self.max_threads and self.caching:
         self.print_verbose(f'current util: {active_count()/self.max_threads}')
         thread_utilization = active_count()/self.max_threads
         self.print_verbose(f"Thread utilization: {thread_utilization}")
         if thread_utilization > 0.8: # over 80% utilization of threads, start returning cached responses
           if "messages" in kwargs and self.caching:
             print(kwargs["messages"])
@@ -117,31 +187,22 @@
                   'recovered_response': result,
                 },
                 errors=['High Thread Utilization'],
                 function_name=str(self.model_function),
                 kwargs=kwargs
               )
               return result
-      # print("received request")
+      
       # Run user request
-      result = self.model_function(*args, **kwargs)
-      if "messages" in kwargs and self.caching:
-        print(kwargs["messages"])
-        input_prompt = "\n".join(message["content"]
-                                 for message in kwargs["messages"])
-        extracted_result = result['choices'][0]['message']['content']
-        self.print_verbose(f'This is extracted result {extracted_result}')
-        self.add_cache(
-          input_prompt, extracted_result
-        )  # [TODO] turn this into a threaded call, reduce latency.
-      self.print_verbose(f"This is the result: {str(result)[:500]}")
-      return result
+      if asyncio.iscoroutinefunction(self.model_function):
+        return self.async_call_model(args=args, kwargs=kwargs)
+      else:
+        return self.call_model(args=args, kwargs=kwargs)
     except Exception as e:
-      self.print_verbose("catches the error")
-      return self.handle_exception(args, kwargs, e)
+      self.print_verbose(f"Error in main call function: {traceback.format_exc()}")
 
   def add_cache(self, input_prompt, response):
     try:
       if self.caching:
         if request:
           if request.args and request.args.get("user_email"):
             customer_id = request.args.get("user_email")
@@ -219,20 +280,26 @@
         result = self.make_LLM_request(new_kwargs)
         if result != None:
           return result
       return None
     except:
       self.print_verbose(traceback.format_exc())
       return None
+    
+  def timeout_handler(self, signum, frame): 
+    raise Exception("timeout occurred")
 
   def make_LLM_request(self, new_kwargs):
     embedding_model = self.model.get_original_embeddings()
     chat_model = self.model.get_original_chat()
     completion_model = self.model.get_original_completion()
     try:
+      # enable the signal alarm 
+      signal.signal(signal.SIGALRM, self.timeout_handler)
+      signal.alarm(60) # model call can hang at times. Timeout after 1 minute. 
       self.print_verbose(f"{new_kwargs.keys()}")
       if "engine" in new_kwargs:
         return chat_model(**new_kwargs)
       if "openai2" in new_kwargs:
         openai.api_type = "openai"
         openai.api_base = "https://api.openai.com/v1"
         openai.api_version = None
@@ -274,14 +341,15 @@
         new_kwargs['prompt'] = " ".join(
           [message["content"] for message in new_kwargs['messages']])
         new_kwargs.pop('messages',
                        None)  # remove messages for completion models
         return completion_model(**new_kwargs)
     except Exception as e:
       print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
+      signal.alarm(0)
       raise ValueError(e)
 
   def api_key_handler(self, args, kwargs, fallback_strategy, user_email,
                       user_token):
     try:
       url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
       response = requests.get(url)
```

### Comparing `reliableGPT-0.2.983/reliablegpt/Model.py` & `reliableGPT-0.2.984/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.983/reliablegpt/main.py` & `reliableGPT-0.2.984/reliablegpt/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # # Prod Imports
-from reliablegpt.IndividualRequest import IndividualRequest
-from reliablegpt.Model import Model
-from reliablegpt.Alerting import Alerting
+# from reliablegpt.IndividualRequest import IndividualRequest
+# from reliablegpt.Model import Model
+# from reliablegpt.Alerting import Alerting
 import requests
+import asyncio 
 
 # # Dev Imports
-# from IndividualRequest import IndividualRequest
-# from Model import Model
-# from Alerting import Alerting
+from IndividualRequest import IndividualRequest
+from Model import Model
+from Alerting import Alerting
 
 from posthog import Posthog
 from flask import Flask, request
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
```

