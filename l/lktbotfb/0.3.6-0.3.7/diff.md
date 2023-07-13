# Comparing `tmp/lktbotfb-0.3.6.tar.gz` & `tmp/lktbotfb-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.3.6.tar", last modified: Wed Jul 12 23:04:23 2023, max compression
+gzip compressed data, was "lktbotfb-0.3.7.tar", last modified: Thu Jul 13 00:39:13 2023, max compression
```

## Comparing `lktbotfb-0.3.6.tar` & `lktbotfb-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.324393 lktbotfb-0.3.6/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-12 23:04:23.322393 lktbotfb-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.6/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 23:04:23.325394 lktbotfb-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-12 23:03:27.000000 lktbotfb-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.269140 lktbotfb-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.282140 lktbotfb-0.3.6/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.6/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8829 2023-07-12 23:02:55.000000 lktbotfb-0.3.6/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.318879 lktbotfb-0.3.6/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.597291 lktbotfb-0.3.7/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-13 00:39:13.595306 lktbotfb-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.7/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 00:39:13.597291 lktbotfb-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-13 00:38:21.000000 lktbotfb-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.512057 lktbotfb-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.552714 lktbotfb-0.3.7/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.7/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     8829 2023-07-12 23:27:28.000000 lktbotfb-0.3.7/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.592295 lktbotfb-0.3.7/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.3.6/LICENSE` & `lktbotfb-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.3.6/PKG-INFO` & `lktbotfb-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.6
+Version: 0.3.7
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.3.6/setup.py` & `lktbotfb-0.3.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.3.6',
+  version='0.3.7',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.3.6/src/botfb/mylib.py` & `lktbotfb-0.3.7/src/botfb/mylib.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 from django.views.decorators.csrf import csrf_exempt
 from django.utils.decorators import method_decorator
 from django.http.response import HttpResponse
 import time
 
 
 ACCESS_TOKEN=
-VERYFY_TOKEN=
+VERIFY_TOKEN=
 
 
 
 start_event{}
 
 
 def post_facebook_message(fbid, received_message):
```

### Comparing `lktbotfb-0.3.6/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.3.7/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.6
+Version: 0.3.7
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

