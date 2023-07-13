# Comparing `tmp/deepchecks-llm-client-0.0.2.tar.gz` & `tmp/deepchecks-llm-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchecks-llm-client-0.0.2.tar", last modified: Wed Jul 12 10:48:51 2023, max compression
+gzip compressed data, was "deepchecks-llm-client-0.0.3.tar", last modified: Thu Jul 13 07:06:24 2023, max compression
```

## Comparing `deepchecks-llm-client-0.0.2.tar` & `deepchecks-llm-client-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-12 10:48:51.916799 deepchecks-llm-client-0.0.2/
--rw-r--r--   0 shay       (501) staff       (20)       18 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.2/MANIFEST.in
--rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-12 10:48:51.916665 deepchecks-llm-client-0.0.2/PKG-INFO
--rw-r--r--   0 shay       (501) staff       (20)      142 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.2/README.md
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-12 10:48:51.915485 deepchecks-llm-client-0.0.2/deepchecks_llm_client/
--rw-r--r--   0 shay       (501) staff       (20)       88 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client/__init__.py
--rw-r--r--   0 shay       (501) staff       (20)     3456 2023-07-12 07:01:44.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client/api.py
--rw-r--r--   0 shay       (501) staff       (20)     3523 2023-07-12 10:40:26.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client/client.py
--rw-r--r--   0 shay       (501) staff       (20)     3682 2023-07-12 10:41:13.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client/openai_instrumentor.py
--rw-r--r--   0 shay       (501) staff       (20)     2887 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client/utils.py
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-12 10:48:51.916124 deepchecks-llm-client-0.0.2/deepchecks_llm_client.egg-info/
--rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-12 10:48:51.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client.egg-info/PKG-INFO
--rw-r--r--   0 shay       (501) staff       (20)      481 2023-07-12 10:48:51.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client.egg-info/SOURCES.txt
--rw-r--r--   0 shay       (501) staff       (20)        1 2023-07-12 10:48:51.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client.egg-info/dependency_links.txt
--rw-r--r--   0 shay       (501) staff       (20)       29 2023-07-12 10:48:51.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client.egg-info/requires.txt
--rw-r--r--   0 shay       (501) staff       (20)       22 2023-07-12 10:48:51.000000 deepchecks-llm-client-0.0.2/deepchecks_llm_client.egg-info/top_level.txt
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-12 10:48:51.916326 deepchecks-llm-client-0.0.2/examples/
--rw-r--r--   0 shay       (501) staff       (20)        0 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.2/examples/__init__.py
--rw-r--r--   0 shay       (501) staff       (20)     2324 2023-07-12 10:44:43.000000 deepchecks-llm-client-0.0.2/examples/usage.py
--rw-r--r--   0 shay       (501) staff       (20)       29 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.2/requirements.txt
--rw-r--r--   0 shay       (501) staff       (20)       38 2023-07-12 10:48:51.916847 deepchecks-llm-client-0.0.2/setup.cfg
--rw-r--r--   0 shay       (501) staff       (20)     3069 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.2/setup.py
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.998999 deepchecks-llm-client-0.0.3/
+-rw-r--r--   0 shay       (501) staff       (20)       18 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.3/MANIFEST.in
+-rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-13 07:06:23.998882 deepchecks-llm-client-0.0.3/PKG-INFO
+-rw-r--r--   0 shay       (501) staff       (20)      142 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/README.md
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.997882 deepchecks-llm-client-0.0.3/deepchecks_llm_client/
+-rw-r--r--   0 shay       (501) staff       (20)       88 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/__init__.py
+-rw-r--r--   0 shay       (501) staff       (20)     3847 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/api.py
+-rw-r--r--   0 shay       (501) staff       (20)     3214 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/client.py
+-rw-r--r--   0 shay       (501) staff       (20)     3682 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/openai_instrumentor.py
+-rw-r--r--   0 shay       (501) staff       (20)     2887 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client/utils.py
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.998444 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/
+-rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/PKG-INFO
+-rw-r--r--   0 shay       (501) staff       (20)      481 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shay       (501) staff       (20)        1 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shay       (501) staff       (20)       29 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/requires.txt
+-rw-r--r--   0 shay       (501) staff       (20)       22 2023-07-13 07:06:23.000000 deepchecks-llm-client-0.0.3/deepchecks_llm_client.egg-info/top_level.txt
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-13 07:06:23.998620 deepchecks-llm-client-0.0.3/examples/
+-rw-r--r--   0 shay       (501) staff       (20)        0 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.3/examples/__init__.py
+-rw-r--r--   0 shay       (501) staff       (20)     2327 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.3/examples/usage.py
+-rw-r--r--   0 shay       (501) staff       (20)       29 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.3/requirements.txt
+-rw-r--r--   0 shay       (501) staff       (20)       38 2023-07-13 07:06:23.999039 deepchecks-llm-client-0.0.3/setup.cfg
+-rw-r--r--   0 shay       (501) staff       (20)     3069 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.3/setup.py
```

### Comparing `deepchecks-llm-client-0.0.2/deepchecks_llm_client/api.py` & `deepchecks-llm-client-0.0.3/deepchecks_llm_client/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,8 +93,17 @@
                  ) -> t.Optional[httpx.Response]:
         try:
             return maybe_raise(self.session.post('annotations', json={"ext_interaction_id": ext_interaction_id,
                                                                       "value": annotation.value}))
         except Exception as ex:
             logger.warning(f'Failed to send annotation data to deepchecks, message: {str(ex)}')
 
