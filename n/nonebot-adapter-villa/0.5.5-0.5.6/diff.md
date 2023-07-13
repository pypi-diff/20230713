# Comparing `tmp/nonebot_adapter_villa-0.5.5.tar.gz` & `tmp/nonebot_adapter_villa-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.5.5.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.5.6.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.5.5.tar` & `nonebot_adapter_villa-0.5.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/LICENSE
--rw-r--r--   0        0        0     6796 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/README.md
--rw-r--r--   0        0        0      235 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10977 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0     2911 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/client.pyi
--rw-r--r--   0        0        0    12460 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9459 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    13338 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      649 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11651 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0    10115 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1435 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/LICENSE
+-rw-r--r--   0        0        0     6796 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/README.md
+-rw-r--r--   0        0        0      235 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10977 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     2911 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    12460 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9443 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    13338 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      649 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11651 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0    10115 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1435 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-13 15:07:19.861204 nonebot_adapter_villa-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.6/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.5.5/LICENSE` & `nonebot_adapter_villa-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/README.md` & `nonebot_adapter_villa-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/client.pyi` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,14 @@
     "RoomType",
     "RoomDefaultNotifyType",
     "SendMsgAuthRange",
     "GroupRoom",
     "ListRoomType",
     "CreateRoomType",
     "CreateRoomDefaultNotifyType",
-    "ListRoom",
     "Group",
     "RoomSort",
     "MemberRole",
     "PermissionDetail",
     "MemberRoleDetail",
     "RoleType",
     "Permission",
```

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.5/pyproject.toml` & `nonebot_adapter_villa-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.5.5"
+version = "0.5.6"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.5.5/PKG-INFO` & `nonebot_adapter_villa-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.5.5
+Version: 0.5.6
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.6 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

