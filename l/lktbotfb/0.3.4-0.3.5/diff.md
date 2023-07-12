# Comparing `tmp/lktbotfb-0.3.4.tar.gz` & `tmp/lktbotfb-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.3.4.tar", last modified: Tue Jul 11 18:10:49 2023, max compression
+gzip compressed data, was "lktbotfb-0.3.5.tar", last modified: Wed Jul 12 22:52:47 2023, max compression
```

## Comparing `lktbotfb-0.3.4.tar` & `lktbotfb-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:10:49.909997 lktbotfb-0.3.4/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-11 18:10:49.908995 lktbotfb-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.4/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:10:49.910994 lktbotfb-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-11 18:09:44.000000 lktbotfb-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:10:49.855996 lktbotfb-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 18:10:49.868997 lktbotfb-0.3.4/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.4/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8445 2023-07-11 18:09:13.000000 lktbotfb-0.3.4/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:10:49.905996 lktbotfb-0.3.4/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-11 18:10:49.000000 lktbotfb-0.3.4/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-11 18:10:49.000000 lktbotfb-0.3.4/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:10:49.000000 lktbotfb-0.3.4/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 18:10:49.000000 lktbotfb-0.3.4/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 18:10:49.000000 lktbotfb-0.3.4/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.598469 lktbotfb-0.3.5/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-12 22:52:47.597469 lktbotfb-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.5/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 22:52:47.599470 lktbotfb-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-12 22:51:31.000000 lktbotfb-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.513533 lktbotfb-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.548473 lktbotfb-0.3.5/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.5/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     8743 2023-07-12 22:50:47.000000 lktbotfb-0.3.5/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:47.593467 lktbotfb-0.3.5/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 22:52:47.000000 lktbotfb-0.3.5/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.3.4/LICENSE` & `lktbotfb-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.3.4/PKG-INFO` & `lktbotfb-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.4
+Version: 0.3.5
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.3.4/setup.py` & `lktbotfb-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.3.4',
+  version='0.3.5',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.3.4/src/botfb/mylib.py` & `lktbotfb-0.3.5/src/botfb/mylib.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,53 +155,58 @@
 
 
 
 start_event{}
 
 
 def post_facebook_message(fbid, received_message):
-    talks = received_message
-    reply = funme(talks)
-    talks += reply
 
 
-    talks_text = reply
+    global talks_text
+
+    if 'attachments' in received_message and received_message['attachments'][0]['type'] == 'image':
+        reply = "شكراً على الإعجاب!"
+        talks_text = reply
+    elif 'text' in received_message:
+        talks = received_message['text']
+        reply = tempmail_bot(talks)
+        talks_text = reply
+    else:
+        talks_text = ""  # Default value if no match in cases
 
     post_message_url = f'https://graph.facebook.com/v2.6/me/messages?access_token={ACCESS_TOKEN}'
     response_msg = json.dumps({"message": {"text": talks_text}, "recipient": {"id": fbid}})
     status = requests.post(post_message_url, headers={"Content-Type": "application/json"}, data=response_msg)
     pprint(status.json())
 
-
 class YoMamaBotView(generic.View):
     def get(self, request, *args, **kwargs):
-        if self.request.GET['hub.verify_token'] == VERYFY_TOKEN:
+        if self.request.GET['hub.verify_token'] == VERIFY_TOKEN:
             return HttpResponse(self.request.GET['hub.challenge'])
         else:
             return HttpResponse('Error, invalid token')
 
     @method_decorator(csrf_exempt)
     def dispatch(self, request, *args, **kwargs):
-        return generic.View.dispatch(self, request, *args, **kwargs)
+        return super().dispatch(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
-        incoming_message = json.loads(self.request.body.decode('utf-8'))
+        incoming_message = json.loads(request.body.decode('utf-8'))
 
         for entry in incoming_message['entry']:
             for message in entry['messaging']:
                 if 'message' in message:
                     pprint(message)
 
-                    received_message = message['message']['text']
+                    received_message = message['message']
                     sender_id = message['sender']['id']
 
                     post_facebook_message(sender_id, received_message)
 
         return HttpResponse()
-
 ''')
         file_view.close()
 
         def replace_word_in_file_view(file_path, old_word, new_word):
             try:
                 with open(file_path, 'r',encoding='utf-8') as file:
                     content = file.read()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lktbotfb-0.3.4/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.3.5/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.4
+Version: 0.3.5
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

