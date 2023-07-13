# Comparing `tmp/explainable-exceptions-1.0.1.tar.gz` & `tmp/explainable-exceptions-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainable-exceptions-1.0.1.tar", last modified: Thu Jul 13 07:38:16 2023, max compression
+gzip compressed data, was "explainable-exceptions-1.0.2.tar", last modified: Thu Jul 13 07:58:48 2023, max compression
```

## Comparing `explainable-exceptions-1.0.1.tar` & `explainable-exceptions-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.1/LICENSE
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      111 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.1/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     3526 2023-07-13 07:17:33.000000 explainable-exceptions-1.0.1/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/explainable_exceptions/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       22 2023-07-13 07:38:11.000000 explainable-exceptions-1.0.1/explainable_exceptions/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      944 2023-07-13 07:38:11.000000 explainable-exceptions-1.0.1/explainable_exceptions/_modidx.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4083 2023-07-13 07:38:11.000000 explainable-exceptions-1.0.1/explainable_exceptions/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      474 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       87 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-11 10:07:23.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       15 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       23 2023-07-13 07:38:16.000000 explainable-exceptions-1.0.1/explainable_exceptions.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      924 2023-07-13 07:38:05.000000 explainable-exceptions-1.0.1/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-07-13 07:38:16.978328 explainable-exceptions-1.0.1/setup.cfg
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     2596 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.1/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:58:48.526354 explainable-exceptions-1.0.2/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.2/LICENSE
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      111 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.2/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:58:48.526354 explainable-exceptions-1.0.2/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     3526 2023-07-13 07:17:33.000000 explainable-exceptions-1.0.2/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:58:48.526354 explainable-exceptions-1.0.2/explainable_exceptions/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       22 2023-07-13 07:58:34.000000 explainable-exceptions-1.0.2/explainable_exceptions/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      944 2023-07-13 07:58:34.000000 explainable-exceptions-1.0.2/explainable_exceptions/_modidx.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4169 2023-07-13 07:58:34.000000 explainable-exceptions-1.0.2/explainable_exceptions/core.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-13 07:58:48.526354 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     5154 2023-07-13 07:58:48.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      474 2023-07-13 07:58:48.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-13 07:58:48.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       87 2023-07-13 07:58:48.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-11 10:07:23.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       15 2023-07-13 07:58:48.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       23 2023-07-13 07:58:48.000000 explainable-exceptions-1.0.2/explainable_exceptions.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      924 2023-07-13 07:58:31.000000 explainable-exceptions-1.0.2/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-07-13 07:58:48.526354 explainable-exceptions-1.0.2/setup.cfg
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     2596 2023-07-10 10:17:06.000000 explainable-exceptions-1.0.2/setup.py
```

### Comparing `explainable-exceptions-1.0.1/LICENSE` & `explainable-exceptions-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-1.0.1/PKG-INFO` & `explainable-exceptions-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainable-exceptions
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module to explain exceptions in execution-time using a magic cell
 Home-page: https://github.com/ruescog/explainable-exceptions
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: explainable-exceptions
         ================
```

### Comparing `explainable-exceptions-1.0.1/README.md` & `explainable-exceptions-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-1.0.1/explainable_exceptions/_modidx.py` & `explainable-exceptions-1.0.2/explainable_exceptions/_modidx.py`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-1.0.1/explainable_exceptions/core.py` & `explainable-exceptions-1.0.2/explainable_exceptions/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     chatbot = hugchat.ChatBot(cookies = cookies.get_dict())
     user_confirmation = None
     
     try:
         while user_confirmation != "n":
             logging.warning("Be careful, the following response has been generated automatically by a Natural Language Processing Model, so the answer may be incorrect or false.")
-            response = chatbot.chat(f"I was coding with Python and I have found this exception message: {exception_message}. How can I solve it?")
+            response = chatbot.chat(f"I was coding with Python and I have found this exception message: {exception_message}. How can I solve it?", temperature=0.85) # https://huggingface.co/spaces/huggingchat/chat-ui/discussions/170
             display(Markdown("## Huggingchat response [(online version)](https://huggingface.co/chat):"))
             display(Markdown(response))
             display(Markdown("---"))
             user_confirmation = input("\nDo you need another answer? (y/n)")
     except ModelOverloadedError as e:
         logging.warning(f"Model is overloaded, trying again in {wait + 5} seconds...")
         _explain_exception(cookies, exception_message, wait + 5)
```

### Comparing `explainable-exceptions-1.0.1/explainable_exceptions.egg-info/PKG-INFO` & `explainable-exceptions-1.0.2/explainable_exceptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainable-exceptions
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module to explain exceptions in execution-time using a magic cell
 Home-page: https://github.com/ruescog/explainable-exceptions
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: explainable-exceptions
         ================
```

### Comparing `explainable-exceptions-1.0.1/settings.ini` & `explainable-exceptions-1.0.2/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = explainable-exceptions
 lib_name = explainable-exceptions
-version = 1.0.1
+version = 1.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = explainable_exceptions
 nbs_path = nbs
 recursive = True
```

### Comparing `explainable-exceptions-1.0.1/setup.py` & `explainable-exceptions-1.0.2/setup.py`

 * *Files identical despite different names*

