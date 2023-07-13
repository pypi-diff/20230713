# Comparing `tmp/pydantic_resolve-1.6.0.tar.gz` & `tmp/pydantic_resolve-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.6.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.6.1.tar", max compression
```

## Comparing `pydantic_resolve-1.6.0.tar` & `pydantic_resolve-1.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.0/LICENSE
--rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      275 2023-07-12 15:10:11.331859 pydantic_resolve-1.6.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2093 2023-07-12 15:11:15.219960 pydantic_resolve-1.6.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     8436 2023-07-13 03:23:57.878973 pydantic_resolve-1.6.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     6475 2023-07-12 15:17:25.868742 pydantic_resolve-1.6.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-13 03:30:22.580634 pydantic_resolve-1.6.0/pyproject.toml
--rw-r--r--   0        0        0    10929 2023-07-13 03:29:52.380099 pydantic_resolve-1.6.0/README.md
--rw-r--r--   0        0        0    11348 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.1/LICENSE
+-rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-12 15:10:11.331859 pydantic_resolve-1.6.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2093 2023-07-12 15:11:15.219960 pydantic_resolve-1.6.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     8436 2023-07-13 03:23:57.878973 pydantic_resolve-1.6.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     6625 2023-07-13 04:47:58.873428 pydantic_resolve-1.6.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-13 04:48:18.272045 pydantic_resolve-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0    10929 2023-07-13 03:29:52.380099 pydantic_resolve-1.6.1/README.md
+-rw-r--r--   0        0        0    11348 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.1/PKG-INFO
```

### Comparing `pydantic_resolve-1.6.0/LICENSE` & `pydantic_resolve-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.0/pydantic_resolve/__init__.py` & `pydantic_resolve-1.6.1/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.0/pydantic_resolve/core.py` & `pydantic_resolve-1.6.1/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.0/pydantic_resolve/resolver.py` & `pydantic_resolve-1.6.1/pydantic_resolve/resolver.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.0/pydantic_resolve/util.py` & `pydantic_resolve-1.6.1/pydantic_resolve/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 import types
 import functools
 from collections import defaultdict
 from dataclasses import is_dataclass
 from pydantic import BaseModel, parse_obj_as
 from inspect import iscoroutine
-from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator
-
+from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator, Dict
 import pydantic_resolve.constant as const
 
 
+
 def get_class_field_annotations(cls: Type):
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
 
 
 T = TypeVar("T")
 V = TypeVar("V")
@@ -42,22 +42,28 @@
     return results
 
 
 def replace_method(cls: Type, cls_name: str, func_name: str, func: Callable):
     KLS = type(cls_name, (cls,), {func_name: func})
     return KLS
 
-
 def output(kls):
     """
-    set required as True for all fields, make typescript code gen result friendly to use
+    set required as True for all fields
+    make typescript code gen result friendly to use
     """
+
     if issubclass(kls, BaseModel):
-        for f in kls.__fields__.values():
-            f.required = True
+        fnames = list(kls.__fields__.keys())
+
+        def schema_extra(schema: Dict[str, Any]) -> None:
+            schema['required'] = fnames
+
+        kls.Config.schema_extra = staticmethod(schema_extra)
+
     else:
         raise AttributeError(f'target class {kls.__name__} is not BaseModel')
     return kls
 
 
 def mapper(func_or_class: Union[Callable, Type]):
     """
```

### Comparing `pydantic_resolve-1.6.0/pyproject.toml` & `pydantic_resolve-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.6.0"
+version = "1.6.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.6.0/README.md` & `pydantic_resolve-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.0/PKG-INFO` & `pydantic_resolve-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.6.0
+Version: 1.6.1
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```

