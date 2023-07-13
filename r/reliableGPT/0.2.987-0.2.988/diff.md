# Comparing `tmp/reliableGPT-0.2.987.tar.gz` & `tmp/reliableGPT-0.2.988.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.987.tar", last modified: Thu Jul 13 15:31:34 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.988.tar", last modified: Thu Jul 13 16:47:22 2023, max compression
```

## Comparing `reliableGPT-0.2.987.tar` & `reliableGPT-0.2.988.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:31:34.617816 reliableGPT-0.2.987/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.987/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 15:31:34.617629 reliableGPT-0.2.987/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.987/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.987/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:31:34.616514 reliableGPT-0.2.987/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 15:31:34.000000 reliableGPT-0.2.987/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 15:31:34.617436 reliableGPT-0.2.987/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.987/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    21936 2023-07-13 15:26:49.000000 reliableGPT-0.2.987/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.987/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.987/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5288 2023-07-13 15:30:45.000000 reliableGPT-0.2.987/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 15:31:34.617864 reliableGPT-0.2.987/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 15:31:31.000000 reliableGPT-0.2.987/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:47:22.048158 reliableGPT-0.2.988/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.988/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 16:47:22.048049 reliableGPT-0.2.988/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.988/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.988/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:47:22.046913 reliableGPT-0.2.988/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-13 16:47:22.000000 reliableGPT-0.2.988/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-13 16:47:22.047880 reliableGPT-0.2.988/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.988/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    21987 2023-07-13 16:42:56.000000 reliableGPT-0.2.988/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.988/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.988/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5370 2023-07-13 16:46:25.000000 reliableGPT-0.2.988/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-13 16:47:22.048202 reliableGPT-0.2.988/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-13 16:47:18.000000 reliableGPT-0.2.988/setup.py
```

### Comparing `reliableGPT-0.2.987/LICENSE` & `reliableGPT-0.2.988/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.987/README.md` & `reliableGPT-0.2.988/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.987/reliablegpt/Alerting.py` & `reliableGPT-0.2.988/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.987/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.988/reliablegpt/IndividualRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,29 +85,33 @@
       if self.set_cooldown:
         if time.time() - self.cooldown_start_time > 900: # endpoint is being cooled down for 15 minutes, default to fallbacks
           error = {"type": "ErrorCooldown"}
           raise(CustomError(error=error))
         else:
           self.set_cooldown = False
       result = self.model_function(*args, **kwargs)
+      if result == None:
+        error = {"type": f"OpenAI Endpoint {self.model_function} returned None"}
+        raise CustomError(error)
       if "messages" in kwargs:
         if "engine" in kwargs:
           self.curr_azure_model = kwargs["engine"]
         if self.caching:
-          print(kwargs["messages"])
+          self.print_verbose(kwargs["messages"])
           input_prompt = "\n".join(message["content"]
                                   for message in kwargs["messages"])
           extracted_result = result['choices'][0]['message']['content']
           self.print_verbose(f'This is extracted result {extracted_result}')
           self.add_cache(
             input_prompt, extracted_result
           )  # [TODO] turn this into a threaded call, reduce latency.
         self.print_verbose(f"This is the result: {str(result)[:500]}")
       return result
     except Exception as e:
+      self.print_verbose(f"Error: {traceback.format_exc()}")
       self.print_verbose("catches the error")
       self.start_cooldown()
       return self.handle_exception(args, kwargs, e)
     
   async def async_call_model(self, args, kwargs):
     try: 
       if self._test: # private function for testing package
@@ -120,15 +124,15 @@
         else:
           self.set_cooldown = False
       result = await self.model_function(*args, **kwargs)
       if "messages" in kwargs:
         if "engine" in kwargs:
           self.curr_azure_model = kwargs["engine"]
         if self.caching:
-          print(kwargs["messages"])
+          self.print_verbose(kwargs["messages"])
           input_prompt = "\n".join(message["content"]
                                   for message in kwargs["messages"])
           extracted_result = result['choices'][0]['message']['content']
           self.print_verbose(f'This is extracted result {extracted_result}')
           self.add_cache(
             input_prompt, extracted_result
           )  # [TODO] turn this into a threaded call, reduce latency.
