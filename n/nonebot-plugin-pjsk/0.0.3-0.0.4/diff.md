# Comparing `tmp/nonebot_plugin_pjsk-0.0.3.tar.gz` & `tmp/nonebot_plugin_pjsk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_pjsk-0.0.3.tar` & `nonebot_plugin_pjsk-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1773 2023-07-12 10:28:29.154900 nonebot_plugin_pjsk-0.0.3/README.md
--rw-r--r--   0        0        0      914 2023-07-12 10:28:29.270900 nonebot_plugin_pjsk-0.0.3/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0      335 2023-07-12 10:28:29.270900 nonebot_plugin_pjsk-0.0.3/nonebot_plugin_pjsk/config.json
--rw-r--r--   0        0        0     3707 2023-07-12 10:28:29.270900 nonebot_plugin_pjsk-0.0.3/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     1078 2023-07-12 10:28:29.274900 nonebot_plugin_pjsk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1838 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/README.md
+-rw-r--r--   0        0        0     1070 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/LICENSE
+-rw-r--r--   0        0        0     1133 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     1393 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0     4186 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0      731 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1078 2023-07-13 03:29:03.000135 nonebot_plugin_pjsk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.0.3/README.md` & `nonebot_plugin_pjsk-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 效果
 
-<img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_pjsk/main/test.png" width="512" height="512"  alt="pjsk_test">
+<img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_pjsk/main/test.png" width="400" height="400"  alt="pjsk_test">
 
 ## 资源包
 
-在release下载，并放入data/pjsk中
+- 启动的时候自动检测并下载
+- （或）在release下载，并放入机器人目录data/pjsk中
 
 ## 指令
 
 - pjsk 【text】
 
 ## 🙈 其他
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_pjsk __â¨PJSKè¡¨æåå¶ä½â¨__ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
-## ææ [pjsk_test] ## èµæºå å¨releaseä¸è½½ï¼å¹¶æ¾å¥data/pjskä¸­ ##
-æä»¤ - pjsk ãtextã ## ð å¶ä» -
+## ææ [pjsk_test] ## èµæºå - å¯å¨çæ¶åèªå¨æ£æµå¹¶ä¸è½½ -
+ï¼æï¼å¨releaseä¸è½½ï¼å¹¶æ¾å¥æºå¨äººç®å½data/pjskä¸­ ## æä»¤ -
+pjsk ãtextã ## ð å¶ä» -
 ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æissæè
 [å ç¾¤](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
 - [ç±åçµ](https://afdian.net/a/agnes_digital)
```

### Comparing `nonebot_plugin_pjsk-0.0.3/pyproject.toml` & `nonebot_plugin_pjsk-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_pjsk"
-version = "0.0.3"
+version = "0.0.4"
 description = "PJSK表情包for Nonebot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 repository = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 keywords = ["pjsk", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_pjsk-0.0.3/PKG-INFO` & `nonebot_plugin_pjsk-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.0.3
+Version: 0.0.4
 Summary: PJSK表情包for Nonebot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 License: MIT
 Keywords: pjsk,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
@@ -48,19 +48,20 @@
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 效果
 
-<img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_pjsk/main/test.png" width="512" height="512"  alt="pjsk_test">
+<img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_pjsk/main/test.png" width="400" height="400"  alt="pjsk_test">
 
 ## 资源包
 
-在release下载，并放入data/pjsk中
+- 启动的时候自动检测并下载
+- （或）在release下载，并放入机器人目录data/pjsk中
 
 ## 指令
 
 - pjsk 【text】
 
 ## 🙈 其他
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.0.4 Summary:
 PJSKè¡¨æåfor Nonebot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_pjsk License: MIT Keywords: pjsk,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -11,13 +11,14 @@
 nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow (>=8.4.0) Project-URL:
 Repository, https://github.com/Agnes4m/nonebot_plugin_pjsk Description-Content-
 Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_pjsk __â¨PJSKè¡¨æåå¶ä½â¨__ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
-## ææ [pjsk_test] ## èµæºå å¨releaseä¸è½½ï¼å¹¶æ¾å¥data/pjskä¸­ ##
-æä»¤ - pjsk ãtextã ## ð å¶ä» -
+## ææ [pjsk_test] ## èµæºå - å¯å¨çæ¶åèªå¨æ£æµå¹¶ä¸è½½ -
+ï¼æï¼å¨releaseä¸è½½ï¼å¹¶æ¾å¥æºå¨äººç®å½data/pjskä¸­ ## æä»¤ -
+pjsk ãtextã ## ð å¶ä» -
 ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æissæè
 [å ç¾¤](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
 - [ç±åçµ](https://afdian.net/a/agnes_digital)
```

