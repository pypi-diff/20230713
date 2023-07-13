# Comparing `tmp/nonebot_plugin_game_collection-2.3.2.tar.gz` & `tmp/nonebot_plugin_game_collection-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.3.2.tar", last modified: Thu Jul 13 13:38:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.3.3.tar", last modified: Thu Jul 13 19:09:43 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.3.2.tar` & `nonebot_plugin_game_collection-2.3.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.879228 nonebot_plugin_game_collection-2.3.2/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.2/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-07-13 13:38:09.876728 nonebot_plugin_game_collection-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.818474 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21627 2023-07-13 13:15:00.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Alchemy.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.828846 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Fortress/
--rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Fortress/core.py
--rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.836788 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10594 2023-07-12 11:14:50.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    21939 2023-07-13 13:36:34.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    32577 2023-07-13 09:58:22.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0    11300 2023-07-13 12:39:26.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.841793 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.868012 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.870013 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.875223 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    21412 2023-06-29 17:01:38.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.827344 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 13:38:09.879228 nonebot_plugin_game_collection-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-07-13 13:38:05.000000 nonebot_plugin_game_collection-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.436160 nonebot_plugin_game_collection-2.3.3/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.3/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-07-13 19:09:43.435660 nonebot_plugin_game_collection-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.377416 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21635 2023-07-13 18:22:12.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.387925 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Fortress/
+-rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Fortress/core.py
+-rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.395432 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10598 2023-07-13 18:15:22.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    23119 2023-07-13 19:07:41.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    32550 2023-07-13 18:50:38.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0    11300 2023-07-13 19:07:21.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.398934 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.419452 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.421454 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.434159 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    21412 2023-06-29 17:01:38.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:09:43.386424 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-13 19:09:43.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-13 19:09:43.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 19:09:43.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-13 19:09:43.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-13 19:09:43.000000 nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 19:09:43.436661 nonebot_plugin_game_collection-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-07-13 19:06:19.000000 nonebot_plugin_game_collection-2.3.3/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.3.2/LICENSE` & `nonebot_plugin_game_collection-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/README.md` & `nonebot_plugin_game_collection-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Account.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
     if company_id in user.group_accounts:
         target_group_account = user.group_accounts[company_id]
     else:
         return f"你在 {company_name} 没有创建账户"
 
     group_account.gold -= gold
     ExRate = group_data[group_account.group_id].company.level/group_data[company_id].company.level
-    ExRate = ExRate if ExRate else 1.0
+    ExRate = min(ExRate,10) if ExRate else 1.0
     tgold = int(ExRate * gold + 0.5)
     fee = transfer_fee(tgold, user.transfer_limit)
     target_group_account.gold += tgold - fee
     user.transfer_limit += tgold
     user.gold -= fee
 
     return f"向 {company_name} 转移{gold}金币。\n汇率：{round(ExRate,2)} 手续费：{fee}({round(100*fee/tgold,2)}%)\n实际到账金额：{tgold - fee}"
```

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Alchemy.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Alchemy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Fortress/core.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Fortress/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             namelist.add(user_id)
             user.group_accounts[group_id] = GroupAccount(event)
             group_account = user.group_accounts[group_id]
             data.save()
     else:
         group_id = user.connect
         if group_id:
-            group_account = user.group_accounts[group_id]
+            group_account = user.group_accounts.get(group_id)
         else:
             group_account = None
 
     return user,group_account
 
 def locate_user_at(event:GroupMessageEvent, user_id:int) ->Tuple[UserDict,GroupAccount]:
     """
```

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Market.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
     )
 
 import random
 import math
 import time
 import datetime
 import asyncio
+import pickle
 
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
-from .utils.chart import linecard, group_info_head, info_splicing
+from .utils.chart import linecard, group_info_head, info_splicing, linecard_to_png
 from .data import GroupAccount, Company, ExchangeInfo
 from .data import OHLC, props_library
 from .config import bot_name, revolt_gini, max_bet_gold, bet_gold, path
 
 from . import Manager
 
 data = Manager.data
@@ -281,71 +282,62 @@
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
 
     company = group_data[company_id].company
     company_name = company.company_name
 
-    exchange = company.exchange
-    user_id = user.user_id
-
-    rank = [x for x in exchange.items() if x[0] != user_id]
+    rank = [x for x in company.exchange.items() if x[0] != user.user_id]
+    if not rank:
+        return f"没有正在出售的 {company_name}"
     rank.sort(key = lambda x:x[1].quote)
-    
-    my_gold = group_account.gold
 
     gold = 0
