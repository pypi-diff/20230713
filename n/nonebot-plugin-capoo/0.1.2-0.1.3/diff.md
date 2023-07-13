# Comparing `tmp/nonebot_plugin_capoo-0.1.2.tar.gz` & `tmp/nonebot_plugin_capoo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_capoo-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_capoo-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_capoo-0.1.2.tar` & `nonebot_plugin_capoo-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-10 14:29:30.893785 nonebot_plugin_capoo-0.1.2/LICENSE
--rw-r--r--   0        0        0     3840 2023-07-10 14:29:30.893785 nonebot_plugin_capoo-0.1.2/README.md
--rw-r--r--   0        0        0     4478 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/__init__.py
--rw-r--r--   0        0        0      520 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/config.py
--rw-r--r--   0        0        0     2805 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/download.py
--rw-r--r--   0        0        0      469 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/sqlite.py
--rw-r--r--   0        0        0      603 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3934 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/README.md
+-rw-r--r--   0        0        0     4524 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/config.py
+-rw-r--r--   0        0        0     2805 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/download.py
+-rw-r--r--   0        0        0      469 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/sqlite.py
+-rw-r--r--   0        0        0      603 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_capoo-0.1.2/LICENSE` & `nonebot_plugin_capoo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.2/README.md` & `nonebot_plugin_capoo-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `capoo` | 群员 | 否 | 群聊 | 随机发送一张 capoo 的表情包 |
-| `添加capoo` | 超管 | 否 | 群聊 | 让 bot 存储图片 |
+| `添加capoo` | 群管 | 否 | 群聊 | 让 bot 存储图片 |
 
 注意 `添加capoo` 指令在配置项 `capoo_download` 为 False 时将不生效。
 
 `添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下，你可以放置图片在这个文件夹里面，插件启动后会检验这里面的图片文件。
 
 ### 效果图
 #### `capoo` 指令
@@ -103,8 +103,9 @@
 
 <img src="./docs/preview3.jpg" style="zoom:30%;" />
 
 ## TODO
 - [x] 指令触发 bot 发送图片
 - [x] 在 QQ 上让 bot 存储 capoo 图片
 - [x] 每次存储图片，判断图片是否已经存在，避免重复加入
-- [ ] 指定某个序号的图片发送
+- [ ] 指定某个序号的图片发送
+- [ ] 由该插件衍生成一个模板插件，即仅需修改参数就能发送别的图片
```

#### html2text {}

```diff
@@ -24,17 +24,18 @@
 ä¸ï¼æ¯å½åçè¿ç¨ä»£ç åºç«ç¹ï¼æä»¥ä¸ç¨æå¿è¢«å¢äºèåä¸åºå¾çã
 åå¦ä½ å¼å¯äºæ¬å°å¾çå­å¨ï¼æä»¶ä¼èªå·±ä» [AC Git](https://
 git.acwing.com/HuParry/capoo)
 å¾æºéä¸è½½ãä½ ä¹å¯ä»¥èªè¡æå¨ä¸è½½ï¼æ¾ç½®å¨ä½ ç bot
 é¡¹ç®æ ¹ç®å½ä¸ç `data/capoo/picture` æä»¶å¤¹ä¸ã ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:|:----:| | `capoo` | ç¾¤å | å¦ | ç¾¤è | éæºåéä¸å¼  capoo
-çè¡¨æå | | `æ·»å capoo` | è¶ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
+çè¡¨æå | | `æ·»å capoo` | ç¾¤ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
 æ³¨æ `æ·»å capoo` æä»¤å¨éç½®é¡¹ `capoo_download` ä¸º False
 æ¶å°ä¸çæã `æ·»å capoo` æä»¤ä¼å°å¾çå¨å­è³ `data/capoo/
 your_picture`
 ä¸ï¼ä½ å¯ä»¥æ¾ç½®å¾çå¨è¿ä¸ªæä»¶å¤¹éé¢ï¼æä»¶å¯å¨åä¼æ£éªè¿éé¢çå¾çæä»¶ã
 ### ææå¾ #### `capoo` æä»¤ [./docs/preview.jpg] #### `æ·»å capoo`
 æä»¤ [./docs/preview2.jpg] [./docs/preview3.jpg] ## TODO - [x] æä»¤è§¦å
 bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
 æ¯æ¬¡å­å¨å¾çï¼å¤æ­å¾çæ¯å¦å·²ç»å­å¨ï¼é¿åéå¤å å¥ - [ ]
-æå®æä¸ªåºå·çå¾çåé
+æå®æä¸ªåºå·çå¾çåé - [ ]
+ç±è¯¥æä»¶è¡çæä¸ä¸ªæ¨¡æ¿æä»¶ï¼å³ä»éä¿®æ¹åæ°å°±è½åéå«çå¾ç
```

### Comparing `nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/__init__.py` & `nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .config import Config, capoo_path, capoo_pic2_path, capoo_pic2
 from httpx import AsyncClient
 from .download import *
 import asyncio
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP, MessageSegment, Message
+from nonebot.adapters.onebot.v11 import MessageSegment, Message
+from nonebot.adapters.onebot.v11 import GROUP, GROUP_ADMIN, GROUP_OWNER
 from nonebot.plugin import on_fullmatch, on_command
-from nonebot.permission import SUPERUSER
 from nonebot.log import logger
 from nonebot import get_driver
 import random
 import os
 from io import BytesIO
 from nonebot.plugin import PluginMetadata
 from nonebot.params import Arg
@@ -18,15 +18,17 @@
     description = "发送capoo指令后bot会随机发出一张capoo的可爱表情包",
     usage = "使用命令：capoo",
     type="application",
     homepage="https://github.com/HuParry/nonebot-plugin-capoo",
     config=Config,
     supported_adapters = {"nonebot.adapters.onebot.v11"},
 )
