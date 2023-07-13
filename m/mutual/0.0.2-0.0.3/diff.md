# Comparing `tmp/mutual-0.0.2.tar.gz` & `tmp/mutual-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.0.2.tar", last modified: Thu Jul 13 01:30:05 2023, max compression
+gzip compressed data, was "mutual-0.0.3.tar", last modified: Thu Jul 13 02:57:36 2023, max compression
```

## Comparing `mutual-0.0.2.tar` & `mutual-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 01:30:05.902041 mutual-0.0.2/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-12 18:54:58.000000 mutual-0.0.2/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     1786 2023-07-13 01:30:05.901697 mutual-0.0.2/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     1359 2023-07-13 01:25:22.000000 mutual-0.0.2/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 01:30:05.900452 mutual-0.0.2/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      618 2023-07-12 21:23:18.000000 mutual-0.0.2/mutual/Auth.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1872 2023-07-12 21:23:23.000000 mutual-0.0.2/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1485 2023-07-12 21:23:32.000000 mutual-0.0.2/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)       74 2023-07-12 21:58:57.000000 mutual-0.0.2/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 01:30:05.901431 mutual-0.0.2/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1786 2023-07-13 01:30:05.000000 mutual-0.0.2/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      242 2023-07-13 01:30:05.000000 mutual-0.0.2/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-13 01:30:05.000000 mutual-0.0.2/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-13 01:30:05.000000 mutual-0.0.2/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-13 01:30:05.000000 mutual-0.0.2/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-13 01:30:05.902094 mutual-0.0.2/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-13 01:29:18.000000 mutual-0.0.2/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 02:57:36.720482 mutual-0.0.3/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-12 18:54:58.000000 mutual-0.0.3/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1786 2023-07-13 02:57:36.720209 mutual-0.0.3/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1359 2023-07-13 01:25:22.000000 mutual-0.0.3/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 02:57:36.718676 mutual-0.0.3/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      615 2023-07-13 02:56:49.000000 mutual-0.0.3/mutual/Auth.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1872 2023-07-12 21:23:23.000000 mutual-0.0.3/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1485 2023-07-12 21:23:32.000000 mutual-0.0.3/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)       74 2023-07-12 21:58:57.000000 mutual-0.0.3/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 02:57:36.719752 mutual-0.0.3/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1786 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      242 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-13 02:57:36.000000 mutual-0.0.3/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-13 02:57:36.720539 mutual-0.0.3/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-13 02:57:35.000000 mutual-0.0.3/setup.py
```

### Comparing `mutual-0.0.2/LICENSE.txt` & `mutual-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.0.2/PKG-INFO` & `mutual-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.0.2/README.md` & `mutual-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mutual-0.0.2/mutual/Auth.py` & `mutual-0.0.3/mutual/Auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import json
 import mutual
 
-def signup(username, email):
+def signup(user_id, email):
     url = "https://api-agent.mutuai.io/api/signup"
     data = {
-        "username": username,
+        "user_id": user_id,
         "email": email
     }
 
     headers = {
         'Content-Type': 'application/json'
     }
```

### Comparing `mutual-0.0.2/mutual/Bot.py` & `mutual-0.0.3/mutual/Bot.py`

 * *Files identical despite different names*

### Comparing `mutual-0.0.2/mutual/Chat.py` & `mutual-0.0.3/mutual/Chat.py`

 * *Files identical despite different names*

### Comparing `mutual-0.0.2/mutual.egg-info/PKG-INFO` & `mutual-0.0.3/mutual.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.0.2/setup.py` & `mutual-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.0.2',  # beta
+    version='0.0.3',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

