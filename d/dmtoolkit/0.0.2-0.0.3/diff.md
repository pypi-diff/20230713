# Comparing `tmp/dmtoolkit-0.0.2.tar.gz` & `tmp/dmtoolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtoolkit-0.0.2.tar", last modified: Tue Jul 11 18:02:41 2023, max compression
+gzip compressed data, was "dmtoolkit-0.0.3.tar", last modified: Thu Jul 13 16:44:22 2023, max compression
```

## Comparing `dmtoolkit-0.0.2.tar` & `dmtoolkit-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.405879 dmtoolkit-0.0.2/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.2/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-11 18:02:41.404879 dmtoolkit-0.0.2/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.2/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1224 2023-07-11 13:42:13.000000 dmtoolkit-0.0.2/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.2/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-11 18:02:41.405879 dmtoolkit-0.0.2/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.2/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.394879 dmtoolkit-0.0.2/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.398879 dmtoolkit-0.0.2/src/dmtoolkit/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-11 18:02:19.000000 dmtoolkit-0.0.2/src/dmtoolkit/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.400879 dmtoolkit-0.0.2/src/dmtoolkit/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      101 2023-07-05 17:45:33.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/dndbeyondapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/foundryapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5806 2023-07-11 12:55:44.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/open5eapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.2/src/dmtoolkit/apis/wikijsapi.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.401879 dmtoolkit-0.0.2/src/dmtoolkit/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-06-20 14:20:28.000000 dmtoolkit-0.0.2/src/dmtoolkit/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      293 2023-06-20 21:35:42.000000 dmtoolkit-0.0.2/src/dmtoolkit/db/dndorm.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12561 2023-07-11 18:01:51.000000 dmtoolkit-0.0.2/src/dmtoolkit/dmtools.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.403879 dmtoolkit-0.0.2/src/dmtoolkit/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1932 2023-07-07 15:02:17.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndcharacter.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      949 2023-07-07 15:28:26.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dnditem.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1808 2023-07-07 16:01:05.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndmonster.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1519 2023-07-07 14:51:57.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndobject.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndshop.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1037 2023-07-07 16:01:33.000000 dmtoolkit-0.0.2/src/dmtoolkit/models/dndspell.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-11 18:02:41.399879 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)      748 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-11 18:02:41.000000 dmtoolkit-0.0.2/src/dmtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.507252 dmtoolkit-0.0.3/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.3/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 16:44:22.507252 dmtoolkit-0.0.3/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.3/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.3/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.3/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-13 16:44:22.507252 dmtoolkit-0.0.3/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.3/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.499252 dmtoolkit-0.0.3/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.502252 dmtoolkit-0.0.3/src/dmtoolkit/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-13 16:44:04.000000 dmtoolkit-0.0.3/src/dmtoolkit/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.505252 dmtoolkit-0.0.3/src/dmtoolkit/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      101 2023-07-05 17:45:33.000000 dmtoolkit-0.0.3/src/dmtoolkit/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.3/src/dmtoolkit/apis/dndbeyondapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.3/src/dmtoolkit/apis/foundryapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     5957 2023-07-11 18:36:58.000000 dmtoolkit-0.0.3/src/dmtoolkit/apis/open5eapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.3/src/dmtoolkit/apis/wikijsapi.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.506252 dmtoolkit-0.0.3/src/dmtoolkit/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-06-20 14:20:28.000000 dmtoolkit-0.0.3/src/dmtoolkit/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      293 2023-06-20 21:35:42.000000 dmtoolkit-0.0.3/src/dmtoolkit/db/dndorm.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.3/src/dmtoolkit/dmtools.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.507252 dmtoolkit-0.0.3/src/dmtoolkit/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1958 2023-07-13 16:05:59.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/dndcharacter.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      951 2023-07-13 14:30:24.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/dnditem.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1824 2023-07-11 18:24:05.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/dndmonster.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1539 2023-07-11 18:26:41.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/dndobject.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/dndshop.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1053 2023-07-11 18:24:41.000000 dmtoolkit-0.0.3/src/dmtoolkit/models/dndspell.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 16:44:22.504252 dmtoolkit-0.0.3/src/dmtoolkit.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 16:44:22.000000 dmtoolkit-0.0.3/src/dmtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      748 2023-07-13 16:44:22.000000 dmtoolkit-0.0.3/src/dmtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-13 16:44:22.000000 dmtoolkit-0.0.3/src/dmtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-13 16:44:22.000000 dmtoolkit-0.0.3/src/dmtoolkit.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-13 16:44:22.000000 dmtoolkit-0.0.3/src/dmtoolkit.egg-info/top_level.txt
```

### Comparing `dmtoolkit-0.0.2/LICENSE` & `dmtoolkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.2/PKG-INFO` & `dmtoolkit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.2/README.md` & `dmtoolkit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.2/pyproject.toml` & `dmtoolkit-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["src"]
 include = ["dmtoolkit*"]
 
 [tool.pytest.ini_options]
