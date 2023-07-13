# Comparing `tmp/Abg-2.3.1.tar.gz` & `tmp/Abg-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.3.1.tar", last modified: Sun Jul  9 05:18:22 2023, max compression
+gzip compressed data, was "Abg-2.3.2.tar", last modified: Thu Jul 13 11:24:17 2023, max compression
```

## Comparing `Abg-2.3.1.tar` & `Abg-2.3.2.tar`

### file list

```diff
@@ -1,50 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.807145 Abg-2.3.1/Abg/
--rw-r--r--   0 root         (0) root         (0)      338 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/chat_status/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/chat_status/chat_status.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/chat_status/custom_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/get_user.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/msg_types.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/ratelimit.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/Abg/patch/decorators/
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/decorators/callback.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/decorators/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.807145 Abg-2.3.1/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5050 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      999 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5050 2023-07-09 05:18:22.815145 Abg-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2486 2023-07-09 05:18:01.000000 Abg-2.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 05:18:22.815145 Abg-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-09 05:18:01.000000 Abg-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.584144 Abg-2.3.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.572145 Abg-2.3.2/Abg/
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.576145 Abg-2.3.2/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/get_user.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/msg_types.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/helpers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.576145 Abg-2.3.2/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/decorators/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11704 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/adminsOnly.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/on_cb.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/decorators/on_cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.580145 Abg-2.3.2/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 11:24:00.000000 Abg-2.3.2/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:24:17.576145 Abg-2.3.2/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5221 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-13 11:24:17.000000 Abg-2.3.2/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5221 2023-07-13 11:24:17.584144 Abg-2.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-07-13 11:24:00.000000 Abg-2.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 11:24:17.584144 Abg-2.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-13 11:24:00.000000 Abg-2.3.2/setup.py
```

### Comparing `Abg-2.3.1/Abg/helpers/__init__.py` & `Abg-2.3.2/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/get_user.py` & `Abg-2.3.2/Abg/helpers/get_user.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/helpers.py` & `Abg-2.3.2/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/http_helper.py` & `Abg-2.3.2/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/human_read.py` & `Abg-2.3.2/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/msg_types.py` & `Abg-2.3.2/Abg/helpers/msg_types.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/parser.py` & `Abg-2.3.2/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/pyro_progress.py` & `Abg-2.3.2/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/ratelimit.py` & `Abg-2.3.2/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/helpers/string.py` & `Abg-2.3.2/Abg/helpers/string.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/inline/inline_keyboard.py` & `Abg-2.3.2/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.3.2/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/inline/reply_keyboard.py` & `Abg-2.3.2/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/bound/message.py` & `Abg-2.3.2/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/decorators/callback.py` & `Abg-2.3.2/Abg/patch/decorators/on_cb.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/decorators/command.py` & `Abg-2.3.2/Abg/patch/decorators/on_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 import typing
 from logging import getLogger
 
 import pyrogram
 from pyrogram.errors import ChatAdminRequired, FloodWait, Forbidden, SlowmodeWait
 from pyrogram.methods import Decorators
 
