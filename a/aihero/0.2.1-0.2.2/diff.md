# Comparing `tmp/aihero-0.2.1.tar.gz` & `tmp/aihero-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihero-0.2.1.tar", last modified: Thu Jul 13 06:50:41 2023, max compression
+gzip compressed data, was "aihero-0.2.2.tar", last modified: Thu Jul 13 06:52:50 2023, max compression
```

## Comparing `aihero-0.2.1.tar` & `aihero-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:50:41.283684 aihero-0.2.1/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.1/LICENSE
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 06:50:41.283877 aihero-0.2.1/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.1/README.md
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:50:41.279384 aihero-0.2.1/aihero/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       29 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/__init__.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     3170 2023-07-13 06:46:01.000000 aihero-0.2.1/aihero/client.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.1/aihero/exceptions.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/openai_helper.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1195 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/project.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     4771 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/promptstash.py
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:50:41.282867 aihero-0.2.1/aihero.egg-info/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/SOURCES.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/dependency_links.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/requires.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/top_level.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2023-07-13 06:50:41.284970 aihero-0.2.1/setup.cfg
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.1/setup.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:52:50.070697 aihero-0.2.2/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.2/LICENSE
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 06:52:50.070854 aihero-0.2.2/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.2/README.md
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:52:50.067470 aihero-0.2.2/aihero/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       29 2023-07-12 04:51:12.000000 aihero-0.2.2/aihero/__init__.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3219 2023-07-13 06:52:41.000000 aihero-0.2.2/aihero/client.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.2/aihero/exceptions.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.2/aihero/openai_helper.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1195 2023-07-12 04:51:12.000000 aihero-0.2.2/aihero/project.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     4771 2023-07-12 04:51:12.000000 aihero-0.2.2/aihero/promptstash.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:52:50.070278 aihero-0.2.2/aihero.egg-info/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 06:52:50.000000 aihero-0.2.2/aihero.egg-info/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-13 06:52:50.000000 aihero-0.2.2/aihero.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-13 06:52:50.000000 aihero-0.2.2/aihero.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2023-07-13 06:52:50.000000 aihero-0.2.2/aihero.egg-info/requires.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-13 06:52:50.000000 aihero-0.2.2/aihero.egg-info/top_level.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2023-07-13 06:52:50.071494 aihero-0.2.2/setup.cfg
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.2/setup.py
```

### Comparing `aihero-0.2.1/LICENSE` & `aihero-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aihero-0.2.1/PKG-INFO` & `aihero-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihero
-Version: 0.2.1
+Version: 0.2.2
 Summary: AI Hero Python SDK
 Home-page: https://github.com/ai-hero/python-client-sdk
 Author: AI Hero Team
 Author-email: team@aihero.studio
 License: MIT
 Keywords: AI Hero,Spotcheck,MLOps,AI,Data Annotation,Labeling,Model Training,Model Serving,Model Deployment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aihero-0.2.1/aihero/client.py` & `aihero-0.2.2/aihero/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self._bearer_token = bearer_token
         self._authorization = f"Bearer {self._bearer_token}"
 
         if server_url:
             self._base_url = server_url
         else:
             self._base_url = PRODUCTION_URL
+        print(f"Connecting to {self._base_url}")
         if self._base_url.endswith("/"):
             self._base_url = self._base_url[:-1]
         self._base_url = f"{self._base_url}/api/v1"
 
     def _get_headers(self) -> dict:
         headers = {
             "Content-Type": "application/json",
```

### Comparing `aihero-0.2.1/aihero/openai_helper.py` & `aihero-0.2.2/aihero/openai_helper.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.1/aihero/project.py` & `aihero-0.2.2/aihero/project.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.1/aihero/promptstash.py` & `aihero-0.2.2/aihero/promptstash.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.1/aihero.egg-info/PKG-INFO` & `aihero-0.2.2/aihero.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihero
-Version: 0.2.1
+Version: 0.2.2
 Summary: AI Hero Python SDK
 Home-page: https://github.com/ai-hero/python-client-sdk
 Author: AI Hero Team
 Author-email: team@aihero.studio
 License: MIT
 Keywords: AI Hero,Spotcheck,MLOps,AI,Data Annotation,Labeling,Model Training,Model Serving,Model Deployment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aihero-0.2.1/setup.cfg` & `aihero-0.2.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aihero
-version = 0.2.1
+version = 0.2.2
 description = AI Hero Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ai-hero/python-client-sdk
 author = AI Hero Team
 author_email = team@aihero.studio
 license = MIT
```