-addopts = "--cov=dmtoolkit -s -rx -l -x --log-level=INFO --ignore=src -v --no-cov-on-fail" #   --cov-reset
+addopts = "--cov=dmtoolkit -s -rx -l -x --log-level=INFO --ignore=src -v --no-cov-on-fail --pdb" #   --cov-reset
 testpaths = [
      "tests",
 ]
 pythonpath = [
     "src/dmtoolkit",
 ]
 log_auto_indent = true
```

### Comparing `dmtoolkit-0.0.2/setup.py` & `dmtoolkit-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/apis/dndbeyondapi.py` & `dmtoolkit-0.0.3/src/dmtoolkit/apis/dndbeyondapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/apis/open5eapi.py` & `dmtoolkit-0.0.3/src/dmtoolkit/apis/open5eapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class Open5e:
     api_url = "https://api.open5e.com"
 
     @classmethod
     def all(cls, endpoint=None):
-        endpoint = endpoint or f"{cls.api_url}"
+        endpoint = f"{cls.api_url}/{endpoint}"
         response = requests.get(endpoint).json()
         results = response["results"]
         while response.get("next"):
             response = requests.get(response["next"]).json()
             results += response["results"]
         return [cls._build(r) for r in results]
 
@@ -26,14 +26,18 @@
         if url:
             results = requests.get(url).json()
             return cls._build(results)
 
 
 class Open5eMonster(Open5e):
     @classmethod
+    def all(cls):
+        return super().all(endpoint="monsters")
+
+    @classmethod
     def search(cls, term, key="search"):
         return super().search(term=term, key=key, endpoint="monsters")
 
     @classmethod
     def _build(cls, data):
         obj = {}
         obj["name"] = data["name"]
@@ -85,14 +89,18 @@
                 obj["spell_list"][spell["name"]] = spell
         obj["desc"] = f'{obj["alignment"]} {obj["subtype"]} {obj["type"]}'
         return obj
 
 
 class Open5eSpell(Open5e):
     @classmethod
+    def all(cls):
+        return super().all(endpoint="spells")
+
+    @classmethod
     def search(cls, term, key="search"):
         return super().search(term=term, key=key, endpoint="spells")
 
     @classmethod
     def _build(cls, data):
         obj = {}
         obj["name"] = data["name"]
@@ -141,15 +149,15 @@
         obj["desc"] = data.get("desc") or f"{obj['type']} {obj['properties']}"
         return obj
 
     @classmethod
     def all(cls):
         results = []
         for endpoint in ["armor/", "weapons/", "magicitems/"]:
-            results += super().all(cls.api_url + endpoint)
+            results += super().all(endpoint)
         return results
 
     @classmethod
     def search(cls, term, key="search"):
         results = []
         for endpoint in ["armor/", "weapons/", "magicitems/"]:
             results += super().search(term=term, key=key, endpoint=endpoint)
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/apis/wikijsapi.py` & `dmtoolkit-0.0.3/src/dmtoolkit/apis/wikijsapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/dmtools.py` & `dmtoolkit-0.0.3/src/dmtoolkit/dmtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 import random
 from slugify import slugify
 import dice
 from autonomous.logger import log
 
 from autonomous.apis import OpenAI
 
-from models import Monster
-from models import Item
-from models import Spell
-from models import Character
-from models import Shop
+from dmtoolkit.models import Monster, Item, Spell, Character, Shop
 
 
 class DMTools:
     """
     _summary_
 
     Returns:
@@ -261,15 +257,15 @@
         primer = """
         You are a D&D 5e Encounter generator that creates level appropriate random encounters and specific loot rewards.
         """
         difficulty = random.choice(list(enumerate(difficulty_list)))
         loot_type = random.choices(
             loot,
             weights=[10, 5, 3, 30, 10, 10],
-            k=(difficulty[0] * DMToolkit.LOOT_MULTIPLIER) + 1,
+            k=(difficulty[0] * DMTools.LOOT_MULTIPLIER) + 1,
         )
         prompt = f"Generate an appropriate Dungeons and Dragons 5e encounter for a party of {num_players} at level {level} that is {difficulty[1]} and rewards the following type of loot items: {loot_type}"
         funcobj = {
             "name": "generate_encounter",
             "description": "Generate an Encounter object",
             "parameters": {
                 "type": "object",
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/models/dndcharacter.py` & `dmtoolkit-0.0.3/src/dmtoolkit/models/dndcharacter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .dndobject import DnDObject
+from dmtoolkit.models.dndobject import DnDObject
 from autonomous import log
-from apis import DnDBeyondAPI
+from dmtoolkit.apis import DnDBeyondAPI
 from slugify import slugify
 from autonomous.storage.cloudinarystorage import CloudinaryStorage
 
 
 class Character(DnDObject):
     attributes = {
         "dnd_id": None,
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/models/dnditem.py` & `dmtoolkit-0.0.3/src/dmtoolkit/models/dnditem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from .dndobject import DnDObject
+from dmtoolkit.models.dndobject import DnDObject
 from autonomous import logger
-import random
 import markdown
 
 
 class Item(DnDObject):
     attributes = {
         "name": "",
         "image": {"url": "", "asset_id": 0, "raw": None},
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/models/dndmonster.py` & `dmtoolkit-0.0.3/src/dmtoolkit/models/dndmonster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .dndobject import DnDObject
+from dmtoolkit.models.dndobject import DnDObject
 from autonomous import log
 import random
 
 
 class Monster(DnDObject):
     attributes = {
         "name": "",
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/models/dndobject.py` & `dmtoolkit-0.0.3/src/dmtoolkit/models/dndobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from apis import open5eapi
-from autonomous.apis import OpenAI
-from db.dndorm import DnDORM
+from dmtoolkit.db.dndorm import DnDORM
+from dmtoolkit.apis import open5eapi
 
+from autonomous.apis import OpenAI
 from autonomous.storage.cloudinarystorage import CloudinaryStorage
 from autonomous.model.automodel import AutoModel
 from autonomous import log
 
 from slugify import slugify
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/models/dndshop.py` & `dmtoolkit-0.0.3/src/dmtoolkit/models/dndshop.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit/models/dndspell.py` & `dmtoolkit-0.0.3/src/dmtoolkit/models/dndspell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .dndobject import DnDObject
+from dmtoolkit.models.dndobject import DnDObject
 from autonomous import logger
 import random
 
 
 class Spell(DnDObject):
     attributes = {
         "name": "",
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit.egg-info/PKG-INFO` & `dmtoolkit-0.0.3/src/dmtoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.2/src/dmtoolkit.egg-info/SOURCES.txt` & `dmtoolkit-0.0.3/src/dmtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

