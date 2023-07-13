# Comparing `tmp/pydantic_resolve-1.5.2.tar.gz` & `tmp/pydantic_resolve-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.5.2.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.6.0.tar", max compression
```

## Comparing `pydantic_resolve-1.5.2.tar` & `pydantic_resolve-1.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.5.2/LICENSE
--rw-r--r--   0        0        0      636 2023-07-09 14:14:07.250336 pydantic_resolve-1.5.2/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      228 2023-07-09 02:37:13.250821 pydantic_resolve-1.5.2/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     3500 2023-07-09 14:33:28.855034 pydantic_resolve-1.5.2/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.5.2/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6466 2023-07-09 14:08:38.068320 pydantic_resolve-1.5.2/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     6308 2023-07-09 14:47:21.962032 pydantic_resolve-1.5.2/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-09 14:53:35.697368 pydantic_resolve-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     7472 2023-07-09 04:03:38.318092 pydantic_resolve-1.5.2/README.md
--rw-r--r--   0        0        0     8050 1970-01-01 00:00:00.000000 pydantic_resolve-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.0/LICENSE
+-rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-12 15:10:11.331859 pydantic_resolve-1.6.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2093 2023-07-12 15:11:15.219960 pydantic_resolve-1.6.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     8436 2023-07-13 03:23:57.878973 pydantic_resolve-1.6.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     6475 2023-07-12 15:17:25.868742 pydantic_resolve-1.6.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-13 03:30:22.580634 pydantic_resolve-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10929 2023-07-13 03:29:52.380099 pydantic_resolve-1.6.0/README.md
+-rw-r--r--   0        0        0    11348 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.0/PKG-INFO
```

### Comparing `pydantic_resolve-1.5.2/LICENSE` & `pydantic_resolve-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.5.2/pydantic_resolve/__init__.py` & `pydantic_resolve-1.6.0/pydantic_resolve/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from .core import resolve
 from .exceptions import (
     ResolverTargetAttrNotFound,
     DataloaderDependCantBeResolved,
     LoaderFieldNotProvidedError,
     MissingAnnotationError)
 from .resolver import Resolver, LoaderDepend
 from .util import build_list, build_object, mapper, ensure_subset, update_forward_refs
 
 __all__ = [
-    'resolve',
     'Resolver',
     'LoaderDepend',
     'ResolverTargetAttrNotFound',
     'DataloaderDependCantBeResolved',
     'LoaderFieldNotProvidedError',
     'MissingAnnotationError',
     'build_list',
```

### Comparing `pydantic_resolve-1.5.2/pydantic_resolve/util.py` & `pydantic_resolve-1.6.0/pydantic_resolve/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,26 @@
 
 
 def replace_method(cls: Type, cls_name: str, func_name: str, func: Callable):
     KLS = type(cls_name, (cls,), {func_name: func})
     return KLS
 
 
+def output(kls):
+    """
+    set required as True for all fields, make typescript code gen result friendly to use
+    """
+    if issubclass(kls, BaseModel):
+        for f in kls.__fields__.values():
+            f.required = True
+    else:
+        raise AttributeError(f'target class {kls.__name__} is not BaseModel')
+    return kls
+
+
 def mapper(func_or_class: Union[Callable, Type]):
     """
     execute post-transform function after the value is reolved
     func_or_class:
         is func: run func
         is class: call auto_mapping to have a try
     """
@@ -172,18 +184,14 @@
         _fields = target.__class__.__fields__
         field_type = _fields[field_name].outer_type_
 
         # handle optional logic
         if data is None and _fields[field_name].required == False:
             return data
 
-        # research/2_update_forward_ref.py
-        if getattr(target.__class__, const.PYDANTIC_FORWARD_REF_UPDATED, False):
-            update_forward_refs(target.__class__)
-
     elif is_dataclass(target):
         _fields = target.__dataclass_fields__
         field_type = _fields[field_name].type
 
     # 2. parse
     if field_type:
         result = parse_obj_as(field_type, data)
```

### Comparing `pydantic_resolve-1.5.2/pyproject.toml` & `pydantic_resolve-1.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.5.2"
+version = "1.6.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

