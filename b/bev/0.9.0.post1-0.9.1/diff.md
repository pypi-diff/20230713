# Comparing `tmp/bev-0.9.0.post1.tar.gz` & `tmp/bev-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bev-0.9.0.post1.tar", last modified: Sun Jun 25 21:54:20 2023, max compression
+gzip compressed data, was "bev-0.9.1.tar", last modified: Wed Jul  5 00:36:36 2023, max compression
```

## Comparing `bev-0.9.0.post1.tar` & `bev-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:20.267780 bev-0.9.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-25 21:54:17.000000 bev-0.9.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 21:54:17.000000 bev-0.9.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-25 21:54:20.267780 bev-0.9.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-25 21:54:17.000000 bev-0.9.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:20.259780 bev-0.9.0.post1/bev/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:20.263780 bev-0.9.0.post1/bev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/blame.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:20.263780 bev-0.9.0.post1/bev/config/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/vc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-25 21:54:17.000000 bev-0.9.0.post1/bev/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:54:20.263780 bev-0.9.0.post1/bev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-25 21:54:20.000000 bev-0.9.0.post1/bev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-25 21:54:20.000000 bev-0.9.0.post1/bev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:54:20.000000 bev-0.9.0.post1/bev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 21:54:20.000000 bev-0.9.0.post1/bev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 21:54:20.000000 bev-0.9.0.post1/bev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-25 21:54:20.000000 bev-0.9.0.post1/bev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-25 21:54:17.000000 bev-0.9.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 21:54:17.000000 bev-0.9.0.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:54:20.267780 bev-0.9.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-25 21:54:17.000000 bev-0.9.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:36.070023 bev-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-05 00:36:33.000000 bev-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-05 00:36:33.000000 bev-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-05 00:36:36.070023 bev-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-05 00:36:33.000000 bev-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:36.066022 bev-0.9.1/bev/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 00:36:33.000000 bev-0.9.1/bev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 00:36:33.000000 bev-0.9.1/bev/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:36.066022 bev-0.9.1/bev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/blame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-05 00:36:33.000000 bev-0.9.1/bev/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:36.070023 bev-0.9.1/bev/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-05 00:36:33.000000 bev-0.9.1/bev/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-05 00:36:33.000000 bev-0.9.1/bev/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-05 00:36:33.000000 bev-0.9.1/bev/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 00:36:33.000000 bev-0.9.1/bev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 00:36:33.000000 bev-0.9.1/bev/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-05 00:36:33.000000 bev-0.9.1/bev/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-05 00:36:33.000000 bev-0.9.1/bev/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-05 00:36:33.000000 bev-0.9.1/bev/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:33.000000 bev-0.9.1/bev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-05 00:36:33.000000 bev-0.9.1/bev/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 00:36:33.000000 bev-0.9.1/bev/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-05 00:36:33.000000 bev-0.9.1/bev/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-05 00:36:33.000000 bev-0.9.1/bev/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-05 00:36:33.000000 bev-0.9.1/bev/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:36:36.066022 bev-0.9.1/bev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-05 00:36:36.000000 bev-0.9.1/bev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-05 00:36:36.000000 bev-0.9.1/bev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:36:36.000000 bev-0.9.1/bev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 00:36:36.000000 bev-0.9.1/bev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 00:36:36.000000 bev-0.9.1/bev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-05 00:36:36.000000 bev-0.9.1/bev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-05 00:36:33.000000 bev-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 00:36:33.000000 bev-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:36:36.070023 bev-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-05 00:36:33.000000 bev-0.9.1/setup.py
```

### Comparing `bev-0.9.0.post1/LICENSE` & `bev-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/PKG-INFO` & `bev-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.9.0.post1
+Version: 0.9.1
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.9.0.post1.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.9.1.tar.gz
 Author-email: NeuroML Group <maxs987@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `bev-0.9.0.post1/README.md` & `bev-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/add.py` & `bev-0.9.1/bev/cli/add.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/app.py` & `bev-0.9.1/bev/cli/app.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/blame.py` & `bev-0.9.1/bev/cli/blame.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/fetch.py` & `bev-0.9.1/bev/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/init.py` & `bev-0.9.1/bev/cli/init.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/pull.py` & `bev-0.9.1/bev/cli/pull.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/storage.py` & `bev-0.9.1/bev/cli/storage.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/update.py` & `bev-0.9.1/bev/cli/update.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/cli/utils.py` & `bev-0.9.1/bev/cli/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/config/base.py` & `bev-0.9.1/bev/config/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 import warnings
 from typing import Any, Dict, Optional, Sequence, Union
 
-from pydantic import root_validator, validator
 from tarn.config import HashConfig
 
+from .compat import field_validator, model_validator
 from .hostname import HostName
 from .include import Include
 from .location import LocationConfig, NoExtra, from_special
 
 
 class StorageConfig(NoExtra):
     local: Optional[LocationConfig] = None
     remote: Optional[LocationConfig] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode='before')
     def locations(cls, values):
         assert values, 'at least one entry must be provided'
         if not set(values) <= {'local', 'remote'}:
-            return {'local': values}
-        return values
+            values = {'local': values}
+        return {k: from_special(v) for k, v in values.items()}
 
 
 class CacheConfig(NoExtra):
     index: StorageConfig
     storage: StorageConfig
 
-    @validator('index', 'storage', pre=True)
+    @field_validator('index', 'storage', mode='before')
     def validate_storage(cls, v):
         res = from_special(v, False)
         if res is not None:
             return StorageConfig(local=res)
         return v
 
 
 class StorageCluster(NoExtra):
     name: str
     default: Dict[str, Any] = None
     hostname: Sequence[HostName] = ()
     storage: StorageConfig
     cache: Optional[CacheConfig] = None
 
-    @validator('hostname', pre=True)
+    @field_validator('hostname', mode='before')
     def from_single(cls, v):
         if isinstance(v, (str, dict, HostName)):
             v = v,
         return v
 
-    @validator('storage', pre=True)
+    @field_validator('storage', mode='before')
     def validate_storage(cls, v):
         res = from_special(v, False)
         if res is not None:
             return StorageConfig(local=res)
         return v
 
-    @validator('cache', pre=True)
+    @field_validator('cache', mode='before')
     def validate_cache(cls, v, values):
         if isinstance(v, CacheConfig):
             return v
         if not (isinstance(v, dict) and set(v) <= {'index', 'storage'}):
             v = {'index': v}
 
         if 'storage' not in v:
+            # FIXME
+            if not isinstance(values, dict):
+                values = values.data
             if 'storage' not in values:
                 raise ValueError('No valid `storage` configuration found')
             v = v.copy()
             v['storage'] = values['storage']
 
         return v
 
@@ -73,28 +76,26 @@
     choose: str = None
     fallback: str = None
     order: str = None
     hash: Union[str, HashConfig] = None
     include: Sequence[Include] = ()
     labels: Optional[Sequence[str]] = None
 
-    _override = 'fallback', 'order', 'choose', 'hash'
-
-    @validator('order')
+    @field_validator('order')
     def deprecate_order(cls, v):
         if v is not None:
             warnings.warn('The field "order" is deprecated and has no effect anymore')
 
-    @validator('hash', pre=True)
+    @field_validator('hash', mode='before')
     def normalize_hash(cls, v):
         if isinstance(v, str):
             v = {'name': v}
         return v
 
-    @validator('include', pre=True)
+    @field_validator('include', mode='before')
     def from_single(cls, v):
         if isinstance(v, (dict, Include)):
             v = v,
         return v
 
 
 class RepositoryConfig(NoExtra):
```

