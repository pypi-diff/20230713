# Comparing `tmp/nonebot-plugin-cfassistant-1.3.tar.gz` & `tmp/nonebot-plugin-cfassistant-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cfassistant-1.3.tar", last modified: Mon Jul 10 07:18:06 2023, max compression
+gzip compressed data, was "nonebot-plugin-cfassistant-1.4.tar", last modified: Thu Jul 13 09:18:43 2023, max compression
```

## Comparing `nonebot-plugin-cfassistant-1.3.tar` & `nonebot-plugin-cfassistant-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:18:06.888471 nonebot-plugin-cfassistant-1.3/
--rw-rw-rw-   0        0        0      264 2023-07-10 07:18:06.887471 nonebot-plugin-cfassistant-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4528 2023-07-10 07:17:18.000000 nonebot-plugin-cfassistant-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 07:18:06.848349 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/
--rw-rw-rw-   0        0        0     6415 2023-07-10 06:57:00.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/__init__.py
--rw-rw-rw-   0        0        0     3784 2023-07-08 12:01:28.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/changeRemind.py
--rw-rw-rw-   0        0        0      110 2023-07-10 06:41:42.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/randomProblems.py
--rw-rw-rw-   0        0        0    10451 2023-07-10 01:53:20.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateContest.py
--rw-rw-rw-   0        0        0     6039 2023-07-10 06:54:58.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateUser.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:18:06.881927 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/
--rw-rw-rw-   0        0        0      264 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-10 07:18:00.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:18:06.889471 nonebot-plugin-cfassistant-1.3/setup.cfg
--rw-rw-rw-   0        0        0      660 2023-07-10 07:17:21.000000 nonebot-plugin-cfassistant-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:18:43.775237 nonebot-plugin-cfassistant-1.4/
+-rw-rw-rw-   0        0        0      264 2023-07-13 09:18:43.774229 nonebot-plugin-cfassistant-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4528 2023-07-10 07:17:18.000000 nonebot-plugin-cfassistant-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 09:18:43.755426 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/
+-rw-rw-rw-   0        0        0     6415 2023-07-10 06:57:00.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/__init__.py
+-rw-rw-rw-   0        0        0     3864 2023-07-13 09:12:26.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/changeRemind.py
+-rw-rw-rw-   0        0        0      110 2023-07-10 06:41:42.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/randomProblems.py
+-rw-rw-rw-   0        0        0    10493 2023-07-13 09:15:32.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/updateContest.py
+-rw-rw-rw-   0        0        0     6048 2023-07-13 09:06:32.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/updateUser.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:18:43.773222 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-07-13 09:18:43.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-13 09:18:43.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:18:43.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 09:18:33.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-07-13 09:18:43.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-13 09:18:43.000000 nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:18:43.775237 nonebot-plugin-cfassistant-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-07-13 09:16:25.000000 nonebot-plugin-cfassistant-1.4/setup.py
```

### Comparing `nonebot-plugin-cfassistant-1.3/README.md` & `nonebot-plugin-cfassistant-1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/__init__.py` & `nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/changeRemind.py` & `nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/changeRemind.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import aiosqlite
 import asyncio 
 import os
 data_path = './data/CFHelper/'
-db_path = os.path.join(data_path, 'reminder.db')
 if not os.path.exists(data_path):
     os.makedirs(data_path)
+db_path = os.path.join(data_path, 'reminder.db')
+db_lock = asyncio.Lock()
 # conn = sqlite3.connect('./data/CFHelper/reminder.db')
 # cursor = conn.cursor()
 # cursor.execute('''
 #     CREATE TABLE IF NOT EXISTS QQUser (
 #         QQ INTEGER PRIMARY KEY,
 #         status INTEGER
 #     )
