# Comparing `tmp/herta_villa_sdk-0.4.0.tar.gz` & `tmp/herta_villa_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.4.0.tar", last modified: Tue Jul 11 03:10:57 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.5.0.tar", last modified: Thu Jul 13 05:07:03 2023, max compression
```

## Comparing `herta_villa_sdk-0.4.0.tar` & `herta_villa_sdk-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1069 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/LICENSE
--rw-r--r--   0        0        0     3954 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/README.md
--rw-r--r--   0        0        0      555 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/__init__.py
--rw-r--r--   0        0        0      782 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/auth.py
--rw-r--r--   0        0        0     1387 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/base.py
--rw-r--r--   0        0        0      520 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/emoticon.py
--rw-r--r--   0        0        0     2174 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/member.py
--rw-r--r--   0        0        0     2710 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/message.py
--rw-r--r--   0        0        0     4422 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/role.py
--rw-r--r--   0        0        0     4190 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/room.py
--rw-r--r--   0        0        0      645 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/villa.py
--rw-r--r--   0        0        0     7235 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/bot.py
--rw-r--r--   0        0        0     5398 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     3799 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1414 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/types.py
--rw-r--r--   0        0        0     6280 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/model.py
--rw-r--r--   0        0        0     2602 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/server.py
--rw-r--r--   0        0        0      564 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/version.py
--rw-r--r--   0        0        0     2144 2023-07-11 03:10:57.239067 herta_villa_sdk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      528 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/tests/test_utils.py
--rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 herta_villa_sdk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4060 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/README.md
+-rw-r--r--   0        0        0      668 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1387 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      520 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0     2174 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2710 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4422 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4190 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      645 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     7235 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     5398 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/event.py
+-rw-r--r--   0        0        0      738 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     3799 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1414 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6280 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/model.py
+-rw-r--r--   0        0        0      970 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/aiohttp.py
+-rw-r--r--   0        0        0     1548 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/fastapi.py
+-rw-r--r--   0        0        0     2888 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/internal.py
+-rw-r--r--   0        0        0      564 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/version.py
+-rw-r--r--   0        0        0     2234 2023-07-13 05:07:03.270099 herta_villa_sdk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-07-13 05:06:36.226119 herta_villa_sdk-0.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4818 1970-01-01 00:00:00.000000 herta_villa_sdk-0.5.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.4.0/README.md` & `herta_villa_sdk-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # Herta-villa-SDK
 
