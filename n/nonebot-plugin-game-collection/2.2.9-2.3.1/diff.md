# Comparing `tmp/nonebot_plugin_game_collection-2.2.9.tar.gz` & `tmp/nonebot_plugin_game_collection-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.2.9.tar", last modified: Sat Jun 24 22:56:07 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.3.1.tar", last modified: Thu Jul 13 13:19:17 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.2.9.tar` & `nonebot_plugin_game_collection-2.3.1.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.588432 nonebot_plugin_game_collection-2.2.9/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.9/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-24 22:56:07.585929 nonebot_plugin_game_collection-2.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.525602 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    19529 2023-06-24 16:29:41.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.544118 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    19306 2023-06-24 22:54:29.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23183 2023-06-24 22:54:29.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.551124 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.577055 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5335 2023-06-24 06:35:42.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.579057 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.583927 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    16012 2023-06-24 16:57:10.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.535610 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1947 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 22:56:07.588432 nonebot_plugin_game_collection-2.2.9/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-06-24 22:56:02.000000 nonebot_plugin_game_collection-2.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.912826 nonebot_plugin_game_collection-2.3.1/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-07-13 13:19:17.912325 nonebot_plugin_game_collection-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.862064 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21627 2023-07-13 13:15:00.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.872572 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Fortress/
+-rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Fortress/core.py
+-rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.880579 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10594 2023-07-12 11:14:50.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    21889 2023-07-13 13:11:29.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    32577 2023-07-13 09:58:22.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0    11300 2023-07-13 12:39:26.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.883582 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.902317 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.903818 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.910324 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    21412 2023-06-29 17:01:38.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.871071 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:19:17.912826 nonebot_plugin_game_collection-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-07-13 13:19:09.000000 nonebot_plugin_game_collection-2.3.1/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.2.9/LICENSE` & `nonebot_plugin_game_collection-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/README.md` & `nonebot_plugin_game_collection-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Account.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 import datetime
 
 from .utils.chart import (
     bar_chart,
     my_info_head,
     my_info_account,
     linecard,
-    info_Splicing
+    info_splicing
     )
-from .data import UserDict, GroupAccount
+from .data import Company, UserDict, GroupAccount
 from .data import props_library, props_index
 from .config import bot_name,sign_gold, revolt_gold, revolt_cd, revolt_gini, max_bet_gold
-from .Manager import BG_path, bot_list
-from .Manager import data, company_index, update_company_index
+
 from . import Manager
 
+data = Manager.data
 user_data = data.user
 group_data = data.group
 
+company_index = Manager.company_index
+
 def gold_create(event:MessageEvent,gold:int) -> str:
     """
     获取金币
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
@@ -105,15 +107,15 @@
         return None
 
     group = group_data[group_id]
 
     if time.time() - group.revolution_time < revolt_cd:
         return f"重置正在冷却中，结束时间：{datetime.datetime.fromtimestamp(group.revolution_time + revolt_cd).strftime('%H:%M:%S')}"
 
-    if (gold := (Manager.group_wealths(group_id) or 0)) < (limit := 15 * max_bet_gold):
+    if (gold := Manager.group_wealths(group_id)) < (limit := 15 * max_bet_gold):
         return f"本群金币（{round(gold,2)}）小于{limit}，未满足重置条件。"
 
     if (gini := Manager.Gini(group_id)) < revolt_gini:
         return f"当前基尼系数为{round(gini,3)}，未满足重置条件。"
 
     rank = Manager.group_ranklist(group_id,"资产")
     user_id = rank[0][0]
@@ -256,17 +258,17 @@
     # 加载全局信息
     nickname = group_account.nickname
     info.append(await my_info_head(user,nickname))
     # 加载卡片
     PropsCard = Manager.PropsCard_list((user,group_account))
     msg = ""
     for x in PropsCard:
-        msg += f"----\n{x}\n"
+        msg += f"----\n[center]{x}\n"
     if msg:
-        info.append(linecard(msg, width = 880,font_size = 60, endline = "成就卡片"))
+        info.append(linecard(msg+"----", width = 880,padding = (0,-28),spacing = 1, font_size = 60))
 
     # 加载成就卡片
     Achieve = Manager.Achieve_list((user,group_account))[:2]
     # 加载本群账户
     gold = group_account.gold
     value = group_account.value
     is_sign = group_account.is_sign
@@ -277,23 +279,23 @@
     security = 3 - group_account.security
     if security:
         security = [security,"green"]
     else:
         security = [security,"red"]
     msg = ""
     for x in Achieve:
-        msg += x + "\n"
+        msg += f"{x}\n"
     msg += (2-len(Achieve))*"\n"
     msg += (
         f"金币 {'{:,}'.format(gold)}\n"
         f"股票 {'{:,}'.format(round(value,2))}\n"
         "签到 [nowrap]\n"
         f"[color][{is_sign[1]}]{is_sign[0]}\n"
         "补贴 还剩 [nowrap]\n"
-        f"[color][{security[1]}]{security[0]} 次"
+        f"[color][{security[1]}]{security[0]}[nowrap]\n 次"
         )
     # 加载资产分析
     dist = []
     for x in user.group_accounts:
         account = user.group_accounts[x]
         if not (group_name := group_data[x].company.company_name):
             group_name = f"（{str(x)[-4:]}）"
@@ -305,17 +307,48 @@
     # 加载股票信息
     msg = ""
     for stock in group_account.stocks:
         company_name = group_data[stock].company.company_name
         if i := group_account.stocks[stock]:
             msg += f"{company_name}[nowrap]\n[right][color][green]{i}\n"
     if msg:
-        info.append(linecard(msg, 880,endline = "股票信息"))
+        info.append(linecard(msg, width = 880,endline = "股票信息"))
+
+    return MessageSegment.image(info_splicing(info,Manager.BG_path(event.user_id)))
+
+async def my_exchange(event:MessageEvent) -> Message:
+    """
+    我的交易信息
+    """
+    user,group_account = Manager.locate_user(event)
+    if not group_account:
+        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
 
-    return MessageSegment.image(info_Splicing(info,BG_path(event.user_id)))
+    info = []
+
+    # 加载股票信息
+    for company_id,stock in group_account.stocks.items():
+        msg = ""
+        if stock:
+            account_name = None
+            company = group_data[company_id].company
+            msg += f"[pixel][20]公司 {company.company_name}\n[pixel][20]结算 [nowrap]\n[color][green]{'{:,}'.format(round(company.float_gold/company.issuance,2))}[nowrap]\n[pixel][400]数量 [nowrap]\n[color][green]{stock}\n"
+            if exchange := company.exchange.get(user.user_id):
+                if exchange.group_id == group_account.group_id:
+                    account_name = "本群"
+                else:
+                    account_name = group_data[exchange.group_id].company.company_name
+                    account_name = account_name if account_name else f"({str(exchange.group_id)[4]}...)"
+                msg += f"[pixel][20]报价 [nowrap]\n[color][green]{exchange.quote}[nowrap]\n[pixel][400]发布 [nowrap]\n[color][green]{exchange.n}\n"
+            info.append(linecard(msg, width = 880,endline = f"报价账户：{account_name}" if account_name else "无报价"))
+    if info:
+        info.insert(0,await my_info_head(user,group_account.nickname))
+        return MessageSegment.image(info_splicing(info,Manager.BG_path(event.user_id)))
+    else:
+        return "你的股票信息为空。"
 
 def my_props(event:MessageEvent) -> Message:
     """
     我的道具
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
@@ -343,18 +376,19 @@
             )
 
         info.append(
             linecard(msg,
                      width = 880,
                      padding=(0,20),
                      endline = "特殊道具" if rare == 0 else rare*'☆',
-                     bg_color = (255,255,255,153)
+                     bg_color = (255,255,255,153),
+                     autowrap = True
                      ))
-    if msg:
-        return MessageSegment.image(info_Splicing(info,BG_path(event.user_id),spacing = 5))
+    if info:
+        return MessageSegment.image(info_splicing(info,Manager.BG_path(event.user_id),spacing = 5))
     else:
         return "您的仓库空空如也。"
 
 async def info_profile(user_id:int) -> list:
     """
     总览资料卡
     """
@@ -414,31 +448,41 @@
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
     user_id = user.user_id
     group_id = group_account.group_id
     if not (ranklist := Manager.group_ranklist(group_id, title)):
         return "无数据。"
     info = await draw_rank(ranklist, title, 20, group_id = group_id)
-    return MessageSegment.image(info_Splicing(info,BG_path(user_id), spacing = 5))
+    return MessageSegment.image(info_splicing(info,Manager.BG_path(user_id), spacing = 5))
 
 async def All_rank(event:MessageEvent, title:str = "金币", top:int = 10) -> list:
     """
     生成总排行榜
     """
     if not (ranklist := Manager.All_ranklist(title)):
         return None
     info = await draw_rank(ranklist, title, 20)
-    return MessageSegment.image(info_Splicing(info,BG_path(event.user_id), spacing = 5))
+    return MessageSegment.image(info_splicing(info,Manager.BG_path(event.user_id), spacing = 5))
+
+def transfer_fee(amount: int, limit: int) -> int:
+    levels = [[0.02, max_bet_gold * 10],[0.2, max_bet_gold * 40],[0.4, max_bet_gold * 50],[0.6, float('inf')]]
+    fee = 0
+    for n,(level_tax, level_step) in enumerate(levels):
+        if limit >= level_step:
+            limit -= level_step
+            continue
+        levels[n][1] -= limit
+        break
+    for level_tax, level_step in levels[n:]:
+        if amount <= level_step:
+            fee += amount * level_tax
+            break
+        fee += level_step * level_tax
+        amount -= level_step
 
-def transfer_fee(amount:int,limit:int) -> int:
-    limit = limit if limit > 0 else 0
-    if amount <= limit:
-        fee = amount * 0.02
-    else:
-        fee = limit * 0.02 + (amount - limit) * 0.2
     return int(fee)
 
 def intergroup_transfer_gold(event:MessageEvent, gold:int, company_name:str):
     """
     跨群转移金币到自己的账户
     """
     user,group_account = Manager.locate_user(event)
@@ -453,43 +497,38 @@
         return f"没有 {company_name} 的注册信息"
 
     if company_id in user.group_accounts:
         target_group_account = user.group_accounts[company_id]
     else:
         return f"你在 {company_name} 没有创建账户"
 
-    user.transfer_limit += gold
-    fee = transfer_fee(gold, (10 * max_bet_gold) - user.transfer_limit)
-    user.gold -= fee
     group_account.gold -= gold
-    target_group_account.gold += gold - fee
+    ExRate = group_data[group_account.group_id].company.level/group_data[company_id].company.level
+    ExRate = ExRate if ExRate else 1.0
+    tgold = int(ExRate * gold + 0.5)
+    fee = transfer_fee(tgold, user.transfer_limit)
+    target_group_account.gold += tgold - fee
+    user.transfer_limit += tgold
+    user.gold -= fee
 
-    return f"向 {company_name} 转移 {gold}金币，扣除手续费：{fee}，实际到账金额{gold - fee}"
+    return f"向 {company_name} 转移{gold}金币。\n汇率：{round(ExRate,2)} 手续费：{fee}({round(100*fee/tgold,2)}%)\n实际到账金额：{tgold - fee}"
 
 def freeze(target:UserDict):
     target_id = target.user_id
     gold = target.gold
     value = 0.0
-    company_ids = set()
     group_accounts = target.group_accounts
-    for group_id in group_accounts:
-        group_account = group_accounts[group_id]
+    for group_id,group_account in group_accounts.items():
         value += group_account.value
-        stocks = group_account.stocks
         group = group_data[group_id]
-        for company_id in stocks:
-            group.company.stock += stocks[company_id]
-            company_ids.add(company_id)
+        for company_id in group_account.stocks:
+            company = group_data[company_id].company
+            company.Buyback(group_account)
         group.namelist.remove(target_id)
 
-    for company_id in company_ids:
-        exchange = group_data[company_id].company.exchange
-        if target_id in exchange:
-            del exchange[target_id]
-
     target.gold = 0
     target.group_accounts = {}
 
     x = gold + value
     if x > 500 * max_bet_gold:
         count = 500
     elif x > 50 * max_bet_gold:
@@ -505,14 +544,15 @@
     return f"【冻结】清算完成，总价值为 {round(x,2)}（金币 {gold} 股票 {round(value,2)}）"
 
 async def delist():
         """
         清理无效账户
         """
         mapping = {}
+        bot_list = Manager.driver.bots.values()
         for bot in bot_list:
             group_list = await bot.get_group_list(no_cache = True)
             for group in group_list:
                 mapping[group["group_id"]] = bot
         if not mapping:
             return "群组获取失败"
 
@@ -555,11 +595,11 @@
             # 删除已注册但不存在的用户
             namelist = group_data[group_id].namelist
             delist_users = namelist - users
             for user_id in delist_users:
                 log += f'删除群账户：{user_id} - {group_id}\n'
                 del user_data[user_id].group_accounts[group_id]
                 namelist.discard(user_id)
-        update_company_index()
+        Manager.update_company_index()
         # 保存数据
         data.save()
         return log[:-1] if log else "没有要清理的数据！"
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Game.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     GroupMessageEvent,
     Message,
     MessageSegment
     )
+    
 import random
 import time
 import asyncio
 
 from .utils.utils import get_message_at
-from .utils.chart import text_to_png
+from .utils.chart import linecard_to_png
 from .data import props_library
 from .config import bot_name, security_gold, bet_gold, max_bet_gold, max_player, min_player
 
-from .HorseRace.start import load_dlcs
-from .HorseRace.race_group import race_group
-
-from .Manager import data, try_send_private_msg
 from . import Manager
 
+data = Manager.data
 user_data = data.user
 group_data = data.group
 
-class GameException(Exception):
+class GameOverException(Exception):
     """
-    GameException
+    GameOverException
     """
 
 class Session(BaseModel):
     """
     游戏场次信息
     """
     time:float = 0.0
@@ -131,38 +129,37 @@
         """
         把session状态切换到下一回合
         """
         self.time = time.time()
         self.round += 1
         self.next = self.player1_id if self.next == self.player2_id else self.player2_id
 
-    def shot_check(self, event:GroupMessageEvent):
+    def shot_check(self, user_id:int):
         """
         开枪前检查游戏是否合法
         如果不合法则返回提示
         如果合法则返回None
         """
         if time.time() - self.time > 60:
             return "这场对决邀请已经过时了，请重新发起决斗..."
-        user_id = event.user_id
         if not self.player1_id:
             return " "
         if not self.player2_id:
             if self.player1_id == user_id:
                 return "目前无人接受挑战哦"
             else:
                 return "请这位勇士先接受挑战"
         if user_id == self.player1_id or user_id == self.player2_id:
             if user_id == self.next:
                 return None
             else:
-                return f"现在是{user_data[self.next].group_accounts[event.group_id].nickname}的回合"
+                return f"现在是{user_data[self.next].group_accounts[self.group_id].nickname}的回合"
         else:
-            player1_name = user_data[self.player1_id].group_accounts[event.group_id].nickname
-            player2_name = user_data[self.player2_id].group_accounts[event.group_id].nickname
+            player1_name = user_data[self.player1_id].group_accounts[self.group_id].nickname
+            player2_name = user_data[self.player2_id].group_accounts[self.group_id].nickname
             return f"{player1_name} v.s. {player2_name}\n正在进行中..."
 
 class Game(ABC):
     """
     对战游戏类：
     需要定义的方法：
         action：游戏进行
@@ -170,14 +167,15 @@
         session_tips：场次提示信息
         end_tips：结束附件
     """
     name:str = "undefined"
     max_bet_gold:int = max_bet_gold
 
     def __init__(self):
+        self.gold:int = 0
         self.session:Session = Session()
 
     @staticmethod
     def parse_arg(arg:str):
         if arg.isdigit():
             gold = int(arg)
         else:
@@ -197,43 +195,45 @@
     @abstractmethod
     def game_tips(self, msg):
         """
         游戏开始的提示
         """
 
     @abstractmethod
-    async def action(self, bot:Bot, event:GroupMessageEvent):
+    async def action(self, bot:Bot, user_id:int):
         """
         游戏进行
         """
 