-HANDLER = ["/", "!", "~", ".", "+", "*"]
+HANDLER = ["/", "!", "~", ".", "+", "*", "$"]
 
 LOGGER = getLogger(__name__)
 
 
 def command(
     self,
     command: typing.Union[str, list],
     is_disabled: typing.Union[bool, bool] = False,
     pm_only: typing.Union[bool, bool] = False,
     group_only: typing.Union[bool, bool] = False,
     self_admin: typing.Union[bool, bool] = False,
     self_only: typing.Union[bool, bool] = False,
-    no_channel: typing.Union[bool, bool] = False,
     handler: typing.Optional[list] = None,
     filter: typing.Union[pyrogram.filters.Filter, pyrogram.filters.Filter] = None,
     *args,
     **kwargs,
 ):
     """
     ### `@Client.on_cmd`
```

### Comparing `Abg-2.3.1/Abg/patch/listen/listen.py` & `Abg-2.3.2/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/listen/utils.py` & `Abg-2.3.2/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/methods/edit_message_text.py` & `Abg-2.3.2/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/methods/send_as_file.py` & `Abg-2.3.2/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg/patch/methods/send_message.py` & `Abg-2.3.2/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.1/Abg.egg-info/PKG-INFO` & `Abg-2.3.2/Abg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3.1
+Version: 2.3.2
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69/Abg
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
-Description: # ᴀʙɢ :->
+Description: # ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
+        
         > 
         ### • Abg
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import CallbackQuery, Message
         from Abg import patch  # type : ignore
@@ -44,23 +45,22 @@
         
           app.run()
         ```
         >
         ### • User Rights 
         
         ```python
-        from Abg import patch  # type : ignore
-        from Abg.chat_status import adminsOnly
+        from Abg import patch  # all patch
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
         @app.on_cmd("del", group_only=True)
-        @adminsOnly("can_delete_messages")
+        @app.adminsOnly(permissions="can_delete_messages", is_both=True)
         async def del_msg(c: Client, m: Message):
             if m.reply_to_message:
                 await m.delete()
                 await c.delete_messages(
                     chat_id=m.chat.id,
                     message_ids=m.reply_to_message.id,
                 )
```

### Comparing `Abg-2.3.1/Abg.egg-info/SOURCES.txt` & `Abg-2.3.2/Abg.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 README.md
 setup.py
 Abg/__init__.py
 Abg.egg-info/PKG-INFO
 Abg.egg-info/SOURCES.txt
 Abg.egg-info/dependency_links.txt
 Abg.egg-info/top_level.txt
-Abg/chat_status/__init__.py
-Abg/chat_status/chat_status.py
-Abg/chat_status/custom_filters.py
 Abg/helpers/__init__.py
 Abg/helpers/get_user.py
 Abg/helpers/helpers.py
 Abg/helpers/http_helper.py
 Abg/helpers/human_read.py
 Abg/helpers/msg_types.py
 Abg/helpers/parser.py
@@ -22,16 +19,17 @@
 Abg/inline/inline_keyboard.py
 Abg/inline/inline_pagination_keyboard.py
 Abg/inline/reply_keyboard.py
 Abg/patch/__init__.py
 Abg/patch/bound/__init__.py
 Abg/patch/bound/message.py
 Abg/patch/decorators/__init__.py
-Abg/patch/decorators/callback.py
-Abg/patch/decorators/command.py
+Abg/patch/decorators/adminsOnly.py
+Abg/patch/decorators/on_cb.py
+Abg/patch/decorators/on_cmd.py
 Abg/patch/listen/__init__.py
 Abg/patch/listen/listen.py
 Abg/patch/listen/utils.py
 Abg/patch/methods/__init__.py
 Abg/patch/methods/edit_message_text.py
 Abg/patch/methods/send_as_file.py
 Abg/patch/methods/send_message.py
```

### Comparing `Abg-2.3.1/PKG-INFO` & `Abg-2.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3.1
+Version: 2.3.2
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69/Abg
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
-Description: # ᴀʙɢ :->
+Description: # ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
+        
         > 
         ### • Abg
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import CallbackQuery, Message
         from Abg import patch  # type : ignore
@@ -44,23 +45,22 @@
         
           app.run()
         ```
         >
         ### • User Rights 
         
         ```python
-        from Abg import patch  # type : ignore
-        from Abg.chat_status import adminsOnly
+        from Abg import patch  # all patch
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
         @app.on_cmd("del", group_only=True)
-        @adminsOnly("can_delete_messages")
+        @app.adminsOnly(permissions="can_delete_messages", is_both=True)
         async def del_msg(c: Client, m: Message):
             if m.reply_to_message:
                 await m.delete()
                 await c.delete_messages(
                     chat_id=m.chat.id,
                     message_ids=m.reply_to_message.id,
                 )
```

### Comparing `Abg-2.3.1/README.md` & `Abg-2.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# ᴀʙɢ :->
+# ᴀʙɢ :-> [![Downloads](https://static.pepy.tech/personalized-badge/abg?period=total&units=abbreviation&left_color=black&right_color=black&left_text=Downloads:)](https://pepy.tech/project/abg)
+
 > 
 ### • Abg
 
 ```python
 from pyrogram import filters, Client
 from pyrogram.types import CallbackQuery, Message
 from Abg import patch  # type : ignore
@@ -31,23 +32,22 @@
 
   app.run()
 ```
 >
 ### • User Rights 
 
 ```python
-from Abg import patch  # type : ignore
-from Abg.chat_status import adminsOnly
+from Abg import patch  # all patch
 from pyrogram.types import Message
 from pyrogram import Client
 
 app = Client("my_account")
 
 @app.on_cmd("del", group_only=True)
-@adminsOnly("can_delete_messages")
+@app.adminsOnly(permissions="can_delete_messages", is_both=True)
 async def del_msg(c: Client, m: Message):
     if m.reply_to_message:
         await m.delete()
         await c.delete_messages(
             chat_id=m.chat.id,
             message_ids=m.reply_to_message.id,
         )
```

### Comparing `Abg-2.3.1/setup.py` & `Abg-2.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="2.3.1",
+    version="2.3.2",
     description="Telegram bot helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69/Abg",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi",
     author_email="Abishnoi69@Abg.org",
```