-[![license](https://img.shields.io/github/license/MingxuanGame/Herta-villa-SDK)](https://github.com/MingxuanGame/Herta-villa-SDK/blob/master/LICENSE)
+[![license](https://img.shields.io/github/license/Herta-villa/Herta-villa-SDK)](https://github.com/Herta-villa/Herta-villa-SDK/blob/master/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/herta-villa-sdk)](https://pypi.python.org/pypi/herta-villa-sdk)
 ![python version](https://img.shields.io/badge/Python-3.8+-green)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 大别野「黑塔」Python SDK
 
 ## 特性
 
-- `aiohttp` 客户端+服务端，完整异步支持
+- 多种服务器后端（内置 `aiohttp` 和 `fastapi` 后端），完整异步支持
 - 完整类型注解支持
 - ...
 
 ## 安装
 
 ```shell
 pip install herta-villa-sdk
 ```
 
+FastAPI 后端支持:
+
+```shell
+pip install herta-villa-sdk[fastapi]
+```
+
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
 from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
 
@@ -92,15 +98,15 @@
 - [x] [CreateRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot) 大别野添加机器人实例
 - [x] [DeleteRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot) 大别野删除机器人实例
 - [x] [AddQuickEmoticon](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon) 用户使用表情回复消息表态
 - [ ] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
 
 ## Bug 反馈及建议
 
-大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/MingxuanGame/Herta-villa-SDK/issues/new) 提出，感谢支持！
+大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/Herta-villa/Herta-villa-SDK/issues/new) 提出，感谢支持！
 
 ## 相关项目
 
 - [CMHopeSunshine/villa-py](https://github.com/CMHopeSunshine/villa-py) 米游社大别野 Bot Python SDK（非官方）
 
 ## 交流
```

### Comparing `herta_villa_sdk-0.4.0/hertavilla/__init__.py` & `herta_villa_sdk-0.5.0/hertavilla/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,9 +13,14 @@
     MentionedRobot as MentionedRobot,
     MentionedUser as MentionedUser,
     MessageChain as MessageChain,
     Post as Post,
     Quote as Quote,
     VillaRoomLink as VillaRoomLink,
 )
-from .server import run as run
+from .server import (
+    AIOHTTPBackend as AIOHTTPBackend,
+    get_backend as get_backend,
+    init_backend as init_backend,
+    run as run,
+)
 from .version import __version__ as __version__
```

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/auth.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/auth.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/base.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/base.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/emoticon.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/emoticon.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/member.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/member.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/message.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/message.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/role.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/role.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/room.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/room.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/apis/villa.py` & `herta_villa_sdk-0.5.0/hertavilla/apis/villa.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/bot.py` & `herta_villa_sdk-0.5.0/hertavilla/bot.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/event.py` & `herta_villa_sdk-0.5.0/hertavilla/event.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/exception.py` & `herta_villa_sdk-0.5.0/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/match.py` & `herta_villa_sdk-0.5.0/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/message/chain.py` & `herta_villa_sdk-0.5.0/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/message/image.py` & `herta_villa_sdk-0.5.0/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/message/post.py` & `herta_villa_sdk-0.5.0/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/message/text.py` & `herta_villa_sdk-0.5.0/hertavilla/message/text.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/model.py` & `herta_villa_sdk-0.5.0/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/typing.py` & `herta_villa_sdk-0.5.0/hertavilla/typing.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/hertavilla/utils.py` & `herta_villa_sdk-0.5.0/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/tests/test_utils.py` & `herta_villa_sdk-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.4.0/PKG-INFO` & `herta_villa_sdk-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
-Project-URL: Homepage, https://github.com/MingxuanGame/Herta-villa-SDK
-Project-URL: Documentation, https://github.com/MingxuanGame/Herta-villa-SDK
-Project-URL: Repository, https://github.com/MingxuanGame/Herta-villa-SDK
-Project-URL: Bug tracker, https://github.com/MingxuanGame/Herta-villa-SDK/issues
+Project-URL: Homepage, https://github.com/Herta-villa/Herta-villa-SDK
+Project-URL: Documentation, https://github.com/Herta-villa/Herta-villa-SDK
+Project-URL: Repository, https://github.com/Herta-villa/Herta-villa-SDK
+Project-URL: Bug tracker, https://github.com/Herta-villa/Herta-villa-SDK/issues
 Requires-Python: >=3.8
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: pydantic<2.0,>=1.10.8
+Requires-Dist: fastapi>=0.100.0; extra == "fastapi"
+Requires-Dist: uvicorn>=0.22.0; extra == "fastapi"
+Provides-Extra: fastapi
 Description-Content-Type: text/markdown
 
 # Herta-villa-SDK
 
-[![license](https://img.shields.io/github/license/MingxuanGame/Herta-villa-SDK)](https://github.com/MingxuanGame/Herta-villa-SDK/blob/master/LICENSE)
+[![license](https://img.shields.io/github/license/Herta-villa/Herta-villa-SDK)](https://github.com/Herta-villa/Herta-villa-SDK/blob/master/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/herta-villa-sdk)](https://pypi.python.org/pypi/herta-villa-sdk)
 ![python version](https://img.shields.io/badge/Python-3.8+-green)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 大别野「黑塔」Python SDK
 
 ## 特性
 
-- `aiohttp` 客户端+服务端，完整异步支持
+- 多种服务器后端（内置 `aiohttp` 和 `fastapi` 后端），完整异步支持
 - 完整类型注解支持
 - ...
 
 ## 安装
 
 ```shell
 pip install herta-villa-sdk
 ```
 
+FastAPI 后端支持:
+
+```shell
+pip install herta-villa-sdk[fastapi]
+```
+
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
 from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
 
@@ -108,15 +117,15 @@
 - [x] [CreateRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot) 大别野添加机器人实例
 - [x] [DeleteRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot) 大别野删除机器人实例
 - [x] [AddQuickEmoticon](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon) 用户使用表情回复消息表态
 - [ ] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
 
 ## Bug 反馈及建议
 
-大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/MingxuanGame/Herta-villa-SDK/issues/new) 提出，感谢支持！
+大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/Herta-villa/Herta-villa-SDK/issues/new) 提出，感谢支持！
 
 ## 相关项目
 
 - [CMHopeSunshine/villa-py](https://github.com/CMHopeSunshine/villa-py) 米游社大别野 Bot Python SDK（非官方）
 
 ## 交流
```