@@ -152,23 +156,23 @@
         # [TODO] make this into a threaded call to reduce impact on latency
         self.save_request(
           user_email=self.user_email,
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.request',
         )
       except:
-        print("ReliableGPT error occured during saving request")
+        self.print_verbose("ReliableGPT error occured during saving request")
       self.print_verbose(f"max threads: {self.max_threads}, caching: {self.caching}")
       if self.max_threads and self.caching:
         self.print_verbose(f'current util: {active_count()/self.max_threads}')
         thread_utilization = active_count()/self.max_threads
         self.print_verbose(f"Thread utilization: {thread_utilization}")
         if thread_utilization > 0.8: # over 80% utilization of threads, start returning cached responses
           if "messages" in kwargs and self.caching:
-            print(kwargs["messages"])
+            self.print_verbose(kwargs["messages"])
             input_prompt = "\n".join(message["content"]
                                     for message in kwargs["messages"])
             self.print_verbose(
               f"queue depth is higher than the threshold, start caching")
             result = self.try_cache_request(query=input_prompt)
             if self.alerting:
               # save_exception
@@ -281,26 +285,20 @@
         result = self.make_LLM_request(new_kwargs)
         if result != None:
           return result
       return None
     except:
       self.print_verbose(traceback.format_exc())
       return None
-    
-  def timeout_handler(self, signum, frame): 
-    raise Exception("timeout occurred")
 
   def make_LLM_request(self, new_kwargs):
     embedding_model = self.model.get_original_embeddings()
     chat_model = self.model.get_original_chat()
     completion_model = self.model.get_original_completion()
     try:
-      # enable the signal alarm 
-      signal.signal(signal.SIGALRM, self.timeout_handler)
-      signal.alarm(60) # model call can hang at times. Timeout after 1 minute. 
       self.print_verbose(f"{new_kwargs.keys()}")
       if "azure_fallback" in new_kwargs:
         new_kwargs_except_azure_fallback_flag = {
           k: v
           for k, v in new_kwargs.items() if k != "azure_fallback"
         }
         return chat_model(**new_kwargs_except_azure_fallback_flag)
@@ -322,50 +320,49 @@
         openai.api_type = new_kwargs["openai2"]["api_type"]
         openai.api_base = new_kwargs["openai2"]["api_base"]
         openai.api_version = new_kwargs["openai2"]["api_version"]
         openai.api_key = new_kwargs["openai2"]["api_key"]
         return completion
       if "embedding" in str(self.model_function):
         # retry embedding with diff key
-        print(colored(f"ReliableGPT: Retrying Embedding request", "blue"))
+        self.print_verbose(colored(f"ReliableGPT: Retrying Embedding request", "blue"))
         return embedding_model(**new_kwargs)
 
       model = str(new_kwargs['model'])
