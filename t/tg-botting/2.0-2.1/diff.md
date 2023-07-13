# Comparing `tmp/tg-botting-2.0.tar.gz` & `tmp/tg-botting-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.0.tar", last modified: Wed Jul 12 19:38:05 2023, max compression
+gzip compressed data, was "tg-botting-2.1.tar", last modified: Thu Jul 13 12:00:47 2023, max compression
```

## Comparing `tg-botting-2.0.tar` & `tg-botting-2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:38:05.357666 tg-botting-2.0/
--rw-rw-rw-   0        0        0     3405 2023-07-12 19:38:05.357076 tg-botting-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 19:38:05.357666 tg-botting-2.0/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:38:05.350094 tg-botting-2.0/tg_botting/
--rw-rw-rw-   0        0        0      771 2023-07-12 19:35:29.000000 tg-botting-2.0/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.0/tg_botting/_types.py
--rw-rw-rw-   0        0        0     1247 2023-07-12 16:09:02.000000 tg-botting-2.0/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/bot.py
--rw-rw-rw-   0        0        0    26953 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.0/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.0/tg_botting/commands.py
--rw-rw-rw-   0        0        0     7686 2023-07-12 16:20:46.000000 tg-botting-2.0/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.0/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.0/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.0/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.0/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.0/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.0/tg_botting/group.py
--rw-rw-rw-   0        0        0    19102 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/message.py
--rw-rw-rw-   0        0        0    29358 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.0/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.0/tg_botting/user.py
--rw-rw-rw-   0        0        0     1021 2023-07-12 15:20:00.000000 tg-botting-2.0/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.0/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:38:05.356078 tg-botting-2.0/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3405 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 12:00:47.120404 tg-botting-2.1/
+-rw-rw-rw-   0        0        0     3405 2023-07-13 12:00:47.104782 tg-botting-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:00:47.120404 tg-botting-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:00:47.104782 tg-botting-2.1/tg_botting/
+-rw-rw-rw-   0        0        0      796 2023-07-13 12:00:23.000000 tg-botting-2.1/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    26954 2023-07-13 11:41:53.000000 tg-botting-2.1/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1/tg_botting/group.py
+-rw-rw-rw-   0        0        0    19102 2023-07-12 16:28:14.000000 tg-botting-2.1/tg_botting/message.py
+-rw-rw-rw-   0        0        0    29358 2023-07-12 16:28:14.000000 tg-botting-2.1/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1021 2023-07-12 15:20:00.000000 tg-botting-2.1/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:00:47.104782 tg-botting-2.1/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3405 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-07-13 12:00:47.000000 tg-botting-2.1/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 12:00:46.000000 tg-botting-2.1/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.0/PKG-INFO` & `tg-botting-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.0
+Version: 2.1
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.0/README.md` & `tg-botting-2.1/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/setup.py` & `tg-botting-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/__init__.py` & `tg-botting-2.1/tg_botting/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.0'
+__version__ = '2.1'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .conversions import Converter
 from .message import *
 from .user import *
 from .utils import *
 from .permissions import *
 from .objects import *
+from .commands import *
 
 
 VersionInfo = namedtuple('VersionInfo', 'major minor micro releaselevel serial')
 
 version_info = VersionInfo(major=0, minor=11, micro=0, releaselevel='development', serial=0)
 
 try:
```

### Comparing `tg-botting-2.0/tg_botting/bot.py` & `tg-botting-2.1/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/client.py` & `tg-botting-2.1/tg_botting/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,15 +474,15 @@
                                                protect_content=protect_content, reply_to_message_id=reply_to_message_id,
                                                allow_sending_without_reply=allow_sending_without_reply,
                                                reply_markup=reply_markup, **kwargs)
             raise TGApiError('[{error_code}] {description}'.format(**res))
         if self.is_group and not as_user:
             params['from'] = self.group.dict
             params['message_id'] = res['result']['message_id']
-            params['chat'] = res['result']['chat']
+            params['chat']  = res['result']['chat']
         else:
             pass
             # params['from_id'] = self.user.id
             # params['id'] = res['response']
         return self.build_msg(params)
 
     async def add_user_token(self, token):
```

### Comparing `tg-botting-2.0/tg_botting/cog.py` & `tg-botting-2.1/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/commands.py` & `tg-botting-2.1/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/context_managers.py` & `tg-botting-2.1/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/conversions.py` & `tg-botting-2.1/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/cooldowns.py` & `tg-botting-2.1/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/exceptions.py` & `tg-botting-2.1/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/general.py` & `tg-botting-2.1/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/group.py` & `tg-botting-2.1/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/message.py` & `tg-botting-2.1/tg_botting/message.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/objects.py` & `tg-botting-2.1/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/permissions.py` & `tg-botting-2.1/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/user.py` & `tg-botting-2.1/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/utils.py` & `tg-botting-2.1/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting/view.py` & `tg-botting-2.1/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.0/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1/tg_botting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.0
+Version: 2.1
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.0/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

