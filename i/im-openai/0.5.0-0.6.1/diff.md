# Comparing `tmp/im_openai-0.5.0.tar.gz` & `tmp/im_openai-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.5.0.tar", last modified: Fri Jul  7 00:55:05 2023, max compression
+gzip compressed data, was "im_openai-0.6.1.tar", last modified: Thu Jul 13 00:40:08 2023, max compression
```

## Comparing `im_openai-0.5.0.tar` & `im_openai-0.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.573552 im_openai-0.5.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.5.0/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.5.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.5.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3128 2023-07-07 00:55:05.574272 im_openai-0.5.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.5.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.493967 im_openai-0.5.0/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.5.0/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.5.0/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.516556 im_openai-0.5.0/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-06 21:35:09.000000 im_openai-0.5.0/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4746 2023-07-07 00:30:31.000000 im_openai-0.5.0/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8835 2023-07-07 00:33:17.000000 im_openai-0.5.0/im_openai/langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3353 2023-07-07 00:30:57.000000 im_openai-0.5.0/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.5.0/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.561558 im_openai-0.5.0/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3128 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-07 00:55:05.000000 im_openai-0.5.0/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-07-07 00:55:05.576660 im_openai-0.5.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-07 00:33:18.000000 im_openai-0.5.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-07 00:55:05.570632 im_openai-0.5.0/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.5.0/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.5.0/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.472920 im_openai-0.6.1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.6.1/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.6.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.6.1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3254 2023-07-13 00:40:08.473461 im_openai-0.6.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.6.1/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.422836 im_openai-0.6.1/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.6.1/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.438664 im_openai-0.6.1/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-13 00:39:40.000000 im_openai-0.6.1/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4792 2023-07-10 22:37:03.000000 im_openai-0.6.1/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14978 2023-07-13 00:23:57.000000 im_openai-0.6.1/im_openai/langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3353 2023-07-07 00:30:57.000000 im_openai-0.6.1/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.6.1/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.462974 im_openai-0.6.1/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3254 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-07-13 00:40:08.475266 im_openai-0.6.1/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-13 00:39:40.000000 im_openai-0.6.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.470694 im_openai-0.6.1/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.6.1/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.6.1/tests/test_im_openai.py
```

### Comparing `im_openai-0.5.0/CONTRIBUTING.rst` & `im_openai-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/LICENSE` & `im_openai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/PKG-INFO` & `im_openai-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.5.0
+Version: 0.6.1
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -122,10 +122,16 @@
 
 - remove stray prints
 
 ## 0.5.0 (2023-07-06)
 
 - Add langchain callbacks handlers
 
+## 0.6.0 (2023-07-10)
 
+- Handle duplicate callbacks, agents, etc
+
+## 0.6.1 (2023-07-12)
+
+- Fix prompt retrieval in deep chains
```

### Comparing `im_openai-0.5.0/README.md` & `im_openai-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/docs/Makefile` & `im_openai-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/docs/conf.py` & `im_openai-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/docs/installation.rst` & `im_openai-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/docs/make.bat` & `im_openai-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/im_openai/client.py` & `im_openai-0.6.1/im_openai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import os
 import time
 import uuid
 import warnings
 from contextlib import asynccontextmanager
-from typing import Dict, List, TypedDict
+from typing import Any, Dict, List, TypedDict
 
 import aiohttp
 
 
 async def send_event(
     session: aiohttp.ClientSession,
     project_key: str,
@@ -16,23 +16,24 @@
     prompt_event_id: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
     prompt_params: Dict | None,
     chat_id: str | None,
     response: str | None = None,
     response_time: float | None = None,
+    prompt: Any | None = None,
 ):
     PROMPT_REPORTING_URL = os.environ.get(
         "PROMPT_REPORTING_URL", "https://app.imaginary.dev/api/event"
     )
     event = {
         "projectKey": project_key,
         "apiName": api_name,
         "params": {},
-        "prompt": {},
+        "prompt": prompt or {},
         "promptEventId": prompt_event_id,
     }
     if prompt_template_text is not None:
         if isinstance(prompt_template_text, str):
             # first default template to just the raw text
             event["promptTemplateText"] = prompt_template_text
             if prompt_params is None and getattr(prompt_template_text, "params", None):
```

### Comparing `im_openai-0.5.0/im_openai/patch.py` & `im_openai-0.6.1/im_openai/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/im_openai.egg-info/PKG-INFO` & `im_openai-0.6.1/im_openai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.5.0
+Version: 0.6.1
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -122,10 +122,16 @@
 
 - remove stray prints
 
 ## 0.5.0 (2023-07-06)
 
 - Add langchain callbacks handlers
 
+## 0.6.0 (2023-07-10)
 
+- Handle duplicate callbacks, agents, etc
+
+## 0.6.1 (2023-07-12)
+
+- Fix prompt retrieval in deep chains
```

### Comparing `im_openai-0.5.0/im_openai.egg-info/SOURCES.txt` & `im_openai-0.6.1/im_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im_openai-0.5.0/setup.py` & `im_openai-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.5.0",
+    version="0.6.1",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.5.0/tests/test_im_openai.py` & `im_openai-0.6.1/tests/test_im_openai.py`

 * *Files identical despite different names*

