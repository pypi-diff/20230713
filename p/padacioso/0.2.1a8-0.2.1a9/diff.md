# Comparing `tmp/padacioso-0.2.1a8.tar.gz` & `tmp/padacioso-0.2.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padacioso-0.2.1a8.tar", last modified: Wed Jul 12 13:11:24 2023, max compression
+gzip compressed data, was "padacioso-0.2.1a9.tar", last modified: Thu Jul 13 21:23:09 2023, max compression
```

## Comparing `padacioso-0.2.1a8.tar` & `padacioso-0.2.1a9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:11:24.370573 padacioso-0.2.1a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-12 13:11:24.370573 padacioso-0.2.1a8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:11:24.366573 padacioso-0.2.1a8/padacioso/
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso/bracket_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:11:24.370573 padacioso-0.2.1a8/padacioso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/padacioso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:11:24.370573 padacioso-0.2.1a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:11:24.370573 padacioso-0.2.1a8/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-12 13:11:24.000000 padacioso-0.2.1a8/test/test_padacioso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:23:09.846497 padacioso-0.2.1a9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-13 21:23:08.000000 padacioso-0.2.1a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 21:23:09.842497 padacioso-0.2.1a9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:23:09.842497 padacioso-0.2.1a9/padacioso/
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-07-13 21:23:08.000000 padacioso-0.2.1a9/padacioso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-13 21:23:08.000000 padacioso-0.2.1a9/padacioso/bracket_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 21:23:08.000000 padacioso-0.2.1a9/padacioso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:23:09.842497 padacioso-0.2.1a9/padacioso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 21:23:09.000000 padacioso-0.2.1a9/padacioso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 21:23:09.000000 padacioso-0.2.1a9/padacioso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:23:09.000000 padacioso-0.2.1a9/padacioso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 21:23:09.000000 padacioso-0.2.1a9/padacioso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 21:23:09.000000 padacioso-0.2.1a9/padacioso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 21:23:09.846497 padacioso-0.2.1a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-13 21:23:08.000000 padacioso-0.2.1a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:23:09.842497 padacioso-0.2.1a9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-13 21:23:08.000000 padacioso-0.2.1a9/test/test_padacioso.py
```

### Comparing `padacioso-0.2.1a8/LICENSE.md` & `padacioso-0.2.1a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.1a8/padacioso/__init__.py` & `padacioso-0.2.1a9/padacioso/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,31 @@
 
 import simplematch
 
 from padacioso.bracket_expansion import expand_parentheses, normalize_example
 
 try:
     from ovos_utils.log import LOG
+    from ovos_utils.parse import fuzzy_match  # uses rapidfuzz for performance
 except ImportError:
     import logging
 
     LOG = logging.getLogger('padacioso')
 
+    from difflib import SequenceMatcher
+
+
+    def fuzzy_match(x, against):
+        """Perform a 'fuzzy' comparison between two strings.
+        Returns:
+            float: match percentage -- 1.0 for perfect match,
+                   down to 0.0 for no match at all.
+        """
+        return SequenceMatcher(None, x, against).ratio()
+
 
 class IntentContainer:
     def __init__(self, fuzz=False, n_workers=4):
         self.intent_samples, self.entity_samples = {}, {}
         # self.intents, self.entities = {}, {}
         self.fuzz = fuzz
         self.workers = n_workers
@@ -164,33 +176,41 @@
                     elif str(v) not in self.entity_samples[k]:
                         # penalize parsed entity value not in samples
                         penalty += 0.1
                 return {"entities": entities or {},
                         "conf": 1 - penalty,
                         "name": intent_name}
 
-            if self.fuzz:
-                penalty += 0.25
-
+        if self.fuzz:
+            for r in regexes:
+                penalty = 0.25
                 for s in self._get_fuzzed(r):
-                    entities = simplematch.match(s, query, case_sensitive=False)
-                    fuzzy_penalty = penalty
-                    if "*" in s:  # very loose regex
-                        fuzzy_penalty += 0.1
-                    if "{" in s:  # capture group
-                        fuzzy_penalty += 0.05
-
-                    # depending on length
-                    diff = max(len(s) - len(query), 0)
-                    fuzzy_penalty += diff * 0.01
-
-                    if entities is not None:
-                        return {"entities": entities or {},
-                                "conf": max(1 - fuzzy_penalty, 0),
-                                "name": intent_name}
+                    entities = self._fuzzy_score(query, s, penalty)
+                    if entities:
+                        entities["name"] = intent_name
+                        return entities
+
+    def _fuzzy_score(self, query, s, penalty=0.25):
+        entities = simplematch.match(s, query, case_sensitive=False)
+
+        fuzzy_penalty = penalty
+        if "*" in s:  # very loose regex
+            fuzzy_penalty += 0.1
+        if "{" in s:  # capture group
+            fuzzy_penalty += 0.05
+        # depending on length
+        diff = max(len(s) - len(query), 0)
+        fuzzy_penalty += diff * 0.01
+        base_score = 1 - max(1 - fuzzy_penalty, 0)
+        fuzzy_score = fuzzy_match(s, query)
+        score = (fuzzy_score + base_score) / 2
+
+        if entities is not None:
+            return {"entities": entities or {},
+                    "conf": (fuzzy_score + base_score) / 2}
 
     def calc_intents(self, query: str) -> Iterator[dict]:
         """
         Determine possible intents for a given query
         @param query: input to evaluate for an intent match
         @return: yields dict intent matches
         """
@@ -220,22 +240,14 @@
             LOG.info("No match")
             return match
 
         best_conf = max(x.get("conf", 0) for x in intents if x.get("name"))
         ties = [i for i in intents if i.get("conf", 0) == best_conf]
 
         if len(ties) > 1:
-            LOG.debug(f"tied intents: {ties}")
-            no_entities = [i for i in intents if not i.get("entities")]
-            entities = [i for i in intents if i.get("entities")]
-            if entities and no_entities:
-                LOG.debug(f"excluding {entities}")
-                ties = no_entities  # prefer more strict regexes
-
-        if len(ties) > 1:
             # TODO - how to untie?
             LOG.info(f"tied intents: {ties}")
 
         match = ties[0]
 
         for entity in set(match['entities'].keys()):
             entities = match['entities'].pop(entity)
```

### Comparing `padacioso-0.2.1a8/padacioso/bracket_expansion.py` & `padacioso-0.2.1a9/padacioso/bracket_expansion.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.1a8/setup.py` & `padacioso-0.2.1a9/setup.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.1a8/test/test_padacioso.py` & `padacioso-0.2.1a9/test/test_padacioso.py`

 * *Files identical despite different names*