### Comparing `bev-0.9.0.post1/bev/config/hostname.py` & `bev-0.9.1/bev/config/hostname.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 import re
 
-from .registry import add_type, find, register
+from .compat import core_schema
+from .registry import RegistryError, add_type, find, register
 
 
 @add_type
 class HostName:
     def __init__(self, value):
         self.value = value
 
     def match(self, name) -> bool:
         raise NotImplementedError
 
     @classmethod
     def __get_validators__(cls):
-        yield cls.validate
+        yield cls._validate
 
     @classmethod
-    def validate(cls, v):
+    def __get_pydantic_core_schema__(cls, _source_type, _handler):
+        return core_schema.no_info_plain_validator_function(cls._validate)
+
+    @classmethod
+    def _validate(cls, v):
         if isinstance(v, HostName):
             return v
         if isinstance(v, str):
             return StrHostName(v)
 
         assert isinstance(v, dict), f'Not a dict: {v}'
         assert len(v) == 1, v
         (k, v), = v.items()
 
-        return find(k, HostName)(v)
+        try:
+            return find(k, HostName)(v)
+        except RegistryError as e:
+            raise ValueError(str(e)) from e
 
 
 @register('str')
 class StrHostName(HostName):
     def match(self, name) -> bool:
         return name == self.value
