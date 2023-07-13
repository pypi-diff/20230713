# Comparing `tmp/mutual-0.0.3.tar.gz` & `tmp/mutual-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.0.3.tar", last modified: Thu Jul 13 02:57:36 2023, max compression
+gzip compressed data, was "mutual-0.0.4.tar", last modified: Thu Jul 13 03:46:59 2023, max compression
```

## Comparing `mutual-0.0.3.tar` & `mutual-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 02:57:36.720482 mutual-0.0.3/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-12 18:54:58.000000 mutual-0.0.3/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     1786 2023-07-13 02:57:36.720209 mutual-0.0.3/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     1359 2023-07-13 01:25:22.000000 mutual-0.0.3/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 02:57:36.718676 mutual-0.0.3/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      615 2023-07-13 02:56:49.000000 mutual-0.0.3/mutual/Auth.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1872 2023-07-12 21:23:23.000000 mutual-0.0.3/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1485 2023-07-12 21:23:32.000000 mutual-0.0.3/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)       74 2023-07-12 21:58:57.000000 mutual-0.0.3/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 02:57:36.719752 mutual-0.0.3/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1786 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      242 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-13 02:57:36.720539 mutual-0.0.3/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-13 02:57:35.000000 mutual-0.0.3/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 03:46:59.504562 mutual-0.0.4/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-13 03:33:58.000000 mutual-0.0.4/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1831 2023-07-13 03:46:59.504316 mutual-0.0.4/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1404 2023-07-13 03:44:59.000000 mutual-0.0.4/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 03:46:59.502982 mutual-0.0.4/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      615 2023-07-13 03:33:58.000000 mutual-0.0.4/mutual/Auth.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1888 2023-07-13 03:45:58.000000 mutual-0.0.4/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1490 2023-07-13 03:45:25.000000 mutual-0.0.4/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)       74 2023-07-13 03:33:58.000000 mutual-0.0.4/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 03:46:59.504000 mutual-0.0.4/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1831 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      257 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-13 03:46:59.504610 mutual-0.0.4/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-13 03:46:57.000000 mutual-0.0.4/setup.py
```

### Comparing `mutual-0.0.3/LICENSE.txt` & `mutual-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.0.3/PKG-INFO` & `mutual-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,7 +64,11 @@
 
 # to print the bot_id
 print(mutual.bot_id)
 
 # you can import the functions directly like so
 from mutual import Bot, Auth, Chat
 ```
+
+python setup.py sdist
+
+twine upload dist/*
```

### Comparing `mutual-0.0.3/README.md` & `mutual-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,8 +49,12 @@
     print(message)
 
 # to print the bot_id
 print(mutual.bot_id)
 
 # you can import the functions directly like so
 from mutual import Bot, Auth, Chat
-```
+```
+
+python setup.py sdist
+
+twine upload dist/*
```

### Comparing `mutual-0.0.3/mutual/Auth.py` & `mutual-0.0.4/mutual/Auth.py`

 * *Files identical despite different names*

### Comparing `mutual-0.0.3/mutual/Bot.py` & `mutual-0.0.4/mutual/Bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,40 +7,40 @@
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     return response.json()
 
-def getBot(bot_id):
-    url = f"https://api-agent.mutuai.io/api/bots/{bot_id}"
+def getBots(bot_id):
+    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     return response.json()
 
 def createBot(bot_id, bot_name, bot_org):
     url = "https://api-agent.mutuai.io/api/bots"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
-        "bot_id": bot_id,
+        "bot_id": str(bot_id),
         "bot_name": bot_name,
         "bot_org": bot_org
     }
     response = requests.post(url, data=json.dumps(data), headers=headers)
     response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     return response.json()
 
 def updateBot(bot_id, bot_name=None, bot_org=None):
-    url = f"https://api-agent.mutuai.io/api/bots/{bot_id}"
+    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "bot_org": bot_org
```

### Comparing `mutual-0.0.3/mutual/Chat.py` & `mutual-0.0.4/mutual/Chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     url = "https://api-agent.mutuai.io/api/chat"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "content": content,
-        "bot_id": bot_id,
+        "bot_id": str(bot_id),
         "username": username
     }
 
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code == 200:
         for line in response.iter_lines():
```

### Comparing `mutual-0.0.3/mutual.egg-info/PKG-INFO` & `mutual-0.0.4/mutual.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,7 +64,11 @@
 
 # to print the bot_id
 print(mutual.bot_id)
 
 # you can import the functions directly like so
 from mutual import Bot, Auth, Chat
 ```
+
+python setup.py sdist
+
+twine upload dist/*
```

### Comparing `mutual-0.0.3/setup.py` & `mutual-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.0.3',  # beta
+    version='0.0.4',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