-    async def play(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def play(self, bot:Bot, user_id:int, *args):
         try:
-            return await self.action(bot, event, *args)
-        except GameException:
+            return await self.action(bot, user_id, *args)
+        except GameOverException:
             pass
 
     def accept(self, event:GroupMessageEvent):
         """
         接受挑战
         """
         session = self.session
         group_id = session.group_id
         if msg := session.try_join_game(event):
             return None if msg == " " else msg
-        group_account = Manager.locate_user(event)[1]
+        user,group_account = Manager.locate_user(event)
         if group_account.gold <  session.gold:
             session.leave()
             return Message(MessageSegment.at(event.user_id) + f"你的金币不足以接受这场对决！\n——你还有{group_account.gold}枚金币。")
-
+        user.connect = group_id
         bet_limit = min(
             user_data[session.player1_id].group_accounts[group_id].gold,
             user_data[session.player2_id].group_accounts[group_id].gold)
         bet_limit = bet_limit if bet_limit > 0 else 0
-        session.gold = random.randint(0, bet_limit)if session.gold == -1 else session.gold
+        if session.gold == -1:
+            session.gold = random.randint(0, bet_limit)
+            self.gold = session.gold
         session.bet_limit = bet_limit
         session.next = session.player1_id
         return self.session_tips()
 
     @abstractmethod
     def session_tips(self):
         """
@@ -248,71 +248,81 @@
         return Message(
             f"{MessageSegment.at(session.player2_id)}接受了对决！\n" +
             tip1 +
             f"赌注为 {session.gold} 金币\n" +
             f"请{MessageSegment.at(session.player1_id)}{tip2}"
             )
 
-    def refuse(self, event:GroupMessageEvent):
+    def refuse(self, user_id:int):
         """
         拒绝挑战
         """
         session = self.session
         group_id = session.group_id
         if time.time() - session.time > 60:
             del current_games[group_id]
-        if session.at == event.user_id:
+        if session.at == user_id:
             if session.player2_id:
                 return "对决已开始，拒绝失败。"
             else:
                 del current_games[group_id]
                 return "拒绝成功，对决已结束。"
 
-    async def overtime(self, bot:Bot, event:GroupMessageEvent):
+    async def overtime(self, bot:Bot):
         """
         超时结算
         """
         session = self.session
         if (time.time() - session.time > 30 and
             session.player1_id and
             session.player2_id):
             try:
-                await self.end(bot, event)
-            except GameException:
+                await self.end(bot)
+            except GameOverException:
                 pass
 
-    async def fold(self, bot:Bot, event:GroupMessageEvent):
+    async def fold(self, bot:Bot, user_id:int):
         """
         认输
         """
         session = self.session
-        user_id = event.user_id
         if (time.time() - session.time < 60 and
             session.player1_id and
             session.player2_id and
             user_id == session.player1_id or user_id == session.player2_id):
             session.win = session.player1_id if user_id == session.player2_id else session.player2_id
             try:
-                await self.end(bot, event)
-            except GameException:
+                await self.end(bot)
+            except GameOverException:
                 pass
 
+    def restart(self):
+        """
+        游戏重置
+        """
+        session = self.session
+        group_id = session.group_id
+        overtime = time.time() - session.time
+        if overtime < 60:
+            return f"当前游戏已创建 {int(overtime)} 秒，未超时。"
+        del current_games[group_id]
+        return "游戏已重置。"
+
     @classmethod
     def start(cls, event:GroupMessageEvent, **kwargs) -> Tuple[bool,Message]:
         """
         发起游戏
         """
         gold = kwargs["gold"]
         limit = cls.max_bet_gold
         if gold > limit:
             return  False, Message(MessageSegment.at(event.user_id) + f"对战金额不能超过{limit}")
-        group_account = Manager.locate_user(event)[1]
+        user,group_account = Manager.locate_user(event)
         if gold > group_account.gold:
             return  False, Message(MessageSegment.at(event.user_id) + f"你没有足够的金币支撑这场对决。\n——你还有{group_account.gold}枚金币。")
-
         group_id = event.group_id
         if group_id in current_games:
             game = current_games[group_id]
             if msg := game.session.create_check(event):
                 return False, msg
 
         game = current_games[group_id] = cls(**kwargs)
@@ -329,25 +339,25 @@
                    f"请 {player2_name} 回复 接受挑战 or 拒绝挑战\n"
                    "【30秒内有效】")
         else:
             player1_name = user_data[session.player1_id].group_accounts[event.group_id].nickname
             msg = (f"{player1_name} 发起挑战！\n"
                    "回复 接受挑战 即可开始对局。\n"
                    "【30秒内有效】")
-
+        user.connect = group_id
         session.round = 1
         return True, msg
 
-    def settle(self, group_id:int):
+    def settle(self):
         """
         游戏结束结算
             return:结算界面
         """
         session = self.session
-
+        group_id = session.group_id
         win = session.win if session.win else session.player1_id if session.next == session.player2_id else session.player2_id
         winner = user_data[win]
         winner_group_account = winner.group_accounts[group_id]
 
         lose = session.player1_id if session.player2_id == win else session.player2_id
         loser = user_data[lose]
         loser_group_account = loser.group_accounts[group_id]
@@ -374,29 +384,26 @@
         else:
             extra_tip = ""
             extra = 0
 
         if gold == loser_group_account.gold and loser_group_account.security < 3:
             loser_group_account.security += 1
             security = random.randint(security_gold[0], security_gold[1])
-            security_tip1 = "◇『金币补贴』\n"
-            security_tip2 = f"◇已领取补贴：{security}\n"
+            security_tip = f"◇『金币补贴』(+{security})\n"
         else:
             security = 0
-            security_tip1 = ""
-            security_tip2 = ""
+            security_tip = ""
 
         if loser_group_account.props.get("52001",0) > 0:
             off = int(gold * 0.1)
             if off < maxgold:
                 off_tip = f"◇『{props_library['52001']['name']}』\n"
             else:
                 off = maxgold
                 off_tip = f"◇『{props_library['52001']['name']}』最大补贴\n"
-
         else:
             off = 0
             off_tip = ""
 
         win_gold = gold - fee + extra
         winner.win += 1
         winner.Achieve_win += 1
@@ -405,31 +412,30 @@
         lose_gold = gold - off
         loser.lose += 1
         loser.Achieve_lose += 1
         loser.Achieve_win = 0
 
         msg = (
             f"结算：\n"
-            "——————————————\n" +
-            (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((winner,winner_group_account)))) else "") +
-            extra_tip +
-            f"◆胜者：{winner_group_account.nickname}\n"
-            f"◆结算：{winner_group_account.gold}（+{win_gold}）\n"
-            f"◆战绩：{winner.win}:{winner.lose}\n"
-            f"◆胜率：{round(winner.win * 100 / (winner.win + winner.lose), 2) if winner.win > 0 else 0}%\n"
-            "——————————————\n" +
-            (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((loser,loser_group_account)))) else "") +
-            security_tip1 +
-            off_tip +
-            f"◇败者：{loser_group_account.nickname}\n"
-            f"◇结算：{loser_group_account.gold}（-{lose_gold}）\n" +
-            security_tip2 +
-            f"◇战绩：{loser.win}:{loser.lose}\n"
-            f"◇胜率：{round(loser.win * 100 / (loser.win + loser.lose), 2) if loser.win > 0 else 0}%\n"
-            "——————————————\n" + 
+            "----\n"
+            + extra_tip
+            + (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((winner,winner_group_account)))) else "") +
+            f"◆胜者 {winner_group_account.nickname}\n"
+            f"◆结算 {winner_group_account.gold}(+{win_gold})\n"
+            f"◆战绩 {winner.win}:{winner.lose}\n"
+            f"◆胜率 {round(winner.win * 100 / (winner.win + winner.lose), 2) if winner.win > 0 else 0}%\n"
+            "----\n"
+            + off_tip
+            + (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((loser,loser_group_account)))) else "") +
+            f"◇败者 {loser_group_account.nickname}\n"
+            f"◇结算 {loser_group_account.gold}(-{lose_gold})\n"
+            + security_tip +
+            f"◇战绩 {loser.win}:{loser.lose}\n"
+            f"◇胜率 {round(loser.win * 100 / (loser.win + loser.lose), 2) if loser.win > 0 else 0}%\n"
+            "----\n" + 
             fee_tip
             )
         winner.gold += win_gold
         winner_group_account.gold += win_gold
         loser.gold -= lose_gold - security
         loser_group_account.gold -= lose_gold - security
 
@@ -438,39 +444,41 @@
 
     @abstractmethod
     def end_tips(self):
         """
         结束附件
         """
 
-    async def end(self, bot:Bot, event:GroupMessageEvent):
+    async def end(self, bot:Bot):
         """
         输出结算界面
         """
-        result = self.settle(event.group_id)
-        tmp = MessageSegment.image(text_to_png(result[1], width_simple = "——————————————"))
-        await bot.send(event,result[0])
-        await bot.send(event,tmp)
-        await asyncio.sleep(0.5)
-        await bot.send(event,result[2])
-        raise GameException
+        group_id = self.session.group_id
+        result = self.settle()
+        await bot.send_group_msg(group_id = group_id, message = result[0])
+        await bot.send_group_msg(group_id = group_id, message = MessageSegment.image(linecard_to_png(result[1], width = 880)))
+        if result[2]:
+            await asyncio.sleep(0.5)
+            await bot.send_group_msg(group_id = group_id, message = result[2])
+        raise GameOverException
 
 current_games:Dict[int,Game] = {}
 
 class Russian(Game):
     """
     俄罗斯轮盘
     """
     name = "Russian"
     max_bet_gold:int = max_bet_gold
 
     def __init__(self, **kwargs):
         super().__init__()
         gold = kwargs["gold"]
-        bullet_num = kwargs["bullet_num"]
+        bullet_num = kwargs.get("bullet_num",1)
+        self.gold:int = gold
         self.bullet_num:int = bullet_num
         self.bullet:list = self.random_bullet(bullet_num)
         self.index:int = 0
         self.session.gold = gold
 
     @staticmethod
     def parse_arg(arg:str):
@@ -503,56 +511,54 @@
             bullet_num:装填子弹数量
         """
         bullet_lst = [0, 0, 0, 0, 0, 0, 0]
         for i in random.sample([0, 1, 2, 3, 4, 5, 6], bullet_num):
             bullet_lst[i] = 1
         return bullet_lst
 
-    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def action(self, bot:Bot, user_id:int, *args):
         """
         开枪！！！
         """
         session = self.session
-        if msg := session.shot_check(event):
+        if msg := session.shot_check(user_id):
             return None if msg == " " else msg
         group_id = session.group_id
 
         index = self.index
         MAG = self.bullet[index:]
         count = args[0] if args[0] else 1
         count = len(MAG) if count < 1 else count
 
         msg = f"连开{count}枪！\n" if count > 1 else ""
 
         if 1 in MAG[:count]:
-            session.win = session.player1_id if event.user_id == session.player2_id else session.player2_id
-            await bot.send(event,(
-                MessageSegment.at(event.user_id) + msg +
+            session.win = session.player1_id if user_id == session.player2_id else session.player2_id
+            await bot.send_group_msg(group_id = group_id, message = (
+                MessageSegment.at(user_id) + msg +
                 random.choice(["嘭！，你直接去世了","眼前一黑，你直接穿越到了异世界...(死亡)","终究还是你先走一步..."]) +
                 f"\n第 {index + MAG.index(1) + 1} 发子弹送走了你..."
                 ))
-            await self.end(bot, event)
+            await self.end(bot)
         else:
             session.nextround()
             self.index += count
             next_name = user_data[session.next].group_accounts[group_id].nickname
-            await bot.send(event,msg + (
-                random.choice(["呼呼，没有爆裂的声响，你活了下来",
-                               "虽然黑洞洞的枪口很恐怖，但好在没有子弹射出来，你活下来了",
-                               f'{"咔 "*count}，看来运气不错，你活了下来']) +
+            await bot.send_group_msg(group_id = group_id, message = (
+                random.choice(["呼呼，没有爆裂的声响，你活了下来","虽然黑洞洞的枪口很恐怖，但好在没有子弹射出来，你活下来了",f'{"咔 "*count}，看来运气不错，你活了下来']) +
                 f"\n下一枪中弹的概率：{round(self.bullet_num * 100 / (len(MAG) - count),2)}%\n"
                 f"轮到 {next_name}了"
                 ))
 
     def game_tips(self, msg):
         """
         发起游戏：俄罗斯轮盘
         """
         return (("咔 " * self.bullet_num)[:-1] + "，装填完毕\n"
-                f'挑战金额：{self.session.gold}\n'
+                f'挑战金额：{self.gold}\n'
                 f'第一枪的概率为：{round(self.bullet_num * 100 / 7,2)}%\n'
                 f'{msg}')
 
     def session_tips(self):
         tip1 = "本场对决为【俄罗斯轮盘】\n"
         tip2 = "开枪！"
         return self.acceptmessage(tip1, tip2);
@@ -561,15 +567,15 @@
         return " ".join(("—" if x == 0 else "|") for x in self.bullet)
 
 class Dice(Game):
     """
     掷色子
     """
     name = "Dice"
-    max_bet_gold:int = max_bet_gold *10
+    max_bet_gold:int = max_bet_gold
 
     def __init__(self, **kwargs):
         super().__init__()
         gold = kwargs["gold"]
         self.gold:int = gold
         self.dice_array1:list = [random.randint(1,6) for i in range(5)]
         self.dice_array2:list = [random.randint(1,6) for i in range(5)]
@@ -624,20 +630,20 @@
     def dice_list(dice_array:list) -> str:
         """
         把骰子列表转成字符串
         """
         lst_dict = {0:"〇",1:"１",2:"２",3:"３",4:"４",5:"５",6:"６",7:"７",8:"８",9:"９"}
         return " ".join(lst_dict[x] for x in dice_array)
 
-    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def action(self, bot:Bot, user_id:int, *args):
         """
         开数！！！
         """
         session = self.session
-        if msg := session.shot_check(event):
+        if msg := session.shot_check(user_id):
             return None if msg == " " else msg
         group_id = session.group_id
 
         session.gold += self.gold
         session.gold = min(session.gold, session.bet_limit)
 
         player1_id = session.player1_id
@@ -656,26 +662,26 @@
         session.nextround()
 
         next_name = "结算" if session.round > 10 else user_data[session.next].group_accounts[group_id].nickname
         msg = (
             f'玩家：{user_data[player1_id].group_accounts[group_id].nickname}\n'
             f"组合：{self.dice_list(dice_array1)}\n"
             f"点数：{self.dice_pt_analyses(pt1)}\n"
-            "———————————\n"
+            "----\n"
             f'玩家：{user_data[player2_id].group_accounts[group_id].nickname}\n'
             f"组合：{self.dice_list(dice_array2)}\n"
             f"点数：{self.dice_pt_analyses(pt2)}\n"
-            "———————————\n"
+            "----\n"
             f"结算金额：{session.gold}\n"
             f'领先：{user_data[session.win].group_accounts[group_id].nickname}\n'
             f'下一回合：{next_name}'
             )
-        await bot.send(event,message = MessageSegment.image(text_to_png(msg, 50, width_simple = "———————————")))
+        await bot.send_group_msg(group_id = group_id, message = MessageSegment.image(linecard_to_png(msg, width = 700)))
         if session.round > 10:
-            await self.end(bot, event)
+            await self.end(bot)
 
     def game_tips(self, msg):
         """
         发起游戏：掷色子
         """
         return ("哗啦哗啦~，骰子准备完毕\n"
                 f'挑战金额：{self.gold}/次\n'
@@ -685,43 +691,45 @@
         tip1 = "本场对决为【掷色子】\n"
         tip2 = "开数！"
         return self.acceptmessage(tip1, tip2);
 
     def end_tips(self):
         return (
             f'玩家 1\n'
-            f'组合：{" ".join(str(x) for x in self.dice_array2)}\n'
+            f'组合：{" ".join(str(x) for x in self.dice_array1)}\n'
             f'玩家 2\n'
             f'组合：{" ".join(str(x) for x in self.dice_array2)}')
 
 class Poker(Game):
     """
     扑克对战
     """
     name = "Poker"
-    max_bet_gold:int = max_bet_gold *10
+    max_bet_gold:int = max_bet_gold *5
 
     def __init__(self, **kwargs):
         super().__init__()
         gold = kwargs["gold"]
-        deck = self.random_poker()
+        deck = self.random_poker(2)
         hand = deck[0:3].copy()
+        self.gold:int = gold
         del deck[0:3]
         self.deck:list = deck + [[0,0],[0,0],[0,0],[0,0]]
         self.ACT:int = 1
         self.P1:dict = {"hand":hand,"HP":20,"ATK":0,"DEF":0,"SP":0}
         self.P2:dict = {"hand":[],"HP":25,"ATK":0,"DEF":0,"SP":2}
         self.session.gold = gold
 
     @staticmethod
-    def random_poker():
+    def random_poker(n:int = 1):
         """
         生成随机牌库
         """
         poker_deck = [[i,j] for i in range(1,5) for j in range(1,14)]
+        poker_deck = poker_deck*n
         random.shuffle(poker_deck)
         return poker_deck
 
     class pokerACT():
         suit = {0:"结束",1:"防御",2:"恢复",3:"技能",4:"攻击"}
         point = {0:"0",1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"11",12:"12",13:"13"}
 
@@ -817,44 +825,44 @@
                 msg += f"♢发动了反击 {point}"
             else:
                 msg += "启动结算程序"
             Player["SP"] -= point
             Player["SP"] = 0 if Player["SP"] < 0 else Player["SP"]
             return msg
 
-    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def action(self, bot:Bot, user_id:int, *args):
         """
         出牌
         """
         session = self.session
         if self.ACT == 0:
             return
-        if msg := session.shot_check(event):
+        if msg := session.shot_check(user_id):
             return None if msg == " " else msg
         if not 1<= (index := args[0]) <= 3:
             return "请发送【出牌 1/2/3】打出你的手牌。"
         group_id = session.group_id
 
         self.ACT = 0
         session.nextround()
         deck = self.deck
-        if event.user_id == session.player1_id:
+        if user_id == session.player1_id:
             Active = self.P1
             Passive = self.P2
         else:
             Active = self.P2
             Passive = self.P1
         
         # 出牌判定
         msg = self.pokerACT.action(index - 1,Active)
         try:
-            await bot.send(event,message = msg,at_sender=True)
+            await bot.send_group_msg(group_id = group_id, message = MessageSegment.at(user_id) + msg)
         except:
             try:
-                await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
+                await bot.send_group_msg(group_id = group_id, message = MessageSegment.at(user_id) + MessageSegment.image(linecard_to_png(msg,font_size = 30)))
             except:
                 pass
 
         await asyncio.sleep(0.03*len(msg))
 
         # 敌方技能判定
         next_name = user_data[session.next].group_accounts[group_id].nickname
@@ -864,18 +872,18 @@
                 msg = f'{next_name} 二十面骰判定为{roll}点，当前技能点{Passive["SP"]}\n技能发动失败...'
             else:
                 msg = f'{next_name} 二十面骰判定为{roll}点，当前技能点{Passive["SP"]}\n技能发动成功！\n'
                 msg += self.pokerACT.skill(deck[0], Passive)
                 del deck[0]
 
             try:
-                await bot.send(event,message = msg)
+                await bot.send_group_msg(group_id = group_id, message = msg)
             except:
                 try:
-                    await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
+                    await bot.send_group_msg(group_id = group_id, message = MessageSegment.image(linecard_to_png(msg,font_size = 30)))
                 except:
                     pass
 
         # 回合结算
         Active["HP"] += Active["DEF"] - Active["ATK"] if Active["DEF"] < Passive["ATK"] else 0
         Passive["HP"] += Passive["DEF"] - Active["ATK"] if Passive["DEF"] < Active["ATK"] else 0
 
@@ -892,54 +900,54 @@
 
         next_name = "游戏结束" if Active["HP"] < 1 or Passive["HP"] < 1 or Passive["HP"] >= 40 or [0,0] in hand else next_name
 
         msg = (
             f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
             "状态：\n"
             f'HP {self.P1["HP"]} SP {self.P1["SP"]} DEF {self.P1["DEF"]}\n'
-            "——————————————\n"
+            "----\n"
             f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
             "状态：\n"
             f'HP {self.P2["HP"]} SP {self.P2["SP"]} DEF {self.P2["DEF"]}\n'
-            "——————————————\n"
+            "----\n"
             f'当前回合：{next_name}\n'
-            "手牌：\n" + 
+            "手牌：\n[center]" + 
             "".join([f'【{self.pokerACT.suit[suit]}{self.pokerACT.point[point]}】' for suit, point in Passive["hand"]])
             )
         await asyncio.sleep(0.5)
-        await bot.send(event, message = MessageSegment.image(text_to_png(msg, 50, width_simple = "——————————————")))
+        await bot.send_group_msg(group_id = group_id, message = MessageSegment.image(linecard_to_png(msg, width = 880)))
 
         if next_name == "游戏结束":
             Passive["HP"] = Passive["HP"] + 100 if Passive["HP"] >= 40 else Passive["HP"]
             session.win = session.player1_id if self.P1["HP"] > self.P2["HP"] else session.player2_id
-            await self.end(bot, event)
+            await self.end(bot)
         else:
             self.ACT = 1
 
     def game_tips(self, msg):
         """
         发起游戏：扑克对战
         """
         return ("唰唰~，随机牌堆已生成\n"
-                f'挑战金额：{self.session.gold}'
+                f'挑战金额：{self.gold}\n'
                 f'{msg}')
 
     def session_tips(self):
         tip1 = "本场对决为【扑克对战】\n"
         tip2 = "出牌！\n"
-        tip2 += MessageSegment.image(text_to_png(
+        tip2 += MessageSegment.image(linecard_to_png((
             "P1初始状态\n"
             f'HP {self.P1["HP"]} SP {self.P1["SP"]} DEF {self.P1["DEF"]}\n'
-            "——————————————\n"
+            "----\n"
             "P2初始状态\n"
             f'HP {self.P2["HP"]} SP {self.P2["SP"]} DEF {self.P2["DEF"]}\n'
-            "——————————————\n"
-            "P1初始手牌\n" + 
+            "----\n"
+            "P1初始手牌\n[center]" + 
             "".join([f'【{self.pokerACT.suit[suit]}{self.pokerACT.point[point]}】' for suit, point in self.P1["hand"]])
-            ), 50, width_simple = "——————————————")
+            ), width = 880))
         return self.acceptmessage(tip1, tip2);
 
     def end_tips(self):
         return "" 
 
 class LuckyNumber(Game):
     """
@@ -959,39 +967,43 @@
     def parse_arg(arg:str):
         if arg.isdigit():
             gold = int(arg)
         else:
             gold = int(bet_gold/10)
         return {"gold":gold}
 
-    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def action(self, bot:Bot, user_id:int, *args):
         """
         猜数字
         """
         session = self.session
-        if msg := session.shot_check(event):
+        if msg := session.shot_check(user_id):
             return None if msg == " " else msg
 
         session.gold += self.gold
         session.gold = min(session.gold, session.bet_limit)
         session.nextround()
 
         N = args[0]
         TrueN = self.number
-        if N > TrueN:
-            return f"{N}比这个数字大\n金额：{session.gold}"
-        if N < TrueN:
-            return f"{N}比这个数字小\n金额：{session.gold}"
 
-        session.win = event.user_id
-        await self.end(bot, event)
+        if N == TrueN:
+            session.win = user_id
+            await self.end(bot)
+        else:
+            if N > TrueN:
+                msg = f"{N}比这个数字大\n金额：{session.gold}"
+            else:
+                msg = f"{N}比这个数字小\n金额：{session.gold}"
+            await bot.send_group_msg(group_id = session.group_id, message = msg)
+
 
     def game_tips(self, msg):
         """
-        发起游戏：扑克对战
+        发起游戏：猜数字
         """
         return (f"随机 1-100 数字已生成。"
                 f"挑战金额：{self.gold}/次\n"
                 f"{msg}")
 
     def session_tips(self):
         tip1 = "本场对决为【猜数字】\n"
@@ -1010,15 +1022,15 @@
 
     cantrell_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
     cantrell_point = {1:"2",2:"3",3:"4",4:"5",5:"6",6:"7",7:"8",8:"9",9:"10",10:"J",11:"Q",12:"K",13:"A"}
 
     def __init__(self, **kwargs):
         super().__init__()
         gold = kwargs["gold"]
-        level = kwargs["level"]
+        level = kwargs.get("level",1)
         level = 1 if level < 1 else level
         level = 5 if level > 5 else level
         deck = Poker.random_poker()
         if level == 1:
             hand1 = deck[0:5]
             pt1 = self.cantrell_pt(hand1)
             hand2 = deck[5:10]
@@ -1152,54 +1164,55 @@
             result = Cantrell.cantrell_pt(hand)
             if result[0] > max_pt:
                 max_pt = result[0]
                 max_name = result[1]
                 max_hand = hand
         return max_hand,(max_pt,max_name)
 
-    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def action(self, bot:Bot, user_id:int, *args):
         """
         看牌|加注
         """
         session = self.session
-        if msg := session.shot_check(event):
+        if msg := session.shot_check(user_id):
             return None if msg == " " else msg
         if args[0] == 0:
-            return await self.cantrell_check(bot, event)
+            await self.cantrell_check(bot, user_id)
         else:
-            return await self.cantrell_play(bot, event, args[1])
+            msg = await self.cantrell_play(bot, user_id, args[1])
+            await bot.send_group_msg(group_id = session.group_id, message = msg)
 
-    async def cantrell_check(self, bot:Bot, event:GroupMessageEvent):
+    async def cantrell_check(self, bot:Bot, user_id:int):
         """
         看牌
         """
         session = self.session
         expose = int(round((session.round  + 0.5)/ 2)) + 3
         expose = min(expose,5)
         session.time = time.time() + 120
-        if event.user_id == session.player1_id:
+        if user_id == session.player1_id:
             hand = self.hand1
         else:
             hand = self.hand2
         msg = (
             "你的手牌：\n"
             + ("|" + "".join([f'{self.cantrell_suit[suit]}{self.cantrell_point[point]}|' for suit, point in hand[0:expose]]) + (5 - expose)*"   |")
             )
-        if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg, 50))):
-            await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
+        if not await Manager.try_send_private_msg(user_id = user_id, message = MessageSegment.image(linecard_to_png(msg))):
+            await bot.send_group_msg(group_id = session.group_id, message = f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
 
-    async def cantrell_play(self, bot:Bot, event:GroupMessageEvent, gold:int):
+    async def cantrell_play(self, bot:Bot, user_id:int, gold:int):
         """
         加注
         """
         session = self.session
         gold = self.gold if gold == None else gold
         gold = min(gold, session.bet_limit - session.gold)
         if gold > self.max_bet_gold:
-            return MessageSegment.at(event.user_id) + f"加注金额不能超过{self.max_bet_gold}"
+            return MessageSegment.at(user_id) + f"加注金额不能超过{self.max_bet_gold}"
         expose = session.round / 2
         session.nextround()
         session.time += 120
         if expose == int(expose):
             gold = max(gold, self.gold)
             session.gold += gold
             group_id = session.group_id
@@ -1209,28 +1222,28 @@
             cantrell_suit = self.cantrell_suit
             cantrell_point = self.cantrell_point
 
             msg = (
                 f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
                 "手牌：\n"
                 f'|{"".join([f"{cantrell_suit[suit]}{cantrell_point[point]}|" for suit, point in hand1])}{(5 - expose)*"   |"}'
-                "\n——————————————\n"
+                "\n----\n"
                 f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
                 "手牌：\n"
                 f'|{"".join([f"{cantrell_suit[suit]}{cantrell_point[point]}|" for suit, point in hand2])}{(5 - expose)*"   |"}'
                 )
 
             if expose == 5:
                 session.win = session.player1_id if self.pt1[0] > self.pt2[0] else session.player2_id
-                await self.end(bot, event)
+                await self.end(bot)
             else:
-                return MessageSegment.image(text_to_png(f"您已跟注{gold}金币\n" + msg, 50, width_simple = "——————————————"))
+                return MessageSegment.image(linecard_to_png(f"您已跟注{gold}金币\n" + msg, width = 880))
         else:
             self.gold = gold
-            return MessageSegment.at(event.user_id) + f"您已加注{gold}金币"
+            return MessageSegment.at(user_id) + f"您已加注{gold}金币"
 
     def game_tips(self, msg):
         """
         发起游戏：港式五张
         """
         return ("唰唰~，随机牌堆已生成\n"
                 f'开局金额：{self.gold}\n'
@@ -1238,38 +1251,34 @@
                 f'{msg}')
 
     def session_tips(self):
         tip1 = "本场对决为【港式五张】\n"
         tip2 = "\n看牌|加注\n"
         cantrell_suit = self.cantrell_suit
         cantrell_point = self.cantrell_point
-        tip2 += MessageSegment.image(text_to_png(
-                "P1初始手牌：\n"
-                "|"
-                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand1[0:3]]) +
-                "   |   |"
-                "\n——————————————\n"
-                'P2初始手牌\n'
-                "|"
-                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand2[0:3]]) +
-                "   |   |"
-                ),50)
+        tip2 += MessageSegment.image(linecard_to_png((
+            "P1初始手牌：\n"
+            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand1[0:3]]) + "   |   |"
+            "\n----\n"
+            'P2初始手牌\n'
+            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand2[0:3]]) + "   |   |"
+            ), width = 880))
         return self.acceptmessage(tip1, tip2);
 
     def end_tips(self):
         cantrell_suit = self.cantrell_suit
         cantrell_point = self.cantrell_point
-        return MessageSegment.image(text_to_png((
+        return MessageSegment.image(linecard_to_png((
             "P1手牌：\n"
             "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand1]) +
             f"\n牌型：\n{self.pt1[1]}"
-            "\n——————————————\n"
+            "\n----\n"
             "P2手牌：\n"
             "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand2]) +
-            f"\n牌型：\n{self.pt2[1]}"),50))
+            f"\n牌型：\n{self.pt2[1]}"), width = 880))
 
 class Blackjack(Game):
     """
     21点
     """
     name = "Blackjack"
     max_bet_gold:int = max_bet_gold *5
@@ -1277,14 +1286,15 @@
     Blackjack_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
     Blackjack_point = {1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"J",12:"Q",13:"K"}
 
     def __init__(self, **kwargs):
         super().__init__()
         gold = kwargs["gold"]
         deck = Poker.random_poker()
+        self.gold:int = gold
         self.deck = deck[2:]
         self.hand1 = [deck[0],]
         self.hand2 = [deck[1],]
         self.session.gold = gold
 
     @staticmethod
     def Blackjack_pt(hand:list) -> int:
@@ -1293,91 +1303,91 @@
         """
         pts = [x[1] if x[1] < 10 else 10 for x in hand]
         pt = sum(pts)
         if 1 in pts and pt <= 11:
             pt += 10
         return pt
 
-    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+    async def action(self, bot:Bot, user_id:int, *args):
         """
         抽牌|停牌|双倍下注
         """
         session = self.session
-        if msg := session.shot_check(event):
+        if msg := session.shot_check(user_id):
             return None if msg == " " else msg
-        code = args[0]
-        if code == 0:
-            return await self.Blackjack_Stand(bot, event)
-        elif code == 1:
-            return await self.Blackjack_Hit(bot, event)
+        card = args[0]
+        if card == "停牌":
+            await self.Blackjack_Stand(bot)
+        elif card == "抽牌":
+            await self.Blackjack_Hit(bot, user_id)
         else:
-            return await self.Blackjack_DoubleDown(bot, event)
+            await self.Blackjack_DoubleDown(bot, user_id)
 
-    async def Blackjack_Hit(self, bot:Bot, event:GroupMessageEvent):
+    async def Blackjack_Hit(self, bot:Bot, user_id:int):
         """
         抽牌
         """
         session = self.session
         session.time = time.time()
 
-        if event.user_id == session.player1_id:
+        if user_id == session.player1_id:
             hand = self.hand1
             session.win = session.player2_id
         else:
             hand = self.hand2
             session.win = session.player1_id
         deck = self.deck
         card = deck[0]
         del deck[0]
         hand.append(card)
         pt = self.Blackjack_pt(hand)
         if pt > 21:
-            await self.end(bot, event)
+            await self.end(bot)
         else:
             msg = (
                 "你的手牌：\n"
                 f'|{"".join([f"{self.Blackjack_suit[suit]}{self.Blackjack_point[point]}|" for suit, point in hand])}\n'
                 + f'合计:{pt}点')
-            if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,50))):
-                await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n你的手牌合计:{pt}点\n游戏继续！")
+            if not await Manager.try_send_private_msg(user_id = user_id, message = MessageSegment.image(linecard_to_png(msg))):
+                await bot.send_group_msg(group_id = session.group_id, message = f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
 
-    async def Blackjack_Stand(self, bot:Bot, event:GroupMessageEvent):
+    async def Blackjack_Stand(self, bot:Bot):
         """
         停牌
         """
         session = self.session
         session.nextround()
         if session.round == 2:
-            return Message(f"请{MessageSegment.at(session.player2_id)}\n抽牌|停牌|双倍下注")
+            await bot.send_group_msg(group_id = session.group_id, message = Message(f"请{MessageSegment.at(session.player2_id)}\n抽牌|停牌|双倍下注"))
         else:
             hand1 = self.hand1
             hand2 = self.hand2
             Blackjack_pt = self.Blackjack_pt
             if Blackjack_pt(hand1) > Blackjack_pt(hand2):
                 session.win = session.player1_id
             else:
                 session.win = session.player2_id
-            await self.end(bot, event)
+            await self.end(bot)
 
-    async def Blackjack_DoubleDown(self, bot:Bot, event:GroupMessageEvent):
+    async def Blackjack_DoubleDown(self, bot:Bot, user_id:int):
         """
         双倍下注
         """
         session = self.session
         session.gold += session.gold
         session.gold = min(session.gold, session.bet_limit)
-        await self.Blackjack_Hit(bot,event)
-        return await self.Blackjack_Stand(bot,event)
+        await self.Blackjack_Hit(bot,user_id)
+        await self.Blackjack_Stand(bot)
 
     def game_tips(self, msg):
         """
         发起游戏：21点
         """
         return ("唰唰~，随机牌堆已生成\n"
-                f'挑战金额：{self.session.gold}\n'
+                f'挑战金额：{self.gold}\n'
                 f'{msg}')
 
     def session_tips(self):
         hand1 = self.hand1[0]
         hand2 = self.hand2[0]
         Blackjack_suit = self.Blackjack_suit
         Blackjack_point = self.Blackjack_point
@@ -1389,266 +1399,615 @@
 
     def end_tips(self):
         hand1 = self.hand1
         hand2 = self.hand2
         Blackjack_suit = self.Blackjack_suit
         Blackjack_point = self.Blackjack_point
         Blackjack_pt = self.Blackjack_pt
-        return MessageSegment.image(text_to_png((
+        return MessageSegment.image(linecard_to_png((
             "P1手牌：\n"
             f'|{"".join([f"{Blackjack_suit[suit]}{Blackjack_point[point]}|" for suit, point in hand1])}\n'
             + f'合计:{Blackjack_pt(hand1)}点'
-            "\n——————————————\n"
+            "\n----\n"
             "P2手牌：\n"
             f'|{"".join([f"{Blackjack_suit[suit]}{Blackjack_point[point]}|" for suit, point in hand2])}\n'
-            f'合计:{Blackjack_pt(hand2)}点'),50))
+            f'合计:{Blackjack_pt(hand2)}点')))
+
+class ABCard(Game):
+    """
+    AB牌
+    """
+    name = "ABCard"
+    max_bet_gold:int = max_bet_gold
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        self.gold:int = gold
+        self.hand1 = ["A","B","1","2","3"]
+        self.hand2 = ["A","B","1","2","3"]
+        self.pt1 = 0
+        self.pt2 = 0
+        self.first = None
+        self.session.gold = gold
+
+    async def action(self, bot:Bot, user_id:int, *args):
+        """
+        出牌
+        """
+        session = self.session
+        if msg := session.shot_check(user_id):
+            return None if msg == " " else msg
+        group_id = session.group_id
+        card = args[0].upper()
+        if user_id == session.player1_id:
+            hand = self.hand1
+            if card in self.hand1:
+                hand.remove(card)
+                self.first = card
+                await bot.send_group_msg(group_id = group_id,message = MessageSegment.at(session.player2_id) + "对方已出牌，现在是你的回合。请打出你的手牌。")
+                session.nextround()
+                return
+            else:
+                return f"出牌失败。你的手牌还剩\n| {' | '.join(hand)} |"
+        else:
+            hand = self.hand2
+            if card in hand:
+                hand.remove(card)
+                msg = f"双方出牌 {self.first} - {card}\n"
+                if self.first == card:
+                    msg += "本轮是平局\n"
+                elif self.first == "A" or card == "B" or (self.first == "1" and card == "2") or (self.first == "2" and card == "3") or (self.first == "3" and card == "1"):
+                    self.pt1 += 1
+                    msg += MessageSegment.at(session.player1_id) + "赢得了本轮对决\n"
+                else:
+                    self.pt2 += 1
+                    msg += MessageSegment.at(session.player2_id) + "赢得了本轮对决\n"
+                msg += f"双方比分 {self.pt1} - {self.pt2}\n"
+                msg += f"当前赌注 {session.gold} 金币\n"
+                msg += f"P1手牌| {' | '.join(self.hand1)} |\n"
+                msg += f"P2手牌| {' | '.join(self.hand2)} |"
+                await bot.send_group_msg(group_id = group_id,message = msg)
+                session.gold += self.gold
+                session.gold = min(session.gold, session.bet_limit)
+                session.nextround()
+                if session.round == 9:
+                    self.first = self.hand1[0]
+                    card = self.hand2[0]
+                    msg = f"双方出牌 {self.first} - {card}\n"
+                    if self.first == card:
+                        msg += "本轮是平局\n"
+                    elif self.first == "A" or card == "B" or (self.first == "1" and card == "2") or (self.first == "2" and card == "3") or (self.first == "3" and card == "1"):
+                        self.pt1 += 1
+                        msg += MessageSegment.at(session.player1_id) + "赢得了本轮对决\n"
+                    else:
+                        self.pt2 += 1
+                        msg += MessageSegment.at(session.player2_id) + "赢得了本轮对决\n"
+                    session.gold += self.gold
+                    session.gold = min(session.gold, session.bet_limit)
+                    msg += f"双方比分 {self.pt1} - {self.pt2}\n"
+                    msg += f"当前赌注 {session.gold} 金币\n"
+                    session.win = session.player1_id if self.pt1 > self.pt2 else session.player2_id
+                    msg+= "获胜者：" + MessageSegment.at(session.win)
+                    await asyncio.sleep(0.5)
+                    await bot.send_group_msg(group_id = group_id,message = msg)
+                    await asyncio.sleep(1)
+                    await self.end(bot)
+                return
+            else:
+                return f"出牌失败。你的手牌还剩\n| {' | '.join(hand)} |"
+
+    def game_tips(self, msg):
+        """
+        发起游戏：AB牌
+        """
+        return ("双方手牌准备完毕\n"
+                f'挑战金额：{self.gold}/轮\n'
+                f'{msg}')
+
+    def session_tips(self):
+        tip1 = "本场对决为【AB牌】\n"
+        tip2 = "暗牌出牌"
+        return self.acceptmessage(tip1, tip2);
+
+    def end_tips(self):
+        return "" 
+
+class GunFight(Game):
+    """
+    西部枪战
+    """
+    name = "GunFight"
+    max_bet_gold:int = max_bet_gold *5
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        self.gold:int = gold
+        self.MAG1 = 1
+        self.MAG2 = 1
+        self.first = None
+        self.session.gold = gold
+
+    async def action(self, bot:Bot, user_id:int, *args):
+        """
+        装弹|开枪|闪避|闪枪|预判开枪
+        """
+        session = self.session
+        if msg := session.shot_check(user_id):
+            return None if msg == " " else msg
+        group_id = session.group_id
+        card = args[0]
+        if user_id == session.player1_id:
+            if card == "装弹":
+                self.MAG1 += 1
+                self.MAG1 = min(self.MAG1,6)
+            elif card in {"开枪","闪枪","预判开枪"}:
+                if self.MAG1 < 1:
+                    return f"行动失败。你的子弹不足"
+                self.MAG1 -= 1
+            self.first = card
+            session.nextround()
+            await bot.send_group_msg(group_id = group_id,message = MessageSegment.at(session.player2_id) + "对方已行动，现在是你的回合。")
+            return
+        else:
+            if card == "装弹":
+                self.MAG2 += 1
+                self.MAG2 = min(self.MAG2,6)
+            elif card in {"开枪","闪枪","预判开枪"}:
+                if self.MAG2 < 1:
+                    return f"行动失败。你的子弹不足"
+                self.MAG2 -= 1
+            session.nextround()
+            msg = f"双方行动 {self.first} - {card}\n"
+            msg += f"剩余子弹 {self.MAG1} - {self.MAG2}\n"
+            if self.first == "开枪" and card in {"装弹","预判开枪"} or self.first == "闪枪" and card in {"装弹","开枪"} or self.first == "预判开枪" and card in {"闪避","闪枪"}:
+                session.win = session.player1_id
+                msg += MessageSegment.at(session.player1_id) + "赢得了对决"
+            elif card == "开枪" and self.first in {"装弹","预判开枪"} or card == "闪枪" and self.first in {"装弹","开枪"} or card == "预判开枪" and self.first in {"闪避","闪枪"}:
+                session.win = session.player2_id
+                msg += MessageSegment.at(session.player2_id) + "赢得了对决"
+            else:
+                self.first = None
+                msg += f"本轮平局。请{MessageSegment.at(session.player1_id)}开始行动！"
+                await bot.send_group_msg(group_id = group_id,message = msg)
+                return
+            await bot.send_group_msg(group_id = group_id,message = msg)
+            await asyncio.sleep(1)
+            await self.end(bot)
+            
+    def game_tips(self, msg):
+        """
+        发起游戏：西部枪战
+        """
+        return ("场地准备完毕\n"
+                f'挑战金额：{self.gold}\n'
+                f'{msg}')
+
+    def session_tips(self):
+        tip1 = "本场对决为【西部枪战】\n"
+        tip2 = "\n装弹|开枪|闪避|闪枪|预判开枪"
+        return self.acceptmessage(tip1, tip2);
+
+    def end_tips(self):
+        return "" 
+
+def random_game(event:GroupMessageEvent, gold:int):
+    """
+    发起游戏：随机对战
+    """
+    group_account = Manager.locate_user(event)[1]
+    if group_account.props.get("32002",0) < 1:
+        return f"你未持有持有【{props_library['32002']['name']}】，无法发起随机对战。"
+
+    cls = random.choice([Russian,Dice,Poker,LuckyNumber,Cantrell,Blackjack,ABCard,GunFight])
+    return cls.creat(event, gold = gold)
 
 class AROF():
     """
     其他类
     """
-    def accept(self, event:GroupMessageEvent):
+    name:str = "AROF"
+
+    def __init__(self):
+        self.session:Session = Session()
+
+    @staticmethod
+    def parse_arg(arg:str):
+        if arg.isdigit():
+            gold = int(arg)
+        else:
+            gold = bet_gold
+        return {"gold":gold}
+
+    @classmethod
+    def creat(cls, event:GroupMessageEvent, **kwargs):
+        """
+        发起多人游戏
+        """
+        flag, msg = cls.start(event, **kwargs)
+        if flag == False:
+            return msg
+        return current_games[event.group_id].game_tips(msg)
+
+    @classmethod
+    def start(cls, event:GroupMessageEvent, **kwargs) -> Tuple[bool,Message]:
+        """
+        创建多人游戏
+        """
+        game = current_games.get(event.group_id)
+        if game:
+            if msg := game.create_check():
+                return False, msg
+            if msg := game.session.create_check(event):
+                return False, msg
+        group_id = kwargs["group_id"] = event.group_id
+        user_id = kwargs["user_id"] = event.user_id
+        game = current_games[group_id] = cls(**kwargs)
+        return True, MessageSegment.at(user_id)
+
+    def create_check(self):
+        session = self.session
+        world = self.world
+        overtime = time.time() - session.time + 180
+        if overtime < 180:
+            if world.start == 0:
+                return "一场游戏正在报名中"
+            else:
+                return f"一场游戏正在进行中，遇到问题可以{f'在{t}秒后' if (t := int(180 - overtime)) > 0 else ''}输入【游戏重置】重置游戏"
+
+    @abstractmethod
+    def join(self, event:GroupMessageEvent, *args):
+        """
+        加入游戏
+        """
+
+    def accept(self):
         """
         接受挑战
         """
         return None
 
-    def refuse(self, event:GroupMessageEvent):
+    def refuse(self):
         """
         拒绝挑战
         """
         return None
 
-    async def overtime(self, bot:Bot, event:GroupMessageEvent):
+    async def overtime(self):
         """
         超时结算
         """
         return None
 
-    async def fold(self, bot:Bot, event:GroupMessageEvent):
+    async def fold(self):
         """
         认输
         """
         return None
 
+    def restart(self):
+        """
+        游戏重置
+        """
+        session = self.session
+        group_id = session.group_id
+        overtime = time.time() - session.time + 180
+        if overtime < 180:
+            return f"当前游戏已创建 {int(overtime)} 秒，未超时。"
+        del current_games[group_id]
+        return "游戏已重置。"
+
+from .HorseRace.start import load_dlcs
+from .HorseRace.race_group import race_group
+
 class HorseRace(AROF):
     """
     赛马小游戏
     """
     name:str = "HorseRace"
 
     events_list = load_dlcs()
 
-    def __init__(self, event:GroupMessageEvent, gold:int ):
-        self.session = Session(
-            time = time.time() + 180,
-            player1_id = event.user_id,
-            at = -1,
-            gold = gold,
-            )
-        self.race_group = race_group()
-
-    def create_check(self):
-        session = self.session
-        race:race_group = self.race_group
-        overtime = time.time() - session.time + 180
-        if race.start == 0:
-            if overtime < 120:
-                return "一场赛马正在报名中"
-        else:
-            return f"一场赛马正在进行中，遇到问题可以{f'在{t}秒后' if (t := int(180 - overtime)) > 0 else ''}输入【赛马重置】重置游戏"
-
-        return None
-
-    @classmethod
-    def RaceNew(cls, event:GroupMessageEvent, gold:int):
-        """
-        赛马创建
-        """
-        game = current_games.get(event.group_id)
-        if game:
-            if game.name == cls.name and (msg := game.create_check()):
-                return msg
-            if msg := game.session.create_check(event):
-                return msg
-        current_games[event.group_id] =  cls(event, gold)
-        return ("\n"
-                 "> 创建赛马比赛成功！\n"
-                 "> 输入 【赛马加入 名字】 即可加入赛马。")
+    def __init__(self, **kwargs):
+        super().__init__()
+        self.session.time = time.time() + 180
+        self.session.group_id = kwargs["group_id"]
+        self.session.player1_id = kwargs["user_id"]
+        self.session.at = -1
+        self.session.gold = kwargs["gold"]
+        self.world = race_group()
 
-    def RaceJoin(self, event:GroupMessageEvent, horsename:str):
+    def join(self, event:GroupMessageEvent, *args):
         """
         赛马加入
         """
         if self.name != "HorseRace":
-            return "其他对战进行中。"
+            return "其他游戏进行中。"
+        session = self.session
         user,group_account = Manager.locate_user(event)
         user_id = user.user_id
-        session = self.session
         if (gold := group_account.gold) < session.gold:
             return f"报名赛马需要{self.session.gold}金币，你的金币：{gold}。"
-        race:race_group = self.race_group
+        race = self.world
         if race.start != 0:
             return
         if (query_of_player := race.query_of_player()) >= max_player:
             return "加入失败！赛马场就那么大，满了满了！"
         if race.is_player_in(user_id) == True:
             return "加入失败！您已经加入了赛马场!"
+        horsename = args[0] if args else None
         if not horsename:
             return "请输入你的马儿名字"
         horsename = horsename[:2]+"酱" if len(horsename) > 5 else horsename
         race.add_player(horsename, user_id, group_account.nickname)
-        user.gold -= session.gold
-        group_account.gold -= session.gold
-        return  ("\n"
-                 "> 加入赛马成功\n"
-                 "> 赌上马儿性命的一战即将开始!\n"
-                 f"> 赛马场位置:{query_of_player + 1}/{max_player}")
+        return  (
+            MessageSegment.at(user_id) + "\n" +
+            "> 加入赛马成功\n"
+            "> 赌上马儿性命的一战即将开始!\n"
+            f"> 赛马场位置:{query_of_player + 1}/{max_player}"
+            )
 
-    async def RaceStart(self, bot:Bot, event:GroupMessageEvent):
+    async def run(self, bot:Bot):
         """
         赛马开始
         """
         events_list = self.events_list
-        race:race_group = self.race_group
+        race = self.world
         if (player_count := race.query_of_player()) == 0:
             return
         if race.start == 1:
             return
         if race.start == 0 or race.start == 2:
             if player_count >= min_player:
                 race.start = 1
             else:
                 return f"开始失败！赛马开局需要最少{min_player}人参与"
 
-        group_id = event.group_id
         session = self.session
+        group_id = session.group_id
         session.time = time.time() + 180
-        await bot.send(event,(f'> 比赛开始\n'
-                              f'> 当前奖金：{session.gold * player_count}金币'))
+        await bot.send_group_msg(group_id = group_id, message = (
+            f'> 比赛开始\n'
+            f'> 当前奖金：{session.gold * player_count}金币'))
         await asyncio.sleep(0.5)
-
         while race.start == 1:
             # 回合数+1
             race.round_add()
             #移除超时buff
             race.del_buff_overtime()
             #马儿全名计算
             race.fullname()
             #回合事件计算
             text = race.event_start(events_list)
             #马儿移动
             race.move()
             #场地显示
             display = race.display()
         
-            output = text_to_png(display,30)
+            output = linecard_to_png(display, font_size = 30)
 
             try:
-                await bot.send(event,(Message(text) + MessageSegment.image(output)))
+                await bot.send_group_msg(group_id = group_id, message = (Message(text) + MessageSegment.image(output)))
             except:
                 text = ""
                 try:
-                    await bot.send(event,(MessageSegment.image(output)))
+                    await bot.send_group_msg(group_id = group_id,message =(MessageSegment.image(output)))
                 except:
                     pass
 
             await asyncio.sleep(0.5 + int(0.06 * len(text)))
             
             #全员失败计算
             if race.is_die_all():
                 for x in race.player:
                     uid = x.playeruid
                     if uid in user_data:
                         user = user_data[uid]
-                        user.gold += session.gold
-                        user.group_accounts[group_id].gold += session.gold
-
+                        user.gold -= session.gold
+                        user.group_accounts[group_id].gold  -= session.gold
                 del current_games[group_id]
-                return "比赛已结束，鉴定为无马生还"
+                await bot.send_group_msg(group_id = group_id,message = "比赛已结束，鉴定为无马生还")
+                return
 
             #全员胜利计算
             winer = race.is_win_all()
             winer_list="\n"
             if winer != []:
-                await bot.send(event,(f'> 比赛结束\n'
-                                      f'> {bot_name}正在为您生成战报...'))
+                await bot.send_group_msg(group_id = group_id,message = (
+                    f'> 比赛结束\n'
+                    f'> {bot_name}正在为您生成战报...'))
                 await asyncio.sleep(1)
                 gold = int(session.gold * player_count / len(winer))
+                for x in race.player:
+                    uid = x.playeruid
+                    if uid in user_data:
+                        user = user_data[uid]
+                        user.gold -= session.gold
+                        user.group_accounts[group_id].gold -= session.gold
                 for x in winer:
                     uid = x[1]
                     winer_list += "> "+ x[0] + "\n"
                     if uid in user_data:
                         user = user_data[uid]
                         user.gold += gold
-                        user.group_accounts[group_id].gold += gold
+                        user.group_accounts[group_id].gold  += gold
                 del current_games[group_id]
-                return (f"> 比赛已结束，胜者为：{winer_list}"
-                        f"> 本次奖金：{gold} 金币")
+                await bot.send_group_msg(group_id = group_id,message = (
+                    f"> 比赛已结束，胜者为：{winer_list}"
+                    f"> 本次奖金：{gold} 金币"))
+                return
             await asyncio.sleep(1)
 
-    def RaceReStart(self, event:GroupMessageEvent):
+    def game_tips(self, msg):
         """
-        赛马重置
+        发起游戏：赛马
         """
-        group_id = event.group_id
-        session = self.session
-        overtime = time.time() - session.time + 180
-        if overtime < 180:
-            return f"当前赛马已创建 {int(overtime)} 秒，未超时。"
-        race:race_group = self.race_group
-        for x in race.player:
-            uid = x.playeruid
-            if uid in user_data:
-                user = user_data[uid]
-                user.gold += session.gold
-                user.group_accounts[group_id].gold += session.gold
+        return (
+            msg + "\n" +
+            "> 创建赛马比赛成功！\n"
+            f"> 本场金额：{self.session.gold}金币\n"
+            "> 输入 【赛马加入 名字】 即可加入赛马。"
+            )
 
-        del current_games[group_id]
-        return "赛马场已重置。"
+from .Fortress.core import World
 
-def slot(event:MessageEvent, gold:int):
+class Fortress(AROF):
     """
-    幸运花色
+    要塞战
     """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
-    if gold > max_bet_gold:
-        return f'幸运花色每次最多{max_bet_gold}金币。'
-    if gold > group_account.gold:
-        return f'你没有足够的金币，你的金币：{user_data["group_account.gold:"]}。'
-    suit = {1:"♤",2:"♡",3:"♧",4:"♢"}
-    x = random.randint(1,4)
-    y = random.randint(1,4)
-    z = random.randint(1,4)
-    res = f"\n| {suit[x]} | {suit[y]} | {suit[z]} |\n"
-    l = len(set([x,y,z]))
-    if l == 1:
-        gold = gold * 7
-        msg =("你抽到的花色为：" +
-              res +
-              f"恭喜你获得了{gold}金币，祝你好运~")
-    elif l == 2:
-        gold = 0
-        msg =("你抽到的花色为：" +
-              res +
-              "祝你好运~")
-    else:
-        gold = -gold
-        msg =("你抽到的花色为：" +
-              res +
-              f"你失去了{-gold}金币 ，祝你好运~")
-    user.gold += gold
-    group_account.gold += gold
-    return msg
+    name:str = "Fortress"
 
-def random_game(event:GroupMessageEvent, gold:int):
-    """
-    发起游戏：随机对战
-    """
-    group_account = Manager.locate_user(event)[1]
-    if group_account.props.get("32002",0) < 1:
-        return f"你未持有持有【{props_library['32002']['name']}】，无法发起随机对战。"
+    def __init__(self, **kwargs):
+        super().__init__()
+        self.session.time = time.time() + 180
+        self.session.group_id = kwargs["group_id"]
+        self.session.player1_id = kwargs["user_id"]
+        self.session.at = -1
+        self.session.gold = kwargs["gold"]
+        self.world = World()
+
+    def join(self, event:GroupMessageEvent, *args):
+        """
+        要塞战加入
+        """
+        if self.name != "Fortress":
+            return "其他游戏进行中。"
+        session = self.session
+        user,group_account = Manager.locate_user(event)
+        user_id = user.user_id
+        if (gold := group_account.gold) < session.gold:
+            return f"报名要塞战需要{self.session.gold}金币，你的金币：{gold}。"
+        world:World = self.world
+        if world.start != 0:
+            return
+        if user_id in world.ids:
+            return "你已经加入了游戏"
+        if len(world.players) > 14:
+            return "人满了"
+        index = None
+        team = None
+        if args:
+            if len(args) == 1:
+                args = args[0]
+                if args.isdigit():
+                    index = int(args)
+                else:
+                    team = args
+            else:
+                index = args[0]
+                team = args[1]
+                if index.isdigit():
+                    index = int(args)
+                else:
+                    team = index
+                    index = None
+        if index:
+            if 0< index <= 14:
+                if index in world.players:
+                    return f"{index}号位置已经有人了\n请选择\n{','.join(i for i in range(1,15) if i not in world.castles)}" 
+            else:
+                return f"位置不存在。请选择\n{','.join(i for i in range(1,15) if i not in world.castles)}"
+        else:
+            index = random.choice([i for i in range(1,15) if i not in world.castles])
+
+        world.add_player(group_account,index,team or user_id)
+        return  (
+            MessageSegment.at(user_id) + "\n" +
+            "> 要塞战加入成功\n"
+            "> 战争即将开始!\n"
+            f"> 你的位置是 {index} 号城\n"
+            f"> 你的队伍是 {team if team else '个人'}"
+            )
 
-    cls = random.choice([Russian,Dice,Poker,LuckyNumber,Cantrell,Blackjack])
-    return cls.creat(event, gold = gold)
+    async def run(self, bot:Bot):
+        """
+        要塞战开始
+        """
+        world:World = self.world
+        N = len(world.players)
+        if N == 0:
+            return
+        if world.start != 0:
+            return
+        if N >= min_player:
+            world.start = 1
+        else:
+            return f"开始失败！要塞战需要最少{min_player}人参与"
+        group_id = self.session.group_id
+        await bot.send_group_msg(group_id = group_id, message = MessageSegment.image(world.draw()))
+        msg = "请" + MessageSegment.at(world.ids[0]) + "开始行动"
+        await bot.send_group_msg(group_id = group_id, message = msg)
+
+    async def AROF_start(self, bot:Bot, user_id:int):
+        """
+        开始行动
+        """
+        world:World = self.world
+        start = world.start
+        if start == 0:
+            return
+        start -= 1
+        if world.ids[start] != user_id:
+            return "现在不是你的回合。"
+        if world.act != 0:
+            return "你的回合已开始。"
+        world.act = 1
+        world.round += 1
+        msg = ""
+        for index in range(0,15):
+            if (castle := world.castles.get(index)) and castle.user_id == world.ids[start]:
+                msg += f"你的{index}号城获得了：\n{castle.turntable()}\n"
+        group_id = self.session.group_id
+        await bot.send_group_msg(group_id = group_id, message = msg[:-1])
+        await asyncio.sleep(1)
+        await bot.send_group_msg(group_id = group_id, message = MessageSegment.image(world.draw()))
+
+    async def AROF_end(self, bot:Bot, user_id:int):
+        """
+        结束行动
+        """
+        world:World = self.world
+        start = world.start
+        if start == 0:
+            return
+        start -= 1
+        if world.ids[start] != user_id:
+            return "现在不是你的回合。"
+        world.act = 0
+        msg = ""
+        world.start += 1
+        if world.start > (len(world.ids)):
+            world.start = 1
+            world.round += 1
+        msg = "请" + MessageSegment.at(world.ids[world.start - 1]) + "开始行动"
+        group_id = self.session.group_id
+        await bot.send_group_msg(group_id = group_id, message = msg)
+
+    async def AROF_action(self, bot:Bot, user_id:int, *args):
+        """
+        行动
+        """
+        world:World = self.world
+        start = world.start
+        if start == 0:
+            return
+        start -= 1
+        if world.ids[start] != user_id:
+            return "现在不是你的回合。"
+        if world.act == 0:
+            await self.AROF_start(bot,user_id)
+            await asyncio.sleep(1)
+        msg = "|".join(args)
+        group_id = self.session.group_id
+        await bot.send_group_msg(group_id = group_id, message = msg)
+
+    def game_tips(self, msg):
+        """
+        发起游戏：要塞战
+        """
+        return (
+            msg + "\n" +
+            "> 要塞战创建成功！\n"
+            f"> 本场金额：{self.session.gold}金币\n"
+            "> 输入 【要塞加入 编号 队伍】 即可加入要塞战。"
+            )
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from typing import Tuple,Dict
 from pathlib import Path
+from collections import Counter
 from nonebot.adapters.onebot.v11 import (
     Bot,
     Message,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment,
     )
-from collections import Counter
+from nonebot import get_driver
+from nonebot.log import logger
 
 from .utils.utils import image_url
-from .utils.chart import text_to_png, gini_coef, default_BG
+from .utils.chart import linecard_to_png, gini_coef, default_BG
 from .utils.avatar import download_url
-from .data import DataBase, UserDict, GroupAccount, GroupDict
-from .data import props_library
+from .data import DataBase, UserDict, GroupAccount, GroupDict, Company, props_library
 from .config import revolt_gold, max_bet_gold, lucky_clover, path, BG_image
 
+driver = get_driver()
+
 # 加载数据
 
 datafile = path / "russian_data.json"
 
 if datafile.exists():
     with open(datafile, "r") as f:
         data = DataBase.loads(f.read())
 else:
     data = DataBase(file = datafile)
 
+log = data.verification()
+logger.info(f"\n{log}")
+
 user_data = data.user
 group_data = data.group
 
 """+++++++++++++++++
 |     ／l、        |
 |   （ﾟ､ 。７      |
 |　   l、 ~ヽ      |
@@ -37,60 +43,52 @@
 +++++++++++++++++"""
 
 def locate_user(event:MessageEvent) ->Tuple[UserDict,GroupAccount]:
     """
     定位个人账户
     """
     user_id = event.user_id
-    user = user_data.setdefault(user_id,UserDict())
-    user.init(event)
+    user = user_data.setdefault(user_id,UserDict(event))
     if isinstance(event,GroupMessageEvent):
         group_id = event.group_id
-        group = group_data.setdefault(group_id,GroupDict())
-        group.init(event.group_id)
+        group = group_data.setdefault(group_id,GroupDict(group_id = group_id,company = Company(company_id = group_id)))
         namelist = group.namelist
         if user_id in namelist:
             group_account = user.group_accounts[group_id]
-            group_account.init(event)
+            group_account.nickname = event.sender.card or event.sender.nickname
         else:
             namelist.add(user_id)
-            user.group_accounts[group_id] = GroupAccount()
+            user.group_accounts[group_id] = GroupAccount(event)
             group_account = user.group_accounts[group_id]
-            group_account.init(event)
             data.save()
     else:
         group_id = user.connect
         if group_id:
             group_account = user.group_accounts[group_id]
         else:
             group_account = None
 
     return user,group_account
 
-async def locate_user_at(bot:Bot, event:GroupMessageEvent, user_id:int) ->Tuple[UserDict,GroupAccount]:
+def locate_user_at(event:GroupMessageEvent, user_id:int) ->Tuple[UserDict,GroupAccount]:
     """
     定位at账户
     """
     if user_id not in user_data:
-        info = await bot.get_group_member_info(group_id = event.group_id, user_id = user_id)
-        user_data[user_id] = UserDict(user_id = user_id, nickname = info["nickname"])
-
+        user_data[user_id] = UserDict(user_id = user_id, nickname = str(user_id))
     user = user_data[user_id]
     group_id = event.group_id
-    group = group_data.setdefault(group_id,GroupDict())
-    group.init(event.group_id)
+    group = group_data.setdefault(group_id,GroupDict(group_id = group_id))
     namelist = group.namelist
 
     if user_id not in namelist:
         namelist.add(user_id)
-        user.group_accounts[group_id] = GroupAccount(group_id = group_id, nickname = user.nickname)
+        user.group_accounts[group_id] = GroupAccount(group_id = group_id,nickname = user.nickname)
         data.save()
-
     group_account = user.group_accounts[group_id]
-
     return user,group_account
 
 company_index:Dict[str,int] = {}
 
 def update_company_index():
     """
     从群数据生成公司名查找群号的字典
@@ -151,42 +149,42 @@
     user,group_account = locate
     rank = []
     count = group_account.gold
     if count > max_bet_gold:
         count = int(count/max_bet_gold)
         count = str(count) if count < 1000 else "MAX"
         level =f"Lv.{count}"
-        rank.append(f"◆ 金库 {level}")
+        rank.append(f"◆金库 {level}")
 
     count = user.Achieve_win
     if count >1:
         count = str(count) if count < 1000 else "MAX"
         level =f"Lv.{count}"
-        rank.append(f"◆ 连胜 {level}")
+        rank.append(f"◆连胜 {level}")
 
     count = user.Achieve_lose
     if count >1:
         count = str(count) if count < 1000 else "MAX"
         level =f"Lv.{count}"
-        rank.append(f"◇ 连败 {level}")
+        rank.append(f"◇连败 {level}")
 
     return rank
 
-def group_wealths(group_id:int) -> float:
+def group_wealths(group_id:int, level:int = 1) -> float:
     """
     群内总资产
     """
     if group_id in group_data:
         namelist = group_data[group_id].namelist
     else:
-        return None
-    total = 0
+        return 0
+    total = 0.0
     for user_id in namelist:
         group_account = user_data[user_id].group_accounts[group_id]
-        total += group_account.gold + group_account.value
+        total += group_account.gold*level + group_account.value
     return total
 
 def group_ranklist(group_id:int , title:str) -> list:
     """
     群内排行榜
         param:
         group_id:群号
@@ -313,92 +311,19 @@
         group_account = user_data[user_id].group_accounts[group_id]
         rank.append(group_account.gold + group_account.value)
 
     rank = [x for x in rank if x > limit]
     rank.sort()
     return gini_coef(rank)
 
-def Newday():
-    """
-    刷新每日
-    """
-    log = ""
-    group_check = {k:set() for k in group_data}
-    update_company_index()
-    company_ids = company_index.values()
-    stock_check = {k:0 for k in company_ids}
-    # 检查user_data
-    for user_id in user_data:
-        user = user_data[user_id]
-        user.transfer_limit = 0
-        props = user.props
-        props = {k:v-1 if k[2] == '0' else v for k, v in props.items()}
-        user.props = {k:v for k, v in props.items() if v > 0}
-        group_accounts = user.group_accounts
-        gold = 0
-        for group_id in list(group_accounts.keys()):
-            if group_id not in group_check:
-                log += f"{user.nickname} 群账户{group_id}无效，已删除。\n"
-                del group_accounts[group_id]
-            else:
-                group_check[group_id].add(user_id)
-                group_account = group_accounts[group_id]
-                group_account.is_sign = False
-                group_account.security = 0
-                gold += group_account.gold
-                props = group_account.props
-                props = {k:v-1 if k[2] == '0' else v for k, v in props.items()}
-                group_account.props = {k:v for k, v in props.items() if v > 0}
-                stocks = group_account.stocks
-                for company_id in list(stocks.keys()):
-                    if company_id in stock_check:
-                        stock_check[company_id] += stocks[company_id]
-                    else:
-                        log += f"{user.nickname} 群账户{group_id}内股票{company_id}回收异常，数据已修正。\n"
-                        del stocks[company_id]
-        if user.gold != gold:
-            log += f"{user.nickname} 金币总数异常。记录值：{user.gold} 实测值：{gold} 数据已修正。\n"
-            user.gold = gold
-
-    # 检查group_data
-    for group_id in group_data:
-        group = group_data[group_id]
-        if group.namelist != group_check[group_id]:
-            log += (
-                f"{group_id} 群名单异常。\n"
-                f"记录多值：{group.namelist - group_check[group_id]}\n"
-                f"记录少值：{group_check[group_id] - group.namelist}\n"
-                "数据已修正。\n"
-                )
-            group.namelist = group_check[group_id]
-
-        if group_id in company_ids:
-            company = group.company
-            if company.stock + stock_check[group_id] != company.issuance:
-                log += (
-                    f"{company.company_name} 股票数量异常。\n"
-                    f"记录值：{company.stock}\n"
-                    f"实测值：{company.issuance - stock_check[group_id]}\n"
-                    "数据已修正。\n"
-                    )
-                company.stock = company.issuance - stock_check[group_id]
-    data.save()
-    return log[:-1] if log else "数据一切正常！"
-
-from nonebot import get_driver
-driver = get_driver()
-bot_list = set()
-driver.on_bot_connect(lambda bot:bot_list.add(bot))
-driver.on_bot_disconnect(lambda bot:bot_list.discard(bot))
-
 async def try_send_private_msg(user_id:int, message: Message) -> bool:
     """
     发送私聊消息
     """
-    global bot_list
+    bot_list = driver.bots.values()
     for bot in bot_list:
         friend_list = await bot.get_friend_list()
         friend_list = [friend["user_id"] for friend in friend_list]
         if user_id in friend_list:
             await bot.send_private_msg(user_id = user_id, message = message)
             return True
     return False
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Market.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,43 +4,44 @@
     Bot,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment
     )
 
 import random
+import math
 import time
 import datetime
 import asyncio
 
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
-from .utils.chart import linecard, group_info_head, info_Splicing
+from .utils.chart import linecard, group_info_head, info_splicing
 from .data import GroupAccount, Company, ExchangeInfo
 from .data import OHLC, props_library
-from .config import bot_name, revolt_gini, max_bet_gold, path
-
-from .Manager import data, company_index
-from .Manager import BG_path, update_company_index
+from .config import bot_name, revolt_gini, max_bet_gold, bet_gold, path
 
 from . import Manager
 
+data = Manager.data
 user_data = data.user
 group_data = data.group
 
+company_index = Manager.company_index
+
 def check_company_name(company_name:str):
     """
     检查公司名是否合法
     """
     if not company_name:
         return f"公司名称不能为空"
-    update_company_index()
+    Manager.update_company_index()
     if company_name in company_index:
         return f"{company_name} 已被注册"
     if " " in company_name or "\n" in company_name:
         return "公司名称不能含有空格或回车"
     count = 0
     for x in company_name:
         if ord(x) < 0x200:
@@ -62,31 +63,31 @@
     """
     group_id = event.group_id
     company = group_data[group_id].company
     if company.company_name:
         return f"本群已在市场注册，注册名：{company.company_name}"
     if check := check_company_name(company_name):
         return check
-    if (gold := (Manager.group_wealths(group_id) or 0)) < (limit := 15 * max_bet_gold):
+    gold = Manager.group_wealths(group_id)
+    if gold < (limit := 15 * max_bet_gold):
         return f"本群金币（{round(gold,2)}）小于{limit}，注册失败。"
     if (gini := Manager.Gini(group_id)) > 0.56:
         return f"本群基尼系数（{round(gini,3)}）过高，注册失败。"
-    gold = Manager.group_wealths(group_id)
     company = group_data[group_id].company
     company.company_id = group_id
     company.company_name = company_name
-    company.level = 1
     company.time = time.time()
-    company.stock = 20000
-    company.issuance = 20000
+    company.level = sum(group_data[group_id].Achieve_revolution.values()) + 1
+    company.issuance = 20000*company.level
+    company.stock = company.issuance
     company.gold = gold * 0.8
     company.float_gold = company.gold
     company.group_gold = gold
     company.intro = f"发行初始信息\n金币 {round(gold,2)}\n基尼系数{round(gini,3)}\n{company_name} 名称检查通过\n发行成功！"
-    update_company_index()
+    Manager.update_company_index()
     data.save()
     return f'{company_name}发行成功，发行价格为每股{round((gold/ 20000),2)}金币'
 
 def rename(event:GroupMessageEvent,company_name:str):
     """
     公司重命名
         company_name:公司名
@@ -98,15 +99,15 @@
     user = Manager.locate_user(event)[0]
     if user.props.get("33001",0) < 1:
         return f"你的【{props_library['33001']['name']}】已失效"
     if check := check_company_name(company_name):
         return check
     old_company_name = company.company_name
     company.company_name = company_name
-    update_company_index()
+    Manager.update_company_index()
     return f'【{old_company_name}】已重命名为【{company_name}】'
 
 def value_update(group_account:GroupAccount):
     """
     刷新持股价值
     group_account:用户群账户
     """
@@ -139,59 +140,60 @@
     company = group_data[company_id].company
     company_name = company.company_name
 
     buy = company.stock if company.stock < buy else buy
     if buy < 1:
         return "已售空，请等待结算或在交易市场购买。"
 
-    group_gold = Manager.group_wealths(company_id) or 0
-    company.group_gold = group_gold
+    group_gold = Manager.group_wealths(company_id,company.level)
+
     if group_gold < 10 * max_bet_gold:
         return f"【{company_name}】金币过少({group_gold})，无法交易。"
-
-    gold = max(group_gold, company.float_gold)
+    float_gold = company.float_gold
     SI = company.issuance
-    gini = Manager.Gini(company_id)
     value = 0.0
-    for _ in range(buy):
-        unit = gold/SI
-        gold += unit * gini
-        value += unit
-    else:
-        value = int(value + 0.5)
+    inner_buy = 0
     my_gold = group_account.gold
-    if value > my_gold:
-        return (
-            f"{company_name}\n"
-            "——————————\n"
-            f"数量：{buy}\n"
-            f"单价：{round(value/buy,2)}\n"
-            f"总计：{value}\n"
-            "——————————\n"
-            f"金币不足（{my_gold}）"
-            )        
-    else:
-        company.stock -= buy
-        group_account.stocks.setdefault(company_id,0)
-        group_account.stocks[company_id] += buy
-        user.gold -= value
-        group_account.gold -= value
-        company.gold += value
-        company.float_gold += value
-        company.group_gold = group_gold
-        value_update(group_account)
-        return (
-            f"{company_name}\n"
-            "——————————\n"
-            f"数量：{buy}\n"
-            f"单价：{round(value/buy,2)}\n"
-            f"总计：{value}\n"
-            "——————————\n"
-            "交易成功！"
-            )
+    for _ in range(buy):
+        value += max(group_gold, float_gold)/SI
+        float_gold += float_gold/SI
+        if my_gold > value:
+            inner_buy += 1
+        else:
+            break
+    value = int(value)
+    if inner_buy < 1:
+        return f"购买失败，你的金币不足（{my_gold}）！"
+    # 结算股票
+    company.stock -= inner_buy
+    group_account.stocks[company_id] = group_account.stocks.get(company_id,0) + inner_buy
+    # 结算金币
+    user.gold -= value
+    group_account.gold -= value
+    company.gold += value
+    # 更新公司信息
+    company.group_gold = group_gold
+    company.float_gold = float_gold
+    ## 自动发布交易信息
+    #if user.user_id not in company.exchange:
+    #    company.exchange[user.user_id] = ExchangeInfo(
+    #        group_id = group_account.group_id,
+    #        quote = round(value * 1.2/inner_buy,2),
+    #        n = inner_buy)
+    # 更新群账户信息
+    value_update(group_account)
+    return (
+        f"{company_name}\n"
+        "——————————\n"
+        f"数量：{inner_buy}\n"
+        f"单价：{round(value/inner_buy,2)}\n"
+        f"总计：{value}\n"
+        "——————————\n"
+        "交易成功！"
+        )
 
 def settle(event:MessageEvent, settle:int, company_name:str):
     """
     以债务价值结算股票
         settle:结算数量
         company_name:股票名
     """ 
@@ -208,51 +210,52 @@
 
     if my_stock < settle:
         return f"你没有足够的股份...你的 {company_name} 还有 {my_stock} 个"
 
     company = group_data[company_id].company
     company_name = company.company_name
 
-    group_gold = Manager.group_wealths(company_id) or 0
-    company.group_gold = group_gold
+    group_gold = Manager.group_wealths(company_id,company.level)
+
     if group_gold < 10 * max_bet_gold:
         return f"【{company_name}】金币过少({group_gold})，无法交易。"
 
-    gold = company.float_gold
+    float_gold = company.float_gold
     SI = company.issuance
-    gini = Manager.Gini(company_id)
     value = 0.0
     for _ in range(settle):
-        unit = gold/SI
-        gold -= unit * gini
-        value += unit
-    else:
-        value = int(value + 0.5)
+        value += float_gold/SI
+        float_gold -= float_gold/SI
+    value = int(value)
 
     if group_account.props.get("42001",0):
         fee = 0
         tips = f"『{props_library['42001']['name']}』免手续费"
     else:
         fee = int(value * 0.02)
         tips = f"扣除2%手续费：{fee}"
 
+    # 结算股票
     company.stock += settle
     if group_account.stocks[company_id] == settle:
         del group_account.stocks[company_id]
+        stock = 0
     else:
-        group_account.stocks[company_id] -= settle
+        stock = group_account.stocks[company_id] = group_account.stocks.get(company_id) - settle
+    # 结算金币
     user.gold += value - fee
     group_account.gold += value - fee
     company.gold -= value
-    company.float_gold -= value
+    # 更新公司信息
     company.group_gold = group_gold
-    if user.user_id in company.exchange:
-        del company.exchange[user.user_id]
+    company.float_gold = float_gold
+    # 更新交易市场
+    exchange.n = stock if (user_id := user.user_id) in company.exchange and (exchange := company.exchange[user_id]).group_id == group_account.group_id and stock< exchange.n else exchange.n
+    # 更新群账户信息
     value_update(group_account)
-
     return (
         f"{company_name}\n"
         "——————————\n"
         f"数量：{settle}\n"
         f"单价：{round(value/settle,2)}\n"
         f"总计：{value} - {fee}\n"
         "——————————\n"
@@ -374,25 +377,48 @@
         if exchange.get(user_id):
             del exchange[user_id]
             tips = "交易信息已注销。"
         else:
             tips = "交易信息无效。"
     else:
         quote = exchange_info.quote
-        unit = company.group_gold if company.group_gold < company.float_gold else company.float_gold
-        unit = unit / company.issuance
-        if quote < (1  if (tmp := unit/4) < 1 else tmp) or quote > (max_bet_gold if (tmp := 10 * unit) < max_bet_gold else tmp):
+        float_gold = company.float_gold
+        SI = company.issuance
+        unit = min(company.group_gold,float_gold) / SI
+        if quote > max(bet_gold, 10 * unit):
             tips = "报价异常，发布失败。"
         else:
-            if exchange.get(user_id):
+            if user_id in exchange:
                 tips = "交易信息已修改。"
             else:
                 tips = "交易信息发布成功！"
             exchange[user_id] = exchange_info
 
+        # 自动结算交易市场上的股票
+        value = 0.0
+        settle = 0
+        for _ in range(n):
+            unit = float_gold/SI
+            if unit < quote:
+                break
+            value += quote
+            float_gold -= float_gold/SI
+            settle += 1
+
+        value = int(value)
+        if settle > 0:
+            # 结算股票
+            company.Buyback(group_account,settle)
+            # 结算金币
+            user.gold += value
+            group_account.gold += value
+            company.gold -= value
+            # 更新公司信息
+            company.float_gold = float_gold
+
     return (
         f"{company.company_name}\n"
         "——————————\n"
         f'报价：{quote}\n'
         f'数量：{n}\n'
         "——————————\n"
         + tips
@@ -407,15 +433,18 @@
         company = group.company
     else:
         return f"没有 {group_id} 的注册信息"
 
     info = []
     # 加载群信息
     company_name = company.company_name
-    group_info = await bot.get_group_info(group_id = group_id)
+    try:
+        group_info = await bot.get_group_info(group_id = group_id)
+    except:
+        group_info = {"group_name":"群聊已注销","member_count":3000}
     group_name = group_info["group_name"]
     member_count = group_info["member_count"]
     if member_count == 0:
         member_count = 3000
     else:
         member_count = member_count - 1
 
@@ -456,26 +485,26 @@
             msg += f"{user_data[x[0]].nickname}\n[pixel][20]单价 {x[1].quote}[nowrap]\n[pixel][400]数量 {x[1].n}\n"
         if msg:
             info.append(linecard(msg, width = 880, font_size = 40,endline = "市场详情"))
         msg = company.intro
         if msg:
             info.append(linecard(msg + '\n', width = 880, font_size = 40,endline = "公司介绍"))
 
-    return MessageSegment.image(info_Splicing(info, BG_path(event.user_id)))
+    return MessageSegment.image(info_splicing(info, Manager.BG_path(event.user_id)))
 
 def stock_profile(company:Company) -> str:
     """
     产业信息
     """
     group_gold = company.group_gold
     float_gold = company.float_gold
     issuance = company.issuance
     msg = (
         f"固定资产 {'{:,}'.format(round(company.gold,2))}\n"
-        f"市场流动 {'{:,}'.format(round(company.group_gold))}\n"
+        f"市场流动 {'{:,}'.format(round(group_gold))}\n"
         f"发行价格 {'{:,}'.format(round(max(group_gold,float_gold)/issuance,2))}\n"
         f"结算价格 {'{:,}'.format(round(float_gold/issuance,2))}\n"
         f"剩余数量 {company.stock}\n"
         )
     return msg
 
 def Market_info_All(event:MessageEvent, ohlc:bool = False):
@@ -496,15 +525,15 @@
         info = []
         for company in seg:
             info.append(linecard(company.company_name +"\n" + "----\n" + stock_profile(company)[:-1],width = 880))
         msg.append({"type":"node",
                     "data":{
                         "name":f"{bot_name}",
                         "uin":str(event.self_id),
-                        "content":MessageSegment.image(info_Splicing(info, BG_path(event.user_id)))}})
+                        "content":MessageSegment.image(info_splicing(info, Manager.BG_path(event.user_id)))}})
     return msg
 
 def update_intro(company_name:str, intro:str):
     if company_name in company_index:
         company_id = company_index[company_name]
     else:
         return f"没有 {company_name} 的注册信息"
@@ -523,29 +552,63 @@
 def company_update(company:Company):
     """
     刷新公司信息
         company:公司账户
     """
     company_id = company.company_id
     # 更新全群金币数
-    group_gold = Manager.group_wealths(company_id)
+    group_gold = Manager.group_wealths(company_id,company.level)
     company.group_gold = group_gold
     # 固定资产回归值 = 80%全群金币数 + 40%股票融资 总计：80%~120%全群金币数
-    line = group_gold * (1.2 - 0.4 * (company.stock / company.issuance))
+    SI = company.issuance
+    line = group_gold * (1.2 - 0.4 * (company.stock / SI))
     # 公司金币数回归到固定资产回归值
-    company.gold += (line - company.gold)/96
-    # 股票价格变化 = 趋势性影响（正态分布） + 随机性影响（平均分布）
-    float_gold = company.float_gold
-    float_gold += company.float_gold * random.gauss(0,0.03) + company.gold * random.uniform(-0.1, 0.1)
-    # 股票价格向债务价值回归
     gold = company.gold
-    deviation = gold - float_gold
-    float_gold += deviation * 0.1 * abs(deviation)/gold
+    gold += (line - gold)/96
+    company.gold = gold
+    if gold > 0.0:
+        # 股票价格变化 = 趋势性影响（正态分布） + 随机性影响（平均分布）
+        float_gold = company.float_gold
+        float_gold += float_gold * random.gauss(0,0.03) + gold * random.uniform(-0.1, 0.1)
+        # 股票价格向债务价值回归
+        deviation = gold - float_gold
+        float_gold +=  0.1 * deviation * abs(deviation / gold)
+        # Nan检查
+        float_gold = group_gold if math.isnan(float_gold) else float_gold
+        # 自动结算交易市场上的股票
+        Exlist = []
+        for user_id,exchange in company.exchange.items():
+            n = 0
+            quote = exchange.quote
+            for _ in range(exchange.n):
+                if quote < float_gold/SI:
+                    float_gold -= float_gold/SI
+                    n += 1
+                else:
+                    break
+            if n:
+                Exlist.append((user_id,quote,n))
+        for user_id,quote,n in Exlist:
+            if not (user := user_data.get(user_id)):
+                continue
+            if not (group_account := user.group_accounts.get(exchange.group_id)):
+                continue
+            value = int(quote*n)
+            # 结算股票
+            company.Buyback(group_account,n)
+            # 结算金币
+            user.gold += value
+            group_account.gold += value
+            company.gold -= value
+    else:
+        float_gold = 0.0
+
     # 更新浮动价格
     company.float_gold = float_gold
+
     # 记录价格历史
     global market_history
     market_history.setdefault(company_id,[]).append((time.time(), group_gold / company.issuance, float_gold / company.issuance))
     market_history[company_id] = market_history[company_id][-720:]
 
 def update():
     """
@@ -559,8 +622,20 @@
         log += f"{company.company_name} 更新成功！\n"
 
     for user_id in user_data:
         group_accounts = user_data[user_id].group_accounts
         for group_id in group_accounts:
             value_update(group_accounts[group_id])
 
-    return log[:-1]
+    return log[:-1]
+
+def reset():
+    """
+    市场重置
+    """
+    company_ids = set([company_index[company_id] for company_id in company_index])
+    for company_id in company_ids:
+        company = group_data[company_id].company
+        group_gold = Manager.group_wealths(company_id,company.level)
+        company.group_gold = group_gold
+        company.float_gold = group_gold * (1.2 - 0.4 * (company.stock / company.issuance))
+        company.gold = company.float_gold
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Prop.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
     MessageEvent,
     GroupMessageEvent,
     MessageSegment
     )
 import random
 
 from .utils.utils import get_message_at
-from .utils.chart import linecard_to_png
-from .data import props_library, props_index, element_library
+from .utils.chart import linecard_to_png,line_splicing
+from .data import GroupAccount, props_library, props_index
 from .config import bot_name, sign_gold, revolt_gold, max_bet_gold, gacha_gold
 
-from .Manager import data
+from .Alchemy import Alchemy
 from . import Manager
 
+data = Manager.data
 user_data = data.user
 group_data = data.group
 
 
-
 def random_props() -> str:
     """
     随机获取道具。
         rare:稀有度
         return:道具代码
         道具代码规则：
         第1位：稀有度
@@ -172,15 +172,15 @@
         elif pt < 2.44:
             level = "[left][color][#003399]☆ ☆ ☆[nowrap][passport]\n[center]高斯分布[nowrap][passport]\n[right]☆ ☆ ☆"
         elif pt < 2.72:
             level = "[left][color][#0033CC]☆ ☆ ☆ ☆[nowrap][passport]\n[center]对称破缺[nowrap][passport]\n[right]☆ ☆ ☆ ☆"
         elif pt < 3:
             level = "[left][color][#0033FF]☆ ☆ ☆ ☆ ☆[nowrap][passport]\n[center]概率之子[nowrap][passport]\n[right]☆ ☆ ☆ ☆ ☆"
         else:
-            level = "[noautowrap][center][color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
+            level = "[center][color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
         msg = (
             f"{level}\n"
             "----\n"
             f"抽卡次数：{N}[nowrap]\n"f"[pixel][450]空气占比：{round(air*100/N,2)}%\n"
             f"获得☆：{star}[nowrap]\n"f"[pixel][450]获得☆：{airstar}\n"
             f"平均每抽☆数：{round(pt,3)}[nowrap]\n"f"[pixel][450]空气质量：{round(airstar/air,3)}\n"
             f"数据来源：{group_account.nickname}\n"
@@ -190,15 +190,15 @@
         msg = (
             f"{group_account.nickname}\n"
             "----\n"
             f"抽卡次数：{N}\n"
             "----\n"
             ) + msg
         
-    return MessageSegment.image(linecard_to_png(msg))
+    return MessageSegment.image(linecard_to_png(msg,font_size = 40 , width = 880, endline = "抽卡结果"))
 
 class Prop(str):
     def use(self, event:MessageEvent, count:int):
         """
         使用道具
         """
         if self == "03101":
@@ -322,56 +322,67 @@
         elif pt < 2.44:
             level = "[left][color][#003399]☆ ☆ ☆[nowrap][passport]\n[center]实验级[nowrap][passport]\n[right]☆ ☆ ☆"
         elif pt < 2.72:
             level = "[left][color][#0033CC]☆ ☆ ☆ ☆[nowrap][passport]\n[center]分析级[nowrap][passport]\n[right]☆ ☆ ☆ ☆"
         elif pt < 3:
             level = "[left][color][#0033FF]☆ ☆ ☆ ☆ ☆[nowrap][passport]\n[center]超纯级[nowrap][passport]\n[right]☆ ☆ ☆ ☆ ☆"
         else:
-            level = "[noautowrap][center][color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
+            level = "[center][color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
 
         msg = (
             f"{level}\n"
             "----\n"
             f"抽卡次数：{N}[nowrap]\n"f"[pixel][450]空气占比：{round(air*100/N,2)}%\n"
             f"获得☆：{star}[nowrap]\n"f"[pixel][450]获得☆：{airstar}\n"
             f"平均每抽☆数：{round(pt,3)}[nowrap]\n"f"[pixel][450]空气质量：{round(airstar/air,3)}\n"
             f"数据来源：{group_account.nickname}\n"
             "----\n"
             ) + msg
 
-        return MessageSegment.image(linecard_to_png(msg))
+        return MessageSegment.image(linecard_to_png(msg,font_size = 40, width = 880,endline = "抽卡结果"))
 
     @classmethod
     def use_33101(cls, event:MessageEvent, count:int) -> str:
         """
         使用道具：初级元素
         """
         user,group_account = Manager.locate_user(event)
         if not group_account:
             return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+
         props = user.props
         if props.get("33101",0) < count:
             return "数量不足"
 
         props["33101"] -= count
         if props["33101"] < 1:
             del props["33101"]
 
         res = {}
-        for i in range(count*4):
-            element_code = f"0{random.randint(1,4)}01"
-            res.setdefault(element_code,0)
-            res[element_code] += 1
-        msg = "你获得了\n"
-        for element_code in res:
-            n = res[element_code]
-            user.alchemy.setdefault(element_code,0)
-            user.alchemy[element_code] += n
-            msg += f'{element_library[element_code]["name"]}：{n}个\n' 
-        return msg + "祝你好运~"
+        info = []
+        if count <= 20:
+            msg = ""
+            for _ in range(count):
+                originproduct = random.choices(Alchemy.elements,k = 3)
+                product = Alchemy.ProductsLibrary.get("".join(list(set(originproduct))),"")
+                msg += f'|{"|".join(Alchemy.ProductsName[x] for x in originproduct)}| >>>> {Alchemy.ProductsName[product]}\n'
+                res[product] = res.get(product, 0) + 1
+            info.append(f"合成结果：\n----\n{msg[:-1]}")
+        else:
+            res = Alchemy.do(count)
+        msg = ""
+        for product,N in res.items():
+            if product:
+                user.alchemy[product] = user.alchemy.get(product, 0) + N
+            msg += f'{Alchemy.ProductsName[product]}：{N}个\n'
+        info.append(f"你获得了：\n----\n{msg[:-1]}")
+        if count < 3:
+            return "\n".join(info) + "\n祝你好运"
+        else:
+            return MessageSegment.image(line_splicing(info))
 
     @classmethod
     def use_42101(cls, event:MessageEvent) -> str:
         """
         使用道具：调查凭证
         """
         if isinstance(event, GroupMessageEvent):
@@ -380,28 +391,26 @@
             return f"此道具只能在群内使用"
 
         if not (at := get_message_at(event.message)):
             return "没有指定用户。"
         else:
             at = int(at[0])
 
-        if at not in group_data[group_id].namelist:
-            return "对方没有账户。"
-
         user,group_account = Manager.locate_user(event)
+        target_user,target_group_account = Manager.locate_user_at(event,at)
+
         props = group_account.props
         if props.get("42101",0) < 1:
             return "数量不足"
 
         props["42101"] -= 1
         if props["42101"] < 1:
             del props["42101"]
 
-        target_user = user_data[at]
-        target_group_account = target_user.group_accounts[group_id]
+
         N = random.randint(0,50)
         if N < 30:
             gold = int(group_account.gold * N / 1000)
             gold = 0 if gold < 0 else gold
             user.gold -= gold
             group_account.gold -= gold
             target_user.gold += gold
@@ -446,16 +455,16 @@
             del props["52101"]
 
         group_id = group_account.group_id
         ranklist = Manager.group_ranklist(group_id,"金币")
         target_id = random.choice([x[0] for x in ranklist if x[1] > revolt_gold[0]])
         if target_id == event.user_id:
             return f"道具使用失败，你损失了一个『{props_library['52101']['name']}』"
-        target_user = user_data[target_id]
-        target_group_account = target_user.group_accounts[group_id]
+
+        target_user,target_group_account = Manager.locate_user_at(event, target_id)
 
         change = int((group_account.gold - target_group_account.gold) / 2)
         limit = min((group_account.gold, target_group_account.gold))
         limit = 0 if limit < 0 else limit
         if change > limit:
             change = limit
         if change < -limit:
@@ -529,15 +538,14 @@
             del props["52102"]
 
         if random.randint(0,X) > 0:
             user.gold += gold
             group_account.gold += gold
             return f"你获得了{gold}金币"
         else:
-            gold = int(group_account.gold/2)
             user.gold -= gold
             group_account.gold -= gold
             user.props.setdefault("53101",0)
             user.props["53101"] += 1
             return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
 
     @classmethod
@@ -607,21 +615,21 @@
         if props["63102"] < 1:
             del props["63102"]
 
         group_id = group_account.group_id
         user_id = user.user_id
         for company_id in group_account.stocks:
             company = group_data[company_id].company
-            company.stock += group_account.stocks[company_id]
-            exchange = company.exchange
-            if user_id in exchange:
-                del exchange[user_id]
+            company.Buyback(group_account)
         user.gold -= group_account.gold
-        group_data[group_id].namelist.remove(user_id)
-        del group_account
+        group_account.__init__(
+            user_id = group_account.user_id,
+            group_id = group_account.group_id,
+            nickname = group_account.nickname
+            )
         return "你在本群的账户已重置，祝你好运~"
 
 def use_prop(event:MessageEvent, prop_name:str, count:int):
     if prop_code := props_index.get(prop_name):
         return Prop(prop_code).use(event,count)
     else:
         return f"没有【{prop_name}】这种道具。"
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from nonebot.adapters.onebot.v11 import (
     GROUP,
-    PRIVATE,
     GROUP_ADMIN,
     GROUP_OWNER,
     Bot,
     MessageEvent,
     GroupMessageEvent,
     Message,
 )
+from nonebot import get_driver
 from nonebot.permission import SUPERUSER
 from nonebot import on_message, on_command, on_regex, on_fullmatch
 from nonebot.params import CommandArg, Arg
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot.rule import to_me
 from nonebot import require
@@ -29,114 +29,164 @@
 import shutil
 
 from . import Manager
 from . import Account
 from . import Market
 from . import Game
 from . import Prop
+from . import Alchemy
 
 from .utils.utils import get_message_at, number
-from .data import ExchangeInfo
-from .config import revolt_cd, bet_gold, path, backup
-from .Manager import data, company_index
-from .Game import current_games
+from .data import ExchangeInfo,menu_data
+from .config import Config, revolt_cd, bet_gold, path, backup
 
+from nonebot.plugin import PluginMetadata
 
-try:
-    from nonebot.plugin import PluginMetadata
-    from .data import menu_data
-    __plugin_meta__ = PluginMetadata(
-        name = "小游戏合集",
-        description = "各种群内小游戏",
-        usage = "",
-        extra = {
-            'menu_data':menu_data,
-            'menu_template':'default'
-            }
-        )
-except ModuleNotFoundError:
-    logger.info("当前nonebot版本无法使用插件元数据。")    
+__plugin_meta__ = PluginMetadata(
+    name = "小游戏合集",
+    description = "各种群内小游戏",
+    usage = "金币签到",
+    config = Config,
+    extra = {'menu_data':menu_data,'menu_template':'default'})
+
+data = Manager.data
+company_index = Manager.company_index
+current_games = Game.current_games
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
+def to_int(arg:Message, default:int = bet_gold):
+    num = arg.extract_plain_text().strip()
+    if num.isdigit():
+        return int(num)
+    else:
+        return default
+
+AllGameTips = {
+    "HorseRace":"赛马活动未开始，请输入【赛马创建】创建赛马场",
+    "Fortress":"要塞战未开始，请输入【要塞战创建】创建要塞战游戏",
+    }
 
-# 赛马创建
-RaceNew = on_command("赛马创建", aliases = {"创建赛马"}, permission = GROUP, priority = 20, block = True)
+# 加入游戏
+AllJoinGameCommand = {
+    "HorseRace":{"赛马加入","加入赛马"},
+    "Fortress":{"要塞加入","堡垒加入","加入要塞","加入堡垒"},
+    }
 
-@RaceNew.handle()
-async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
+AllJoinGameCommand = {cmd: name for name, cmds in AllJoinGameCommand.items() for cmd in cmds}
+async def join_game_rule(bot:Bot, event:GroupMessageEvent, state:T_State) -> bool:
+    """
+    规则：加入游戏
+    """
+    msg = event.message.extract_plain_text()
+    for cmd in AllJoinGameCommand:
+        if msg.startswith(cmd):
+            game = current_games.get(event.group_id)
+            name = AllJoinGameCommand[cmd]
+            if game:
+                if game.name == name:
+                    state["Game"] = game
+                    state["arg"] = msg[len(cmd):].strip()
+                    return True
+                return False
+            else:
+                await bot.send(event,AllGameTips[name])
+                return False
     else:
-        gold = bet_gold
-    msg =  Game.HorseRace.RaceNew(event, gold)
-    await RaceNew.finish(msg, at_sender = True)
-
-# 赛马加入
-RaceJoin = on_command(
-    "赛马加入",
-    aliases = {"加入赛马"},
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
+        return False
 
-@RaceJoin.handle()
-async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    if not (game := current_games.get(event.group_id)):
-        msg = "赛马活动未开始，请输入【赛马创建】创建赛马场"
-    elif game.name == "HorseRace":
-        msg =  game.RaceJoin(event, arg.extract_plain_text().strip())
-    await RaceJoin.finish(msg, at_sender = True)
-
-# 赛马开始
-RaceStart = on_command(
-    "赛马开始",
-    aliases = {"开始赛马"},
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
-@RaceStart.handle()
+join_game = on_message(rule = join_game_rule, permission = GROUP, priority = 20, block = True)
+
+@join_game.handle()
+async def _(event:GroupMessageEvent, state:T_State):
+    game = state["Game"]
+    msg = game.join(event,state["arg"])
+    await join_game.finish(msg)
+
+# 开始游戏
+AllRunGameCommand = {
+    "HorseRace":{"赛马开始","开始赛马"},
+    "Fortress":{"游戏开始","开始游戏"},
+    }
+AllRunGameCommand = {cmd: name for name, cmds in AllRunGameCommand.items() for cmd in cmds}
+
+async def run_game_rule(bot:Bot, event:GroupMessageEvent, state:T_State) -> bool:
+    """
+    规则：开始游戏
+    """
+    msg = event.message.extract_plain_text()
+    for cmd in AllRunGameCommand:
+        if msg.startswith(cmd):
+            game = current_games.get(event.group_id)
+            name = AllRunGameCommand[cmd]
+            if game:
+                if game.name == name:
+                    state["Game"] = game
+                    return True
+                return False
+            else:
+                await bot.send(event,AllGameTips[name])
+                return False
+    else:
+        return False
+
+async def AROF_check(event:GroupMessageEvent, state:T_State):
+    """
+    本群有AROF
+    """
+    group_id = event.group_id
+    if group_id in current_games and current_games[group_id].name in {"Fortress"}:
+        state["game"] = current_games[group_id]
+        return True
+    else:
+        return False
+
+# 回合开始
+AROF_start = on_command("回合开始", rule = AROF_check, priority = 20, block = True)
+
+@AROF_start.handle()
 async def _(bot:Bot, event:GroupMessageEvent):
-    if not (game := current_games.get(event.group_id)):
-        msg = "赛马活动未开始，请输入【赛马创建】创建赛马场"
-    elif game.name == "HorseRace":
-        msg = await game.RaceStart(bot, event)
-    await RaceStart.finish(msg)
-
-# 赛马重置
-RaceReStart = on_command(
-    "赛马重置",
-    aliases = {"重置赛马"},
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
+    game = current_games[event.group_id]
+    msg = await game.AROF_start(bot,event.user_id)
+    await AROF_start.finish(msg)
+
+# 回合结束
+AROF_end = on_command("回合结束", rule = AROF_check, priority = 20, block = True)
+@AROF_end.handle()
+async def _(bot:Bot, event:GroupMessageEvent):
+    game = current_games[event.group_id]
+    msg = await game.AROF_end(bot,event.user_id)
+    await AROF_end.finish(msg)
 
-@RaceReStart.handle()
+# 行动
+AROF_action = on_command("行动", rule = AROF_check, priority = 20, block = True)
 
-async def _(event:GroupMessageEvent):
-    if not (game := current_games.get(event.group_id)):
-        msg = "赛马活动未开始，请输入【赛马创建】创建赛马场"
-    elif game.name == "HorseRace":
-        msg = game.RaceReStart(event)
-    await RaceReStart.finish(msg)
+@AROF_action.handle()
+async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
+    game = current_games[event.group_id]
+    msg = await game.AROF_action(bot,event.user_id,*arg.extract_plain_text().strip().split())
+    await AROF_action.finish(msg)
+
+run_game = on_message(rule = run_game_rule, permission = GROUP, priority = 20, block = True)
+
+@run_game.handle()
+async def _(bot:Bot, state:T_State):
+    game = state["Game"]
+    msg = await game.run(bot)
+    await run_game.finish(msg)
 
 # 赛马暂停
 RaceStop = on_command(
     "赛马暂停",
     aliases = {"暂停赛马"},
     rule = lambda event:isinstance(event,GroupMessageEvent) and event.group_id in current_games and current_games[event.group_id].name == "HorseRace",
     permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority = 20,
     block = True
     )
-
 @RaceStop.handle()
 async def _(event:GroupMessageEvent):
     current_games[event.group_id].race_group.start = 2
 
 # GameClear
 GameClear = on_command(
     "GameClear",
@@ -152,19 +202,15 @@
     del current_games[event.group_id]
 
 # 获取金币
 gold_create = on_command("获取金币", permission = SUPERUSER, priority = 20, block = True)
 
 @gold_create.handle()
 async def _(event:MessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = 0
+    gold = to_int(arg,bet_gold)
     msg =  Account.gold_create(event,gold)
     await gold_create.finish(msg, at_sender=True)
 
 # 获取道具
 props_create = on_command("获取道具", permission = SUPERUSER, priority = 20, block = True)
 
 @props_create.handle()
@@ -177,15 +223,14 @@
     elif test >1:
         prop_name = arg[0]
         count = number(arg[1])
         if count < 1:
             count = 1
     else:
         return
-
     msg = Account.props_create(event, prop_name, count)
     await give_props.finish(msg, at_sender = True)
 
 # 金币签到
 sign = on_command("金币签到", aliases = {"轮盘签到"}, priority = 20, block = True)
 
 @sign.handle()
@@ -225,23 +270,23 @@
         gold = int(gold)
     else:
         return
     if at := get_message_at(event.message):
         at = int(at[0])
     else:
         return
-    target = await Manager.locate_user_at(bot, event, at)
+    target = Manager.locate_user_at(event, at)
     msg = Account.transfer_gold(event, target, gold)
     await give_gold.finish(msg, at_sender = True)
 
 # 送道具
 give_props = on_command("送道具", aliases = {"赠送道具"}, permission = GROUP, priority = 20, block = True)
 
 @give_props.handle()
-async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg(),):
+async def _(event:GroupMessageEvent, arg:Message = CommandArg(),):
     arg = arg.extract_plain_text().strip().split()
     at = get_message_at(event.message)
     test = len(arg)
     if test and at:
         at = at[0]
         if test == 1:
             prop_name = arg[0]
@@ -250,46 +295,56 @@
             prop_name = arg[0]
             count = number(arg[1])
             if count < 1:
                 count = 1
     else:
         return
 
-    target = await Manager.locate_user_at(bot, event, int(at))
+    target = Manager.locate_user_at(event, int(at))
     msg = Account.transfer_props(event, target, prop_name, count)
     await give_props.finish(msg, at_sender = True)
 
 from .Game import current_games
 
 # 创建游戏
 
 AllCreateGameCommand = {
     "Russian":{"俄罗斯轮盘","装弹"},
     "Dice":{"掷色子", "摇色子", "掷骰子", "摇骰子"},
     "Poker":{"扑克对战", "扑克对决", "扑克决斗"},
     "LuckyNumber":{"猜数字"},
     "Cantrell":{"同花顺","港式五张","梭哈"},
     "Blackjack":{"21点"},
+    "ABCard":{"AB牌","ab牌"},
+    "GunFight":{"西部枪战","西部对战","牛仔对战","牛仔对决"},
+    "HorseRace":{"赛马创建","创建赛马"},
+    "Fortress":{"堡垒战创建","要塞战创建","创建堡垒战","创建要塞战"},
     }
 
 AllCreateGameCommand = {cmd: name for name, cmds in AllCreateGameCommand.items() for cmd in cmds}
 
+AllGames = {
+    "Russian":Game.Russian,
+    "Dice":Game.Dice,
+    "Poker":Game.Poker,
+    "LuckyNumber":Game.LuckyNumber,
+    "Cantrell":Game.Cantrell,
+    "Blackjack":Game.Blackjack,
+    "ABCard":Game.ABCard,
+    "GunFight":Game.GunFight,
+    "HorseRace":Game.HorseRace,
+    "Fortress":Game.Fortress,
+    }
+
 def create_game_rule(event:GroupMessageEvent, state:T_State)-> bool:
     """
     规则：创建对局
     """
-    msg = str(event.message)
-    AllGames = {
-        "Russian":Game.Russian,
-        "Dice":Game.Dice,
-        "Poker":Game.Poker,
-        "LuckyNumber":Game.LuckyNumber,
-        "Cantrell":Game.Cantrell,
-        "Blackjack":Game.Blackjack,
-        }
+    msg = event.message.extract_plain_text()
+
     for cmd in AllCreateGameCommand:
         if msg.startswith(cmd):
             state["Game"] = AllGames[AllCreateGameCommand[cmd]]
             state["arg"] = msg[len(cmd):].strip()
             return True
     else:
         return False
@@ -308,68 +363,73 @@
 AllPlayGameCommand = {
     "Russian":{"开枪","咔", "嘭", "嘣"},
     "Dice":{"取出","开数", "开点"},
     "Poker":{"出牌"},
     "LuckyNumber":{"^\d{1,3}$"},
     "Cantrell":{"看牌","加注","跟注","开牌"},
     "Blackjack":{"停牌","抽牌","双倍下注"},
+    "ABCard":{"A","a","B","b","1","2","3"},
+    "GunFight":{"装弹","开枪","闪避","闪枪","预判开枪"},
     }
 
-def game_play_rule(event:GroupMessageEvent, state:T_State)-> bool:
+def game_play_rule(event:MessageEvent, state:T_State)-> bool:
     """
     规则：游戏进行
     """
-    group_id = event.group_id
+    user,group_account = Manager.locate_user(event)
+    if not group_account:
+        return False
+    group_id = user.connect
     game = current_games.get(group_id)
-    if game and (Name := game.name) not in ["HorseRace"]:
-        msg = str(event.message)
+    if game and (Name := game.name) not in {"HorseRace"}:
+        cmdlst = AllPlayGameCommand.get(Name)
+        if not cmdlst:
+            return False
+        msg = event.message.extract_plain_text()
         state["game"] = game
         if Name == "LuckyNumber":
             if msg.isdigit() and 0 < (N := int(msg)) <= 100:
-                state["arg"] = [N]
+                state["arg"] = (N,)
+                return True
+        elif Name in {"Blackjack","ABCard","GunFight"}:
+            if msg in cmdlst:
+                state["arg"] = (msg,)
                 return True
         else:
-            cmdlst = AllPlayGameCommand.get(Name)
             for cmd in cmdlst:
                 if msg.startswith(cmd):
                     msg = msg[len(cmd):].strip()
                     if Name == "Cantrell":
                         if msg.isdigit():
                             gold = int(msg)
                         else:
                             gold = None
-                        state["arg"] = [{"看牌":0,"加注":1,"跟注":1,"开牌":1}[cmd], gold]
-                    elif Name == "Blackjack":
-                        state["arg"] = [{"停牌":0,"抽牌":1,"双倍下注":2}[cmd]]
+                        state["arg"] = ({"看牌":0,"加注":1,"跟注":1,"开牌":1}[cmd], gold)
                     elif msg.isdigit():
-                        state["arg"] = [int(msg)]
+                        state["arg"] = (int(msg),)
                     else:
-                        state["arg"] = [None]
+                        state["arg"] = (None,)
 
                     return True
     return False
 
-game_play = on_message(rule = game_play_rule, permission = GROUP, priority = 20, block = True)
+game_play = on_message(rule = game_play_rule, priority = 15, block = True)
 
 @game_play.handle()
-async def _(bot:Bot, event:GroupMessageEvent, state:T_State):
+async def _(bot:Bot, event:MessageEvent, state:T_State):
     game = state["game"]
-    msg = await game.play(bot, event, *state["arg"])
-    await create_game.finish(msg)
+    msg = await game.play(bot, event.user_id, *state["arg"])
+    await game_play.finish(msg)
 
 # 随机对战
 random_game = on_command("随机对战", permission = GROUP, priority = 5, block = True)
 
 @random_game.handle()
 async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = -1
+    gold = to_int(arg,-1)
     msg = Game.random_game(event, gold)
     await random_game.finish(msg)
 
 async def session_check(event:GroupMessageEvent, state:T_State):
     """
     本群有对局
     """
@@ -391,46 +451,42 @@
 
 # 拒绝挑战
 refuse = on_command("拒绝挑战", aliases={"拒绝决斗", "拒绝对决"}, rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @refuse.handle()
 async def _(event:GroupMessageEvent, state:T_State):
     game = state["game"]
-    msg = game.refuse(event)
+    msg = game.refuse(event.user_id)
     await refuse.finish(msg)
 
 # 超时结算
 overtime = on_command("超时结算", rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @overtime.handle()
-async def _(bot:Bot, event:GroupMessageEvent, state:T_State):
+async def _(bot:Bot, state:T_State):
     game = state["game"]
-    msg = await game.overtime(bot, event)
+    msg = await game.overtime(bot)
     await overtime.finish(msg)
 
 # 认输结算
 fold = on_fullmatch(("认输", "投降", "结束"), rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @fold.handle()
 async def _(bot:Bot, event:GroupMessageEvent, state:T_State):
     game = state["game"]
-    await game.fold(bot, event)
+    await game.fold(bot, event.user_id)
 
-# 幸运花色
-slot = on_command("幸运花色", aliases = {"抽花色"}, permission = PRIVATE, priority = 20, block = True)
+# 游戏重置
+restart = on_command("游戏重置", aliases={"重置游戏"}, rule = session_check, permission = GROUP, priority = 20, block = True)
 
-@slot.handle()
-async def _(event:MessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = bet_gold
-    msg = Game.slot(event, gold)
-    await slot.finish(msg, at_sender=True)
+@restart.handle()
+async def _(state:T_State):
+    game = state["game"]
+    msg = game.restart()
+    await restart.finish(msg)
 
 # 抽卡
 gacha = on_regex("^.+连抽?卡?|单抽", rule = to_me(), priority = 20, block = True)
 
 @gacha.handle()
 async def _(bot:Bot, event:MessageEvent):
     cmd = event.get_plaintext()
@@ -495,14 +551,39 @@
 my_info = on_command("我的信息", aliases = {"我的资料"}, priority = 20, block = True)
 
 @my_info.handle()
 async def _(event:MessageEvent):
     msg = await Account.my_info(event)
     await my_info.finish(msg)
 
+# 我的交易信息
+my_exchange = on_fullmatch(("我的交易信息","我的报价","我的股票"), priority = 20, block = True)
+
+@my_exchange.handle()
+async def _(event:MessageEvent):
+    msg = await Account.my_exchange(event)
+    await my_exchange.finish(msg)
+
+# 元素精炼
+alchemy_refine = on_command("元素精炼", priority = 20, block = True)
+
+@alchemy_refine.handle()
+async def _(event:MessageEvent, arg:Message = CommandArg()):
+    Products = arg.extract_plain_text().strip().split()
+    msg = Alchemy.alchemy_refine(event,Products)
+    await alchemy_refine.finish(msg)
+
+# 炼金资料卡
+alchemy_info = on_command("炼金账户", aliases = {"炼金资料"}, priority = 20, block = True)
+
+@alchemy_info.handle()
+async def _(event:MessageEvent):
+    msg = await Alchemy.my_info(event)
+    await alchemy_info.finish(msg)
+
 # 我的道具
 my_props = on_command("我的道具", aliases = {"我的仓库"}, priority = 20, block = True)
 
 @my_props.handle()
 async def _(event:MessageEvent):
     msg = Account.my_props(event)
     await my_props.finish(msg)
@@ -790,25 +871,25 @@
     confirm = random.randint(1000,9999)
     matcher.set_arg("freeze", (int(at),str(confirm)))
     nickname = (await bot.get_group_member_info(group_id = event.group_id, user_id = at))["nickname"]
     await freeze.send(f"您即将冻结 {nickname}（{at}），请输入{confirm}来确认。")
 
 @freeze.got("code")
 
-async def _(bot:Bot, event:MessageEvent, matcher:Matcher, code :Message = Arg()):
+async def _(event:MessageEvent, matcher:Matcher, code :Message = Arg()):
     at,confirm = matcher.get_arg("freeze")
     if confirm == str(code):
-        target = await Manager.locate_user_at(bot, event, at)
+        target = Manager.locate_user_at(event, at)
         msg = Account.freeze(target[0])
         await freeze.finish(msg)
     else:
         await freeze.finish("【冻结】已取消。")
 
 # 清理无效账户
-delist = on_command("清理无效账户", rule = to_me(), permission = SUPERUSER, priority = 20, block = True)
+delist = on_fullmatch("清理无效账户", rule = to_me(), permission = SUPERUSER, priority = 20, block = True)
 
 @delist.handle()
 async def _():
     await delist.send("正在启动清理程序。")
     log = await Account.delist()
     logger.info("\n" + log)
     with open(path / "delist.log","a",encoding = "utf8") as f:
@@ -823,14 +904,22 @@
 # 股市更新
 @scheduler.scheduled_job("cron", minute = "0,*/5")
 async def _():
     log = Market.update()
     if log:
         logger.info("\n" + log)
 
+# 市场重置
+Market_reset = on_fullmatch("市场重置", permission = SUPERUSER, priority = 20, block = True)
+
+@Market_reset.handle()
+async def _():
+    Market.reset()
+    await Market_reset.finish("市场已重置。")
+
 # 数据备份
 Backup = on_command("Backup", aliases = {"数据备份", "游戏备份"}, permission = SUPERUSER, priority = 20, block = True)
 
 @Backup.handle()
 @scheduler.scheduled_job("cron", hour = "0,*/4")
 async def _():
     now = time.strftime('%Y-%m-%d %H-%M-%S', time.localtime(time.time()))
@@ -844,24 +933,23 @@
 
 # 刷新每日
 Newday = on_command("Newday", aliases = {"刷新每日", "刷新签到"}, permission = SUPERUSER, priority = 20, block = True)
 
 @Newday.handle()
 @scheduler.scheduled_job("cron", hour = 0)
 async def _():
-    log = Manager.Newday()
-    logger.info("\n" + log)
+    Manager.update_company_index()
+    log = data.verification()
+    logger.info(f"\n{log}")
+    data.Newday()
     with open(path / "Newday.log","a",encoding = "utf8") as f:
-        f.write(
-            f"\n{datetime.datetime.fromtimestamp(time.time()).strftime('%Y 年 %m 月 %d 日 %H:%M:%S')}\n"
-            "——————————————\n"
-            + log + "\n"
-            "——————————————\n"
-            )
-
+        f.write(f"\n{datetime.datetime.fromtimestamp(time.time()).strftime('%Y 年 %m 月 %d 日 %H:%M:%S')}\n"
+                "——————————————\n"
+                f"{log}\n"
+                "——————————————\n")
     folders = [f for f in backup.iterdir() if f.is_dir()]
     for folder in folders:
         if time.time() - folder.stat().st_ctime > 604800:
             shutil.rmtree(folder)
             logger.info(f'备份 {folder} 已删除！')
 
 # 保存数据
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Tuple
 from pydantic import BaseModel, Extra
 
-class Config(BaseModel, extra=Extra.ignore):
+class Config(BaseModel, extra = Extra.ignore):
     # 每日签到的范围
     sign_gold:Tuple[int, int] = (200, 500)
     # 每日补贴的范围
     security_gold:Tuple[int, int] = (100, 300)
     # 重置签到的范围
     revolt_gold:Tuple[int, int] = (1000, 2000)
     # 重置冷却时间，设置为0禁用发起重置
@@ -18,14 +18,31 @@
     bet_gold:int = 200
     # 单抽所需金币
     gacha_gold:int = 50
     # 一个测试字符串，不要动（
     lucky_clover = "• ＬＵＣＫＹ  ＣＬＯＶＥＲ •"
     # 默认显示字体
     game_fontname = "simsun"
+    game_fallback_fonts = [
+        "Arial",
+        "Tahoma",
+        "Microsoft YaHei",
+        "Segoe UI",
+        "Segoe UI Emoji",
+        "Segoe UI Symbol",
+        "Helvetica Neue",
+        "PingFang SC",
+        "Hiragino Sans GB",
+        "Source Han Sans SC",
+        "Noto Sans SC",
+        "Noto Sans CJK JP",
+        "WenQuanYi Micro Hei",
+        "Apple Color Emoji",
+        "Noto Color Emoji",
+        ]
 
     """+++++++++++++++++
     ——————————
        下面是赛马设置
     ——————————
     +++++++++++++++++"""
 
@@ -78,14 +95,15 @@
 revolt_cd = config.revolt_cd
 revolt_gini = config.revolt_gini
 max_bet_gold = config.max_bet_gold
 bet_gold = config.bet_gold
 gacha_gold = config.gacha_gold
 lucky_clover = config.lucky_clover
 fontname = config.game_fontname
+fallback_fonts = config.game_fallback_fonts
 setting_track_length = config.setting_track_length
 setting_random_min_length = config.setting_random_min_length
 setting_random_max_length = config.setting_random_max_length
 base_move_min = config.base_move_min
 base_move_max = config.base_move_max
 max_player = config.max_player
 min_player = config.min_player
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6560975609756097%*

 * *Differences: {'1': "{'detail_des': '金币签到：\\n玩家每日可签到一次，每日0点刷新。\\n重置签到：\\n每次重置后可领取一次，每日刷新有几率刷新重置签到。'}",*

 * * '10': "{'detail_des': '道具分为全局道具和群内道具\\n群内道具最多叠 30 天/个\\n部分道具可使用。'}",*

 * * '12': "{'detail_des': '总金币排行\\n总资产排行\\n金币排行\\n资产排行\\n胜率排行\\n胜场排行\\n败场排行\\n路灯挂件排行'}",*

 * * '13': "{'func': '总排行榜', 'trigger_method': '金币总排行', 'brief_des': '查看排行榜', 'detail_des': "*

 * *       "'金币总排行\\n资产总排行\\n胜率总排行\\n胜场总排行\\n败场总排行\\n路灯挂件总排行'}",*

 * * '14': "{'trigger_method': '接受挑战 拒绝挑战 认输 超时结算 游戏重置'}",*

 * * '16': "{'trigger_condition': '赌注上限为1倍赌注上限', 'brief_des': '开枪 […]*

```diff
@@ -4,39 +4,46 @@
         "detail_des": "\u83b7\u53d6\u91d1\u5e01 \u6570\u91cf\uff1a\n\u83b7\u53d6\u91d1\u5e01\n\u83b7\u53d6\u9053\u5177 \u9053\u5177\u540d \u6570\u91cf\uff1a\n\u6bcf\u6b21\u91cd\u7f6e\u540e\u53ef\u9886\u53d6\u4e00\u6b21\u3002\u5237\u65b0\u6bcf\u65e5\uff1a\n\u5237\u65b0\u6bcf\u65e5\u7b7e\u5230\uff0c\u8865\u8d34\uff0c\u91d1\u5e01\u8f6c\u79fb\u4e0a\u9650\uff0c\u6240\u6709\u4eba\u65f6\u6548\u9053\u5177\u7684\u5269\u4f59\u65f6\u95f4-1\n\u4fdd\u5b58\u6570\u636e\uff1a\n\u5728\u5173bot\u524d\u9700\u8981\u4fdd\u5b58\u6570\u636e\uff0c\u4e0d\u7136\u4f1a\u56de\u6863\u5230\u4e0a\u6b21\u81ea\u52a8\u4fdd\u5b58\u7684\u65f6\u95f4\u70b9\n\u6570\u636e\u5907\u4efd\uff1a\n\u5907\u4efd\u6e38\u620f\u6570\u636e\u6587\u4ef6\n\u6e05\u9664\u5bf9\u51b3\uff1a\n\u5220\u9664\u6b63\u5728\u8fdb\u884c\u7684\u6e38\u620f",
         "func": "\u7ba1\u7406\u5458\u6307\u4ee4",
         "trigger_condition": "\u65e0",
         "trigger_method": ""
     },
     {
         "brief_des": "\u83b7\u53d6\u91d1\u5e01",
-        "detail_des": "\u91d1\u5e01\u7b7e\u5230\uff1a\n\u73a9\u5bb6\u6bcf\u65e5\u53ef\u7b7e\u5230\u4e00\u6b21\uff0c\u6bcf\u65e50\u70b9\u5237\u65b0\u3002\n\u91cd\u7f6e\u7b7e\u5230\uff1a\n\u6bcf\u6b21\u91cd\u7f6e\u540e\u53ef\u9886\u53d6\u4e00\u6b21\u3002",
+        "detail_des": "\u91d1\u5e01\u7b7e\u5230\uff1a\n\u73a9\u5bb6\u6bcf\u65e5\u53ef\u7b7e\u5230\u4e00\u6b21\uff0c\u6bcf\u65e50\u70b9\u5237\u65b0\u3002\n\u91cd\u7f6e\u7b7e\u5230\uff1a\n\u6bcf\u6b21\u91cd\u7f6e\u540e\u53ef\u9886\u53d6\u4e00\u6b21\uff0c\u6bcf\u65e5\u5237\u65b0\u6709\u51e0\u7387\u5237\u65b0\u91cd\u7f6e\u7b7e\u5230\u3002",
         "func": "\u83b7\u53d6\u91d1\u5e01",
         "trigger_condition": "\u65e0",
         "trigger_method": "1.\u91d1\u5e01\u7b7e\u5230 2.\u91cd\u7f6e\u7b7e\u5230"
     },
     {
         "brief_des": "\u6e05\u7a7a\u524d\u5341\u540d\u7684\u91d1\u5e01\u3002",
         "detail_des": "\u5f53\u91d1\u5e01\u6392\u884c\u699c\u7b2c\u4e00\u540d\u7684\u91d1\u5e01\u8d85\u8fc7\u7b2c\u4e8c\u540d\u5230\u7b2c\u5341\u540d\u7684\u603b\u548c\uff0c\u53ef\u4ee5\u53d1\u8d77\u91cd\u7f6e\u3002",
         "func": "\u53d1\u8d77\u91cd\u7f6e",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u53d1\u8d77\u91cd\u7f6e"
     },
     {
         "brief_des": "\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\u8d44\u6599",
-        "detail_des": "\u6211\u7684\u91d1\u5e01\uff1a\n\u67e5\u770b\u81ea\u5df1\u7684\u91d1\u5e01\u6570\u91cf\n\u6211\u7684\u4ed3\u5e93\uff1a\n\u67e5\u770b\u81ea\u5df1\u83b7\u5f97\u7684\u7684\u9053\u5177\n\u6211\u7684\u8d44\u6599\u5361\uff1a\n\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\u8be6\u7ec6\u8d44\u6599\n\u6211\u7684\u8d44\u4ea7\uff1a\n\u67e5\u770b\u81ea\u5df1\u7684\u5168\u5c40\u8d44\u4ea7\u5206\u5e03",
+        "detail_des": "\u6211\u7684\u91d1\u5e01\uff1a\n\u67e5\u770b\u81ea\u5df1\u7684\u91d1\u5e01\u6570\u91cf\n\u6211\u7684\u4ed3\u5e93\uff1a\n\u67e5\u770b\u81ea\u5df1\u83b7\u5f97\u7684\u7684\u9053\u5177\n\u6211\u7684\u8d44\u6599\u5361\uff1a\n\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\u8be6\u7ec6\u8d44\u6599\n\u70bc\u91d1\u8d44\u6599\u5361\uff1a\n\u67e5\u770b\u4e2a\u4eba\u70bc\u91d1\u8d44\u6599",
         "func": "\u4e2a\u4eba\u8d26\u6237",
         "trigger_condition": "\u65e0",
-        "trigger_method": "1.\u6211\u7684\u91d1\u5e01 2.\u6211\u7684\u4ed3\u5e93 3.\u6211\u7684\u8d44\u6599\u5361"
+        "trigger_method": "1.\u6211\u7684\u91d1\u5e01 2.\u6211\u7684\u4ed3\u5e93 3.\u6211\u7684\u8d44\u6599\u5361 4.\u70bc\u91d1\u8d44\u6599\u5361"
+    },
+    {
+        "brief_des": "\u67e5\u770b\u7fa4\u8d44\u6599\u5361",
+        "detail_des": "",
+        "func": "\u7fa4\u8d44\u6599\u5361",
+        "trigger_condition": "\u65e0",
+        "trigger_method": "\u7fa4\u8d44\u6599\u5361"
     },
     {
         "brief_des": "\u8bbe\u7f6e\u6211\u7684\u8d44\u6599\u5361\u663e\u793a\u7684\u80cc\u666f\u56fe\u7247",
         "detail_des": "",
         "func": "\u8bbe\u7f6e\u80cc\u666f\u56fe\u7247",
         "trigger_condition": "\u9700\u8981\u6709\u7279\u5b9a\u9053\u5177",
-        "trigger_method": "\u8bbe\u7f6e\u80cc\u666f\u56fe\u7247[\u56fe\u7247] \u8bbe\u7f6e\u80cc\u666f\u56fe\u7247(\u56de\u590d\u4e00\u5f20\u56fe\u7247\uff0c\u5220\u6389at)"
+        "trigger_method": "\u8bbe\u7f6e\u80cc\u666f\u56fe\u7247[\u56fe\u7247] \u8bbe\u7f6e\u80cc\u666f\u56fe\u7247(\u56de\u590d\u4e00\u5f20\u56fe\u7247)"
     },
     {
         "brief_des": "\u5c06\u8d44\u6599\u5361\u663e\u793a\u7684\u80cc\u666f\u56fe\u7247\u8bbe\u7f6e\u4e3a\u9ed8\u8ba4",
         "detail_des": "",
         "func": "\u5220\u9664\u80cc\u666f\u56fe\u7247",
         "trigger_condition": "",
         "trigger_method": ""
@@ -60,188 +67,202 @@
         "detail_des": "\u8f6c\u79fb\u76ee\u6807\u5df2\u6ce8\u518c\u516c\u53f8\uff0c\u4f60\u5728\u76ee\u6807\u7fa4\u5185\u6709\u8d26\u6237\u3002",
         "func": "\u91d1\u5e01\u8f6c\u79fb",
         "trigger_condition": "\u8f6c\u79fb\u76ee\u6807\u5df2\u6ce8\u518c\u516c\u53f8\u3002",
         "trigger_method": "\u91d1\u5e01\u8f6c\u79fb \u3010\u516c\u53f8\u540d\u3011 \u3010\u91d1\u989d\u3011"
     },
     {
         "brief_des": "\u83b7\u53d6\u9053\u5177\n\u53ef\u6307\u5b9a\u62bd\u5361\u6b21\u6570\n\u4f8b\u5982\uff1a @bot 30\u8fde",
-        "detail_des": "\u9053\u5177\u5206\u4e3a\u5168\u5c40\u9053\u5177\u548c\u7fa4\u5185\u9053\u5177\n\u4e5f\u53ef\u5206\u4e3a\u6c38\u4e45\u9053\u5177\u548c\u65f6\u6548\u9053\u5177\n\u65f6\u6548\u9053\u5177\u6700\u957f\u53e0\u52a07\u5929\n\u6c38\u4e45\u9053\u5177\u6700\u591a\u53e010\u4e2a\n\u90e8\u5206\u9053\u5177\u53ef\u4f7f\u7528\uff1a\n\u4f7f\u7528\u65b9\u6cd5\uff1a\u4f7f\u7528\u9053\u5177 \u3010\u9053\u5177\u540d\u3011 \u3010\u6570\u91cf/\u53c2\u6570\u3011",
+        "detail_des": "\u9053\u5177\u5206\u4e3a\u5168\u5c40\u9053\u5177\u548c\u7fa4\u5185\u9053\u5177\n\u7fa4\u5185\u9053\u5177\u6700\u591a\u53e0 30 \u5929/\u4e2a\n\u90e8\u5206\u9053\u5177\u53ef\u4f7f\u7528\u3002",
         "func": "\u62bd\u5361",
         "trigger_condition": "\u9700\u8981@bot\u6216\u53ebbot\u7684\u540d\u5b57\u3002",
         "trigger_method": "\u5355\u62bd/10\u8fde"
     },
     {
         "brief_des": "\u90e8\u5206\u9053\u5177\u65e0\u6cd5\u4f7f\u7528",
         "detail_des": "",
         "func": "\u4f7f\u7528\u9053\u5177",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u4f7f\u7528\u9053\u5177 \u3010\u9053\u5177\u540d\u3011 \u3010\u6570\u91cf/\u53c2\u6570\u3011"
     },
     {
         "brief_des": "\u67e5\u770b\u6392\u884c\u699c",
-        "detail_des": "\u91d1\u5e01\u6392\u884c\n\u80dc\u573a\u6392\u884c\n\u8d25\u573a\u6392\u884c\n\u6b27\u6d32\u4eba\u6392\u884c\n\u6148\u5584\u5bb6\u6392\u884c\n\u67e5\u770b\u8def\u706f\u6302\u4ef6",
+        "detail_des": "\u603b\u91d1\u5e01\u6392\u884c\n\u603b\u8d44\u4ea7\u6392\u884c\n\u91d1\u5e01\u6392\u884c\n\u8d44\u4ea7\u6392\u884c\n\u80dc\u7387\u6392\u884c\n\u80dc\u573a\u6392\u884c\n\u8d25\u573a\u6392\u884c\n\u8def\u706f\u6302\u4ef6\u6392\u884c",
         "func": "\u6392\u884c\u699c",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u91d1\u5e01\u6392\u884c"
     },
     {
-        "brief_des": "\u79c1\u804a\u6307\u4ee4\u5173\u8054\u5230\u7fa4\u3002",
-        "detail_des": "\u4f60\u53ef\u4ee5\u5728\u79c1\u804a\u5b8c\u6210\u4ee5\u4e0b\u64cd\u4f5c\uff1a\n\u7b7e\u5230\n\u62bd\u5361\n\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\uff1a\n\u67e5\u770b\u6392\u884c\n\u8d2d\u4e70\u6216\u7ed3\u7b97\u80a1\u7968",
-        "func": "\u8fde\u63a5\u8d26\u6237",
+        "brief_des": "\u67e5\u770b\u6392\u884c\u699c",
+        "detail_des": "\u91d1\u5e01\u603b\u6392\u884c\n\u8d44\u4ea7\u603b\u6392\u884c\n\u80dc\u7387\u603b\u6392\u884c\n\u80dc\u573a\u603b\u6392\u884c\n\u8d25\u573a\u603b\u6392\u884c\n\u8def\u706f\u6302\u4ef6\u603b\u6392\u884c",
+        "func": "\u603b\u6392\u884c\u699c",
         "trigger_condition": "\u65e0",
-        "trigger_method": "1.\u7fa4\u5185\uff1a@bot\u5173\u8054\u8d26\u6237 2.\u79c1\u804a\uff1a\u5173\u8054\u8d26\u6237\n"
+        "trigger_method": "\u91d1\u5e01\u603b\u6392\u884c"
     },
     {
         "brief_des": "",
         "detail_des": "",
         "func": "\u5bf9\u5c40\u5904\u7406",
         "trigger_condition": "\u8d85\u65f6\u7ed3\u7b97\u9700\u8981\u5bf9\u5c40\u5b58\u5728\u8d85\u8fc760s",
-        "trigger_method": "\u63a5\u53d7\u6311\u6218 \u62d2\u7edd\u6311\u6218 \u8ba4\u8f93 \u8d85\u65f6\u7ed3\u7b97"
+        "trigger_method": "\u63a5\u53d7\u6311\u6218 \u62d2\u7edd\u6311\u6218 \u8ba4\u8f93 \u8d85\u65f6\u7ed3\u7b97 \u6e38\u620f\u91cd\u7f6e"
     },
     {
         "brief_des": "\u53d1\u8d77\u968f\u673a\u5bf9\u6218",
         "detail_des": "\u968f\u673a\u6e38\u620f\uff0c\u5982\u4e0d\u6307\u5b9a\u91d1\u989d\u5c31\u662f\u968f\u673a\u91d1\u989d",
         "func": "\u968f\u673a\u5bf9\u6218",
         "trigger_condition": "\u9700\u8981\u7279\u5b9a\u9053\u5177",
         "trigger_method": "\u968f\u673a\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
-        "brief_des": "\u53d1\u8d77\u4fc4\u7f57\u65af\u8f6e\u76d8",
-        "detail_des": "\u901a\u8fc7 \u88c5\u5f39 \u6765\u5bf9\u5176\u4ed6\u4eba\u53d1\u8d77\u51b3\u6597\n\u4e0d@\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\n\u8f6e\u6d41\u5f00\u67aa\uff0c\u76f4\u5230\u8fd0\u6c14\u4e0d\u597d\u7684\u4eba\u5148\u53bb\u4e16\u3002\n\u3010\u7279\u6b8a\u6280\u80fd\u3011\uff1a\u5f00\u67aa0\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u88c5\u5f39 \u3010\u5b50\u5f39\u6570\u3011 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u5f00\u67aa/\u5494/\u562d/\u5623 [\u5b50\u5f39\u6570]\uff08\u9ed8\u8ba41)\uff08\u8f6e\u6d41\u5f00\u67aa\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97 \uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u672a\u5f00\u67aa\uff0c\u53ef\u4f7f\u7528\u8be5\u547d\u4ee4\u7ed3\u675f\u5bf9\u51b3\u5e76\u80dc\u5229\uff09",
+        "brief_des": "\u5f00\u67aa/\u5494/\u562d/\u5623 [\u5b50\u5f39\u6570]\uff08\u9ed8\u8ba41)\uff08\u8f6e\u6d41\u5f00\u67aa\uff09",
+        "detail_des": "\u8f6e\u6d41\u5f00\u67aa\uff0c\u76f4\u5230\u8fd0\u6c14\u4e0d\u597d\u7684\u4eba\u5148\u53bb\u4e16\u3002",
         "func": "\u4fc4\u7f57\u65af\u8f6e\u76d8",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a1\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u88c5\u5f39 \u3010\u5b50\u5f39\u6570\u3011 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
-        "brief_des": "\u53d1\u8d77\u63b7\u9ab0\u5b50",
-        "detail_des": "\u901a\u8fc7 \u63b7\u9ab0\u5b50 \u6765\u5bf9\u5176\u4ed6\u4eba\u53d1\u8d77\u51b3\u6597\n\u8f6e\u6d41\u5f00\u6570\u6bd4\u5927\u5c0f\n\u4e2d\u9014\u53ef\u7ed3\u675f\n\u8f6e\u6d41\u5f00\u6570\uff0c\u5148\u6bd4\u7ec4\u5408\uff0c\u518d\u6bd4\u70b9\u6570\u3002\n\u7ec4\u5408\uff1a\n\u5f79\u6ee1 > \u4e32 > \u6761 > \u4e24\u5bf9 > \u5bf9 > \u6563\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u6447\u9ab0\u5b50/\u63b7\u8272\u5b50 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u5f00\u6570/\u5f00\u70b9/\u53d6\u51fa\uff08\u8f6e\u6d41\u5f00\u6570\uff09\n\u3010\u7ed3\u675f\u3011\n\u7ed3\u675f\uff08\u53ea\u6709\u6682\u8d25\u65b9\u53ef\u53d1\u8d77\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97\uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u6ca1\u6709\u56de\u5e94\uff0c\u4ee5\u76ee\u524d\u6bd4\u5206\u7ed3\u7b97\uff09",
+        "brief_des": "\u5f00\u6570",
+        "detail_des": "\u8f6e\u6d41\u5f00\u6570\u6bd4\u5927\u5c0f\uff0c\u6bcf\u6b21\u5f00\u6570\u90fd\u4f1a\u8ba9\u7ed3\u7b97\u91d1\u989d\u4e0a\u6da8\uff0c\u4e2d\u9014\u7ed3\u675f\u6309\u7167\u5f53\u524d\u91d1\u989d\u7ed3\u7b97\u3002\n\u7ec4\u5408\uff1a\n\u5f79\u6ee1 > \u4e32 > \u6761 > \u4e24\u5bf9 > \u5bf9 > \u6563",
         "func": "\u63b7\u9ab0\u5b50",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u5341\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a1\u500d\u8d4c\u6ce8\u4e0a\u9650\u6bcf\u8f6e",
         "trigger_method": "\u6447\u9ab0\u5b50/\u63b7\u8272\u5b50 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
-        "brief_des": "\u53d1\u8d77\u6251\u514b\u5bf9\u6218",
-        "detail_des": "\u901a\u8fc7 \u6251\u514b\u5bf9\u6218 \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\n\u6253\u51fa\u81ea\u5df1\u7684\u624b\u724c\n\u5f53\u5bf9\u65b9\u7684\u8840\u91cf\u5c0f\u4e8e1\u6216\u8005\u5728\u81ea\u5df1\u56de\u5408\u51fa\u724c\u524d\u8840\u91cf>40\u5373\u53ef\u83b7\u80dc\n\u724c\u5e93\u4e00\u517152\u5f20\u724c\uff0c\u5f53\u724c\u5e93\u6ca1\u6709\u724c\u4e86\u5c31\u4ee5\u76ee\u524d\u8840\u91cf\u7ed3\u7b97\uff0c\u7ed3\u675f\u6e38\u620f\u3002\n\n\u5148\u624b\u521d\u59cb\u70b9\u6570\uff1aHP 20 SP 0 DEF 0\n\u540e\u624b\u521d\u59cb\u70b9\u6570\uff1aHP 25 SP 2 DEF 0\n\u6bcf\u56de\u5408\u62bd\u4e09\u5f20\u724c\uff0c\u6253\u51fa\u5176\u4e2d\u7684\u4e00\u5f20\u4f5c\u4e3a\u884c\u52a8\u724c\uff0c\u5f03\u6389\u5269\u4f59\u624b\u724c\u3002\n\uff08\u7279\u522b\u6ce8\u610f\uff1a\u9632\u5fa1\u724c\u4f5c\u4e3a\u884c\u52a8\u724c\u662f\u653b\u51fb\uff09\n\u4e4b\u540e\u5bf9\u65b9\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\uff0c\n\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u5bf9\u65b9SP\u5219\u4ece\u724c\u5e93\u7ffb\u51fa\u4e00\u5f20\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\u3002\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u5bf9\u65b9SP\u70b9\u3002\n\n<ft size=30 color=black>\u9ed1\u6843</ft>\n\u63cf\u8ff0\uff1a\u9632\u5fa1\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u6253\u51fa\u653b\u51fb\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u589e\u52a0DEF\n<ft size=30 color=red>\u7ea2\u6843</ft>\n\u63cf\u8ff0\uff1a\u751f\u547d\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u6062\u590dHP\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u6062\u590dHP\n<ft size=30 color=black>\u6885\u82b1</ft>\n\u63cf\u8ff0\uff1a\u6280\u80fd\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u4e3b\u52a8\u6280\u80fd\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u589e\u52a0SP\n<ft size=30 color=red>\u65b9\u7247</ft>\n\u63cf\u8ff0\uff1a\u653b\u51fb\u884c\u52a8\u724c\u6548\u679c\uff1a\u6253\u51fa\u653b\u51fb\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u6253\u51fa\u53cd\u51fb\n\n\u4e3b\u52a8\u6280\u80fd\uff1a\n\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\n\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u81ea\u8eabSP\u5219\u628a\u5269\u4f59\u4e24\u5f20\u624b\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u5168\u90e8\u6253\u51fa\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9ACE\u6280\u80fd\uff1a\n\u6447\u4e00\u4e2a6\u9762\u9ab0\u5b50\n\u628a\u6253\u51fa\u7684ACE\u724c\u70b9\u66ff\u6362\u6210\u6447\u51fa\u7684\u70b9\u6570\n\u518d\u628a\u4e09\u5f20\u624b\u724c\u5168\u90e8\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u6251\u514b\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u51fa\u724c 1/2/3\uff08\u8f6e\u6d41\u51fa\u724c\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97\uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u6ca1\u6709\u56de\u5e94\uff0c\u4ee5\u76ee\u524d\u8840\u91cf\u7ed3\u7b97\uff09",
+        "brief_des": "\u51fa\u724c 1/2/3",
+        "detail_des": "\u5f53\u5bf9\u65b9\u7684\u8840\u91cf\u5c0f\u4e8e1\u6216\u8005\u5728\u81ea\u5df1\u56de\u5408\u51fa\u724c\u524d\u8840\u91cf>40\u5373\u53ef\u83b7\u80dc\u3002\n\u6bcf\u56de\u5408\u62bd\u4e09\u5f20\u724c\uff0c\u6253\u51fa\u5176\u4e2d\u7684\u4e00\u5f20\u4f5c\u4e3a\u884c\u52a8\u724c\uff0c\u5f03\u6389\u5269\u4f59\u624b\u724c\u3002\n\u7279\u522b\u6ce8\u610f\uff1a\u9632\u5fa1\u724c\u4f5c\u4e3a\u884c\u52a8\u724c\u662f\u653b\u51fb\n\u4e4b\u540e\u5bf9\u65b9\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\uff0c\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u5bf9\u65b9SP\u5219\u4ece\u724c\u5e93\u7ffb\u51fa\u4e00\u5f20\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\uff0c\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u5bf9\u65b9SP\u70b9\u3002\n\u4e3b\u52a8\u6280\u80fd\uff1a\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\uff0c\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u81ea\u8eabSP\u5219\u628a\u5269\u4f59\u4e24\u5f20\u624b\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u5168\u90e8\u6253\u51fa\uff0c\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9\nACE\u6280\u80fd\uff1a\u6447\u4e00\u4e2a6\u9762\u9ab0\u5b50\uff0c\u628a\u6253\u51fa\u7684ACE\u724c\u70b9\u66ff\u6362\u6210\u6447\u51fa\u7684\u70b9\u6570\uff0c\u518d\u628a\u4e09\u5f20\u624b\u724c\u5168\u90e8\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\uff0c\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9",
         "func": "\u6251\u514b\u5bf9\u6218",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a5\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u6251\u514b\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
-        "brief_des": "\u53d1\u8d77\u731c\u6570\u5b57",
-        "detail_des": "\u901a\u8fc7 \u731c\u6570\u5b57 \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\uff0c\u8f6e\u6d41\u731c\u6570\u5b57\uff0c\u731c\u4e2d\u6570\u5b57\u5373\u53ef\u83b7\u80dc\u3002\u6bcf\u8f6e\u8d4c\u6ce8\u90fd\u4f1a\u589e\u957f\u4e00\u500d",
+        "brief_des": "\uff081-100\u7684\u6570\u5b57\uff09",
+        "detail_des": "\u8f6e\u6d41\u731c\u6570\u5b57\uff0c\u731c\u4e2d\u6570\u5b57\u5373\u53ef\u83b7\u80dc\u3002",
         "func": "\u731c\u6570\u5b57",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e\u5341\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e1\u500d\u8d4c\u6ce8\u4e0a\u9650\u6bcf\u8f6e",
         "trigger_method": "\u731c\u6570\u5b57 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
-        "brief_des": "\u53d1\u8d77\u540c\u82b1\u987a",
-        "detail_des": "\u901a\u8fc7 \u540c\u82b1\u987a \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\uff0c\u5148\u624b\u770b\u724c\u52a0\u6ce8\uff0c\u540e\u624b\u770b\u724c\u8ddf\u6ce8\uff0c\u76f4\u5230\u4e00\u65b9\u8ba4\u8f93\u6216\u70b9\u6570\u5927\u7684\u83b7\u80dc\u3002",
+        "brief_des": "\u770b\u724c/\u52a0\u6ce8 \u3010\u91d1\u989d\u3011",
+        "detail_des": "\u5728\u52a0\u6ce8\u524d\u53ef\u4ee5\u67e5\u770b\u624b\u724c\u786e\u8ba4\u81ea\u5df1\u662f\u5426\u8981\u52a0\u6ce8\u3002\n\u624b\u724c\u4ee5\u79c1\u804a\u5f62\u5f0f\u53d1\u9001\uff0c\u770b\u724c\u7684\u73a9\u5bb6\u9700\u8981\u6dfb\u52a0bot\u597d\u53cb\n\u5148\u624b\u51b3\u5b9a\u672c\u8f6e\u52a0\u6ce8\u6700\u5c0f\u91d1\u989d\uff0c\u540e\u624b\u51b3\u5b9a\u672c\u8f6e\u91d1\u989d\uff0c\u52a0\u6ce8\u9ed8\u8ba4\u4e3a\u521d\u59cb\u91d1\u989d\u3002",
         "func": "\u540c\u82b1\u987a",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e\u4e94\u500d\u8d4c\u6ce8\u4e0a\u9650",
-        "trigger_method": "\u540c\u82b1\u987a \u3010\u91d1\u989d\u3011 \u3010at\u3011"
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u5355\u6b21\u52a0\u6ce810\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_method": "\u540c\u82b1\u987a \u3010\u91d1\u989d\u3011 \u3010\u7b49\u7ea7\u3011 \u3010at\u3011"
+    },
+    {
+        "brief_des": "\u62bd\u724c/\u505c\u724c/\u53cc\u500d\u4e0b\u6ce8",
+        "detail_des": "\u5bf9\u6218\u53cc\u65b9\u9700\u8981\u6dfb\u52a0bot\u597d\u53cb\u3002",
+        "func": "21\u70b9",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u5355\u6b215\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_method": "21\u70b9 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
+    },
+    {
+        "brief_des": "A/B/1/2/3 \uff08\u79c1\u804a\uff09",
+        "detail_des": "\u53cc\u65b9\u624b\u724c\u5747\u4e3aAB123\u4e94\u5f20\u724c\uff0c\u6bcf\u8f6e\u6697\u724c\u53d1\u724c\uff08\u79c1\u804abot\uff09\uff0c\u6bcf\u8f6e\u7ed3\u675f\u540e\u5f00\u724c\u3002\n\u53cc\u65b9\u51fa\u724c\u76f8\u540c\u4e3a\u5e73\u5c40\n\u6b64\u5916\nA\u4e3a\u5fc5\u80dc\u724c\uff0cB\u4e3a\u5fc5\u8d25\u724c\u3002\n1\u80dc2\uff0c2\u80dc3\uff0c3\u80dc1\n\u672c\u8f6e\u80dc\u5229\u8005+1\u5206\n\u6253\u51fa\u6240\u6709\u624b\u724c\u540e\u7ed3\u7b97\u3002\u5206\u6570\u591a\u7684\u80dc\u5229\n\u6bcf\u8f6e\u8d4c\u6ce8\u7ffb\u500d\n\u73a9\u6cd5\u6807\u6ce8\uff1a\u56e0\u4e3aB\u5fc5\u8d25\u6240\u4ee5\u5728\u5bf9\u65b9\u51faA\u7684\u65f6\u5019\u6df7\u51fa\u53bb\u662f\u6700\u4f18\u89e3\u3002\u603b\u4e4b\u4f60\u9700\u8981\u6253\u51faAB123\u5168\u90e8\u7684\u724c\u3002",
+        "func": "AB\u724c",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e1\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_method": "AB\u724c \u3010\u91d1\u989d\u3011 \u3010at\u3011"
+    },
+    {
+        "brief_des": "\u88c5\u5f39/\u5f00\u67aa/\u95ea\u907f/\u95ea\u67aa/\u9884\u5224\u5f00\u67aa \uff08\u79c1\u804a\uff09",
+        "detail_des": "\u53cc\u65b9\u79c1\u804abot\u672c\u8f6e\u7684\u884c\u52a8\n\u53cc\u65b9\u521d\u59cb1\u53d1\u5b50\u5f39\uff0c\u88c5\u5f39\u4e0a\u9650\u4e3a6\u53d1\u5b50\u5f39\uff086\u53d1\u53ef\u4ee5\u7ee7\u7eed\u88c5\u5f39\uff0c\u4f46\u662f\u5b50\u5f39\u6570\u4e0d\u4f1a\u518d\u589e\u52a0\u4e86\uff09\u3002\n\u5982\u679c\u53cc\u65b9\u540c\u65f6 \u5f00\u67aa\uff0c\u90a3\u4e48\u5b50\u5f39\u4f1a\u53d1\u751f\u78b0\u649e\u3002\u672c\u8f6e\u5e73\u5c40\n\u88c5\u5f39\n\u5728 \u521d\u59cb\u4f4d\u7f6e \u884c\u52a8\uff0c\u5269\u4f59\u5b50\u5f39\u6570+1\u3002\u4f1a\u88ab \u5f00\u67aa \u95ea\u67aa \u51fb\u6740\n\u95ea\u907f\n\u53bb \u95ea\u907f\u4f4d\u7f6e \uff0c\u4e0d\u4f1a\u6d88\u8017\u5b50\u5f39\u3002\u4f1a\u88ab \u9884\u5224\u5f00\u67aa \u51fb\u6740\n\u5f00\u67aa\n\u5728 \u521d\u59cb\u4f4d\u7f6e \u884c\u52a8\uff0c\u6253\u5bf9\u65b9 \u521d\u59cb\u4f4d\u7f6e \uff0c\u5269\u4f59\u5b50\u5f39\u6570-1 \u51fb\u6740 \u88c5\u5f39 \u9884\u5224\u5f00\u67aa\n\u95ea\u67aa\n\u53bb \u95ea\u907f\u4f4d\u7f6e \uff0c\u6253\u5bf9\u65b9 \u521d\u59cb\u4f4d\u7f6e \uff0c\u5269\u4f59\u5b50\u5f39\u6570-1 \u51fb\u6740 \u88c5\u5f39 \u5f00\u67aa\n\u9884\u5224\u5f00\u67aa\n\u5728 \u521d\u59cb\u4f4d\u7f6e \u884c\u52a8\uff0c\u6253\u5bf9\u65b9 \u95ea\u907f\u4f4d\u7f6e \uff0c\u5269\u4f59\u5b50\u5f39\u6570-1 \u51fb\u6740 \u95ea\u907f \u95ea\u67aa",
+        "func": "\u897f\u90e8\u5bf9\u6218",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a5\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_method": "\u897f\u90e8\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
         "brief_des": "\u521b\u5efa\u8d5b\u9a6c\u5c0f\u6e38\u620f",
-        "detail_des": "\u6d41\u7a0b\uff1a\n\u8d5b\u9a6c\u521b\u5efa\uff1a\u7b2c\u4e00\u4f4d\u73a9\u5bb6\u53d1\u8d77\u6d3b\u52a8 \u2192\n\u8d5b\u9a6c\u52a0\u5165 \u3010\u4f60\u7684\u9a6c\u513f\u540d\u79f0\u3011\uff1a\u73a9\u5bb6\u53c2\u8d5b \u2192\n\u8d5b\u9a6c\u5f00\u59cb\uff1a\u6e38\u620f\u8fdb\u884c \u2192\n\u8fdb\u884c\u4e2d \u2192\n\u7ed3\u7b97\n\n\u5f53\u9047\u5230\u9519\u8bef\u6216\u5176\u4ed6\u60c5\u51b5\u53ef\u4f7f\u7528\u8d5b\u9a6c\u91cd\u7f6e\u6765\u91cd\u7f6e\u9a6c\u573a\u3002",
+        "detail_des": "\u6d41\u7a0b\uff1a\n\u8d5b\u9a6c\u521b\u5efa\uff1a\u7b2c\u4e00\u4f4d\u73a9\u5bb6\u53d1\u8d77\u6d3b\u52a8 \u2192\n\u8d5b\u9a6c\u52a0\u5165 \u3010\u4f60\u7684\u9a6c\u513f\u540d\u79f0\u3011\uff1a\u73a9\u5bb6\u53c2\u8d5b \u2192\n\u8d5b\u9a6c\u5f00\u59cb\uff1a\u6e38\u620f\u8fdb\u884c \u2192\n\u8fdb\u884c\u4e2d \u2192\n\u7ed3\u7b97\n\n\u5f53\u9047\u5230\u9519\u8bef\u53ef\u4f7f\u7528\u6e38\u620f\u91cd\u7f6e\u6765\u91cd\u7f6e\u6e38\u620f",
         "func": "\u8d5b\u9a6c\u5c0f\u6e38\u620f",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u8d5b\u9a6c\u521b\u5efa"
     },
     {
-        "brief_des": "\u67e5\u770b\u5e02\u573a\u4fe1\u606f",
-        "detail_des": "\u67e5\u770b\u5e02\u573a\u4e0a\u6240\u6709\u516c\u53f8\u7684\u5b98\u65b9\u7ed3\u7b97\u4ef7\u683c",
-        "func": "\u5e02\u573a\u4fe1\u606f",
-        "trigger_condition": "\u65e0",
-        "trigger_method": "\u5e02\u573a\u4fe1\u606f"
+        "brief_des": "\u67e5\u5c01at\u7684\u7fa4\u53cb\u7684\u5168\u90e8\u8d44\u4ea7\u3002",
+        "detail_des": "\u67e5\u5c01\u540e\u7684\u7528\u6237\u4f1a\u6301\u6709\u6700\u591a500\u4e2a\u5168\u5c40\u9053\u5177\u3010\u88ab\u51bb\u7ed3\u7684\u8d44\u4ea7\u3011\n\u6b64\u9053\u5177\u53ef\u4ee5\u5728\u4efb\u610f\u7fa4\u4f7f\u7528\n\u6bcf\u4e2a\u3010\u88ab\u51bb\u7ed3\u7684\u8d44\u4ea7\u3011\u4f7f\u7528\u540e\u4f1a\u5728\u4f7f\u7528\u7684\u7fa4\u83b7\u5f97\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650\u7684\u91d1\u5e01\u3002",
+        "func": "\u51bb\u7ed3\u8d44\u4ea7",
+        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u8d85\u7ba1",
+        "trigger_method": "\u51bb\u7ed3\u8d44\u4ea7@someone"
+    },
+    {
+        "brief_des": "@bot\u4e5f\u53ef\u4ee5\u6362\u6210\u53ebbot\u7684\u540d\u5b57",
+        "detail_des": "bot\u4e0d\u5728\u7684\u7fa4\uff0c\u9000\u7fa4\u7684\u7528\u6237\u7b49\u3010\u65e0\u6548\u8d26\u6237\u3011\u53ef\u4ee5\u4f7f\u7528 \u6e05\u7406\u65e0\u6548\u8d26\u6237 \u5220\u9664",
+        "func": "\u6e05\u7406\u65e0\u6548\u8d26\u6237",
+        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u8d85\u7ba1",
+        "trigger_method": "@bot\u6e05\u7406\u65e0\u6548\u8d26\u6237"
     },
     {
-        "brief_des": "\u67e5\u770b\u3010\u516c\u53f8\u540d\u79f0\u3011\u80a1\u4efd\u62a5\u4ef7",
+        "brief_des": "\u7fa4\u6307\u4ee4\u5173\u8054\u5230\u79c1\u804a\u3002",
         "detail_des": "",
-        "func": "\u73a9\u5bb6\u5e02\u573a\u4fe1\u606f",
+        "func": "\u8fde\u63a5\u8d26\u6237",
         "trigger_condition": "\u65e0",
-        "trigger_method": "\u5e02\u573a\u4fe1\u606f \u3010\u516c\u53f8\u540d\u79f0\u3011"
+        "trigger_method": "1.\u7fa4\u5185\uff1a@bot\u5173\u8054\u8d26\u6237 2.\u79c1\u804a\uff1a\u5173\u8054\u8d26\u6237\n"
     },
     {
-        "brief_des": "\u67e5\u770b\u5e02\u573a\u884c\u60c5",
-        "detail_des": "",
-        "func": "\u5e02\u573a\u884c\u60c5",
+        "brief_des": "\u67e5\u770b\u5e02\u573a\u4fe1\u606f",
+        "detail_des": "\u67e5\u770b\u5e02\u573a\u4e0a\u6240\u6709\u516c\u53f8\u7684\u5b98\u65b9\u7ed3\u7b97\u4ef7\u683c",
+        "func": "\u5e02\u573a\u4fe1\u606f",
         "trigger_condition": "\u65e0",
-        "trigger_method": "\u5e02\u573a\u884c\u60c5"
+        "trigger_method": "\u5e02\u573a\u4fe1\u606f"
     },
     {
-        "brief_des": "\u67e5\u770b\u516c\u53f8\u7684\u8be6\u7ec6\u4fe1\u606f",
+        "brief_des": "\u67e5\u770b\u3010\u516c\u53f8\u540d\u79f0\u3011\u7684\u7fa4\u8d44\u6599\u5361\u3002",
         "detail_des": "",
-        "func": "\u516c\u53f8\u4fe1\u606f",
+        "func": "\u6307\u5b9a\u516c\u53f8\u5e02\u573a\u4fe1\u606f",
         "trigger_condition": "\u65e0",
-        "trigger_method": "\u516c\u53f8\u4fe1\u606f \u3010\u516c\u53f8\u540d\u79f0\u3011"
+        "trigger_method": "\u5e02\u573a\u4fe1\u606f \u3010\u516c\u53f8\u540d\u79f0\u3011"
     },
     {
         "brief_des": "\u4ece\u5b98\u65b9\u8d2d\u4e70\u80a1\u7968",
         "detail_des": "\u4ee5\u53d1\u884c\u4ef7\u683c\u4ece \u3010\u516c\u53f8\u540d\u79f0\u3011\u8d2d\u4e70N\u80a1\u672c\u516c\u53f8\u80a1\u4efd\u3002",
         "func": "\u53d1\u884c\u8d2d\u4e70",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u53d1\u884c\u8d2d\u4e70 \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010N\u3011"
     },
     {
         "brief_des": "\u4ece\u5b98\u65b9\u7ed3\u7b97\u80a1\u7968",
         "detail_des": "\u4ee5\u7ed3\u7b97\u4ef7\u683c\u5411\u3010\u516c\u53f8\u540d\u79f0\u3011\u5356\u51faN\u80a1\u672c\u516c\u53f8\u80a1\u4efd\u3002",
-        "func": "\u5b98\u65b9\u7ed3\u7b97",
+        "func": "\u7ed3\u7b97",
         "trigger_condition": "\u65e0",
-        "trigger_method": "\u5b98\u65b9\u7ed3\u7b97 \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010N\u3011"
+        "trigger_method": "\u7ed3\u7b97 \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010N\u3011"
     },
     {
         "brief_des": "\u4ece\u73a9\u5bb6\u5e02\u573a\u8d2d\u4e70\u80a1\u7968",
         "detail_des": "\u4ee5\u4ece\u4f4e\u5230\u9ad8\u7684\u62a5\u4ef7\u4e70\u5165N\u80a1\u5e02\u573a\u4e2d\u7684\u3010\u516c\u53f8\u540d\u79f0\u3011\u3002",
-        "func": "\u8d2d\u4e70\u80a1\u7968",
+        "func": "\u5e02\u573a\u8d2d\u4e70",
         "trigger_condition": "\u65e0",
-        "trigger_method": "\u8d2d\u4e70 \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010N\u3011"
+        "trigger_method": "\u5e02\u573a\u8d2d\u4e70 \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010N\u3011"
     },
     {
         "brief_des": "\u4ece\u73a9\u5bb6\u5e02\u573a\u51fa\u552e\u80a1\u7968",
         "detail_des": "\u5c06\u81ea\u5df1\u624b\u4e2d\u7684\u3010\u516c\u53f8\u540d\u79f0\u3011 \u4ee5\u3010\u62a5\u4ef7\u3011\u53d1\u5e03\u5230\u5e02\u573aN\u80a1\u3002",
-        "func": "\u51fa\u552e\u80a1\u7968",
+        "func": "\u51fa\u552e",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u51fa\u552e \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010\u62a5\u4ef7\u3011 \u3010N\u3011"
     },
     {
         "brief_des": "\u6210\u7acb\u516c\u53f8",
-        "detail_des": "\u5c06\u672c\u7fa4\u4ee5\u3010\u516c\u53f8\u540d\u79f0\u3011\u6ce8\u518c\u5230\u5e02\u573a\uff0c\n\u5982\u679c\u5168\u7fa4\u91d1\u5e01\u6570\u5c0f\u4e8e\u4e24\u4e07\u5219\u4f1a\u6ce8\u518c\u5931\u8d25\u3002",
+        "detail_des": "\u5c06\u672c\u7fa4\u4ee5\u3010\u516c\u53f8\u540d\u79f0\u3011\u6ce8\u518c\u5230\u5e02\u573a\u3002",
         "func": "\u5e02\u573a\u6ce8\u518c",
-        "trigger_condition": "\u9700\u8981@bot\u6216\u53ebbot\u7684\u540d\u5b57\uff0c\u6307\u4ee4\u6743\u9650\uff1a\u7ba1\u7406\u5458\u3002",
-        "trigger_method": "\u5e02\u573a\u6ce8\u518c \u3010\u516c\u53f8\u540d\u79f0\u3011"
+        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u7ba1\u7406\u5458",
+        "trigger_method": "@bot\u5e02\u573a\u6ce8\u518c \u3010\u516c\u53f8\u540d\u79f0\u3011"
+    },
+    {
+        "brief_des": "\u516c\u53f8\u91cd\u547d\u540d",
+        "detail_des": "\u5c06\u672c\u7fa4\u516c\u53f8\u540d\u6539\u6210\u3010\u516c\u53f8\u540d\u79f0\u3011\u3002",
+        "func": "\u516c\u53f8\u91cd\u547d\u540d",
+        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u7ba1\u7406\u5458",
+        "trigger_method": "@bot\u516c\u53f8\u91cd\u547d\u540d \u3010\u516c\u53f8\u540d\u79f0\u3011"
     },
     {
         "brief_des": "\u66f4\u65b0\u516c\u53f8\u7b80\u4ecb",
         "detail_des": "\u5c06\u3010\u7b80\u4ecb\u5185\u5bb9\u3011\u6dfb\u52a0\u5230\u672c\u7fa4\u516c\u53f8\u8d44\u6599\u7684\u7b80\u4ecb\u4e2d",
         "func": "\u66f4\u65b0\u516c\u53f8\u7b80\u4ecb",
         "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u7ba1\u7406\u5458",
         "trigger_method": "\u66f4\u65b0\u516c\u53f8\u7b80\u4ecb \u3010\u7b80\u4ecb\u5185\u5bb9\u3011"
     },
     {
         "brief_des": "\u66f4\u65b0\u516c\u53f8\u7b80\u4ecb",
         "detail_des": "\u5c06\u3010\u7b80\u4ecb\u5185\u5bb9\u3011\u6dfb\u52a0\u5230\u3010\u516c\u53f8\u540d\u79f0\u3011\u8d44\u6599\u7684\u7b80\u4ecb\u4e2d\u3002",
         "func": "\u7ba1\u7406\u5458\u66f4\u65b0\u516c\u53f8\u7b80\u4ecb",
         "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u8d85\u7ba1",
         "trigger_method": "\u7ba1\u7406\u5458\u66f4\u65b0\u516c\u53f8\u7b80\u4ecb \u3010\u516c\u53f8\u540d\u79f0\u3011 \u3010\u7b80\u4ecb\u5185\u5bb9\u3011"
-    },
-    {
-        "brief_des": "\u8c03\u67e5\u7528\u6237\u7684\u8d44\u4ea7\u5206\u5e03\u60c5\u51b5\u3002",
-        "detail_des": "\u5982\u679c\u672a\u6307\u5b9a\u7528\u6237\uff0c\u5219\u8c03\u67e5\u73a9\u5bb6\u603b\u8d44\u4ea7\u524d\u5341\u540d\u7684\u8d44\u4ea7\u5206\u5e03\u60c5\u51b5\u3002",
-        "func": "\u8d44\u4ea7\u8c03\u67e5",
-        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u7ba1\u7406\u5458",
-        "trigger_method": "1.\u8d44\u4ea7\u8c03\u67e5 2.\u8d44\u4ea7\u8c03\u67e5@someone\n"
-    },
-    {
-        "brief_des": "\u67e5\u5c01at\u7684\u7fa4\u53cb\u7684\u5168\u90e8\u8d44\u4ea7\u3002",
-        "detail_des": "\u67e5\u5c01\u540e\u7684\u7528\u6237\u4f1a\u6301\u6709\u6700\u591a500\u4e2a\u5168\u5c40\u9053\u5177\u3010\u88ab\u51bb\u7ed3\u7684\u8d44\u4ea7\u3011\uff0c\n\u6b64\u9053\u5177\u53ef\u4ee5\u5728\u4efb\u610f\u7fa4\u4f7f\u7528\uff0c\n\u6bcf\u4e2a\u3010\u88ab\u51bb\u7ed3\u7684\u8d44\u4ea7\u3011\u4f7f\u7528\u540e\u4f1a\u5728\u4f7f\u7528\u7684\u7fa4\u83b7\u5f97\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650\u7684\u91d1\u5e01\u3002",
-        "func": "\u51bb\u7ed3\u8d44\u4ea7",
-        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u8d85\u7ba1",
-        "trigger_method": "\u51bb\u7ed3\u8d44\u4ea7@someone"
-    },
-    {
-        "brief_des": "\u6e05\u7406\u65e0\u6548\u8d26\u6237",
-        "detail_des": "\u65e0\u6548\u8d26\u6237\u8303\u56f4\uff1a\nbot\u4e0d\u5728\u7684\u7fa4\n\u9000\u7fa4\u7684\u7528\u6237\n\u957f\u671f\u4e0d\u5192\u6ce1\u7684\u7fa4\u53cb\n\u8d44\u4ea7\u8fc7\u5c0f\u7684\u516c\u53f8",
-        "func": "\u6e05\u7406\u65e0\u6548\u8d26\u6237",
-        "trigger_condition": "\u6307\u4ee4\u6743\u9650\uff1a\u8d85\u7ba1",
-        "trigger_method": "\u6e05\u7406\u65e0\u6548\u8d26\u6237"
     }
 ]
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998%*

 * *Differences: {"'63102'": "{'intro': '重置自己的本群账户'}"}*

```diff
@@ -166,12 +166,12 @@
         "intro": "\u670950%\u7684\u6982\u7387\u91d1\u5e01\u7ffb\u500d\uff0c50%\u7684\u6982\u7387\u91d1\u5e01\u6e05\u96f6\u3002\u6ca1\u6709\u4e0a\u9650",
         "name": "\u8d85\u7ea7\u5e78\u8fd0\u786c\u5e01",
         "rare": 6
     },
     "63102": {
         "color": "#006633",
         "des": "\u4e8b\u4e86\u62c2\u8863\u53bb\uff0c\u6df1\u85cf\u8eab\u4e0e\u540d\u3002",
-        "intro": "\u6e05\u7a7a\u81ea\u5df1\u7684\u91d1\u5e01\uff0c\u80a1\u7968",
+        "intro": "\u91cd\u7f6e\u81ea\u5df1\u7684\u672c\u7fa4\u8d26\u6237",
         "name": "\u91cd\u5f00\u5238",
         "rare": 6
     }
 }
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import httpx
 import asyncio
 from io import BytesIO
 from PIL import Image
 
 async def download_avatar(user_id:int) -> bytes:
-    url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
+    url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
     if data := await download_url(url):
         return BytesIO(data)
-    url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
+    url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
     if data := await download_url(url):
         return BytesIO(data)
 
     output = BytesIO()
     Image.new("RGBA", (300, 300),color = "gray").save(output, format = "png")
     return output
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,80 @@
 from typing import Tuple,Dict,List
 from pathlib import Path
 from io import BytesIO
 from PIL import Image,ImageDraw,ImageFont
 from PIL.Image import Image as IMG
+from fontTools.ttLib import TTFont
+from collections import Counter
 
-import numpy as np
 import matplotlib.pyplot as plt
+import matplotlib.font_manager as fm
 import seaborn as sns
+import numpy as np
+
+import re
 
 from .avatar import download_avatar,download_groupavatar
 
 from ..data import UserDict, GroupAccount
 from ..data import resourcefile
 
-from ..config import BG_image,fontname
+from ..config import BG_image,fontname,fallback_fonts
 
 sns.set(font = fontname)
 
 default_BG = BG_image / "default.png"
 
 if not default_BG.exists():
     Image.new('RGB', (200, 200), (0, 51, 102)).save(default_BG)
 
 font_big = ImageFont.truetype(font = fontname, size = 60, encoding = "utf-8")
-
 font_normal = ImageFont.truetype(font = fontname, size = 40, encoding = "utf-8")
-
 font_small = ImageFont.truetype(font = fontname, size = 30, encoding = "utf-8")
 
-def text_to_png(
+cmap_default = TTFont(font_big.path, fontNumber = font_big.index).getBestCmap()
+
+global fallback_fonts_cmap
+fallback_fonts_cmap = {}
+default_fallback_path = fm.findfont(fm.FontProperties())
+for fallback in fallback_fonts:
+    fallback_path = fm.findfont(fm.FontProperties(family=fallback))
+    if  fallback_path != default_fallback_path:
+        fallback_fonts_cmap[fallback_path] = TTFont(fallback_path, fontNumber = 0).getBestCmap()
+else:
+    fallback_path = default_fallback_path
+    fallback_fonts_cmap[fallback_path] = TTFont(fallback_path, fontNumber = 0).getBestCmap()
+del default_fallback_path
+
+def linecard_to_png(
     text:str,
-    font_size = 50,
-    image_size:tuple = (0,0),
-    width_simple:str = None,
-    fontname = fontname,
+    font_size = 60,
+    width:int = None,
+    height:int = None,
     padding:tuple = (20,20),
     spacing:float = 1.2,
-    text_color = "black",
-    bg_color = "white"
+    bg_color = "white",
+    autowrap:bool = False,
+    endline = None
     ):
     '''
     文字转png
     '''
-    # 创建字体对象
-    if fontname:
-        font = ImageFont.truetype(fontname, font_size)
-    else:
-        font = ImageFont.load_default().font
-
-    # 计算文字所需图片的大小
-
-    text = text.replace("\r\n","\n")
-    lines = text.split('\n')
-    line_height = int(font_size * spacing)
-
-
-    image_width = image_size [0]
-    image_height = image_size [1]
-    if width_simple:
-        image_width = int(font.getlength(width_simple))
-    image_width = image_width if image_width else int(max(font.getlength(line) for line in lines))
-    image_height = image_height if image_height else line_height * len(lines)
-
-    # 添加边距
-    x = padding[0]
-    y = padding[1]
-    image_width = image_width + 2*x
-    image_height = image_height +2*y
-
-    # 创建空白图片
-    image = Image.new('RGB', (image_width, image_height), bg_color)
-    draw = ImageDraw.Draw(image)
-    # 在图片上绘制文本
-    for line in lines:
-        draw.text((x, y), line, font = font, fill = text_color)
-        y += line_height
-
     output = BytesIO()
-    image.save(output, format="png")
+    linecard(
+        text = text,
+        font_size = font_size,
+        width = width,
+        height = height,
+        padding = padding,
+        spacing = spacing,
+        bg_color = bg_color,
+        endline = endline).save(output, format = "png")
     return output
 
-import re
-
 class linecard_pattern:
     align = re.compile(r"\[left\]|\[right\]|\[center\]|\[pixel\]\[.*?\]")
     font = re.compile(r"\[font_big\]|\[font_normal\]|\[font_small\]|\[font\]\[.*?\]\[.*?\]")
     color = re.compile(r"\[color\]\[.*?\]")
     passport = re.compile(r"\[passport\]")
     nowrap = re.compile(r"\[nowrap\]")
     noautowrap = re.compile(r"\[noautowrap\]")
@@ -95,36 +84,35 @@
     if match:
         start = match.start()
         end = match.end()
         return string[:start] + string[end:],string[start:end]
     else:
         return None
 
-def line_warp(line:str,width:int,font):
-    text_x = 0
-    line_count = 1
+def line_wrap(line:str,width:int,font, start:int = 0):
+    text_x = start
     new_str = ""
     for char in line:
         text_x += font.getlength(char)
         if text_x > width:
             new_str += "\n" + char
             text_x = 0
-            line_count += 1 
         else:
             new_str += char
-    return new_str,line_count
+    return new_str
 
 def linecard(
     text:str,
+    font_size:int = None,
     width:int = None,
     height:int = None,
-    font_size:int = None,
     padding:tuple = (20,20),
     spacing:float = 1.2,
     bg_color:str = None,
+    autowrap:bool = False,
     endline = None,
     canvas = None
     ):
     '''
     指定宽度单行文字
         ----:横线
 
@@ -148,169 +136,182 @@
     lines = text.split('\n')
 
     if font_size:
         font_default = ImageFont.truetype(font = fontname, size = font_size, encoding = "utf-8")
     else:
         font_default = font_normal
 
-    paddingX = padding[0]
-    paddingY = padding[1]
+    cmap_default = TTFont(font_default.path, fontNumber = font_default.index).getBestCmap()
 
-    X = []
-    Y = [0,]
-    Text = []
-
-    line_length = []
-
-    text_y = 0
-    maxFontLine = 0 # 如果本行是通过[nowrap]不换行标记拼接的多个行，那么记录最大的字体宽度以在换行时使用最大的字体
+    padding_x = padding[0]
+    padding_y = padding[1]
 
     align = "left"
+
     font = font_default
+    cmap = cmap_default
     color = None
     passport = 0
-    autowrap = True
+    noautowrap = True
+    nowrap = False
 
+    x,max_x,y,charlist = (0.0,0.0,0.0,[])
     for line in lines:
         passport -= 1
-
         if res := remove_tag(line,linecard_pattern.align):
             line, align = res
             if align.startswith("[pixel]["):
                 align = align[8:-1]
+                x = 0
             else:
                 align = align[1:-1]
+        elif nowrap:
+            align = "nowrap"
         else:
             if passport == 1:
                 pass
             else:
                 align = "left"
 
         if res := remove_tag(line,linecard_pattern.font):
             line, font = res
             if font.startswith("[font]["):
                 font = font[7:-1]
                 inner_font_name,inner_font_size = font.split("][",1)
                 inner_font_size = int(inner_font_size)
                 inner_font_size = inner_font_size if inner_font_size else font_size
-                font = ImageFont.truetype(font = inner_font_name, size = inner_font_size, encoding = "utf-8")
+                try:
+                    font = ImageFont.truetype(font = inner_font_name, size = inner_font_size, encoding = "utf-8")
+                    cmap = TTFont(font.path, fontNumber = font.index).getBestCmap()
+                except OSError:
+                    font, cmap = font_default, cmap_default
             elif font == "[font_big]":
-                font = font_big
+                font, cmap = font_big, cmap_default
+            elif font == "[font_normal]":
+                font, cmap = font_normal, cmap_default
             elif font == "[font_small]":
-                font = font_small
+                font, cmap = font_small, cmap_default
             else:
-                font = font_normal
+                font, cmap = font_default, cmap_default
         else:
             if passport == 1:
                 pass
             else:
-                font = font_default
+                font, cmap = font_default, cmap_default
 
         if res := remove_tag(line,linecard_pattern.color):
             line, color = res
             color = color[8:-1]
         else:
             if passport == 1:
                 pass
             else:
                 color = None
 
         if res := remove_tag(line,linecard_pattern.noautowrap):
             line = res[0]
-            autowrap = False
+            noautowrap = True
         else:
             if passport == 1:
                 pass
             else:
-                autowrap = True
+                noautowrap = False
 
         if res := remove_tag(line,linecard_pattern.nowrap):
             line = res[0]
-            maxFontLine = max(maxFontLine,int(font.size * spacing))
+            nowrap = True
         else:
-            if autowrap and width and font.getlength(line) > width:
-                line,inner_line_count = line_warp(line,width - paddingX,font)
-                text_y += max(maxFontLine,inner_line_count * int(font.size * spacing))
-            else:
-                text_y += max(maxFontLine,int(font.size * spacing))
-            maxFontLine = 0
+            nowrap = False
 
         if res := remove_tag(line,linecard_pattern.passport):
             line = res[0]
             passport = 2
 
-        line_length.append(int(font.getlength(line) if align == "left" else 0))
-        Y.append(text_y)
-        Text.append([line, font, color, align])
-
-    for i in range(len(lines)):
-        if Y[i] == Y[i-1]:
-            X.append(line_length[i-1])
-            line_length[i] += line_length[i-1]
-        else:
-            X.append(0)
+        if autowrap and not noautowrap and width and font.getlength(line) > width:
+            line = line_wrap(line,width - padding_x,font,x)
 
-    width = width if width else (max(line_length) + paddingX*2)
-    height = height if height else (Y[-1] + paddingY*2)
+        if line == "----":
+            inner_tmp = font.size * spacing
+            charlist.append([line, None, y, inner_tmp, color, None])
+            y += inner_tmp
+        else:
+            linesegs = line.split('\n')
+            for seg in linesegs:
+                for char in seg:
+                    ordchar = ord(char)
+                    if ordchar in cmap:
+                        inner_font = font
+                    else:
+                        for fallback_font in fallback_fonts_cmap:
+                            if ordchar in fallback_fonts_cmap[fallback_font]:
+                                inner_font = ImageFont.truetype(font = fallback_font, size = font.size, encoding="utf-8")
+                                break
+                        else:
+                            char = "□"
+                            inner_font = font
+                    charlist.append([char, x, y, inner_font, color, align])
+                    x += inner_font.getlength(char)
+                max_x = max(max_x,x)
+                x,y = (x,y) if nowrap else (0, y + font.size * spacing)
 
+    width = width if width else int(max_x + padding_x*2)
+    height = height if height else int(y + padding_y*2)
     canvas = canvas if canvas else Image.new("RGBA", (width, height), bg_color)
     draw = ImageDraw.Draw(canvas)
 
-    for i in range(len(lines)):
-        line, font, color, align = Text[i]
-        text_y = Y[i] + paddingY
-        if line == "----":
-            tmp = text_y + font.size//2
+    for i, (char, x, y, font, color, align)in enumerate(charlist):
+        if char == "----":
             color = color if color else 'gray'
-            draw.line(((0, tmp), (width, tmp)), fill = color, width = 4)
+            inner_y = y + (font - 0.5)//2 + padding_y
+            draw.line(((0, inner_y), (width, inner_y)), fill = color, width = 4)
         else:
-            color = color if color else 'black'
-            if align == "right":
-                text_x = int(width - font.getlength(line) - paddingX)
-            elif align == "center":
-                text_x = (width - font.getlength(line) )//2
+            if align == "left":
+                start_x = padding_x
+            elif align == "nowrap":
+                pass
             elif align.isdigit():
-                text_x = int(align)
+                start_x = int(align)
             else:
-                text_x = X[i] + paddingX
-            draw.text((text_x, text_y),line, fill = color, font = font)
+                for inner_i,inner_y in enumerate(map(lambda x:(x[2]),charlist[i:])):
+                    if inner_y != y:
+                        inner_index = charlist[i + inner_i - 1]
+                        break
+                else:
+                    inner_index = charlist[-1]
+                inner_char = inner_index[0]
+                inner_font = inner_index[3]
+                inner_x = inner_index[1]
+                inner_x += inner_font.getlength(inner_char)
+                if align == "right":
+                    start_x = width - inner_x - padding_x
+                elif align == "center":
+                    start_x = (width - inner_x)//2
+                else:
+                    start_x = padding_x
+            color = color if color else 'black'
+            draw.text((start_x + x, y + padding_y), char, fill = color, font = font)
 
     if endline:
         draw.line(((0, height - 60), (width, height - 60)), fill = "gray", width = 4)
         text_x = int(width - font_small.getlength(endline) - 20)
         draw.text((text_x,height - 45),endline, fill = "gray", font = font_small)
 
     return canvas
 
-def linecard_to_png(msg):
-    output = BytesIO()
-    linecard(msg,width = 880,bg_color = "white",endline = "抽卡结果").save(output, format = "png")
-    return output
-
-def gacha_info0(report:IMG, info:List[IMG]):
+def line_splicing(info:list):
     """
     抽卡信息拼接
-        report:抽卡报告
-        info:信息图片列表
     """
-    x = 880
-    y = report.size[1] + 10
-    length = len(info)
-    if length%2 == 1:
-        info.append(None)
-        length += 1
-
-    canvas = Image.new("RGB", (880,(130*length)//2 + report.size[1]), '#99CCFF')
-    canvas.paste(report)
-    for i in range(0, length, 2):
-        l,r = info[i:i+2]
-        canvas.paste(l, (0, y))
-        if r:
-            canvas.paste(r, (442, y))
-        y += 130
+    if len(info) == 1:
+        return linecard_to_png(info[0])
+    l = linecard(info[0],bg_color = "white")
+    r = linecard(info[1],bg_color = "white") 
+    canvas = Image.new("RGB", (l.size[0]+r.size[0],l.size[1]),"white")
+    canvas.paste(l, (0, 0))
+    canvas.paste(r, (l.size[0], 0))
     output = BytesIO()
     canvas.save(output,'png')
     return output
     
 async def bar_chart(user_id:int, info:str, lenth:float):
     """
     带头像的条形图
@@ -323,27 +324,126 @@
     canvas.paste(avatar, (5, 0), circle_mask)
     draw = ImageDraw.Draw(canvas)
     draw.rectangle(((70,10), (860, 50)), fill = "#00000033")
     draw.rectangle(((70,10), (80 + int(lenth*780), 50)), fill = "#99CCFF")
     draw.text((80,10), info, fill = (0,0,0), font = font_normal)
     return canvas
 
+def integer_log(number, base):
+    result = 0
+    while number >= base:
+        number //= base
+        result += 1
+    return result
+
+async def alchemy_info(user:UserDict,nickname:str):
+    """
+    炼金账户
+    """
+    canvas = Image.new("RGBA", (880, 400))
+    avatar = Image.open(await download_avatar(user.user_id))
+    avatar = avatar.resize((160,160))
+    circle_mask = Image.new("RGBA", avatar.size, (255, 255, 255, 0))
+    ImageDraw.Draw(circle_mask).ellipse(((0,0),avatar.size), fill="black")
+    canvas.paste(avatar, (20, 20), circle_mask)
+    draw = ImageDraw.Draw(canvas)
+    draw.line(((20, 200), (480, 200)), fill = "gray", width = 4)
+
+    alchemy = Counter(user.alchemy)
+    # 创建变量标签
+    labels = ['蒸汽', '雷电', '岩浆', '尘埃', '沼泽', '寒冰']
+    # 创建变量值
+    values = [alchemy["5"], alchemy["9"], alchemy["8"], alchemy["0"], alchemy["6"], alchemy["7"]]
+    products = max(values)
+    # 计算角度
+    angles = np.linspace(0.5*np.pi,2.5*np.pi,6,endpoint = False).tolist()
+    angles = [(x if x < 2*np.pi else x-2*np.pi) for x in angles]
+    # 闭合雷达图
+    values.append(values[0])
+    angles.append(angles[0])
+    # 绘制雷达图
+    mainproduct = max(values)
+    mainproduct = max(mainproduct,1)
+    values = [x*4/mainproduct for x in values]
+    sns.set(font = "simsun")
+    plt.figure(figsize=(4, 4))
+    ax = plt.subplot(111, polar = True)
+    ax.plot(angles, values, linewidth=2, linestyle='solid')
+    ax.fill(angles, values, 'b', alpha=0.1)
+    ax.set_yticklabels([])
+    plt.xticks(angles[:-1], labels, fontsize = 12)
+    output = BytesIO()
+    plt.savefig(output,transparent = True)
+    canvas.paste(Image.open(output), (480, 0))
+
+    water,fire,earth,wind = alchemy["1"],alchemy["2"],alchemy["3"],alchemy["4"]
+    elements = [water, fire, earth, wind]
+    max_value = max(elements)
+    ethereum = max(min([water,fire,earth,wind]) -2,0)
+    tag = f'{"元素炼金师" if ethereum*4 > products else "传统炼金师"} Lv.{integer_log(ethereum,2)}'
+    draw.text((20,240),tag, fill = (0,0,0),font = font_big)
+    draw.text((21,241),tag, fill = (0,0,0),font = font_big)
+    tag = f"主要元素 {'|'.join({0:'水',1:'火',2:'土',3:'风'}[i] for i, value in enumerate(elements) if value == max_value)}"
+    draw.text((20,320),tag, fill = (0,0,0),font = font_big)
+    draw.text((21,321),tag, fill = (0,0,0),font = font_big)
+    draw.text((200,70),nickname, fill = (0,0,0), font = font_big)
+    info = [canvas]
+    def bar_chart(info:str, lenth:float, color:str = '99CCFF'):
+        """
+        条形图
+        """
+        canvas = Image.new("RGBA", (880, 60))
+        draw = ImageDraw.Draw(canvas)
+        draw.rectangle(((20,10), (860, 50)), fill = "#00000033")
+        draw.rectangle(((20,10), (80 + int(lenth*780), 50)), fill = color)
+        draw.text((30,10), info, fill = (0,0,0), font = font_normal)
+        return canvas
+
+    level = integer_log(water,2)
+    info.append(bar_chart(f"水元素Lv.{level}",water/2**(level+1),"#66CCFFCC"))
+    level = integer_log(fire,2)
+    info.append(bar_chart(f"火元素Lv.{level}",fire/2**(level+1),"#CC3300CC"))
+    level = integer_log(earth,2)
+    info.append(bar_chart(f"土元素Lv.{level}",earth/2**(level+1),"#996633CC"))
+    level = integer_log(wind,2)
+    info.append(bar_chart(f"风元素Lv.{level}",wind/2**(level+1),"#99CCFFCC"))
+
+    element = alchemy["5"]
+    level = integer_log(element,2)
+    info.append(bar_chart(f"蒸汽Lv.{level}",element/2**(level+1),"#CCFFFFCC"))
+    element = alchemy["6"]
+    level = integer_log(element,2)
+    info.append(bar_chart(f"沼泽Lv.{level}",element/2**(level+1),"#666633CC"))
+    element = alchemy["7"]
+    level = integer_log(element,2)
+    info.append(bar_chart(f"寒冰Lv.{level}",element/2**(level+1),"#0099FFCC"))
+    element = alchemy["8"]
+    level = integer_log(element,2)
+    info.append(bar_chart(f"岩浆Lv.{level}",element/2**(level+1),"#990000CC"))
+    element = alchemy["9"]
+    level = integer_log(element,2)
+    info.append(bar_chart(f"雷电Lv.{level}",element/2**(level+1),"#9900FFCC"))
+    element = alchemy["0"]
+    level = integer_log(element,2)
+    info.append(bar_chart(f"尘埃Lv.{level}",element/2**(level+1),"#99CCCCCC"))
+    return info
+
 async def my_info_head(user:UserDict, nickname:str):
     """
     我的资料卡第一个信息
     """
     gold = user.gold
     win = user.win
     lose = user.lose
     canvas = Image.new("RGBA", (880, 300))
     avatar = Image.open(await download_avatar(user.user_id))
-    avatar = avatar.resize((250,250))
+    avatar = avatar.resize((260,260))
     circle_mask = Image.new("RGBA", avatar.size, (255, 255, 255, 0))
     ImageDraw.Draw(circle_mask).ellipse(((0,0),avatar.size), fill="black")
-    canvas.paste(avatar, (25, 25), circle_mask)
+    canvas.paste(avatar, (20, 20), circle_mask)
     draw = ImageDraw.Draw(canvas)
     draw.text((300,40),f"{nickname}", fill = (0,0,0),font = font_big)
     draw.line(((300, 120), (860, 120)), fill = "gray", width = 4)
     draw.text((300,140),f"金币 {'{:,}'.format(gold)}", fill = (0,0,0),font = font_normal)
     draw.text((300,190),f"战绩 {win}:{lose}", fill = (0,0,0),font = font_normal)
     draw.text((300,240),f"胜率 {(round(win * 100 / (win + lose), 2) if win > 0 else 0)}%\n", fill=(0,0,0),font = font_normal)
     return canvas
@@ -386,52 +486,52 @@
             'edgecolor':"none",
             }, 
         textprops = {'fontsize':20},
         pctdistance = 0.81,
         labeldistance = 1.05
         )
     plt.axis('equal')
-    plt.subplots_adjust(top = 0.95, bottom = 0.05, right = 0.9, left = 0.5, hspace = 0, wspace = 0)
+    plt.subplots_adjust(top = 0.95, bottom = 0.05, left = 0.32, hspace = 0, wspace = 0)
     plt.savefig(output,format='png', dpi = 100, transparent = True)
     plt.close()
     return Image.open(output)
 
 def my_info_account(msg:str, dist):
     """
     我的资料卡账户分析
     """
     canvas = Image.new("RGBA", (880, 400))
     statistics = my_info_statistics(dist)
     canvas.paste(statistics, (880 - statistics.size[0], 0))
-    linecard(msg, 880, 400,padding = (20,30),endline = "账户信息",canvas = canvas)
+    linecard(msg, width = 880, height = 400,padding = (20,30),endline = "账户信息",canvas = canvas)
     return canvas
 
 async def group_info_head(group_name:str, company_name:str, group_id:int, member_count:Tuple[int,int]):
     """
     群资料卡第一个信息
     """
     canvas = Image.new("RGBA", (880, 300))
     avatar = Image.open(await download_groupavatar(group_id))
-    avatar = avatar.resize((250,250))
+    avatar = avatar.resize((260,260))
     circle_mask = Image.new("RGBA", avatar.size, (255, 255, 255, 0))
     ImageDraw.Draw(circle_mask).ellipse(((0,0),avatar.size), fill="black")
-    canvas.paste(avatar, (25, 25), circle_mask)
+    canvas.paste(avatar, (20, 20), circle_mask)
     draw = ImageDraw.Draw(canvas)
     font = ImageFont.truetype(font = fontname, size = 40, encoding = "utf-8")
     draw.text((300,40),f"{group_name}", fill = (0,0,0),font = font_big)
     draw.line(((300, 120), (860, 120)), fill = "gray", width = 6)
     draw.text((300,140),f"公司：{company_name if company_name else '未注册'}", fill = (0,0,0),font = font_normal)
     draw.text((300,190),f"单位：{str(group_id)[:4]}...", fill = (0,0,0),font = font_normal)
     draw.rectangle(((300,240), (740,280)), fill = "#00000033")
     draw.rectangle(((300,240), (300 + int(440 * member_count[0]/(member_count[1])),280)), fill = "#99CCFF")
     draw.text((310,240),f"{member_count[0]}/{member_count[1]}", fill = (0,0,0),font = font_normal )
     draw.text((750,240),f"{round(100 * member_count[0]/member_count[1],1)}%", fill = (0,0,0),font = font_normal)
     return canvas
 
-def info_Splicing(info:List[IMG],BG_path, spacing:int = 20):
+def info_splicing(info:List[IMG],BG_path, spacing:int = 20):
     """
     信息拼接
         info:信息图片列表
         bg_path:背景地址
     """
     bg = Image.open(BG_path).convert("RGBA")
     x = 880 # 设定信息宽度880像素
```

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 nonebot_plugin_game_collection/Account.py
+nonebot_plugin_game_collection/Alchemy.py
 nonebot_plugin_game_collection/Game.py
 nonebot_plugin_game_collection/Manager.py
 nonebot_plugin_game_collection/Market.py
 nonebot_plugin_game_collection/Prop.py
 nonebot_plugin_game_collection/__init__.py
 nonebot_plugin_game_collection/config.py
 nonebot_plugin_game_collection/data.py
 nonebot_plugin_game_collection.egg-info/PKG-INFO
 nonebot_plugin_game_collection.egg-info/SOURCES.txt
 nonebot_plugin_game_collection.egg-info/dependency_links.txt
 nonebot_plugin_game_collection.egg-info/requires.txt
 nonebot_plugin_game_collection.egg-info/top_level.txt
+nonebot_plugin_game_collection/Fortress/core.py
 nonebot_plugin_game_collection/HorseRace/events_main.py
 nonebot_plugin_game_collection/HorseRace/horse.py
 nonebot_plugin_game_collection/HorseRace/race_group.py
 nonebot_plugin_game_collection/HorseRace/start.py
-nonebot_plugin_game_collection/resource/element_library.json
 nonebot_plugin_game_collection/resource/menu_data.json
 nonebot_plugin_game_collection/resource/props_library.json
 nonebot_plugin_game_collection/resource/horserace/Stand.json
 nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
 nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
 nonebot_plugin_game_collection/resource/horserace/基础事件.json
 nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
```

### Comparing `nonebot_plugin_game_collection-2.2.9/setup.py` & `nonebot_plugin_game_collection-2.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.2.9',
+version='2.3.1',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
 platforms='all',
-install_requires=["nonebot2","nonebot-adapter-onebot","nonebot_plugin_apscheduler","mplfinance","seaborn"],
+install_requires=["nonebot2","nonebot-adapter-onebot","nonebot_plugin_apscheduler","mplfinance","seaborn","fonttools","httpx"],
 url='https://github.com/KarisAya/nonebot_plugin_game_collection',
 )
```

