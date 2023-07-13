# Comparing `tmp/tg-botting-2.1.tar.gz` & `tmp/tg-botting-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.1.tar", last modified: Thu Jul 13 12:00:47 2023, max compression
+gzip compressed data, was "tg-botting-2.1.1.tar", last modified: Thu Jul 13 14:59:43 2023, max compression
```

## Comparing `tg-botting-2.1.tar` & `tg-botting-2.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 12:00:47.120404 tg-botting-2.1/
--rw-rw-rw-   0        0        0     3405 2023-07-13 12:00:47.104782 tg-botting-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 12:00:47.120404 tg-botting-2.1/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:00:47.104782 tg-botting-2.1/tg_botting/
--rw-rw-rw-   0        0        0      796 2023-07-13 12:00:23.000000 tg-botting-2.1/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1/tg_botting/bot.py
--rw-rw-rw-   0        0        0    26954 2023-07-13 11:41:53.000000 tg-botting-2.1/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1/tg_botting/group.py
--rw-rw-rw-   0        0        0    19102 2023-07-12 16:28:14.000000 tg-botting-2.1/tg_botting/message.py
--rw-rw-rw-   0        0        0    29358 2023-07-12 16:28:14.000000 tg-botting-2.1/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1/tg_botting/user.py
--rw-rw-rw-   0        0        0     1021 2023-07-12 15:20:00.000000 tg-botting-2.1/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:00:47.104782 tg-botting-2.1/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3405 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-07-13 12:00:47.000000 tg-botting-2.1/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 14:59:43.907504 tg-botting-2.1.1/
+-rw-rw-rw-   0        0        0     3407 2023-07-13 14:59:43.907504 tg-botting-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 14:59:43.907504 tg-botting-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:59:43.907504 tg-botting-2.1.1/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-13 14:59:25.000000 tg-botting-2.1.1/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.1/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.1/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.1/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    27119 2023-07-13 14:59:13.000000 tg-botting-2.1.1/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.1/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.1/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.1/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.1/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.1/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.1/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.1/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.1/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.1/tg_botting/group.py
+-rw-rw-rw-   0        0        0    19098 2023-07-13 14:58:01.000000 tg-botting-2.1.1/tg_botting/message.py
+-rw-rw-rw-   0        0        0    29358 2023-07-12 16:28:14.000000 tg-botting-2.1.1/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.1/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.1/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1021 2023-07-12 15:20:00.000000 tg-botting-2.1.1/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.1/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:59:43.907504 tg-botting-2.1.1/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.1/PKG-INFO` & `tg-botting-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1
+Version: 2.1.1
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1/README.md` & `tg-botting-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/setup.py` & `tg-botting-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/__init__.py` & `tg-botting-2.1.1/tg_botting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.1'
+__version__ = '2.1.1'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .conversions import Converter
 from .message import *
```

### Comparing `tg-botting-2.1/tg_botting/abstract.py` & `tg-botting-2.1.1/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/bot.py` & `tg-botting-2.1.1/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/client.py` & `tg-botting-2.1.1/tg_botting/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,17 +497,21 @@
         while True:
             try:
                 lp = self.loop.create_task(self.longpoll(offset))
                 for update in updates:
                     self.handle_update(update)
                 offset, updates = await lp
             except Exception as e:
+                if self.use_stack_trace:
+                    traceback.print_exc(file=sys.stderr)
                 print('Ignoring exception in longpoll cycle:\n{}'.format(e), file=sys.stderr)
+                offset+=1
 
     def run(self, token, user_id=None, user_hash=None):
+        self.use_stack_trace = False
         self.token = token
         self.user_id = user_id
         self.user_hash = user_hash
         self.loop.create_task(self._run())
         self.loop.run_forever()
 
 # class UserClient(Client):
```

### Comparing `tg-botting-2.1/tg_botting/cog.py` & `tg-botting-2.1.1/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/commands.py` & `tg-botting-2.1.1/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/context.py` & `tg-botting-2.1.1/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/context_managers.py` & `tg-botting-2.1.1/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/conversions.py` & `tg-botting-2.1.1/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/cooldowns.py` & `tg-botting-2.1.1/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/exceptions.py` & `tg-botting-2.1.1/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/general.py` & `tg-botting-2.1.1/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/group.py` & `tg-botting-2.1.1/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/message.py` & `tg-botting-2.1.1/tg_botting/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self.forward_from_chat = Chat(data.get('forward_from_chat')) if 'forward_from_chat' in data else None
         self.message_thread_id = data.get('message_thread_id') if 'message_thread_id' in data else None
         self.forward_signature = data.get('forward_signature') if 'forward_signature' in data else None
         self.forward_sender_name = data.get('forward_sender_name') if 'forward_sender_name' in data else None
         self.forward_date = datetime.fromtimestamp(data.get('forward_date')) if 'forward_date' in data else None
         self.is_topic_message = data.get('is_topic_message') if 'is_topic_message' in data else False
         self.is_automatic_forward = data.get('is_automatic_forward') if 'is_automatic_forward' in data else False
-        self.reply_to_message = Message(data.get('is_automatic_forward')) if 'reply_to_message' in data else None
+        self.reply_to_message = Message(data.get('reply_to_message')) if 'reply_to_message' in data else None
         self.via_bot = User(data.get('via_bot')) if 'via_bot' in data else None
         self.edit_date = datetime.fromtimestamp(data.get('edit_date')) if 'edit_date' in data else None
         self.has_protected_content = data.get('has_protected_content') if 'has_protected_content' in data else False
         self.media_group_id = data.get('media_group_id') if 'media_group_id' in data else None
         self.author_signature = data.get('author_signature') if 'author_signature' in data else None
         self.text = data.get('text') if 'text' in data and data.get('text', None) is not None else None
         self.entities = [MessageEntity(r) for r in data.get('entities')] if 'entities' in data and data.get('entities',
```

### Comparing `tg-botting-2.1/tg_botting/objects.py` & `tg-botting-2.1.1/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/permissions.py` & `tg-botting-2.1.1/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/user.py` & `tg-botting-2.1.1/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/utils.py` & `tg-botting-2.1.1/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting/view.py` & `tg-botting-2.1.1/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1.1/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1
+Version: 2.1.1
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1.1/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

