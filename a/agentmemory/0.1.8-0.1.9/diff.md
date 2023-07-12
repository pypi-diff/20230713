# Comparing `tmp/agentmemory-0.1.8.tar.gz` & `tmp/agentmemory-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.1.8.tar", last modified: Fri Jul  7 12:04:56 2023, max compression
+gzip compressed data, was "agentmemory-0.1.9.tar", last modified: Mon Jul 10 23:05:34 2023, max compression
```

## Comparing `agentmemory-0.1.8.tar` & `agentmemory-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:04:56.543482 agentmemory-0.1.8/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.8/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     3102 2023-07-07 12:04:56.543318 agentmemory-0.1.8/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2499 2023-07-07 12:04:09.000000 agentmemory-0.1.8/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:04:56.541899 agentmemory-0.1.8/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)      624 2023-07-07 12:04:52.000000 agentmemory-0.1.8/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.8/agentmemory/memory.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.8/agentmemory/memory_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:04:56.543080 agentmemory-0.1.8/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     3102 2023-07-07 12:04:56.000000 agentmemory-0.1.8/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 12:04:56.000000 agentmemory-0.1.8/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 12:04:56.000000 agentmemory-0.1.8/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 12:04:56.000000 agentmemory-0.1.8/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 12:04:56.000000 agentmemory-0.1.8/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 12:04:56.543539 agentmemory-0.1.8/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-07 12:04:52.000000 agentmemory-0.1.8/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 23:05:34.312327 agentmemory-0.1.9/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.9/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5834 2023-07-10 23:05:34.312152 agentmemory-0.1.9/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5231 2023-07-10 22:49:00.000000 agentmemory-0.1.9/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 23:05:34.310574 agentmemory-0.1.9/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      622 2023-07-10 23:05:30.000000 agentmemory-0.1.9/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    14173 2023-07-10 23:04:22.000000 agentmemory-0.1.9/agentmemory/main.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2367 2023-07-10 23:02:02.000000 agentmemory-0.1.9/agentmemory/test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 23:05:34.311907 agentmemory-0.1.9/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5834 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      264 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 23:05:34.312381 agentmemory-0.1.9/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-10 23:05:30.000000 agentmemory-0.1.9/setup.py
```

### Comparing `agentmemory-0.1.8/LICENSE` & `agentmemory-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.8/agentmemory/__init__.py` & `agentmemory-0.1.9/agentmemory/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 agentmemory
 
 Simple agent memory, powered by chromadb
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/agentmemory and https://www.trychroma.com/"
 
-from .memory import (
+from .main import (
     create_memory,
     get_memories,
     search_memory,
     get_memory,
     update_memory,
     delete_memory,
     count_memories,
```

### Comparing `agentmemory-0.1.8/agentmemory/memory_test.py` & `agentmemory-0.1.9/agentmemory/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from memory import (
+from main import (
     search_memory,
     get_memory,
     create_memory,
     get_memories,
     update_memory,
     delete_memory,
     count_memories,
     wipe_category,
-    wipe_all_memories
+    wipe_all_memories,
+    collection_to_list,
+    list_to_collection,
 )
 
-from memory import client, collection_to_list, list_to_collection
-
-client.reset()
+wipe_all_memories()
 
 # create_memory tests
 create_memory("test", "document 1", metadata={"test": "test"})
 create_memory("test", "document 2", metadata={"test": "test"})
 create_memory("test", "document 3", metadata={"test": "test"})
 create_memory("test", "document 4", metadata={"test": "test"})
 create_memory("test", "document 5", metadata={"test": "test"})
@@ -35,25 +35,25 @@
 collection = client.get_or_create_collection("test")
 test_collection_data = collection.peek()
 list = collection_to_list(test_collection_data)
 
 assert list[0]["document"] == "document 1"
 print("Passed collection_to_list tests")
 
-# # list_to_collection
 new_collection_data = list_to_collection(list)
 
 assert test_collection_data["documents"][0] == "document 1"
 print("Passed list_to_collection tests")
 
-# # assert collection == new_collection
 assert new_collection_data == test_collection_data
 print("Passed equality of collection test")
 
-search_results = search_memory("test", "document 1", n_results=5, filter_metadata=None, contains_text=None)
+search_results = search_memory(
+    "test", "document 1", n_results=5, filter_metadata=None, contains_text=None
+)
 
 assert search_results[0]["document"] == "document 1"
 print("Passed search_memory tests")
 
 num_memories = count_memories("test")
 # test delete_memory
 delete_memory("test", 1)
@@ -73,8 +73,8 @@
 
 update_memory("test", 0, "document 1 updated", metadata={"test": "test"})
 assert get_memory("test", 0)["document"] == "document 1 updated"
 print("Passed update_memory tests")
 
 wipe_all_memories()
 assert count_memories("test") == 0
-print("Passed wipe_all_memories tests")
+print("Passed wipe_all_memories tests")
```

### Comparing `agentmemory-0.1.8/setup.py` & `agentmemory-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.1.8',
+    version='0.1.9',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

