# Comparing `tmp/nonebot_plugin_cp_broadcast-0.2.3.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.2.3.tar` & `nonebot_plugin_cp_broadcast-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/LICENSE
--rw-r--r--   0        0        0     4488 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/README.md
--rw-r--r--   0        0        0     7505 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2598 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     1946 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      438 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0      732 2023-07-10 15:48:15.465262 nonebot_plugin_cp_broadcast-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4488 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/README.md
+-rw-r--r--   0        0        0     7505 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2699 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     1946 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      438 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0      732 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/LICENSE` & `nonebot_plugin_cp_broadcast-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/README.md` & `nonebot_plugin_cp_broadcast-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import urllib.request
+#import urllib.request
+from httpx import AsyncClient
 import datetime
 from bs4 import BeautifulSoup
 from nonebot.plugin import on_fullmatch
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.log import logger
 import asyncio
 import re
@@ -15,16 +16,19 @@
     global atc
     url = f'https://atcoder.jp/contests/?lang=en'
     num = 0 #爬取次数，最多爬三次
     while num < 3 :
         try:
             if len(atc) > 0:
                 atc.clear()
-            html = urllib.request.urlopen(url, timeout=20.0).read()
-            soup = BeautifulSoup(html,'lxml').find_all(name = 'div', attrs = {'id' : 'contest-table-upcoming'})[0].find_all('tbody')[0].find_all('td')
+            
+            async with AsyncClient() as client:
+                resp = await client.get(url=url, timeout=10.0)
+        
+            soup = BeautifulSoup(resp.text,'lxml').find_all(name = 'div', attrs = {'id' : 'contest-table-upcoming'})[0].find_all('tbody')[0].find_all('td')
             ans1 = str(soup[1].contents[5].contents[0])
             url1 = 'https://atcoder.jp' + re.findall(r'<a href="(.+?)">',str(soup[1]))[0]
             ss = str(soup[0].contents[0].contents[0].contents[0]).replace('+0900', '')
             ans2 = str(datetime.datetime.strptime(ss, '%Y-%m-%d %H:%M:%S') - datetime.timedelta(hours = 1))
             ans2 = ans2[0:-3]
             ans3 = str(soup[5].contents[5].contents[0])
             url2 = 'https://atcoder.jp' + re.findall(r'<a href="(.+?)">',str(soup[5]))[0]
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/codeforces.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/nonebot_plugin_cp_broadcast/nowcoder.py` & `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/pyproject.toml` & `nonebot_plugin_cp_broadcast-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "0.2.3"
+version = "0.3.0"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.3/PKG-INFO` & `nonebot_plugin_cp_broadcast-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.2.3
+Version: 0.3.0
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.2.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.3.0 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
 HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