+    def get_application(self,
+                 app_name: str,
+                 ) -> t.Optional[httpx.Response]:
+        try:
+            return maybe_raise(self.session.get('applications', params={"name": [app_name]})).json()
+        except Exception as ex:
+            logger.warning(f'Failed to get application name: {app_name} from deepchecks, message: {str(ex)}')
+            return []
+
```

### Comparing `deepchecks-llm-client-0.0.2/deepchecks_llm_client/client.py` & `deepchecks-llm-client-0.0.3/deepchecks_llm_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,73 +7,71 @@
 
 
 class Tags:
     """
     Namespace for useful tags that deepchecks case use
     You can use `AppContext` to pass user tags to deepchecks
 
-    USER_PROMPT
+    USER_INPUT
         Relevant only for auto_collect=True and for cases where there is no clear understanding
-        For what is the "user prompt" (like in the case of `openai.Completion`)
+        For what is the "user input" (like in the case of `openai.Completion`)
 
     USER_ID
         The external user that used the AI model
-
-    EXT_INTERACTION_ID
-        user generated unique id to be used later for reporting annotation results (good/bad) to deepchecks
-        if this tag is not set, we will try to get the unique id that was supplied by the AI vendor
-        (in the case of OpenAI - it will be response.id)
     """
-    USER_PROMPT: str = "user_prompt"
+    USER_INPUT: str = "user_input"
     USER_ID: str = "user_id"
-    EXT_INTERACTION_ID: str = "ext_interaction_id"
 
 DEFAULT_APP_NAME = 'DefaultApp'
 DEFAULT_VERSION_NAME = '0.0.1'
 DEFAULT_ENV_TYPE = EnvType.PROD
 
 class DeepchecksLLMClient:
 
     def __init__(self):
         self.api = None
         self.instrumentor = None
 
