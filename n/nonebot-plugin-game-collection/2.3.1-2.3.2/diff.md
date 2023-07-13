# Comparing `tmp/nonebot_plugin_game_collection-2.3.1.tar.gz` & `tmp/nonebot_plugin_game_collection-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.3.1.tar", last modified: Thu Jul 13 13:19:17 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.3.2.tar", last modified: Thu Jul 13 13:38:09 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.3.1.tar` & `nonebot_plugin_game_collection-2.3.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.912826 nonebot_plugin_game_collection-2.3.1/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.1/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-07-13 13:19:17.912325 nonebot_plugin_game_collection-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.862064 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21627 2023-07-13 13:15:00.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Alchemy.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.872572 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Fortress/
--rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Fortress/core.py
--rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.880579 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10594 2023-07-12 11:14:50.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    21889 2023-07-13 13:11:29.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    32577 2023-07-13 09:58:22.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0    11300 2023-07-13 12:39:26.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.883582 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.902317 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.903818 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.910324 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    21412 2023-06-29 17:01:38.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:19:17.871071 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-13 13:19:17.000000 nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 13:19:17.912826 nonebot_plugin_game_collection-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-07-13 13:19:09.000000 nonebot_plugin_game_collection-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.879228 nonebot_plugin_game_collection-2.3.2/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.2/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-07-13 13:38:09.876728 nonebot_plugin_game_collection-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.818474 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21627 2023-07-13 13:15:00.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.828846 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Fortress/
+-rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Fortress/core.py
+-rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.836788 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10594 2023-07-12 11:14:50.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    21939 2023-07-13 13:36:34.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    32577 2023-07-13 09:58:22.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0    11300 2023-07-13 12:39:26.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.841793 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.868012 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.870013 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.875223 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    21412 2023-06-29 17:01:38.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:38:09.827344 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-13 13:38:09.000000 nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:38:09.879228 nonebot_plugin_game_collection-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-07-13 13:38:05.000000 nonebot_plugin_game_collection-2.3.2/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.3.1/LICENSE` & `nonebot_plugin_game_collection-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/README.md` & `nonebot_plugin_game_collection-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Alchemy.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Alchemy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Fortress/core.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Fortress/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Market.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,20 @@
     user.gold += value - fee
     group_account.gold += value - fee
     company.gold -= value
     # 更新公司信息
     company.group_gold = group_gold
     company.float_gold = float_gold
     # 更新交易市场
-    exchange.n = stock if (user_id := user.user_id) in company.exchange and (exchange := company.exchange[user_id]).group_id == group_account.group_id and stock< exchange.n else exchange.n
+    user_id = user.user_id
+    if user_id in company.exchange:
+        exchange = company.exchange[user_id]
+        if exchange.group_id == group_account.group_id:
+            if stock < exchange.n:
+                exchange.n = stock
     # 更新群账户信息
     value_update(group_account)
     return (
         f"{company_name}\n"
         "——————————\n"
         f"数量：{settle}\n"
         f"单价：{round(value/settle,2)}\n"
```

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.3.2/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.1/setup.py` & `nonebot_plugin_game_collection-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.3.1',
+version='2.3.2',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

