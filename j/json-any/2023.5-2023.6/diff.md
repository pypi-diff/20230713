# Comparing `tmp/json-any-2023.5.tar.gz` & `tmp/json-any-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.5.tar", last modified: Thu Jul 13 13:56:27 2023, max compression
+gzip compressed data, was "json-any-2023.6.tar", last modified: Thu Jul 13 17:07:40 2023, max compression
```

## Comparing `json-any-2023.5.tar` & `json-any-2023.6.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.5/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 13:56:27.843092 json-any-2023.5/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.5/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.5/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.839759 json-any-2023.5/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.5/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.5/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.5/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     4597 2023-07-13 13:50:35.000000 json-any-2023.5/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.5/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any/extension/
--rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.5/json_any/extension/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)     4245 2023-07-13 13:14:00.000000 json-any-2023.5/json_any/extension/type.py
--rw-r--r--   0 eric      (1000) users      (984)    11912 2023-07-13 13:42:10.000000 json-any-2023.5/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)    12700 2023-07-13 13:46:55.000000 json-any-2023.5/json_any/object_to_json.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-13 13:53:47.000000 json-any-2023.5/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      461 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.5/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-13 13:56:27.843092 json-any-2023.5/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5293 2023-07-11 12:01:48.000000 json-any-2023.5/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.6/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 17:07:40.539948 json-any-2023.6/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.6/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.6/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.536614 json-any-2023.6/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.536614 json-any-2023.6/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.6/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.536614 json-any-2023.6/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.6/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.6/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     4964 2023-07-13 14:00:49.000000 json-any-2023.6/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.6/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.6/json_any/extension/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.6/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     3671 2023-07-13 15:38:58.000000 json-any-2023.6/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)    11552 2023-07-13 14:17:27.000000 json-any-2023.6/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    12704 2023-07-13 15:16:14.000000 json-any-2023.6/json_any/object_to_json.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any/task/
+-rw-r--r--   0 eric      (1000) users      (984)     3300 2023-07-13 17:01:02.000000 json-any-2023.6/json_any/task/compression.py
+-rw-r--r--   0 eric      (1000) users      (984)     5049 2023-07-13 16:38:45.000000 json-any-2023.6/json_any/task/storage.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-13 17:05:36.000000 json-any-2023.6/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.6/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-13 17:07:40.539948 json-any-2023.6/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.6/setup.py
```

### Comparing `json-any-2023.5/PKG-INFO` & `json-any-2023.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.5
+Version: 2023.6
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.5/README-LICENCE-utf8.txt` & `json-any-2023.6/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/README.rst` & `json-any-2023.6/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/documentation/wiki/description.asciidoc` & `json-any-2023.6/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/json_any/__init__.py` & `json-any-2023.6/json_any/__init__.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/json_any/catalog/module.py` & `json-any-2023.6/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/json_any/catalog/type.py` & `json-any-2023.6/json_any/catalog/type.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from datetime import time as time_t
 from datetime import timedelta as time_delta_t
 from datetime import timezone as time_zone_t
 from enum import Enum as enum_t
 from io import BytesIO as io_bytes_t
 from pathlib import PurePath as path_t
 from typing import NamedTuple as named_tuple_t
-from typing import Sequence
+from typing import Any, Sequence
 from uuid import UUID as uuid_t
 
 from json_any.catalog.module import grph, nmpy, pnds, pypl, sprs
 from json_any.constant import MODULE_TYPE_SEPARATOR
 
 BUILTIN_BYTES_CONTAINERS = (bytes, bytearray)
 BUILTIN_CONTAINERS = (frozenset, list, set, tuple)
@@ -61,14 +61,27 @@
     """"""
     if name in BUILTIN_BYTES_CONTAINERS_NAMES:
         return BUILTIN_BYTES_CONTAINERS[BUILTIN_BYTES_CONTAINERS_NAMES.index(name)]
     else:
         return BUILTIN_CONTAINERS[BUILTIN_CONTAINERS_NAMES.index(name)]
 
 
+def TypeIsInModule(json_type: str, module: Any, /) -> bool:
+    """"""
+    module_name = module.__name__
+    return json_type.startswith(module_name) and (
+        json_type[module_name.__len__()] in (".", MODULE_TYPE_SEPARATOR)
+    )
+
+
+def TypeNameOf(json_type: str, /) -> str:
+    """"""
+    return json_type[(json_type.rindex(MODULE_TYPE_SEPARATOR) + 1) :]
+
+
 def _AddJsonTypes(types: Sequence[type], /) -> None:
     """"""
     global JSON_TYPE
 
     for type_ in types:
         JSON_TYPE[type_] = f"{type_.__module__}{MODULE_TYPE_SEPARATOR}{type_.__name__}"
```

### Comparing `json-any-2023.5/json_any/constant.py` & `json-any-2023.6/json_any/constant.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/json_any/extension/numpy.py` & `json-any-2023.6/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.5/json_any/extension/type.py` & `json-any-2023.6/json_any/extension/type.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,21 +26,20 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-import importlib as imlb
-import sys as sstm
 from types import GenericAlias
 from typing import Any, Callable, Union, get_origin
 
 from json_any.catalog.type import enum_t
 from json_any.constant import MODULE_TYPE_SEPARATOR