-    def connect(self,
-                host: str,
-                api_token: str,
-                app_name: str = DEFAULT_APP_NAME,
-                version_name: str = DEFAULT_VERSION_NAME,
-                env_type: EnvType = DEFAULT_ENV_TYPE,
-                auto_collect: bool = True
+    def init(self,
+             host: str,
+             api_token: str,
+             app_name: str,
+             version_name: str = DEFAULT_VERSION_NAME,
+             env_type: EnvType = DEFAULT_ENV_TYPE,
+             auto_collect: bool = True
              ):
         """
-                Connect to Deepchecks LLM Server
+            Connect to Deepchecks LLM Server
 
-                Parameters
-                ----------
-                host : str
-                    Deepchecks host to communicate with
-                api_token : str
-                    Deepchecks API Token (can be generated from the UI)
-                auto_collect : bool, default=True
-                    Auto collect calls to LLM Models
-                app_name : str, default='DefaultApp'
-                    Application name to connect to, if Application name does not exist SDK will create it
-                    automatically
-                version_name : str, default='1.0.0'
-                    Version name to connect to inside the application,
-                    if Version name does not exist SDK will create it automatically,
-                env_type : EnvType, default=EnvType.PROD
-                    could be EnvType.PROD (for 'Production') or EnvType.EVAL (for 'Evaluation')
-                """
+            Parameters
+            ----------
+            host : str
+                Deepchecks host to communicate with
+            api_token : str
+                Deepchecks API Token (can be generated from the UI)
+            auto_collect : bool, default=True
+                Auto collect calls to LLM Models
+            app_name : str
+                Application name to connect to, if Application name does not exist
+                SDK will create it automatically
+            version_name : str, default='1.0.0'
+                Version name to connect to inside the application,
+                if Version name does not exist SDK will create it automatically,
+            env_type : EnvType, default=EnvType.PROD
+                could be EnvType.PROD (for 'Production') or EnvType.EVAL (for 'Evaluation')
+        """
         if host is not None and api_token is not None:
             self.api = API.instantiate(host=host, token=api_token)
         else:
             raise ValueError('host/token parameters must be provided')
 
+        app = self.api.get_application(app_name)
+        if not app:
+            raise Exception(f'Application: "{app_name}", does not exist, please create it via the UI')
+
         self.instrumentor = None
         if auto_collect:
             self.instrumentor = OpenAIInstrumentor(self.api, app_name, version_name, env_type)
             self.instrumentor.perform_patch()
 
     def set_context(self,
                     app_name: str = DEFAULT_APP_NAME,
```

### Comparing `deepchecks-llm-client-0.0.2/deepchecks_llm_client/openai_instrumentor.py` & `deepchecks-llm-client-0.0.3/deepchecks_llm_client/openai_instrumentor.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.2/deepchecks_llm_client/utils.py` & `deepchecks-llm-client-0.0.3/deepchecks_llm_client/utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.0.2/examples/usage.py` & `deepchecks-llm-client-0.0.3/examples/usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     coloredlogs.install(level='DEBUG')
 
     dotenv.load_dotenv()
 
     deepchecks_api_key = os.environ.get("DEEPCHECKS_LLM_API_KEY")
     # auto_collect=True wraps `openai.ChatCompletion` and `openai.Completion` APIs
     # so any OpenAI invocation will fire an event to deepchecks with the relevant data
-    dc_client.connect(host='http://localhost:8000',
-                      api_token=deepchecks_api_key,
-                      app_name="ShaysApp",
-                      version_name="0.0.1-shay",
-                      env_type=EnvType.EVAL,
-                      auto_collect=True)
+    dc_client.init(host='http://localhost:8000',
+                   api_token=deepchecks_api_key,
+                   app_name="ShaysApp",
+                   version_name="0.0.1-shay",
+                   env_type=EnvType.EVAL,
+                   auto_collect=True)
 
     # Adding context to the call, deepchecks will monitor the context together with any OpenAI's request/response
-    dc_client.set_tags({Tags.USER_ID: "mycustomer@gmail.com"})
+    dc_client.set_tags({Tags.USER_ID: "A05fdfbb2035e@gmail.com"})
 
     # Set up your OpenAI API credentials
     openai.api_key = os.environ.get("OPENAI_API_KEY")
     chat_completion = openai.ChatCompletion.create(model="gpt-3.5-turbo", temperature=0.7,
                                                    messages=[{"role": "user", "content": "How much is 2 plus 2?"}])
 
     # print the chat completion`
@@ -41,32 +41,31 @@
 
     ### Next Iteration ###
     ######################
 
 
     dc_client.set_context(app_name="ShaysApp", version_name="0.0.2-shay", env_type=EnvType.EVAL)
 
-    user_prompt = "how many trees in the garden?"
-    external_id = "myGenID1" + str(uuid.uuid4())
-    dc_client.set_tags({Tags.USER_ID: "mycustomer2@gmail.com", Tags.USER_PROMPT: user_prompt,
-                        Tags.EXT_INTERACTION_ID: external_id})
-
+    user_input = "what is the most dominant color of tulips?"
+    dc_client.set_tags({Tags.USER_ID: "B05fdfbb2035e@gmail.com",
+                        Tags.USER_INPUT: user_input})
+    full_input = f"Answering the following question as you were a gardener: {user_input}"
     response = openai.Completion.create(
       model="text-davinci-003",
-      prompt=user_prompt,
+      prompt=full_input,
       temperature=0.5,
       max_tokens=150,
       top_p=1.0,
       frequency_penalty=0.0,
       presence_penalty=0.0,
       stop=["#", ";"]
     )
 
     print(response)
 
-    # Annotating based on external id
-    dc_client.annotate(external_id, annotation=AnnotationType.BAD)
+    # Annotating based on openai id
+    dc_client.annotate(response.openai_id, annotation=AnnotationType.BAD)
 
 
 if __name__ == "__main__":
     #asyncio.run(run())
     run()
```

### Comparing `deepchecks-llm-client-0.0.2/setup.py` & `deepchecks-llm-client-0.0.3/setup.py`

 * *Files identical despite different names*

