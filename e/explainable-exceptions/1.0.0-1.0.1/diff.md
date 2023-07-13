# Comparing `tmp/explainable-exceptions-1.0.0.tar.gz` & `tmp/explainable-exceptions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainable-exceptions-1.0.0.tar", last modified: Thu Jul 13 07:18:16 2023, max compression
+gzip compressed data, was "explainable-exceptions-1.0.1.tar", last modified: Thu Jul 13 07:38:16 2023, max compression
```

## Comparing `explainable-exceptions-1.0.0.tar` & `explainable-exceptions-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:18:16.718303 explainable-exceptions-1.0.0/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.0/LICENSE
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      111 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.0/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:18:16.718303 explainable-exceptions-1.0.0/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     3526 2023-07-13 07:17:33.000000 explainable-exceptions-1.0.0/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:18:16.718303 explainable-exceptions-1.0.0/explainable_exceptions/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       22 2023-07-13 07:18:12.000000 explainable-exceptions-1.0.0/explainable_exceptions/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      852 2023-07-13 07:18:12.000000 explainable-exceptions-1.0.0/explainable_exceptions/_modidx.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     3199 2023-07-13 07:18:12.000000 explainable-exceptions-1.0.0/explainable_exceptions/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:18:16.718303 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:18:16.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      474 2023-07-13 07:18:16.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-13 07:18:16.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       87 2023-07-13 07:18:16.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-11 10:07:23.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       15 2023-07-13 07:18:16.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       23 2023-07-13 07:18:16.000000 explainable-exceptions-1.0.0/explainable_exceptions.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      924 2023-07-13 07:18:00.000000 explainable-exceptions-1.0.0/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-07-13 07:18:16.718303 explainable-exceptions-1.0.0/setup.cfg
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     2596 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.0/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.1/LICENSE
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      111 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.1/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     3526 2023-07-13 07:17:33.000000 explainable-exceptions-1.0.1/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/explainable_exceptions/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       22 2023-07-13 07:38:11.000000 explainable-exceptions-1.0.1/explainable_exceptions/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      944 2023-07-13 07:38:11.000000 explainable-exceptions-1.0.1/explainable_exceptions/_modidx.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4083 2023-07-13 07:38:11.000000 explainable-exceptions-1.0.1/explainable_exceptions/core.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      474 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       87 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-11 10:07:23.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       15 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       23 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      924 2023-07-13 07:38:05.000000 explainable-exceptions-1.0.1/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/setup.cfg
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     2596 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.1/setup.py
```

### Comparing `explainable-exceptions-1.0.0/LICENSE` & `explainable-exceptions-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-1.0.0/PKG-INFO` & `explainable-exceptions-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainable-exceptions
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module to explain exceptions in execution-time using a magic cell
 Home-page: https://github.com/ruescog/explainable-exceptions
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: explainable-exceptions
         ================
```

### Comparing `explainable-exceptions-1.0.0/README.md` & `explainable-exceptions-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-1.0.0/explainable_exceptions/_modidx.py` & `explainable-exceptions-1.0.1/explainable_exceptions/_modidx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/explainable-exceptions',
                 'doc_host': 'https://ruescog.github.io',
                 'git_url': 'https://github.com/ruescog/explainable-exceptions',
                 'lib_path': 'explainable_exceptions'},
-  'syms': { 'explainable_exceptions.core': { 'explainable_exceptions.core.explain': ('core.html#explain', 'explainable_exceptions/core.py'),
-                                             'explainable_exceptions.core.explain_exception': ( 'core.html#explain_exception',
-                                                                                                'explainable_exceptions/core.py'),
-                                             'explainable_exceptions.core.login': ('core.html#login', 'explainable_exceptions/core.py')}}}
+  'syms': { 'explainable_exceptions.core': { 'explainable_exceptions.core._explain_exception': ( 'core.html#_explain_exception',
+                                                                                                 'explainable_exceptions/core.py'),
+                                             'explainable_exceptions.core._login': ('core.html#_login', 'explainable_exceptions/core.py'),
+                                             'explainable_exceptions.core.explain': ( 'core.html#explain',
+                                                                                      'explainable_exceptions/core.py')}}}
```

### Comparing `explainable-exceptions-1.0.0/explainable_exceptions/core.py` & `explainable-exceptions-1.0.1/explainable_exceptions/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['login', 'explain_exception', 'explain']
+__all__ = ['explain']
 
 # %% ../nbs/00_core.ipynb 3
 from hugchat import hugchat
 from hugchat.exceptions import ModelOverloadedError
 from hugchat.login import Login
 from IPython.core.magic import register_cell_magic, needs_local_scope
 from IPython.display import display, Markdown
 from time import sleep
 
 import logging
 import os
 import traceback
 
 # %% ../nbs/00_core.ipynb 4