+from json_any.extension.module import ElementInModule
 
 builders_h = dict[str, Callable[[Any], Any]]
 description_h = tuple[str, Any]
 descriptors_h = dict[str, Callable[[Any], Any]]
 
 
 class unfound_t:
@@ -61,34 +60,16 @@
 def TypeFromJsonType(
     json_type: str, /, *, prefix: str = "", should_continue_on_error: bool = False
 ) -> type:
     """"""
     module, type_ = json_type[prefix.__len__() :].split(
         MODULE_TYPE_SEPARATOR, maxsplit=1
     )
-    error = None
-
-    imported = sstm.modules.get(module, None)
-    if imported is None:
-        # Do not put instead of "None" in "get" above since it will then be evaluated
-        # all the time, I suppose.
-        try:
-            imported = imlb.import_module(module)
-        except ModuleNotFoundError:
-            error = f'{module}: Module not found when looking for type "{type_}".'
-
-    if imported is None:
-        output = None
-    else:
-        try:
-            output = getattr(imported, type_)
-        except AttributeError:
-            output = None
-            error = f'{type_}: Type not found in module "{module}".'
 
+    output, error = ElementInModule(type_, module)
     if output is None:
         if should_continue_on_error:
             output = unfound_t
         else:
             raise TypeError(error)
 
     return output
```

### Comparing `json-any-2023.5/json_any/json_to_object.py` & `json-any-2023.6/json_any/json_to_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,29 +38,30 @@
 from json_any.catalog.type import (
     BUILTIN_BYTES_CONTAINERS_NAMES,
     BUILTIN_CONTAINERS_NAMES,
     JSON_TYPE,
     JSON_TYPE_NUMPY_SCALAR,
     JSON_TYPE_PREFIX_PATHLIB,
     ContainerWithName,
+    TypeIsInModule,
+    TypeNameOf,
     date_t,
     date_time_t,
     enum_t,
     io_bytes_t,
     named_tuple_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
 )
 from json_any.constant import (
     CUSTOM_PREFIX,
     DATACLASS_PREFIX,
-    MODULE_TYPE_SEPARATOR,
     NEW_FROM_JSON_DESCRIPTION,
     STANDARD_PREFIX,
     UNHANDLED_PREFIX,
 )
 from json_any.extension.numpy import AsNumpyArray
 from json_any.extension.type import (
     TypeFromJsonType,
@@ -102,22 +103,22 @@
         )
         return None
 
     if builders is None:
         builders = {}
 
     if json_type.startswith(CUSTOM_PREFIX):
-        fully_qualified = json_type[CUSTOM_PREFIX.__len__() :]
-        if fully_qualified in builders:
-            Rebuilt = builders[fully_qualified]
+        qualified_type = json_type[CUSTOM_PREFIX.__len__() :]
+        if qualified_type in builders:
+            Rebuilt = builders[qualified_type]
         elif highest_level_call and ("" in builders):
             Rebuilt = builders[""]
         else:
             output_t = TypeFromJsonType(
-                fully_qualified, should_continue_on_error=should_continue_on_error
+                qualified_type, should_continue_on_error=should_continue_on_error
             )
             Rebuilt = getattr(output_t, NEW_FROM_JSON_DESCRIPTION, None)
         if Rebuilt is None:
             output = None
             print(f"{json_type}: Unfound type or type without builder. Returning None.")
         else:
             output = Rebuilt(
@@ -133,31 +134,31 @@
             prefix=DATACLASS_PREFIX,
             should_continue_on_error=should_continue_on_error,
         )
         if output_t is unfound_t:
             output = None
             print(f"{json_type}: Unfound type. Returning None.")
         else:
-            as_dict = _ObjectFromUnJSONed(
+            unjsoned = _ObjectFromUnJSONed(
                 instance,
                 builders=builders,
                 should_continue_on_error=should_continue_on_error,
             )
 
-            for_init = {}
+            kwargs = {}
             for field in dtcl.fields(output_t):
                 if field.init:
                     # This could be limited to init fields without default values. However, all kind of things can happen in
                     # init or post_init, so hopefully, the choice to ignore default values here works...
                     name = field.name
-                    for_init[name] = as_dict[name]
-            output = output_t(**for_init)
+                    kwargs[name] = unjsoned[name]
+            output = output_t(**kwargs)
             # Despite initial values being passed above, all the fields are reset here to their values at JSONing time,
             # again in case things happen in init or post_init.
-            for key, value in as_dict.items():
+            for key, value in unjsoned.items():
                 setattr(output, key, value)
     elif json_type in BUILTIN_BYTES_CONTAINERS_NAMES:
         output_t = ContainerWithName(json_type)
         output = instance.encode(encoding="iso-8859-1")
         if type(output) is not output_t:
             # In practice, this is only for bytearray since bytes are already bytes.
             output = output_t(output)
@@ -185,21 +186,21 @@
         type_name = TypeNameOf(json_type)
         output_t = getattr(sprs, type_name)
         output = output_t(AsNumpyArray(*instance))
     elif (json_type != JSON_TYPE_NUMPY_SCALAR) and TypeIsInModule(json_type, nmpy):
         output = AsNumpyArray(*instance)
     elif TypeIsInModule(json_type, pnds):
         type_name = TypeNameOf(json_type)
-        as_dict = _ObjectFromUnJSONed(
+        unjsoned = _ObjectFromUnJSONed(
             instance,
             builders=builders,
             should_continue_on_error=should_continue_on_error,
         )
         output_t = getattr(pnds, type_name)
-        output = output_t(as_dict)
+        output = output_t(unjsoned)
     elif json_type == JSON_TYPE_NUMPY_SCALAR:
         dtype, value = instance
         if isinstance(value, list):
             output = nmpy.dtype(dtype).type(complex(*value))
         else:
             output = nmpy.dtype(dtype).type(value)
     elif TypeIsInModule(json_type, pypl):
@@ -220,21 +221,21 @@
             time.second,
             time.microsecond,
             time.tzinfo,
             fold=time.fold,
         )
     elif json_type == JSON_TYPE[time_t]:
         time_zone = _ObjectFromUnJSONed(instance[4])
-        as_dict = dict(
+        kwargs = dict(
             zip(
                 ("hour", "minute", "second", "microsecond", "tzinfo", "fold"),
                 (*instance[:4], time_zone, *instance[5:]),
             )
         )
-        output = time_t(**as_dict)
+        output = time_t(**kwargs)
     elif json_type == JSON_TYPE[time_zone_t]:
         time_delta, name = _ObjectFromUnJSONed(instance)
         output = time_zone_t(time_delta, name=name)
     elif json_type.startswith(JSON_TYPE[enum_t]):
         output_t = TypeFromJsonType(
             json_type,
             prefix=JSON_TYPE[enum_t],
@@ -315,20 +316,7 @@
         grph.set_node_attributes(output, attributes)
     elif json_type.startswith(STANDARD_PREFIX):
         output = instance
     else:
         raise ValueError(f"{json_type}: Invalid JSON type or error while unJSONing.")
 
     return output
-
-
-def TypeIsInModule(json_type: str, module: Any, /) -> bool:
-    """"""
-    module_name = module.__name__
-    return json_type.startswith(module_name) and (
-        json_type[module_name.__len__()] in (".", MODULE_TYPE_SEPARATOR)
-    )
-
-
-def TypeNameOf(json_type: str, /) -> str:
-    """"""
-    return json_type[(json_type.rindex(MODULE_TYPE_SEPARATOR) + 1) :]
```

### Comparing `json-any-2023.5/json_any/object_to_json.py` & `json-any-2023.6/json_any/object_to_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     IsNamedTuple,
     QualifiedType,
     TypeOfInstance,
     description_h,
     descriptors_h,
 )
 
-_HISTORY_INDENTATION = "    "
+_HISTORY_INDENTATION = 4 * " "
 
 
 def JsonStringOf(
     instance: Any, /, *, descriptors: descriptors_h = None
 ) -> tuple[str, Sequence[str] | None]:
     """"""
     history = []
@@ -200,16 +200,16 @@
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif IsNumpyScalar(instance_type):
         json_type = JSON_TYPE_NUMPY_SCALAR
-        representation = AsScalarRepresentation(instance, instance_type)
-        jsonable = (instance.dtype.char, representation)
+        description = AsScalarRepresentation(instance, instance_type)
+        jsonable = (instance.dtype.char, description)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type in MATPLOTLIB_CLASSES:
         fake_file = io_bytes_t()
         instance.canvas.draw()
         instance.savefig(
             fake_file,
             bbox_inches="tight",
@@ -254,18 +254,18 @@
             instance.value,
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
     elif IsNamedTuple(instance):
         json_type = f"{JSON_TYPE[named_tuple_t]}{qualified_type}"
-        as_tuple = tuple(instance)
-        history.append(f"{history_level}{json_type}[{as_tuple.__len__()}]")
+        description = tuple(instance)
+        history.append(f"{history_level}{json_type}[{description.__len__()}]")
         jsonable = _JsonableVersionOf(
-            as_tuple,
+            description,
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
     elif instance_type in BUILTIN_CONTAINERS:
         json_type = instance_type.__name__
         history.append(f"{history_level}{json_type}[{instance.__len__()}]")
```

### Comparing `json-any-2023.5/json_any/version.py` & `json-any-2023.6/json_any/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.5"
+__version__ = "2023.6"
```

### Comparing `json-any-2023.5/json_any.egg-info/PKG-INFO` & `json-any-2023.6/json_any.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.5
+Version: 2023.6
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.5/setup.py` & `json-any-2023.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 PYPI_STATUS = "4 - Beta"
 
 IMPORT_NAME = "json_any"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.catalog",
     f"{IMPORT_NAME}.extension",
+    f"{IMPORT_NAME}.task",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
 )
 ENTRY_POINTS = {
     "console_scripts": [],
 }
```