@@ -38,15 +39,15 @@
         ''')
         await conn.commit()
 
 asyncio.run(create_reminder())
 
 async def onUser(QQ):
     try:
-        async with aiosqlite.connect(db_path) as conn:
+        async with db_lock, aiosqlite.connect(db_path) as conn:
             cursor = await conn.cursor()
             await cursor.execute('''
             INSERT OR REPLACE INTO QQUser (QQ,status)
             VALUES (?, ?)
         ''', (
             QQ,
             1
@@ -56,15 +57,15 @@
     except:
         return False
         
         
 
 async def onGroup(QQGroup):
     try:
-        async with aiosqlite.connect(db_path) as conn:
+        async with db_lock, aiosqlite.connect(db_path) as conn:
             cursor = await conn.cursor()        
             await cursor.execute('''
             INSERT OR REPLACE INTO QQGroup (QQGroup,status)
             VALUES (?, ?)
         ''', (
             QQGroup,
             1
@@ -72,15 +73,15 @@
             await conn.commit()
         return True
     except:
         return False
 
 async def disUser(QQ):
     try:
-        async with aiosqlite.connect(db_path) as conn:
+        async with db_lock, aiosqlite.connect(db_path) as conn:
             cursor = await conn.cursor()
             await cursor.execute('''
             INSERT OR REPLACE INTO QQUser (QQ,status)
             VALUES (?, ?)
         ''', (
             QQ,
             0
@@ -89,15 +90,15 @@
         return True
     except:
         return False
 
 
 async def disGroup(QQGroup):
     try:
-        async with aiosqlite.connect(db_path) as conn:
+        async with db_lock, aiosqlite.connect(db_path) as conn:
             cursor = await conn.cursor()
             await cursor.execute('''
             INSERT OR REPLACE INTO QQGroup (QQGroup,status)
             VALUES (?, ?)
         ''', (
             QQGroup,
             0
@@ -105,29 +106,29 @@
             await conn.commit()
         return True
     except:
         return False
     
 async def returnReminderUserList():
     ReminderUserList=[]
-    async with aiosqlite.connect(db_path) as conn:
+    async with db_lock, aiosqlite.connect(db_path) as conn:
         cursor = await conn.cursor()
         await cursor.execute('SELECT * FROM QQUser')
         RS= await cursor.fetchall()
         if not RS:
             return ReminderUserList
         for row in RS:
             QQ,status = row
             if(status==1):
                 ReminderUserList.append({'QQ':QQ})
     return ReminderUserList
 
 async def returnReminderGroupList():
     ReminderGroupList=[]
-    async with aiosqlite.connect(db_path) as conn:
+    async with db_lock, aiosqlite.connect(db_path) as conn:
         cursor = await conn.cursor()
         await cursor.execute('SELECT * FROM QQGroup')
         RS= await cursor.fetchall()
         if not RS:
             return ReminderGroupList
         for row in RS:
             QQGroup,status = row
```

### Comparing `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateContest.py` & `nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/updateContest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import aiohttp
 import json
 import datetime
 import aiosqlite
 import asyncio 
 import os
-
+db_lock = asyncio.Lock()
 contest_url = "https://codeforces.com/api/contest.list?gym=false"
 data_path = './data/CFHelper/'
 if not os.path.exists(data_path):
     os.makedirs(data_path)
 db_path = os.path.join(data_path, 'data.db')
 # conn = sqlite3.connect('./data/CFHelper/data.db')
 # cursor = conn.cursor()
@@ -110,15 +110,15 @@
                 contest_relative_time=f"{re_hours}小时{re_minutes}分钟"
             else:
                 contest_relative_time=f"{re_days}天{re_hours}小时{re_minutes}分钟"
             
             contest=ContestType(result["id"],result["name"],result["type"],result["phase"],result["durationSeconds"],result["startTimeSeconds"],abs(result["relativeTimeSeconds"]),contest_duration,contest_start_time,contest_relative_time)
             Contests.append(contest)
 
-            async with aiosqlite.connect(db_path) as conn:
+            async with db_lock, aiosqlite.connect(db_path) as conn:
                 cursor = await conn.cursor()
                 await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
                 remind_status=0
 
                 status = await cursor.fetchone()
                 if status is not None:
                     remind_status = status[0]
@@ -144,15 +144,15 @@
         print("数据请求失败")
 
     return Contests
 
 async def returnreminderInfo():
     Contests=await updateContest()
     output=""
-    async with aiosqlite.connect(db_path) as conn:
+    async with db_lock, aiosqlite.connect(db_path) as conn:
         remind_status=3
         cursor = await conn.cursor()
         for contest in Contests:
             await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
             ids = await cursor.fetchone()
             if ids is not None:
                 remind_status = ids[0]
```

### Comparing `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateUser.py` & `nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant/updateUser.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         await cursor.execute('SELECT * FROM User')
         RS= await cursor.fetchall()
         if not RS:
             return Users
         for row in RS:
             Oid, Onow_rating, Oupdate_time, OQQ, Ostatus ,Olast_rating = row
             user_info_url=user_info_baseurl+Oid
-            time.sleep(0.3)
+            await asyncio.sleep(0.3)
             try:
                 async with aiohttp.ClientSession() as session:
                     async with session.get(user_info_url) as response:
                         response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
                         data = await response.json()
             except aiohttp.ClientError as e:
                 print("请求错误:", e)
```

### Comparing `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/SOURCES.txt` & `nonebot-plugin-cfassistant-1.4/nonebot_plugin_cfassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.3/setup.py` & `nonebot-plugin-cfassistant-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '1.3'
+VERSION = '1.4'
 
 setup(
     name='nonebot-plugin-cfassistant', 
     version=VERSION,  
     description='一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件', 
     packages=find_packages(),
     zip_safe=False,
```