```

### Comparing `bev-0.9.0.post1/bev/config/include.py` & `bev-0.9.1/bev/config/include.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import importlib
 from pathlib import Path
 from typing import Tuple, Union
 
 from yaml import safe_load
 
-from .registry import add_type, find, register
+from .compat import core_schema
+from .registry import RegistryError, add_type, find, register
 
 
 @add_type
 class Include:
     def __init__(self, value, optional: bool):
         self.value = value
         self.optional = optional
 
     def read(self, parent: Union[Path, None]) -> Tuple[Union[Path, None], Union[dict, None]]:
         raise NotImplementedError
 
     @classmethod
     def __get_validators__(cls):
-        yield cls.validate
+        yield cls._validate
 
     @classmethod
-    def validate(cls, v):
+    def __get_pydantic_core_schema__(cls, _source_type, _handler):
+        return core_schema.no_info_plain_validator_function(cls._validate)
+
+    @classmethod
+    def _validate(cls, v):
         if isinstance(v, Include):
             return v
 
         assert isinstance(v, dict), f'Not a dict: {v}'
         optional = v.pop('optional', False)
         assert len(v) == 1, v
         (k, v), = v.items()
 
-        return find(k, Include)(v, optional)
+        try:
+            return find(k, Include)(v, optional)
+        except RegistryError as e:
+            raise ValueError(str(e)) from e
 
 
 @register('file')
 class FileInclude(Include):
     def __init__(self, value, optional):
         super().__init__(Path(value).expanduser(), optional)
```

### Comparing `bev-0.9.0.post1/bev/config/legacy.py` & `bev-0.9.1/bev/config/legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from pathlib import Path
-from pydantic import ValidationError, root_validator, validator
+
+from jboc import collect
+from pydantic import ValidationError
 from typing import Any, Dict, Optional, Sequence
 
 from .base import StorageConfig
+from .compat import model_validator, field_validator
 from .hostname import HostName
 from .location import LocationConfig, NoExtra
-from .registry import find
+from .registry import RegistryError, find
 
 
 class LegacyLocationConfig(NoExtra):
     root: Path = None
     remote: Sequence[LocationConfig] = ()
     optional: bool = False
 
-    @root_validator(pre=True)
+    @model_validator(mode='before')
     def from_string(cls, v):
         if isinstance(v, str):
             return cls(root=v)
         return v
 
-    @root_validator(pre=True)
+    @model_validator(mode='before')
     def gather_remote(cls, values):
-        values = values.copy()
+        if isinstance(values, StorageLevelConfig):
+            return values
+        values = to_values(values).copy()
         remote = list(values.pop('remote', []))
         for key in list(values):
             if key not in ['root', 'optional']:
                 remote.append({key: values.pop(key)})
 
         values['remote'] = tuple(remote)
         return values
 
-    @validator('remote', pre=True)
+    @field_validator('remote', mode='before')
     def from_single(cls, v):
         if isinstance(v, (str, dict, LocationConfig)):
             v = v,
 
         return list(map(cls.parse_entry, v))
 
     @staticmethod
@@ -44,59 +49,62 @@
 
         assert isinstance(entry, dict), f'Not a dict: {entry}'
         assert len(entry) == 1, entry
         (k, entry), = entry.items()
         if isinstance(entry, LocationConfig):
             return entry
 
-        kls = find(k, LocationConfig)
+        try:
+            kls = find(k, LocationConfig)
+        except RegistryError as e:
+            raise ValueError(str(e)) from e
         if isinstance(entry, str):
             return kls.from_special(entry)
         return kls.parse_obj(entry)
 
 
 class StorageLevelConfig(NoExtra):
     default: Dict[str, Any] = None
     locations: Sequence[LegacyLocationConfig]
     write: bool = True
     replicate: bool = True
     name: Optional[str] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode='before')
     def from_builtins(cls, v):
         if isinstance(v, dict):
             return v
         return cls(locations=v)
 
