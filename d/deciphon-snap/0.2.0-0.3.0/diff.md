# Comparing `tmp/deciphon_snap-0.2.0.tar.gz` & `tmp/deciphon_snap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.2.0.tar", max compression
+gzip compressed data, was "deciphon_snap-0.3.0.tar", max compression
```

## Comparing `deciphon_snap-0.2.0.tar` & `deciphon_snap-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/LICENSE
--rw-r--r--   0        0        0     2453 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/README.md
--rw-r--r--   0        0        0      355 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/amino.py
--rw-r--r--   0        0        0     1564 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2178 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     2680 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/interval.py
--rw-r--r--   0        0        0     2773 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/path_like.py
--rw-r--r--   0        0        0      913 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/prod.py
--rw-r--r--   0        0        0      724 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      347 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2495 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      541 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2453 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/README.md
+-rw-r--r--   0        0        0      355 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     2553 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     2980 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     1346 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      541 2023-07-13 00:23:43.957548 deciphon_snap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.3.0/PKG-INFO
```

### Comparing `deciphon_snap-0.2.0/LICENSE` & `deciphon_snap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/README.md` & `deciphon_snap-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/deciphon_snap/hmmer.py` & `deciphon_snap-0.3.0/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/deciphon_snap/interval.py` & `deciphon_snap-0.3.0/deciphon_snap/interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/deciphon_snap/match.py` & `deciphon_snap-0.3.0/deciphon_snap/match.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from typing import List
-from deciphon_snap.interval import PyInterval
-from deciphon_snap.amino import AminoInterval
 
-from pydantic import BaseModel, RootModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, RootModel
+
+from deciphon_snap.amino import AminoInterval
+from deciphon_snap.interval import PyInterval
 
 __all__ = ["Match", "MatchList", "LazyMatchList", "MatchListInterval"]
 
 
 class Match(BaseModel):
     query: str
     state: str
     codon: str
     amino: str
+    _position: int | None
 
     @classmethod
     def from_string(cls, x: str):
         y = x.split(",", 3)
         return cls(query=y[0], state=y[1], codon=y[2], amino=y[3])
 
+    @property
+    def position(self):
+        assert self._position
+        return self._position
+
+    @position.setter
+    def position(self, x: int):
+        self._position = x
+
     def __str__(self):
         query = self.query if len(self.query) > 0 else "∅"
         state = self.state
         codon = self.codon if len(self.codon) > 0 else "∅"
         amino = self.amino if len(self.amino) > 0 else "∅"
         return f"({query},{state},{codon},{amino})"
```

### Comparing `deciphon_snap-0.2.0/deciphon_snap/prod.py` & `deciphon_snap-0.3.0/deciphon_snap/prod.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pydantic import BaseModel, RootModel
 from typing import List
 
 from deciphon_snap.hmmer import H3Result
 from deciphon_snap.match import LazyMatchList
+from deciphon_snap.query_interval import QueryIntervalBuilder
+from deciphon_snap.hit import HitList
 
 __all__ = ["Prod"]
 
 
 class Prod(BaseModel):
     id: int
     seq_id: int
@@ -15,14 +17,24 @@
     alt: float
     null: float
     evalue: float
     match_list: LazyMatchList
     h3result: H3Result | None = None
 
     @property
+    def hits(self):
+        qibuilder = QueryIntervalBuilder(self.match_list)
+        hits = []
+        for hit in HitList.make(self.match_list):
+            hit.interval = qibuilder.make(hit.match_list_interval)
+            hit.match_list = self.match_list.evaluate()
+            hits.append(hit)
+        return hits
+
+    @property
     def hmmer(self):
         assert self.h3result
         return self.h3result
 
     @property
     def query(self):
         return self.match_list.query
```

### Comparing `deciphon_snap-0.2.0/deciphon_snap/query_interval.py` & `deciphon_snap-0.3.0/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/deciphon_snap/shorten.py` & `deciphon_snap-0.3.0/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/deciphon_snap/snap_file.py` & `deciphon_snap-0.3.0/deciphon_snap/snap_file.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.2.0/pyproject.toml` & `deciphon_snap-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-snap"
-version = "0.2.0"
+version = "0.3.0"
 description = "Reader for Deciphon snap files."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon_snap" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphon_snap-0.2.0/PKG-INFO` & `deciphon_snap-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.2.0
+Version: 0.3.0
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

