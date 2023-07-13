# Comparing `tmp/fgo_api_types-2023.7.7.16.36.40.tar.gz` & `tmp/fgo_api_types-2023.7.9.5.5.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.7.7.16.36.40.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.7.9.5.5.49.tar", max compression
```

## Comparing `fgo_api_types-2023.7.7.16.36.40.tar` & `fgo_api_types-2023.7.9.5.5.49.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-07-07 16:36:20.421844 fgo_api_types-2023.7.7.16.36.40/LICENSE
--rw-r--r--   0        0        0      449 2023-07-07 16:36:20.421844 fgo_api_types-2023.7.7.16.36.40/README.md
--rw-r--r--   0        0        0        0 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/enums.py
--rw-r--r--   0        0        0   160313 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    78590 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/nice.py
--rw-r--r--   0        0        0    53238 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19183 2023-07-07 16:36:40.117894 fgo_api_types-2023.7.7.16.36.40/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-07-07 16:36:40.465895 fgo_api_types-2023.7.7.16.36.40/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.7.7.16.36.40/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-09 05:05:22.886548 fgo_api_types-2023.7.9.5.5.49/LICENSE
+-rw-r--r--   0        0        0      449 2023-07-09 05:05:22.886548 fgo_api_types-2023.7.9.5.5.49/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   160313 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    78686 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    53238 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4207 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19183 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-07-09 05:05:49.882686 fgo_api_types-2023.7.9.5.5.49/pyproject.toml
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.7.9.5.5.49/PKG-INFO
```

### Comparing `fgo_api_types-2023.7.7.16.36.40/LICENSE` & `fgo_api_types-2023.7.9.5.5.49/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/basic.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/common.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/enums.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/gameenums.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/nice.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2214,14 +2214,15 @@
     CALL = "call"
     SHIFT = "shift"
     CHANGE = "change"
     TRANSFORM = "transform"
     SKILL_SHIFT = "skillShift"
     MISSION_TARGET_SKILL_SHIFT = "missionTargetSkillShift"
     AI_NPC = "aiNpc"
+    SVT_FOLLOWER = "svtFollower"
 
 
 class QuestEnemy(BaseModelORJson):
     deck: DeckType
     deckId: int
     userSvtId: int
     uniqueId: int
@@ -2339,14 +2340,15 @@
     noblePhantasm: SupportServantTd
     limit: SupportServantLimit
     flags: list[NiceNpcServantFollowerFlag]
 
 
 class SupportServant(BaseModelORJson):
     id: int
+    npcSvtFollowerId: int
     priority: int
     name: str
     svt: BasicServant
     releaseConditions: list[SupportServantRelease]
     lv: int
     atk: int
     hp: int
@@ -2354,14 +2356,15 @@
     skills: EnemySkill
     noblePhantasm: SupportServantTd
     flags: list[NiceNpcServantFollowerFlag]
     equips: list[SupportServantEquip]
     script: SupportServantScript
     limit: SupportServantLimit
     misc: SupportServantMisc
+    detail: QuestEnemy | None = None
 
 
 class NiceQuestPhaseAiNpc(BaseModelORJson):
     npc: NpcServant
     detail: QuestEnemy | None = None
     aiIds: list[int]
```

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/raw.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/rayshift.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/rayshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
     addedTime: datetime
     region: int
     questId: int
     questPhase: int
     questSelect: int
     eventId: int
     battleType: int
+    myDeck: Deck | None = None
     enemyDeck: list[Deck]
     transformDeck: Deck
     callDeck: list[Deck]
     aiNpcDeck: Deck | None = None
     shiftDeck: list[Deck]
     raidInfo: list[RaidInfo]
     startRaidInfo: list[RaidInfo]
```

### Comparing `fgo_api_types-2023.7.7.16.36.40/fgo_api_types/search.py` & `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.7.16.36.40/pyproject.toml` & `fgo_api_types-2023.7.9.5.5.49/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.07.07.16.36.40"
+version = "2023.07.09.05.05.49"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.7.7.16.36.40/PKG-INFO` & `fgo_api_types-2023.7.9.5.5.49/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.7.7.16.36.40
+Version: 2023.7.9.5.5.49
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