-    count = 0
-    n = 0
-    i = 0
-
-    if (l := len(rank)) < 1:
-        return f"没有正在出售的 {company_name}"
-
-    lastinfo = None
-
-    while count < buy and i < l:
-        tmp = rank[i]
-        n = tmp[1].n
-        quote = tmp[1].quote
-        count += n
-        if count > buy:
-            lastinfo = (tmp[0],ExchangeInfo(group_id = tmp[1].group_id, quote = quote,n = (count - buy)))
-            n = n - (count - buy)
-            count = buy
-        unsettled = int((quote * n) + 0.5)
+    Exlist = []
+    my_gold = group_account.gold
+    for user_id,exchange in rank:
+        n = exchange.n
+        Exlist.append([user_id,n])
+        if buy < n:
+            Exlist[-1][1] = buy
+            break
+        buy -= n
+        unsettled = int((exchange.quote * n) + 0.5)
         gold += unsettled
-        rank[i] = [tmp[0], tmp[1].group_id, n, unsettled]
         if gold > my_gold:
             return f"你的金币不足（{my_gold}）"
-        i += 1
-
+    gold = 0
+    count = 0
     group_account.stocks.setdefault(company_id,0)
-    rank = rank[:i]
-    for x in rank:
-        seller_user = user_data[x[0]]
-        seller_group_account = seller_user.group_accounts[x[1]]
-        unsettled = x[3]
+    for user_id,n in Exlist:
+        exchange = company.exchange[user_id]
+        # 定位卖家
+        seller_user = user_data[user_id]
+        seller_group_account = seller_user.group_accounts[exchange.group_id]
+        # 金币结算
+        unsettled = int((exchange.quote * n) + 0.5)
+        gold += unsettled
         user.gold -=  unsettled
         group_account.gold -= unsettled
         if seller_group_account.props.get("42001",0):
             fee = 0
         else:
             fee = int(unsettled * 0.02)
         seller_user.gold += unsettled - fee
         seller_group_account.gold += unsettled - fee
-        n = x[2]
-        group_account.stocks[company_id] += n
+        # 股票结算
         seller_group_account.stocks[company_id] -= n
+        group_account.stocks[company_id] += n
+        count += n
+        # 更新卖家群账户信息
         value_update(seller_group_account)
-        del exchange[x[0]]
-    else:
-        value_update(group_account)
-    if lastinfo:
-        exchange[lastinfo[0]] = lastinfo[1]
+        exchange.n -= n
+    # 更新买家群账户信息
+    value_update(group_account)
+    company.exchange = {k:v for k,v in company.exchange.items() if v.n > 0}
 
     return (
         f"{company_name}\n"
         "——————————\n"
         f"数量：{count}\n"
         f"单价：{round(gold/count,2)}\n"
         f"总计：{gold}\n"
@@ -508,39 +500,68 @@
         f"市场流动 {'{:,}'.format(round(group_gold))}\n"
         f"发行价格 {'{:,}'.format(round(max(group_gold,float_gold)/issuance,2))}\n"
         f"结算价格 {'{:,}'.format(round(float_gold/issuance,2))}\n"
         f"剩余数量 {company.stock}\n"
         )
     return msg
 
-def Market_info_All(event:MessageEvent, ohlc:bool = False):
+def Market_info_All(event:MessageEvent):
     """
     市场信息总览
     """
     global company_index
     company_ids = set([company_index[company_id] for company_id in company_index])
     companys = []
     for company_id in company_ids:
         company = group_data[company_id].company
         companys.append(company)
     companys.sort(key = lambda x:x.group_gold, reverse = True)
-
-    lst = [companys[i:i+5] for i in range(0, len(companys), 5)]
+    lst = []
+    l = 0
+    for company in companys:
+        lst.append(company.company_name +"\n" + "——————————————\n" + stock_profile(company)[:-1])
+        l += 1
+    lst = [lst[i:i+5] for i in range(0, l, 5)]
     msg = []
-    for seg in lst:
-        info = []
-        for company in seg:
-            info.append(linecard(company.company_name +"\n" + "----\n" + stock_profile(company)[:-1],width = 880))
+    for x in lst:
         msg.append({"type":"node",
                     "data":{
                         "name":f"{bot_name}",
                         "uin":str(event.self_id),
-                        "content":MessageSegment.image(info_splicing(info, Manager.BG_path(event.user_id)))}})
+                        "content":"——————————————\n".join(x)}})
     return msg
 