-      print(
+      self.print_verbose(
         colored(f"ReliableGPT: Checking request model {model} {new_kwargs}",
                 "blue"))
       if "3.5" in model or "4" in model:  # call ChatCompletion
-        print(
+        self.print_verbose(
           colored(
             f"ReliableGPT: Retrying request with model CHAT {model} {new_kwargs}",
             "blue"))
         return chat_model(**new_kwargs)
       else:
-        print(
+        self.print_verbose(
           colored(f"ReliableGPT: Retrying request with model TEXT {model}",
                   "blue"))
         new_kwargs['prompt'] = " ".join(
           [message["content"] for message in new_kwargs['messages']])
         new_kwargs.pop('messages',
                        None)  # remove messages for completion models
         return completion_model(**new_kwargs)
     except Exception as e:
-      print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
-      signal.alarm(0)
+      self.print_verbose(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
       raise ValueError(e)
 
   def api_key_handler(self, args, kwargs, fallback_strategy, user_email,
                       user_token):
     try:
       url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
       response = requests.get(url)
       if response.status_code == 200:
         result = response.json()
         if result['status'] == 'failed':
-          print(
+          self.print_verbose(
             colored(
               f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}",
               "red"))
           return None
 
         fallback_keys = result['response'][
           'openai_api_keys']  # list of fallback keys
@@ -373,15 +370,15 @@
           return None
         for fallback_key in fallback_keys:
           openai.api_key = fallback_key
           result = self.make_LLM_request(kwargs)
           if result != None:
             return result
       else:
-        print(
+        self.print_verbose(
           colored(
             f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}",
             "red"))
       return None
     except Exception as e:
       raise ValueError(e)
 
@@ -409,43 +406,43 @@
 
     error_type = None  # defalt to being None
     if openAI_error != None and 'type' in openAI_error:
       error_type = openAI_error['type']
     if error_type == 'invalid_request_error' or error_type == 'InvalidRequestError':
       # check if this is context window related, try with a 16k model
       if openAI_error.code == 'context_length_exceeded':
-        print(
+        self.print_verbose(
           colored(
             "ReliableGPT: invalid request error - context_length_exceeded",
             "red"))
         fallback_strategy = ['gpt-3.5-turbo-16k'] + fallback_strategy
         result = self.fallback_request(args=args,
                                        kwargs=kwargs,
                                        fallback_strategy=fallback_strategy)
         if result == None:
           return graceful_string
         else:
           return result
       if openAI_error.code == "invalid_api_key":
-        print(
+        self.print_verbose(
           colored("ReliableGPT: invalid request error - invalid_api_key",
                   "red"))
         result = self.api_key_handler(args=args,
                                       kwargs=kwargs,
                                       fallback_strategy=fallback_strategy,
                                       user_email=user_email,
                                       user_token=user_token)
         if result == None:
           return graceful_string
         else:
           return result
 
     # todo: alert on user_email that there is now an auth error
     elif error_type == 'authentication_error' or error_type == 'AuthenticationError':
-      print(colored("ReliableGPT: Auth error", "red"))
+      self.print_verbose(colored("ReliableGPT: Auth error", "red"))
       return graceful_string
 
     # catch all
     result = self.fallback_request(args=args,
                                    kwargs=kwargs,
                                    fallback_strategy=fallback_strategy)
     if result == None:
@@ -463,22 +460,21 @@
         args=args,
         kwargs=kwargs,
         openAI_error=e,
         fallback_strategy=self.fallback_strategy,
         graceful_string=self.graceful_string,
         user_email=self.user_email,
         user_token=self.user_token)
-      print(f"result: {result}")
       self.print_verbose(
         colored(f"ReliableGPT: Recovered got a successful response {result}",
                 "green"))
       if result == self.graceful_string:
         # did a retry with model fallback, so now try caching.
         if "messages" in kwargs and self.caching:
-          print(kwargs["messages"])
+          self.print_verbose(kwargs["messages"])
           input_prompt = "\n".join(message["content"]
                                    for message in kwargs["messages"])
           cached_response = self.try_cache_request(query=input_prompt)
           if cached_response == None:
             pass
           else:
             self.save_request(
@@ -491,15 +487,14 @@
                 'recovered_response': cached_response,
               },
               errors=['High Thread Utilization'],
               function_name=str(self.model_function),
               kwargs=kwargs
             )
             return cached_response
-        print("returns graceful string")
         self.save_request(
           user_email=self.user_email,
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.recovered_request_exception',
           result=result,
           posthog_metadata={
             'error': str(e),
@@ -520,15 +515,15 @@
                           },
                           errors=[e],
                           function_name=str(self.model_function),
                           kwargs=kwargs)
     except Exception as e2:
       # Exception 2, After trying to rescue
       traceback.print_exc()
-      print("gets 2nd error: ", e2)
+      self.print_verbose("gets 2nd error: ", e2)
       self.save_request(
         user_email=self.user_email,
         graceful_string=self.graceful_string,
         posthog_event='reliableGPT.recovered_request_exception',
         result="",
         posthog_metadata={
           'original_error': str(e),
```

### Comparing `reliableGPT-0.2.987/reliablegpt/Model.py` & `reliableGPT-0.2.988/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.987/reliablegpt/main.py` & `reliableGPT-0.2.988/reliablegpt/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,64 +33,66 @@
             'error2': error2,
             'function_name': function_name,
             'kwargs': kwargs
         }
     #print(f"in save exception on reliableGPT, sending req {data}")
     response = requests.post(url, json=data)
   except Exception as e:
-      return
+      pass
   
   return response
 
 
 
 # Parent Logging function
 def save_request(user_email,
                  graceful_string,
                  posthog_event="",
                  result="",
                  posthog_metadata={},
                  errors=[], function_name="", kwargs={}):
-  try:
-    if posthog_event != "":
-      posthog.capture(user_email, posthog_event,
-                      posthog_metadata)  # save posthog event
+  pass
+  # try:
+  #   if posthog_event != "":
+  #     posthog.capture(user_email, posthog_event,
+  #                     posthog_metadata)  # save posthog event
       
-      # Log handled and unahndled exceptions in R-GPT servers
-      if posthog_event == 'reliableGPT.recovered_request':
-        original_error = ""
-        if 'error' in posthog_metadata:
-          original_error = posthog_metadata['error']
-        save_exception(type = 'handled', user_email=user_email, result=result, original_error=original_error, function_name=function_name, kwargs=kwargs)
-
-      # Log handled and unahndled exceptions in R-GPT servers
-      if posthog_event == 'reliableGPT.recovered_request_cache':
-        original_error = ""
-        if 'error' in posthog_metadata:
-          original_error = posthog_metadata['error']
-        save_exception(type = 'handled cache', user_email=user_email, result=result, original_error=original_error, function_name=function_name, kwargs=kwargs)
-
-      # Log unhandled exceptions in R-GPT servers
-      if posthog_event == 'reliableGPT.recovered_request_exception':
-        original_error = ""
-        error2 = ""
-        if 'error' in posthog_metadata:
-          original_error = posthog_metadata['error']
-        if 'error2' in posthog_metadata:
-          error2 = posthog_metadata['error2']
-        save_exception(type = 'unhandled', user_email=user_email, result=result, original_error=original_error, error2=error2, function_name=function_name, kwargs=kwargs)
+  #     # Log handled and unahndled exceptions in R-GPT servers
+  #     if posthog_event == 'reliableGPT.recovered_request':
+  #       original_error = ""
+  #       if 'error' in posthog_metadata:
+  #         original_error = posthog_metadata['error']
+  #       save_exception(type = 'handled', user_email=user_email, result=result, original_error=original_error, function_name=function_name, kwargs=kwargs)
+
+  #     # Log handled and unahndled exceptions in R-GPT servers
+  #     if posthog_event == 'reliableGPT.recovered_request_cache':
+  #       original_error = ""
+  #       if 'error' in posthog_metadata:
+  #         original_error = posthog_metadata['error']
+  #       save_exception(type = 'handled cache', user_email=user_email, result=result, original_error=original_error, function_name=function_name, kwargs=kwargs)
+
+  #     # Log unhandled exceptions in R-GPT servers
+  #     if posthog_event == 'reliableGPT.recovered_request_exception':
+  #       original_error = ""
+  #       error2 = ""
+  #       if 'error' in posthog_metadata:
+  #         original_error = posthog_metadata['error']
+  #       if 'error2' in posthog_metadata:
+  #         error2 = posthog_metadata['error2']
+  #       save_exception(type = 'unhandled', user_email=user_email, result=result, original_error=original_error, error2=error2, function_name=function_name, kwargs=kwargs)
       
-    if result == graceful_string or len(
-        errors) == 2:  # returns a graceful string or got a 2nd exception
-      # send an email and alert
-      for error in errors:
-        alerting.add_error(error)
-      # send_emails_task(self.user_email, posthog_metadata, self.send_notification)
-  except:
-    return  # safe function, should not impact error handling if logging fails
+  #   if result == graceful_string or len(
+  #       errors) == 2:  # returns a graceful string or got a 2nd exception
+  #     # send an email and alert
+  #     for error in errors:
+  #       alerting.add_error(error)
+  #     # send_emails_task(self.user_email, posthog_metadata, self.send_notification)
+  # except:
+  #   pass
+    # return  # safe function, should not impact error handling if logging fails
 
 
 def reliableGPT(openai_create_function,
            fallback_strategy=[
              'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'
            ],
            azure_fallback_strategy=None,
```

