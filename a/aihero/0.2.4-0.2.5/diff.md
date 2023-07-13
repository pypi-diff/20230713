# Comparing `tmp/aihero-0.2.4.tar.gz` & `tmp/aihero-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihero-0.2.4.tar", last modified: Thu Jul 13 07:03:38 2023, max compression
+gzip compressed data, was "aihero-0.2.5.tar", last modified: Thu Jul 13 15:08:09 2023, max compression
```

## Comparing `aihero-0.2.4.tar` & `aihero-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 07:03:38.366564 aihero-0.2.4/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.4/LICENSE
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 07:03:38.366868 aihero-0.2.4/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.4/README.md
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 07:03:38.359298 aihero-0.2.4/aihero/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       29 2023-07-12 04:51:12.000000 aihero-0.2.4/aihero/__init__.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     3143 2023-07-13 06:56:18.000000 aihero-0.2.4/aihero/client.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.4/aihero/exceptions.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.4/aihero/openai_helper.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1257 2023-07-13 06:57:26.000000 aihero-0.2.4/aihero/project.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     4771 2023-07-12 04:51:12.000000 aihero-0.2.4/aihero/promptstash.py
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 07:03:38.365835 aihero-0.2.4/aihero.egg-info/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 07:03:38.000000 aihero-0.2.4/aihero.egg-info/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-13 07:03:38.000000 aihero-0.2.4/aihero.egg-info/SOURCES.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-13 07:03:38.000000 aihero-0.2.4/aihero.egg-info/dependency_links.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2023-07-13 07:03:38.000000 aihero-0.2.4/aihero.egg-info/requires.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-13 07:03:38.000000 aihero-0.2.4/aihero.egg-info/top_level.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2023-07-13 07:03:38.367887 aihero-0.2.4/setup.cfg
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.4/setup.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 15:08:09.096153 aihero-0.2.5/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.5/LICENSE
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 15:08:09.096412 aihero-0.2.5/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.5/README.md
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 15:08:09.092381 aihero-0.2.5/aihero/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       29 2023-07-12 04:51:12.000000 aihero-0.2.5/aihero/__init__.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3143 2023-07-13 14:51:50.000000 aihero-0.2.5/aihero/client.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.5/aihero/exceptions.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.5/aihero/openai_helper.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1202 2023-07-13 14:38:04.000000 aihero-0.2.5/aihero/project.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     5086 2023-07-13 14:49:15.000000 aihero-0.2.5/aihero/promptstash.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 15:08:09.095618 aihero-0.2.5/aihero.egg-info/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/requires.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/top_level.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2023-07-13 15:08:09.097592 aihero-0.2.5/setup.cfg
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.5/setup.py
```

### Comparing `aihero-0.2.4/LICENSE` & `aihero-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aihero-0.2.4/PKG-INFO` & `aihero-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihero
-Version: 0.2.4
+Version: 0.2.5
 Summary: AI Hero Python SDK
 Home-page: https://github.com/ai-hero/python-client-sdk
 Author: AI Hero Team
 Author-email: team@aihero.studio
 License: MIT
 Keywords: AI Hero,Spotcheck,MLOps,AI,Data Annotation,Labeling,Model Training,Model Serving,Model Deployment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aihero-0.2.4/aihero/client.py` & `aihero-0.2.5/aihero/client.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.4/aihero/openai_helper.py` & `aihero-0.2.5/aihero/openai_helper.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.4/aihero/project.py` & `aihero-0.2.5/aihero/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .client import Client
-from .promptstash import PromptTemplate
+from .promptstash import PromptStash
 
 
 class Project:
     """Main sync client class to talk to AI Hero"""
 
     def __init__(
         self,
@@ -26,9 +26,9 @@
         )
         if verbose:
             print(f"Project id:\t{project_dict['project_id']}")
             print(f"Project name:\t{project_dict['name']}")
             print(f"Project desc:\t{project_dict['description']}")
             print(f"Created on:\t{project_dict['created_at']}")
 
-    def prompt_template(self, prompt_template_id: str):
-        return PromptTemplate(self._project_id, self._client, prompt_template_id)
+    def promptstash(self):
+        return PromptStash(self._project_id, self._client)
```

### Comparing `aihero-0.2.4/aihero.egg-info/PKG-INFO` & `aihero-0.2.5/aihero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihero
-Version: 0.2.4
+Version: 0.2.5
 Summary: AI Hero Python SDK
 Home-page: https://github.com/ai-hero/python-client-sdk
 Author: AI Hero Team
 Author-email: team@aihero.studio
 License: MIT
 Keywords: AI Hero,Spotcheck,MLOps,AI,Data Annotation,Labeling,Model Training,Model Serving,Model Deployment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aihero-0.2.4/setup.cfg` & `aihero-0.2.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aihero
-version = 0.2.4
+version = 0.2.5
 description = AI Hero Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ai-hero/python-client-sdk
 author = AI Hero Team
 author_email = team@aihero.studio
 license = MIT
```