+def pricelist(user_id:int):
+    """
+    市场价格表
+    """
+    global company_index
+    company_ids = set([company_index[company_id] for company_id in company_index])
+    companys = []
+    for company_id in company_ids:
+        company = group_data[company_id].company
+        companys.append(company)
+    companys.sort(key = lambda x:x.group_gold, reverse = True)
+    msg = ""
+    for company in companys:
+        group_gold = company.group_gold
+        float_gold = company.float_gold
+        gold = max(group_gold,float_gold)
+        issuance = company.issuance
+        stock = company.stock
+        msg += (
+            "----\n"
+            f"[pixel][20]{company.company_name}\n"
+            f"[pixel][20]发行 [nowrap]\n[color][{'green' if gold == float_gold else 'red'}]{'{:,}'.format(round(gold/issuance,2))}[nowrap]\n"
+            f"[pixel][300]结算 [nowrap]\n[color][green]{'{:,}'.format(round(float_gold/issuance,2))}[nowrap]\n"
+            f"[pixel][600]数量 [nowrap]\n[color][{'green' if stock else 'red'}]{stock}\n"
+            )
+
+    return MessageSegment.image(info_splicing([linecard(msg,width = 880,endline = "市场价格表")], Manager.BG_path(user_id)))
+
 def update_intro(company_name:str, intro:str):
     if company_name in company_index:
         company_id = company_index[company_name]
     else:
         return f"没有 {company_name} 的注册信息"
     group_data[company_id].company.intro = intro
     return "简介更新完成!"
```

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -749,15 +749,15 @@
             matcher.set_arg("company_id", company_id)
     else:
         await Exchange_sell.finish()
 
 @Exchange_sell.got("info", prompt = "请输入出售数量和单价，用空格隔开。")
 async def _(matcher:Matcher, event:MessageEvent, info:Message = Arg()):
     info = info.extract_plain_text().strip().split()
-    if len(info) == 2 and info[1].isdigit():
+    if len(info) == 2 and info[0].isdigit():
         n = int(info[0])
     elif info[0] == "取消":
         await Exchange_sell.finish()
     else:
         await Exchange_sell.reject("格式错误，请重新输入正确格式或输入【取消】中止对话。")
     try:
         quote = float(info[1])
@@ -780,43 +780,44 @@
         group_id = event.group_id
     else:
         return
     msg = await Market.group_info(bot,event,group_id)
     await group_info.finish(msg)
 
 # 市场信息
-Market_info_0 = on_command("市场信息",aliases={"查看市场"}, priority = 20, block = True)
+Market_info = on_command("市场信息",aliases={"查看市场"}, priority = 20, block = True)
 
-@Market_info_0.handle()
+@Market_info.handle()
 async def _(bot:Bot, event:MessageEvent, arg:Message = CommandArg()):
     company_name = arg.extract_plain_text().strip()
     if company_name:
         if company_name in company_index:
             company_id = company_index[company_name]
             msg = await Market.group_info(bot,event,company_id)
         else:
             msg = f"没有 {company_name} 的注册信息"
-        await Market_info_0.send(msg)
+        await Market_info.send(msg)
     else:
-        if msg := Market.Market_info_All(event,False):
+        if msg := Market.Market_info_All(event):
             if len(msg) == 1:
-                await Market_info_0.send(msg[0]["data"]["content"])
+                await Market_info.send(msg[0]["data"]["content"])
             elif isinstance(event, GroupMessageEvent):
                 await bot.send_group_forward_msg(group_id = event.group_id, messages = msg)
             else:
                 await bot.send_private_forward_msg(user_id = event.user_id, messages = msg)
         else:
-            await Market_info_0.send("市场为空")
+            await Market_info.send("市场为空")
 
-#Market_info_1 = on_command("市场行情",aliases={"市场走势"}, priority = 20, block = True)
+# 市场价格表
+Market_pricelist = on_command("市场价格表",aliases={"股票价格表"}, priority = 20, block = True)
 
-#@Market_info_1.handle()
-#async def _(bot:Bot, event:MessageEvent, arg:Message = CommandArg()):
-#    msg = Market.Market_info_All(event,True)
-#    await Market_info_1.finish(msg)
+@Market_pricelist.handle()
+async def _(event:MessageEvent):
+    msg = Market.pricelist(event.user_id)
+    await Market_pricelist.finish(msg)
 
 # 更新公司简介
 update_intro = on_command(
     "更新公司简介",
     aliases = {"添加公司简介", "修改公司简介"},
     permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority = 20,
```

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.3.3/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.2/setup.py` & `nonebot_plugin_game_collection-2.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.3.2',
+version='2.3.3',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