-def login(user: str = None, password: str = None, *, credentials_dir: str = "."):
+def _login(user: str = None, # username of the huggingchat account that is going to be used to send the messages. If None, it will be infered from possible json files in the working directory or requested to the user.
+          password: str = None, # in plain-text, the password of that account. Not necessary if there exist a credentials file. Requested to the user otherwise.
+          credentials_dir: str = "." # the path where the credentials file is. The working directory will be selected by default.
+         ):
     """
     Logs the user into the huggingface chat using the user + password or the user + credentials json.
     """
     try:
         cookies = None
         json_file = [f for f in os.listdir() if ".json" in f]
         
@@ -48,15 +51,18 @@
         if confirm == "y":
             path = sign.saveCookiesToDir(credentials_dir)
             print(f"Your credentials file has been saved at: {path}")
 
     finally:
         return cookies
     
-def explain_exception(cookies, exception_message, wait = 0):
+def _explain_exception(cookies, # cookies used in the connection.
+                      exception_message, # error message sent to the model.
+                      wait = 0 # number of seconds to wait until sending the message.
+                     ):
     if not wait:
         logging.info("Conecting with hugchat to obtain the information about the exception.")
     else:
         sleep(wait)
 
     chatbot = hugchat.ChatBot(cookies = cookies.get_dict())
     user_confirmation = None
@@ -67,24 +73,27 @@
             response = chatbot.chat(f"I was coding with Python and I have found this exception message: {exception_message}. How can I solve it?")
             display(Markdown("## Huggingchat response [(online version)](https://huggingface.co/chat):"))
             display(Markdown(response))
             display(Markdown("---"))
             user_confirmation = input("\nDo you need another answer? (y/n)")
     except ModelOverloadedError as e:
         logging.warning(f"Model is overloaded, trying again in {wait + 5} seconds...")
-        explain_exception(cookies, exception_message, wait + 5)
+        _explain_exception(cookies, exception_message, wait + 5)
     
 @register_cell_magic
 @needs_local_scope
-def explain(line, cell, local_ns):
+def explain(line, # additional information added to the execution of the magic command. If provided, it will be trated as the username.
+            cell, # cell that potentially raised the exception.
+            local_ns # infered from the decorator. The local variables (needed to catch the imports).
+           ):
     try:
         exec(cell, globals(), local_ns)
     except Exception as e:
         exception_message = traceback.format_exc()
         logging.critical(exception_message)
         
         user = line if line else None
-        cookies = login(user)
+        cookies = _login(user)
         
-        explain_exception(cookies, exception_message)
+        _explain_exception(cookies, exception_message)
         
         raise e
```

### Comparing `explainable-exceptions-1.0.0/explainable_exceptions.egg-info/PKG-INFO` & `explainable-exceptions-1.0.1/explainable_exceptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainable-exceptions
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module to explain exceptions in execution-time using a magic cell
 Home-page: https://github.com/ruescog/explainable-exceptions
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: explainable-exceptions
         ================
```

### Comparing `explainable-exceptions-1.0.0/settings.ini` & `explainable-exceptions-1.0.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = explainable-exceptions
 lib_name = explainable-exceptions
-version = 1.0.0
+version = 1.0.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = explainable_exceptions
 nbs_path = nbs
 recursive = True
```

### Comparing `explainable-exceptions-1.0.0/setup.py` & `explainable-exceptions-1.0.1/setup.py`

 * *Files identical despite different names*