-    @validator('default', pre=True, always=True)
+    @field_validator('default', mode='before', always=True)
     def fill(cls, v):
         if v is None:
             return {}
         return v
 
-    @validator('locations', pre=True)
-    def from_string(cls, v):
-        if not isinstance(v, (list, tuple)):
-            v = v,
-        return v
-
-    @validator('locations', each_item=True, pre=True)
-    def add_defaults(cls, v, values):
-        default = (values['default'] or {}).copy()
-        if isinstance(v, str):
-            v = {'root': v}
-
-        if default:
-            assert isinstance(v, dict), type(v)
-            default.update(v)
-            return default
+    @field_validator('locations', mode='before')
+    @collect
+    def add_defaults(cls, vs, values):
+        if not isinstance(vs, (list, tuple)):
+            vs = vs,
+        values = to_values(values)
+        for v in vs:
+            default = (values['default'] or {}).copy()
+            if isinstance(v, str):
+                v = {'root': v}
+
+            if default:
+                assert isinstance(v, dict), type(v)
+                default.update(v)
+                yield default
 
-        return v
+            else:
+                yield v
 
-    @validator('locations')
+    @field_validator('locations')
     def to_tuple(cls, v):
         return tuple(v)
 
 
 class LegacyCacheConfig(NoExtra):
     index: Sequence[StorageLevelConfig]
     storage: Sequence[StorageLevelConfig]
@@ -136,32 +144,36 @@
     def new_cache(self):
         if self.cache is not None:
             index = self._new(self.cache.index)
             print(self.cache, self.cache.index, index, self._new(self.cache.storage))
             if index is not None:
                 return {'index': index, 'storage': self._new(self.cache.storage)}
 
-    @validator('hostname', pre=True)
+    @field_validator('hostname', mode='before')
     def from_single(cls, v):
         if isinstance(v, (str, dict, HostName)):
             v = v,
         return v
 
-    @validator('storage', pre=True)
+    @field_validator('storage', mode='before')
     def validate_storage(cls, v, values):
+        values = to_values(values)
         default = (values['default'] or {}).copy()
         return cls._parse_storage_levels(v, default)
 
-    @validator('cache', pre=True)
+    @field_validator('cache', mode='before')
     def validate_cache(cls, v, values):
+        values = to_values(values)
         default = (values['default'] or {}).copy()
 
         if isinstance(v, dict) and 'index' in v:
             v = v.copy()
             default.update(v.pop('default', {}))
+            if 'storage' not in values:
+                raise ValueError('No valid storage config found')
             storage = cls._parse_storage_levels(v.pop('storage', values['storage']), default)
             index = cls._parse_storage_levels(v.pop('index'), default)
             return LegacyCacheConfig(**v, index=index, default=default, storage=storage)
 
         index = cls._parse_storage_levels(v, default)
         if 'storage' not in values:
             raise ValueError('No valid storage config found')
@@ -195,7 +207,11 @@
                     entry = StorageLevelConfig(**local_entry)
                 else:
                     entry = StorageLevelConfig(locations=entry, default=default)
 
             result.append(entry)
 
         return tuple(result)
+
+
+def to_values(x):
+    return x if isinstance(x, dict) else x.data
```

### Comparing `bev-0.9.0.post1/bev/config/location.py` & `bev-0.9.1/bev/config/location.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import warnings
 from pathlib import Path
 from typing import Optional, Sequence
 
 import yaml
+from jboc import collect
 from paramiko.config import SSHConfig
-from pydantic import BaseModel, Extra, validator
 from tarn import SCP, DiskDict, Fanout, Level, Levels, Location, Nginx
 from tarn.config import CONFIG_NAME as STORAGE_CONFIG_NAME, StorageConfig as TarnStorageConfig
 from tarn.utils import mkdir
 
-from .registry import add_type, find, register
-
-
-class NoExtra(BaseModel):
-    class Config:
-        extra = Extra.forbid
+from .compat import field_validator, NoExtra, core_schema, model_validate, model_dump
+from .registry import RegistryError, add_type, find, register
 
 
 @add_type
 class LocationConfig(NoExtra):
     @classmethod
     def __get_validators__(cls):
         yield lambda v: from_special(v)
         yield from super().__get_validators__()
 
     @classmethod
