# Comparing `tmp/lktbotfb-0.3.5.tar.gz` & `tmp/lktbotfb-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.3.5.tar", last modified: Wed Jul 12 22:52:47 2023, max compression
+gzip compressed data, was "lktbotfb-0.3.6.tar", last modified: Wed Jul 12 23:04:23 2023, max compression
```

## Comparing `lktbotfb-0.3.5.tar` & `lktbotfb-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.598469 lktbotfb-0.3.5/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-12 22:52:47.597469 lktbotfb-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.5/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 22:52:47.599470 lktbotfb-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-12 22:51:31.000000 lktbotfb-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.513533 lktbotfb-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.548473 lktbotfb-0.3.5/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.5/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8743 2023-07-12 22:50:47.000000 lktbotfb-0.3.5/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.593467 lktbotfb-0.3.5/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.324393 lktbotfb-0.3.6/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-12 23:04:23.322393 lktbotfb-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.6/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:04:23.325394 lktbotfb-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-12 23:03:27.000000 lktbotfb-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.269140 lktbotfb-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.282140 lktbotfb-0.3.6/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.6/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     8829 2023-07-12 23:02:55.000000 lktbotfb-0.3.6/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:04:23.318879 lktbotfb-0.3.6/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 23:04:23.000000 lktbotfb-0.3.6/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.3.5/LICENSE` & `lktbotfb-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.3.5/PKG-INFO` & `lktbotfb-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.5
+Version: 0.3.6
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.3.5/setup.py` & `lktbotfb-0.3.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.3.5',
+  version='0.3.6',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.3.5/src/botfb/mylib.py` & `lktbotfb-0.3.6/src/botfb/mylib.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         creatbotapp = f"python manage.py startapp {startapp}"
         os.system(creatbotapp)
         startapp_edit="done create a app"   
         print(startapp_edit)
         time.sleep(2)
         os.chdir(os.path.join(current_path, namebot_,startapp))
         name_urls = "urls.py"
-        with open(name_urls, 'w') as files:
+        with open(name_urls, 'w',encoding='utf-8') as files:
             files.write(
 f'''
 # yomamabot/fb_yomamabot/urls.py
 from django.urls import re_path, include
 from .views import YoMamaBotView
 urlpatterns = [
     re_path(r'^page{code_srt}/?$', YoMamaBotView.as_view()) 
@@ -44,15 +44,15 @@
 '''
             )
             files.close()
 
         os.chdir(os.path.join(current_path, namebot_, namebot_))
         files_urls = "urls.py"
 
-        with open(files_urls, 'w') as files:
+        with open(files_urls, 'w',encoding='utf-8') as files:
             files.write(
 f'''
 from django.urls import re_path, include
 from django.contrib import admin
 urlpatterns = [
     re_path(r'^admin/', admin.site.urls),
     re_path(r'^fb/', include('{startapp}.urls')),
@@ -82,20 +82,20 @@
         hostname=self.hostname
         file_path_setting =os.path.join(current_path, namebot_, namebot_)
         os.chdir(file_path_setting)
         name_setting = "settings.py"
         
         def replace_word_in_file(file_path, old_word, new_word):
             try:
-                with open(file_path, 'r') as file:
+                with open(file_path, 'r',encoding='utf-8') as file:
                     content = file.read()
     
                 modified_content = content.replace(old_word, new_word)
     
-                with open(file_path, 'w') as file:
+                with open(file_path, 'w',encoding='utf-8') as file:
                     file.write(modified_content)
     
             except FileNotFoundError:
                 print("error in this file try again")
 
         file_path = name_setting
         old_word = 'ALLOWED_HOSTS = []'
@@ -133,15 +133,15 @@
         self.replying=relkt
         replying = self.replying
         
         self.funsing=funsme
         funsing = self.funsing
         os.chdir(os.path.join(current_path, namebot_, startapp))
         file_path_view = "views.py"
-        with open(file_path_view, 'w') as file_view:
+        with open(file_path_view, 'w', encoding='utf-8') as file_view:
             file_view.write('''
 
 from django.shortcuts import render
 from pprint import pprint
 import json, requests, random, re
 from django.views import generic
 from django.views.decorators.csrf import csrf_exempt
```

### Comparing `lktbotfb-0.3.5/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.3.6/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.5
+Version: 0.3.6
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

