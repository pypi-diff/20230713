# Comparing `tmp/nonebot_plugin_pjsk-0.0.4.tar.gz` & `tmp/nonebot_plugin_pjsk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_pjsk-0.0.4.tar` & `nonebot_plugin_pjsk-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1838 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/README.md
--rw-r--r--   0        0        0     1070 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/LICENSE
--rw-r--r--   0        0        0     1133 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     1393 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0     4186 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0      731 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1078 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2202 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/README.md
+-rw-r--r--   0        0        0     1070 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/LICENSE
+-rw-r--r--   0        0        0     1148 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0     4225 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0      951 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1078 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.0.4/README.md` & `nonebot_plugin_pjsk-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -22,26 +22,35 @@
 <a href="https://pypi.python.org/pypi/nonebot_plugin_pjsk">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_pjsk.svg" alt="pypi">
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
-## 效果
+## 指令
+
+- pjsk 【text】
+
+## 示例图
 
 <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_pjsk/main/test.png" width="400" height="400"  alt="pjsk_test">
 
+## 安装
+
+以下方法任意选其一
+
+        pip install nonebot_plugin_pjsk
+        nb plugin install nonebot_plugin_pjsk
+
 ## 资源包
 
 - 启动的时候自动检测并下载
 - （或）在release下载，并放入机器人目录data/pjsk中
-
-## 指令
-
-- pjsk 【text】
+- __启动自动下载需要重启再加载一次__
+- 读取资源的目录应该为：`data/pjsk/resource/{文件夹}/{图片}`
 
 ## 🙈 其他
 