+    def __get_pydantic_core_schema__(cls, _source_type, _handler):
+        return core_schema.no_info_before_validator_function(
+            lambda v: from_special(v) if cls is LocationConfig else v,
+            _handler(_source_type),
+        )
+
+    @classmethod
     def from_special(cls, v):
         """ Parse an object different from a dict """
 
     def build(self) -> Optional[Location]:
         """ Build a live object from its config """
         raise NotImplementedError
 
@@ -51,15 +54,15 @@
 
     def init(self, meta, permissions, group):
         if not self.root.exists():
             mkdir(self.root, permissions, group, parents=True)
             conf_path = self.root / STORAGE_CONFIG_NAME
             if not conf_path.exists():
                 with open(conf_path, 'w') as file:
-                    yaml.safe_dump(TarnStorageConfig(hash=meta.hash).dict(exclude_defaults=True), file)
+                    yaml.safe_dump(model_dump(TarnStorageConfig(hash=meta.hash), exclude_defaults=True), file)
 
 
 @register('fanout')
 class FanoutConfig(LocationConfig):
     locations: Sequence[LocationConfig]
 
     @classmethod
@@ -83,19 +86,23 @@
     replicate: bool = True
 
 
 @register('levels')
 class LevelsConfig(LocationConfig):
     levels: Sequence[LevelConfig]
 
-    @validator('levels', pre=True, each_item=True)
-    def _from_location(cls, v):
-        if (isinstance(v, dict) and set(v) <= {'location', 'write', 'replicate'}) or isinstance(v, LevelConfig):
-            return v
-        return {'location': v}
+    # TODO: https://docs.pydantic.dev/latest/usage/validators/#generic-validated-collections
+    @field_validator('levels', mode='before')
+    @collect
+    def _from_location(cls, vs):
+        for v in vs:
+            if (isinstance(v, dict) and set(v) <= {'location', 'write', 'replicate'}) or isinstance(v, LevelConfig):
+                yield v
+            else:
+                yield {'location': v}
 
     @classmethod
     def from_special(cls, v):
         if isinstance(v, (list, tuple)):
             return cls(levels=v)
 
     def build(self) -> Location:
@@ -163,20 +170,20 @@
     if isinstance(x, (list, tuple)):
         return FanoutConfig(locations=x)
     if isinstance(x, dict) and len(x) == 1:
         (name, args), = x.items()
         if isinstance(name, str):
             try:
                 cls = find(name, LocationConfig)
-            except ValueError:
+            except RegistryError:
                 pass
 
             else:
                 if not isinstance(args, dict):
                     result = cls.from_special(args)
                     if result is None:
                         raise ValueError(f'Unsupported type {type(args).__name__!r}')
                     return result
-                return cls.parse_obj(args)
+                return model_validate(cls, args)
 
     if passthrough:
         return x
```

### Comparing `bev-0.9.0.post1/bev/config/parse.py` & `bev-0.9.1/bev/config/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Callable, NamedTuple, Sequence, Tuple
 
 from jboc import collect
 from pydantic import ValidationError
 from tarn import HashKeyStorage, Location, Writable
 from yaml import safe_load
 
+from .compat import model_validate, model_copy
 from ..exceptions import ConfigError
 from .base import ConfigMeta, RepositoryConfig, StorageCluster
 from .legacy import LegacyStorageCluster
 from .utils import CONFIG, choose_local, default_choose
 
 
 class CacheStorageIndex(NamedTuple):
@@ -88,34 +89,34 @@
         raise ConfigError(f'{name}: The key "name" is not available')
     entry = entry.copy()
     entry['name'] = name
     # TODO: a lot of legacy code that will be removed after a few releases
     try:
         return StorageCluster(**entry)
     except ValidationError as e:
-        exp = e
+        exc = e
     try:
         cluster = LegacyStorageCluster(**entry)
     except ValidationError:
         pass
     else:
         kwargs = dict(name=cluster.name, hostname=cluster.hostname, storage=cluster.new_storage())
         cache = cluster.new_cache()
         if cache is not None:
             kwargs['cache'] = cache
         return StorageCluster(**kwargs)
-    raise exp
+    raise exc
 
 
 def _parse(name, config, root):
     if not isinstance(config, dict):
         raise ConfigError(f'{name}: The config must be a dict')
 
     config = config.copy()
