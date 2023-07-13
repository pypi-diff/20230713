# Comparing `tmp/nonebot_plugin_rename-1.6.0.tar.gz` & `tmp/nonebot_plugin_rename-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.6.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.6.1.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.6.0.tar` & `nonebot_plugin_rename-1.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/LICENSE
--rw-r--r--   0        0        0     6175 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/README.md
--rw-r--r--   0        0        0      542 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      479 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/exam_time.py
--rw-r--r--   0        0        0      689 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0     1763 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      450 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0     1500 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/mhy_time.py
--rw-r--r--   0        0        0      601 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      307 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      697 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/year_time.py
--rw-r--r--   0        0        0      621 2023-06-28 03:36:56.252143 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8733 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      264 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      970 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1528 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      400 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      700 2023-06-28 03:36:56.268142 nonebot_plugin_rename-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     7080 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/LICENSE
+-rw-r--r--   0        0        0     6175 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/README.md
+-rw-r--r--   0        0        0      542 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      479 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/exam_time.py
+-rw-r--r--   0        0        0      689 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0     1763 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0     1483 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/mhy_time.py
+-rw-r--r--   0        0        0      601 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      307 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      697 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/year_time.py
+-rw-r--r--   0        0        0      621 2023-07-13 08:57:00.985990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8754 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      264 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      970 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1528 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      700 2023-07-13 08:57:01.001990 nonebot_plugin_rename-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7080 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.6.0/LICENSE` & `nonebot_plugin_rename-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/README.md` & `nonebot_plugin_rename-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/__init__.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.plugin import PluginMetadata
 
 from .config import Config
 from .main import *  # noqa
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 __plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_rename",
     description="用于更改qq机器人的群名片，内置多种有趣名片",
     usage="查看本仓库readme",
     supported_adapters={"~onebot.v11"},
     type="application",
     config=Config,
```

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/exam_time.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/exam_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/mhy_time.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/mhy_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         while during_time <= 0:
             during_time += 42 * 24 * 60 * 60 * 1000
             index += 1
         version = (self.version_list[index] / 10).__round__(1)
         days = int(during_time / (24 * 3600 * 1000))
         leave1 = during_time % (24 * 3600 * 1000)
         hours = int(leave1 / (3600 * 1000))
-        leave2 = leave1 % (3600 * 1000)
-        minutes = int(leave2 / (60 * 1000))
-        return f"离{self.name}{version}版本还有{days}天{hours}小时{minutes}分钟"
+        # leave2 = leave1 % (3600 * 1000)
+        # minutes = int(leave2 / (60 * 1000))
+        return f"离{self.name}{version}还有{days}天{hours}小时"
 
 
 starrail = MhyGameVersion(
     "2023-6-7 11:00:00",
     [11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24],
     "崩铁",
 ).get_version_time
```

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/card/year_time.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/card/year_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/config.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .config import env_config
 from .utils import card_list, choice_card, generate_card_image, read_yaml, write_yaml
 
 require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler  # noqa
+from nonebot_plugin_apscheduler import scheduler  # noqa: E402
 
 driver: Driver = get_driver()
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
     NICKNAME = env_config.self_name or list(driver.config.nickname)[0]
 else:
     NICKNAME = env_config.self_name or "bot"
@@ -144,17 +144,17 @@
     await view_card.finish(message=MessageSegment.text(result) + img)
 
 
 # on_command "立即更改群名片"
 @set_card_now.handle()
 async def _(
     bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()  # noqa: B008
-):  # noqa: B008
+):
     card_number = arg.extract_plain_text().strip()
-    if not card_number:
+    if not card_number or not card_number.isdigit():
         await set_card_now.finish("请输入序号或序号输入错误")
     elif card_number not in map(str, range(1, len(card_list) + 1)):
         await set_card_now.finish("没有这种类型的群名片哦，可以发送[查看群名片列表]命令查看吧")
     card_names = await choice_card(card_number)
     if env_config.use_nickname_front:
         card_names = f"{NICKNAME}|{card_names}"
     try:
```

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.6.1/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.6.0/pyproject.toml` & `nonebot_plugin_rename-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.6.0"
+version = "1.6.1"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
```

### Comparing `nonebot_plugin_rename-1.6.0/PKG-INFO` & `nonebot_plugin_rename-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.6.0
+Version: 1.6.1
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.6.1 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
```