-- 由于本人没玩过啤酒烧烤，可能出现一些小问题，可以提iss或者[加群](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈
-- 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
+- 由于本人没玩过啤酒烧烤，可能出现一些小问题，可以提iss或者[加群](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈~~或者单纯进来玩~~
+- 本项目仅供学习使用，图片资源来自于游戏解包，请勿用于商业用途，喜欢该项目可以Star或者提供PR，如果构成侵权将在24小时内删除
 - [爱发电](https://afdian.net/a/agnes_digital)
```

#### html2text {}

```diff
@@ -1,11 +1,16 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_pjsk __â¨PJSKè¡¨æåå¶ä½â¨__ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
-## ææ [pjsk_test] ## èµæºå - å¯å¨çæ¶åèªå¨æ£æµå¹¶ä¸è½½ -
-ï¼æï¼å¨releaseä¸è½½ï¼å¹¶æ¾å¥æºå¨äººç®å½data/pjskä¸­ ## æä»¤ -
-pjsk ãtextã ## ð å¶ä» -
+## æä»¤ - pjsk ãtextã ## ç¤ºä¾å¾ [pjsk_test] ## å®è£
+ä»¥ä¸æ¹æ³ä»»æéå¶ä¸ pip install nonebot_plugin_pjsk nb plugin install
+nonebot_plugin_pjsk ## èµæºå - å¯å¨çæ¶åèªå¨æ£æµå¹¶ä¸è½½ -
+ï¼æï¼å¨releaseä¸è½½ï¼å¹¶æ¾å¥æºå¨äººç®å½data/pjskä¸­ -
+__å¯å¨èªå¨ä¸è½½éè¦éå¯åå è½½ä¸æ¬¡__ -
+è¯»åèµæºçç®å½åºè¯¥ä¸ºï¼`data/pjsk/resource/{æä»¶å¤¹}/{å¾ç}` ##
+ð å¶ä» -
 ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æissæè
-[å ç¾¤](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ -
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
+[å ç¾¤](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦~~æèåçº¯è¿æ¥ç©~~
+-
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼å¾çèµæºæ¥èªäºæ¸¸æè§£åï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PRï¼å¦æææä¾µæå°å¨24å°æ¶åå é¤
 - [ç±åçµ](https://afdian.net/a/agnes_digital)
```

### Comparing `nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/LICENSE` & `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from nonebot.params import CommandArg
 from nonebot.log import logger
 from nonebot.plugin import PluginMetadata
 
 from .draw import make_ramdom
 from .utils import check_res
 
-__version__ = "0.0.4"
+driver = get_driver()
+
+__version__ = "0.1.0"
 __plugin_meta__ = PluginMetadata(
     name="pjsk表情",
     description="pjsk表情包生成,适配nonebot2的插件",
     usage="pjsk 【text】",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     supported_adapters={"~onebot.v11"},
@@ -28,12 +30,12 @@
 
 @pjsk.handle()
 async def _(matcher: Matcher, arg: Message = CommandArg()) -> None:
     if text := arg.extract_plain_text():
         await matcher.send(MessageSegment.image(await make_ramdom(text)))
 
 
-@get_driver().on_startup()
+@driver.on_startup
 async def _():
     logger.info("检查pjsk资源")
     msg = await check_res()
     logger.success(msg)
```

### Comparing `nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from PIL import ImageFont
 
 from typing import Dict, List
 from pathlib import Path
 
+from nonebot.log import logger
+
 
 # 插件资源目录
 module_path = Path("data/pjsk")
 
 # 资源目录
 background_path: Path = module_path / "resource"
 
@@ -25,25 +27,29 @@
     "cyan": ["KAITO", "Miku", "Shizuku"],
     "aqua": ["Kanade"],
     "orange": ["Kohane", "Nene", "Len", "Rin", "Saki", "Tsukasa"],
     "purple": ["Mafuyu", "Rui"],
 }
 
 # 资源模板, key为文件夹名，value为文件夹下的图片，都是相对路径Path对象
-template: Dict[Path, List[Path]] = {
-    role: [i for i in role.iterdir() if i.suffix == ".png"]
-    for role in [i for i in background_path.iterdir() if i.is_dir()]
-}
-
+try:
+    template: Dict[Path, List[Path]] = {
+        role: [i for i in role.iterdir() if i.suffix == ".png"]
+        for role in [i for i in background_path.iterdir() if i.is_dir()]
+    }
+except FileNotFoundError:
+    logger.warning("未下载素材")
+    template =None
 stroke_color = "white"
 stroke_width = 7
 default_font_size = 50
 # rotation_angle = 10
 
-
-font_style: ImageFont.FreeTypeFont = ImageFont.truetype(
-    str(font_file), size=default_font_size, encoding="utf-8"
-)
-
+try:
+    font_style: ImageFont.FreeTypeFont = ImageFont.truetype(
+        str(font_file), size=default_font_size, encoding="utf-8"
+    )
+except OSError:
+    font_style = None
 
 gh_proxy = "https://ghproxy.com/https://github.com/Agnes4m/nonebot_plugin_pjsk"
 download_url = f"{gh_proxy}/releases/download/v0.0.4/resource.zip"
```

### Comparing `nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     role: Path = random.choice(list(template.keys()))
     random_img: Path = random.choice(template[role])
     image: Image.Image = Image.open(random_img)
     text_image = Image.new("RGBA", image.size, (0, 0, 0, 0))
     draw = ImageDraw.Draw(text_image)
 
     if len(text_list) == 1:
-        text_config = await text_draw(text, image.size, draw, role)
+        text_config:TextConfig = await text_draw(text, image.size, draw, role)
         text_position = text_config.font_start
         draw.text(
             text_position,
             text_config.text,
             font=font_style,
             fill=stroke_color,
             stroke_width=text_config.stroke_width,
@@ -52,17 +52,17 @@
             text=text_config.text,
             font=font_style,
             fill=text_config.text_color,
         )
 
     elif len(text_list) >= 2:
         for i, one_text in enumerate(text_list, start=0):
-            text_config = await text_draw(one_text, image.size, draw, role)
+            text_config:TextConfig = await text_draw(one_text, image.size, draw, role)
             text_position = text_config.font_start
-            text_position[-1] = text_position[-1] + (i * text_config.font_size)
+            text_position = (text_position[0],(text_position[-1] + (i * text_config.font_size)))
             draw.text(
                 text_position,
                 text_config.text,
                 font=font_style,
                 fill=stroke_color,
                 stroke_width=text_config.stroke_width,
             )
```

### Comparing `nonebot_plugin_pjsk-0.0.4/pyproject.toml` & `nonebot_plugin_pjsk-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_pjsk"
-version = "0.0.4"
+version = "0.1.0"
 description = "PJSK表情包for Nonebot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 repository = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 keywords = ["pjsk", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_pjsk-0.0.4/PKG-INFO` & `nonebot_plugin_pjsk-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.0.4
+Version: 0.1.0
 Summary: PJSK表情包for Nonebot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 License: MIT
 Keywords: pjsk,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
@@ -46,27 +46,36 @@
 <a href="https://pypi.python.org/pypi/nonebot_plugin_pjsk">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_pjsk.svg" alt="pypi">
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
-## 效果
+## 指令
+
+- pjsk 【text】
+
+## 示例图
 
 <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_pjsk/main/test.png" width="400" height="400"  alt="pjsk_test">
 
+## 安装
+
+以下方法任意选其一
+
+        pip install nonebot_plugin_pjsk
+        nb plugin install nonebot_plugin_pjsk
+
 ## 资源包
 
 - 启动的时候自动检测并下载
 - （或）在release下载，并放入机器人目录data/pjsk中
-
-## 指令
-
-- pjsk 【text】
+- __启动自动下载需要重启再加载一次__
+- 读取资源的目录应该为：`data/pjsk/resource/{文件夹}/{图片}`
 
 ## 🙈 其他
 
-- 由于本人没玩过啤酒烧烤，可能出现一些小问题，可以提iss或者[加群](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈
-- 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
+- 由于本人没玩过啤酒烧烤，可能出现一些小问题，可以提iss或者[加群](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈~~或者单纯进来玩~~
+- 本项目仅供学习使用，图片资源来自于游戏解包，请勿用于商业用途，喜欢该项目可以Star或者提供PR，如果构成侵权将在24小时内删除
 - [爱发电](https://afdian.net/a/agnes_digital)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.1.0 Summary:
 PJSKè¡¨æåfor Nonebot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_pjsk License: MIT Keywords: pjsk,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -11,14 +11,19 @@
 nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow (>=8.4.0) Project-URL:
 Repository, https://github.com/Agnes4m/nonebot_plugin_pjsk Description-Content-
 Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_pjsk __â¨PJSKè¡¨æåå¶ä½â¨__ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
-## ææ [pjsk_test] ## èµæºå - å¯å¨çæ¶åèªå¨æ£æµå¹¶ä¸è½½ -
-ï¼æï¼å¨releaseä¸è½½ï¼å¹¶æ¾å¥æºå¨äººç®å½data/pjskä¸­ ## æä»¤ -
-pjsk ãtextã ## ð å¶ä» -
+## æä»¤ - pjsk ãtextã ## ç¤ºä¾å¾ [pjsk_test] ## å®è£
+ä»¥ä¸æ¹æ³ä»»æéå¶ä¸ pip install nonebot_plugin_pjsk nb plugin install
+nonebot_plugin_pjsk ## èµæºå - å¯å¨çæ¶åèªå¨æ£æµå¹¶ä¸è½½ -
+ï¼æï¼å¨releaseä¸è½½ï¼å¹¶æ¾å¥æºå¨äººç®å½data/pjskä¸­ -
+__å¯å¨èªå¨ä¸è½½éè¦éå¯åå è½½ä¸æ¬¡__ -
+è¯»åèµæºçç®å½åºè¯¥ä¸ºï¼`data/pjsk/resource/{æä»¶å¤¹}/{å¾ç}` ##
+ð å¶ä» -
 ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æissæè
-[å ç¾¤](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ -
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
+[å ç¾¤](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦~~æèåçº¯è¿æ¥ç©~~
+-
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼å¾çèµæºæ¥èªäºæ¸¸æè§£åï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PRï¼å¦æææä¾µæå°å¨24å°æ¶åå é¤
 - [ç±åçµ](https://afdian.net/a/agnes_digital)
```