-capoo_download = Config.parse_obj(get_driver().config.dict()).capoo_download
+capoo_config = Config.parse_obj(get_driver().config.dict())
+capoo_download = capoo_config.capoo_download
+
 driver = get_driver()
 @driver.on_startup
 async def _():
     global capoo_download
     if capoo_download:
         logger.info("配置项选择了本地存储图片，正在检查资源文件...")
         asyncio.create_task(check_resources())
@@ -64,15 +66,15 @@
             await picture.send(MessageSegment.image(picbytes))
         except:
             await picture.send(f'capoo出不来了，稍后再试试吧~')
 
 def reply_rule():
     return capoo_download
 
-add = on_fullmatch('添加capoo', rule=reply_rule, permission=SUPERUSER, priority=1, block=True)
+add = on_fullmatch('添加capoo', rule=reply_rule, permission= GROUP_ADMIN | GROUP_OWNER, priority=1, block=True)
 @add.got("pic", prompt="请发送图片！")
 async def add_pic(pic_list: Message = Arg('pic')):
     conn = sqlite3.connect(capoo_path / 'md5.db')
     cursor = conn.cursor()
     cursor.execute('''
         CREATE TABLE IF NOT EXISTS Picture (
             md5 TEXT PRIMARY KEY,
```

### Comparing `nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/config.py` & `nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/download.py` & `nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.2/pyproject.toml` & `nonebot_plugin_capoo-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-capoo"
-version = "0.1.2"
+version = "0.1.3"
 description = "一个发送 capoo 表情包的插件"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_capoo"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-capoo"
 repository = "https://github.com/HuParry/nonebot-plugin-capoo"
```

### Comparing `nonebot_plugin_capoo-0.1.2/PKG-INFO` & `nonebot_plugin_capoo-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-capoo
-Version: 0.1.2
+Version: 0.1.3
 Summary: 一个发送 capoo 表情包的插件
 Home-page: https://github.com/HuParry/nonebot-plugin-capoo
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -106,15 +106,15 @@
 
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `capoo` | 群员 | 否 | 群聊 | 随机发送一张 capoo 的表情包 |
-| `添加capoo` | 超管 | 否 | 群聊 | 让 bot 存储图片 |
+| `添加capoo` | 群管 | 否 | 群聊 | 让 bot 存储图片 |
 
 注意 `添加capoo` 指令在配置项 `capoo_download` 为 False 时将不生效。
 
 `添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下，你可以放置图片在这个文件夹里面，插件启动后会检验这里面的图片文件。
 
 ### 效果图
 #### `capoo` 指令
@@ -126,7 +126,8 @@
 <img src="./docs/preview3.jpg" style="zoom:30%;" />
 
 ## TODO
 - [x] 指令触发 bot 发送图片
 - [x] 在 QQ 上让 bot 存储 capoo 图片
 - [x] 每次存储图片，判断图片是否已经存在，避免重复加入
 - [ ] 指定某个序号的图片发送
+- [ ] 由该插件衍生成一个模板插件，即仅需修改参数就能发送别的图片
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.3 Summary:
 ä¸ä¸ªåé capoo è¡¨æåçæä»¶ Home-page: https://github.com/HuParry/
 nonebot-plugin-capoo License: MIT Author: HuParry Author-email:
 huparry@outlook.com Requires-Python: >=3.8 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: asyncio (>=3.4.3)
@@ -35,17 +35,18 @@
 ä¸ï¼æ¯å½åçè¿ç¨ä»£ç åºç«ç¹ï¼æä»¥ä¸ç¨æå¿è¢«å¢äºèåä¸åºå¾çã
 åå¦ä½ å¼å¯äºæ¬å°å¾çå­å¨ï¼æä»¶ä¼èªå·±ä» [AC Git](https://
 git.acwing.com/HuParry/capoo)
 å¾æºéä¸è½½ãä½ ä¹å¯ä»¥èªè¡æå¨ä¸è½½ï¼æ¾ç½®å¨ä½ ç bot
 é¡¹ç®æ ¹ç®å½ä¸ç `data/capoo/picture` æä»¶å¤¹ä¸ã ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:|:----:| | `capoo` | ç¾¤å | å¦ | ç¾¤è | éæºåéä¸å¼  capoo
-çè¡¨æå | | `æ·»å capoo` | è¶ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
+çè¡¨æå | | `æ·»å capoo` | ç¾¤ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
 æ³¨æ `æ·»å capoo` æä»¤å¨éç½®é¡¹ `capoo_download` ä¸º False
 æ¶å°ä¸çæã `æ·»å capoo` æä»¤ä¼å°å¾çå¨å­è³ `data/capoo/
 your_picture`
 ä¸ï¼ä½ å¯ä»¥æ¾ç½®å¾çå¨è¿ä¸ªæä»¶å¤¹éé¢ï¼æä»¶å¯å¨åä¼æ£éªè¿éé¢çå¾çæä»¶ã
 ### ææå¾ #### `capoo` æä»¤ [./docs/preview.jpg] #### `æ·»å capoo`
 æä»¤ [./docs/preview2.jpg] [./docs/preview3.jpg] ## TODO - [x] æä»¤è§¦å
 bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
 æ¯æ¬¡å­å¨å¾çï¼å¤æ­å¾çæ¯å¦å·²ç»å­å¨ï¼é¿åéå¤å å¥ - [ ]
-æå®æä¸ªåºå·çå¾çåé
+æå®æä¸ªåºå·çå¾çåé - [ ]
+ç±è¯¥æä»¶è¡çæä¸ä¸ªæ¨¡æ¿æä»¶ï¼å³ä»éä¿®æ¹åæ°å°±è½åéå«çå¾ç
```