-    meta = ConfigMeta.parse_obj(config.pop('meta', {}))
+    meta = model_validate(ConfigMeta, config.pop('meta', {}))
     # parse own items
     entries = {}
     for name, entry in config.items():
         entries[name] = _parse_entry(name, entry)
 
     # parse parents
     override = {}
@@ -128,27 +129,27 @@
 
         parent_meta, items = _parse(parent.value, parent_config, parent_root)
         common = set(items) & set(entries)
         if common:
             raise ConfigError(f'{name}: Trying to override the names {common} from parent config {parent.value}')
 
         override.update({
-            k: getattr(parent_meta, k) for k in ConfigMeta._override if getattr(meta, k) is None
+            k: getattr(parent_meta, k) for k in ('fallback', 'order', 'choose', 'hash') if getattr(meta, k) is None
         })
         if meta.hash is None:
-            meta = meta.copy(update=dict(hash=parent_meta.hash))
+            meta = model_copy(meta, update=dict(hash=parent_meta.hash))
         elif parent_meta.hash is not None and meta.hash != parent_meta.hash:
             raise ConfigError(
                 f'{name}: The parent config ({parent.value}) has a different hash spec: '
                 f'{meta.hash} vs {parent_meta.hash}'
             )
 
         entries.update(items)
 
-    meta = meta.copy(update=override)
+    meta = model_copy(meta, update=override)
     return meta, entries
 
 
 class GetItemPatch(Writable):
     def __init__(self, location):
         self.location = location
         self.locations = [location]
```

### Comparing `bev-0.9.0.post1/bev/config/registry.py` & `bev-0.9.1/bev/config/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import importlib
 from typing import Optional, Type
 
 _REGISTRY = {}
 
 
+class RegistryError(Exception):
+    pass
+
+
 def register(name, cls: Optional[Type] = None):
     def decorator(kls: Type):
         if not isinstance(kls, type):
             raise TypeError(f'{kls} is not a type')
 
         match = {kind for kind in _REGISTRY if issubclass(kls, kind)}
         if len(match) != 1:
@@ -33,18 +37,18 @@
         module, name = name.rsplit('.', 1)
         module = importlib.import_module(module)
         value = getattr(module, name)
         assert issubclass(value, kind), value
         return value
 
     if kind not in _REGISTRY:
-        raise ValueError(f'{kind} not found')
+        raise RegistryError(f'{kind} not found')
     local = _REGISTRY[kind]
     if name not in local:
-        raise ValueError(f'Invalid key "{name}" for "{kind.__name__}"')
+        raise RegistryError(f'Invalid key "{name}" for "{kind.__name__}"')
 
     return local[name]
 
 
 def add_type(kind):
     _REGISTRY[kind] = {}
     return kind
```

### Comparing `bev-0.9.0.post1/bev/config/utils.py` & `bev-0.9.1/bev/config/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/hash.py` & `bev-0.9.1/bev/hash.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/interface.py` & `bev-0.9.1/bev/interface.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/ops.py` & `bev-0.9.1/bev/ops.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/shortcuts.py` & `bev-0.9.1/bev/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/testing.py` & `bev-0.9.1/bev/testing.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/utils.py` & `bev-0.9.1/bev/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/vc.py` & `bev-0.9.1/bev/vc.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev/wc.py` & `bev-0.9.1/bev/wc.py`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/bev.egg-info/PKG-INFO` & `bev-0.9.1/bev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.9.0.post1
+Version: 0.9.1
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.9.0.post1.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.9.1.tar.gz
 Author-email: NeuroML Group <maxs987@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `bev-0.9.0.post1/bev.egg-info/SOURCES.txt` & `bev-0.9.1/bev.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 bev/cli/init.py
 bev/cli/pull.py
 bev/cli/storage.py
 bev/cli/update.py
 bev/cli/utils.py
 bev/config/__init__.py
 bev/config/base.py
+bev/config/compat.py
 bev/config/hostname.py
 bev/config/include.py
 bev/config/legacy.py
 bev/config/location.py
 bev/config/parse.py
 bev/config/registry.py
 bev/config/remote.py
```

### Comparing `bev-0.9.0.post1/pyproject.toml` & `bev-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bev-0.9.0.post1/setup.py` & `bev-0.9.1/setup.py`

 * *Files identical despite different names*

