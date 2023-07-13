# Comparing `tmp/mongodantic_python-0.2.3.tar.gz` & `tmp/mongodantic_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodantic_python-0.2.3.tar", max compression
+gzip compressed data, was "mongodantic_python-0.3.0.tar", max compression
```

## Comparing `mongodantic_python-0.2.3.tar` & `mongodantic_python-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1506 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     5869 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/README.md
--rw-r--r--   0        0        0      260 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/mongodantic/__init__.py
--rw-r--r--   0        0        0      315 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/mongodantic/conftest.py
--rw-r--r--   0        0        0     4625 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/mongodantic/model.py
--rw-r--r--   0        0        0     2301 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/mongodantic/test_mongodantic.py
--rw-r--r--   0        0        0      848 2023-07-13 14:51:53.156407 mongodantic_python-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6827 1970-01-01 00:00:00.000000 mongodantic_python-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     5869 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/README.md
+-rw-r--r--   0        0        0      260 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/mongodantic/__init__.py
+-rw-r--r--   0        0        0      440 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/mongodantic/conftest.py
+-rw-r--r--   0        0        0     5684 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/mongodantic/model.py
+-rw-r--r--   0        0        0     2308 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/mongodantic/test_mongodantic.py
+-rw-r--r--   0        0        0      847 2023-07-13 16:55:54.697388 mongodantic_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6826 1970-01-01 00:00:00.000000 mongodantic_python-0.3.0/PKG-INFO
```

### Comparing `mongodantic_python-0.2.3/LICENSE.md` & `mongodantic_python-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mongodantic_python-0.2.3/README.md` & `mongodantic_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mongodantic_python-0.2.3/mongodantic/model.py` & `mongodantic_python-0.3.0/mongodantic/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 from abc import ABC
+from datetime import datetime
 from typing import List, Optional, Sequence, Type, TypeVar
 
+import bson
 import motor.motor_asyncio
 import pydantic
 from bson import ObjectId
 from bson.codec_options import CodecOptions
 from pymongo import IndexModel
 
 _DB: motor.motor_asyncio.AsyncIOMotorDatabase
 _ENV: str = "unknown"
 _INIT_MODELS = set()
 
 CODEC_OPTIONS = CodecOptions(tz_aware=True)
 TModel = TypeVar("TModel", bound="Model")
 
+BSON_TYPES = [
+    type(None),
+    bool,
+    int,
+    bson.int64.Int64,
+    float,
+    str,
+    list,
+    dict,
+    datetime,
+    bson.regex.Regex,
+    bson.binary.Binary,
+    bson.objectid.ObjectId,
+    bson.dbref.DBRef,
+    bson.code.Code,
+    bytes,
+]
+
 
 class ModelNotFoundError(Exception):
     pass
 
 
 def set_database(db: motor.motor_asyncio.AsyncIOMotorDatabase, env: str = "unknown"):
     global _DB, _ENV
@@ -30,51 +50,74 @@
         raise Exception(
             "You need to call set_database before attempting to access the database"
         )
 
     if collection_name in _INIT_MODELS:
         return
 
-    indexes = model.__fields__["indexes"].default
+    indexes = model.model_fields["indexes"].default
 
     if _ENV == "unittest":
         # mongomock doesn't support codec_options
         collection = _DB.get_collection(collection_name)
     else:
         collection = _DB.get_collection(collection_name, codec_options=CODEC_OPTIONS)
 
     await collection.create_indexes(indexes)
 
     _INIT_MODELS.add(collection_name)
 
 
 class Model(pydantic.BaseModel, ABC):
+    model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
+
     # https://pymongo.readthedocs.io/en/4.1.1/api/pymongo/operations.html#pymongo.operations.IndexModel
     indexes: Sequence[IndexModel]
     id: Optional[str] = None
 
-    class Config:
-        # IndexModel validation is missing for pydantic so it requires this
-        arbitrary_types_allowed = True
-
     @classmethod
     def get_collection_name(cls) -> str:
         return cls.__name__
 
     @classmethod
     async def make(cls, **data) -> TModel:
         instance = cls(**data)
         await instance.after_load()
         return instance
 
     def get_data(self) -> dict:
-        data = self.dict(by_alias=True)
+        data = self.model_dump(by_alias=True)
         del data["id"]
         del data["indexes"]
 
+        def _convert_map(map):
+            for key in map:
+                item = map[key]
+                t = type(item)
+                if t not in BSON_TYPES:
+                    map[key] = str(item)
+                elif t == list:
+                    map[key] = _convert_list(item)
+                elif t == dict:
+                    map[key] = _convert_map(item)
+            return map
+
+        def _convert_list(items):
+            for idx, item in enumerate(items):
+                t = type(item)
+                if t not in BSON_TYPES:
+                    items[idx] = str(item)
+                elif t == list:
+                    items[idx] = _convert_list(item)
+                elif t == dict:
+                    items[idx] = _convert_map(item)
+            return items
+
+        data = _convert_map(data)
+
         return data
 
     async def reload(self) -> None:
         coll = await self._get_collection()
         doc = await coll.find_one({"_id": ObjectId(self.id)})
         if not doc:
             raise ModelNotFoundError()
```

### Comparing `mongodantic_python-0.2.3/mongodantic/test_mongodantic.py` & `mongodantic_python-0.3.0/mongodantic/test_mongodantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         IndexModel([("last_login", ASCENDING)], expireAfterSeconds=5),
     ]
 
     external_uuid: str
     first_name: str
     last_name: str
     last_login: int
-    new_prop: Optional[str]
+    new_prop: Optional[str] = None
 
     async def after_load(self):
         if not self.new_prop:
             self.new_prop = "new"
 
 
 class GuestbookEntry(BaseModel):
```

### Comparing `mongodantic_python-0.2.3/pyproject.toml` & `mongodantic_python-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "mongodantic-python"
-version = "0.2.3"
+version = "0.3.0"
 description = "Pydantic models for MongoDB"
 authors = ["Janne Enberg <janne.enberg@lietu.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/cocreators-ee/mongodantic/"
 repository = "https://github.com/cocreators-ee/mongodantic/"
 documentation = "https://github.com/cocreators-ee/mongodantic/"
 keywords = ["database", "mongodb", "pymongo", "odm", "async"]
 packages = [
     { include = "mongodantic" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
-pydantic = ">=1.10.4"
+pydantic = ">=2.0.0"
 motor = "^3.1.1"
 pymongo = "^4.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-watch = "^4.2.0"
```

### Comparing `mongodantic_python-0.2.3/PKG-INFO` & `mongodantic_python-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodantic-python
-Version: 0.2.3
+Version: 0.3.0
 Summary: Pydantic models for MongoDB
 Home-page: https://github.com/cocreators-ee/mongodantic/
 License: BSD-3-Clause
 Keywords: database,mongodb,pymongo,odm,async
 Author: Janne Enberg
 Author-email: janne.enberg@lietu.net
 Requires-Python: >=3.7,<4
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: motor (>=3.1.1,<4.0.0)
-Requires-Dist: pydantic (>=1.10.4)
+Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Project-URL: Documentation, https://github.com/cocreators-ee/mongodantic/
 Project-URL: Repository, https://github.com/cocreators-ee/mongodantic/
 Description-Content-Type: text/markdown
 
 # Mongodantic
```

