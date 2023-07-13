# Comparing `tmp/py-pane-0.2.tar.gz` & `tmp/py-pane-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pane-0.2.tar", last modified: Tue Jul 11 22:56:10 2023, max compression
+gzip compressed data, was "py-pane-0.3.tar", last modified: Thu Jul 13 17:43:39 2023, max compression
```

## Comparing `py-pane-0.2.tar` & `py-pane-0.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.599717 py-pane-0.2/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2023-06-16 22:13:24.000000 py-pane-0.2/LICENSE.txt
--rw-r--r--   0 colin      (501) staff       (20)     4182 2023-07-11 22:56:10.599592 py-pane-0.2/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2186 2023-06-16 22:11:09.000000 py-pane-0.2/README.md
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.598464 py-pane-0.2/pane/
--rw-r--r--   0 colin      (501) staff       (20)    16253 2023-07-08 21:41:28.000000 py-pane-0.2/pane/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)    19184 2023-07-08 20:24:00.000000 py-pane-0.2/pane/convert.py
--rw-r--r--   0 colin      (501) staff       (20)     5260 2023-06-19 17:59:16.000000 py-pane-0.2/pane/field.py
--rw-r--r--   0 colin      (501) staff       (20)     6763 2023-06-08 19:22:13.000000 py-pane-0.2/pane/sketch.py
--rw-r--r--   0 colin      (501) staff       (20)     3583 2023-07-08 17:25:04.000000 py-pane-0.2/pane/test_converter.py
--rw-r--r--   0 colin      (501) staff       (20)     1132 2023-06-16 15:49:27.000000 py-pane-0.2/pane/test_field.py
--rw-r--r--   0 colin      (501) staff       (20)     1587 2023-06-19 15:52:18.000000 py-pane-0.2/pane/test_util.py
--rw-r--r--   0 colin      (501) staff       (20)     4075 2023-07-11 21:59:06.000000 py-pane-0.2/pane/util.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.599201 py-pane-0.2/py_pane.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)     4182 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      344 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)       56 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)        5 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/top_level.txt
--rw-r--r--   0 colin      (501) staff       (20)     1060 2023-07-11 22:49:09.000000 py-pane-0.2/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-11 22:56:10.599753 py-pane-0.2/setup.cfg
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.599313 py-pane-0.2/tests/
--rw-r--r--   0 colin      (501) staff       (20)     6847 2023-07-08 19:58:17.000000 py-pane-0.2/tests/test_pane.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-13 17:43:39.314208 py-pane-0.3/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2023-06-16 22:13:24.000000 py-pane-0.3/LICENSE.txt
+-rw-r--r--   0 colin      (501) staff       (20)     4182 2023-07-13 17:43:39.314088 py-pane-0.3/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2186 2023-06-16 22:11:09.000000 py-pane-0.3/README.md
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-13 17:43:39.313072 py-pane-0.3/pane/
+-rw-r--r--   0 colin      (501) staff       (20)      726 2023-07-12 18:50:48.000000 py-pane-0.3/pane/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)     3895 2023-07-12 18:42:08.000000 py-pane-0.3/pane/annotations.py
+-rw-r--r--   0 colin      (501) staff       (20)    17115 2023-07-12 18:50:55.000000 py-pane-0.3/pane/classes.py
+-rw-r--r--   0 colin      (501) staff       (20)     6771 2023-07-13 17:38:05.000000 py-pane-0.3/pane/convert.py
+-rw-r--r--   0 colin      (501) staff       (20)    17654 2023-07-13 17:38:05.000000 py-pane-0.3/pane/converters.py
+-rw-r--r--   0 colin      (501) staff       (20)     4864 2023-07-13 16:41:32.000000 py-pane-0.3/pane/errors.py
+-rw-r--r--   0 colin      (501) staff       (20)     5357 2023-07-12 04:51:14.000000 py-pane-0.3/pane/field.py
+-rw-r--r--   0 colin      (501) staff       (20)     5701 2023-07-12 18:07:00.000000 py-pane-0.3/pane/test_converter.py
+-rw-r--r--   0 colin      (501) staff       (20)     1135 2023-07-12 04:31:18.000000 py-pane-0.3/pane/test_field.py
+-rw-r--r--   0 colin      (501) staff       (20)     1587 2023-06-19 15:52:18.000000 py-pane-0.3/pane/test_util.py
+-rw-r--r--   0 colin      (501) staff       (20)      708 2023-07-12 18:41:42.000000 py-pane-0.3/pane/types.py
+-rw-r--r--   0 colin      (501) staff       (20)     5307 2023-07-13 17:38:05.000000 py-pane-0.3/pane/util.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-13 17:43:39.313661 py-pane-0.3/py_pane.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)     4182 2023-07-13 17:43:39.000000 py-pane-0.3/py_pane.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      413 2023-07-13 17:43:39.000000 py-pane-0.3/py_pane.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-13 17:43:39.000000 py-pane-0.3/py_pane.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)       56 2023-07-13 17:43:39.000000 py-pane-0.3/py_pane.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)        5 2023-07-13 17:43:39.000000 py-pane-0.3/py_pane.egg-info/top_level.txt
+-rw-r--r--   0 colin      (501) staff       (20)     1681 2023-07-13 17:42:13.000000 py-pane-0.3/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-13 17:43:39.314242 py-pane-0.3/setup.cfg
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-13 17:43:39.313781 py-pane-0.3/tests/
+-rw-r--r--   0 colin      (501) staff       (20)     6821 2023-07-12 04:38:58.000000 py-pane-0.3/tests/test_pane.py
```

### Comparing `py-pane-0.2/LICENSE.txt` & `py-pane-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-pane-0.2/PKG-INFO` & `py-pane-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pane
-Version: 0.2
+Version: 0.3
 Summary: A modern dataclass & data conversion library, focused on speed and expressiveness.
 Author-email: Colin Gilgenbach <hexane@mit.edu>
 License: MIT License
         
         Copyright (c) 2023 Colin Gilgenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `py-pane-0.2/README.md` & `py-pane-0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-pane-0.2/pane/__init__.py` & `py-pane-0.3/pane/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""
+Pane dataclasses.
+"""
+
 from __future__ import annotations
 
-import sys
 from dataclasses import dataclass, KW_ONLY, replace, FrozenInstanceError
 from inspect import Signature, Parameter
 from types import NotImplementedType
 import typing as t
 from typing_extensions import dataclass_transform, Self
 
-from .convert import DataType, IntoData, FromData, from_data, into_data, convert
-from .convert import Converter, make_converter, ConvertError
-from .convert import ParseInterrupt, WrongTypeError, ProductErrorNode, DuplicateKeyError
+from .convert import DataType, FromData, from_data, into_data, convert
+from .converters import Converter, make_converter
+from .errors import ParseInterrupt, ErrorNode, WrongTypeError, ProductErrorNode, DuplicateKeyError
 from .field import Field, FieldSpec, field, RenameStyle, _MISSING
 from .util import FileOrPath, open_file, get_type_hints, list_phrase
 
 
 ClassLayout = t.Literal['tuple', 'struct']
 T = t.TypeVar('T')
 
@@ -37,15 +40,15 @@
     kw_only: bool = False
     out_format: ClassLayout = 'struct'
     in_format: t.Sequence[ClassLayout] = ('struct',)
     in_rename: t.Optional[t.Sequence[RenameStyle]] = None
     out_rename: t.Optional[RenameStyle] = None
     allow_extra: bool = False
 
-    def replace(self, **changes):
+    def replace(self, **changes: t.Any):
         changes['name'] = changes.get('name', None)
         return replace(self, **{k: v for (k, v) in changes.items() if v is not None})
 
 
 @dataclass_transform(
     eq_default=True,
     order_default=True,
@@ -57,28 +60,28 @@
     __pane_opts__: PaneOptions
     __pane_fields__: t.Sequence[Field]
     __pane_specs__: t.Dict[str, FieldSpec]
     __pane_set__: t.Set[str]
 
     def __init_subclass__(
         cls,
-        *args,
+        *args: t.Any,
         name: t.Optional[str] = None,
         ser_format: t.Optional[ClassLayout] = None,
         de_format: t.Optional[t.Sequence[ClassLayout]] = None,
         eq: t.Optional[bool] = None,
         order: t.Optional[bool] = None,
         frozen: t.Optional[bool] = None,
         init: t.Optional[bool] = None,
         kw_only: t.Optional[bool] = None,
         rename: t.Optional[RenameStyle] = None,
         in_rename: t.Optional[t.Union[RenameStyle, t.Sequence[RenameStyle]]] = None,
         out_rename: t.Optional[RenameStyle] = None,
         allow_extra: t.Optional[bool] = None,
-        **kwargs,
+        **kwargs: t.Any,
     ):
         old_params = getattr(cls, '__parameters__', ())
         super().__init_subclass__(*args, **kwargs)
         setattr(cls, '__parameters__', old_params + getattr(cls, '__parameters__', ()))
 
         if rename is not None:
             if in_rename is not None or out_rename is not None:
@@ -95,28 +98,29 @@
             eq=eq, order=order, frozen=frozen, init=init, allow_extra=allow_extra,
             kw_only=kw_only, in_rename=in_rename, out_rename=out_rename,
         )
         setattr(cls, PANE_OPTS, opts)
 
         _process(cls, opts)
 
-    def __class_getitem__(cls, params):
+    def __class_getitem__(cls, params: t.Union[type, t.Tuple[type, ...]]):
         typevars = getattr(cls, '__parameters__', ())
         if not isinstance(params, tuple):
             params = (params,)
 
         if not hasattr(super(), '__class_getitem__'):
             raise TypeError(f"type '{cls}' is not subscriptable")
 
-        alias = super().__class_getitem__(params)  # type: ignore
+        alias: t.Type[PaneBase] = super().__class_getitem__(params)  # type: ignore
 
         # return subclass with bound type variables
         bound_vars = dict(zip(typevars, params))
         bound = type(cls.__name__, (cls,), {
-            PANE_BOUNDVARS: bound_vars, '__parameters__': alias.__parameters__,
+            PANE_BOUNDVARS: bound_vars,
+            '__parameters__': getattr(alias, '__parameters__'),  # type: ignore
         })
         return bound
 
     def __repr__(self) -> str:
         inside = ", ".join(f"{field.name}={getattr(self, field.name)!r}" for field in self.__pane_fields__)
         return f"{self.__class__.__name__}({inside})"
 
@@ -124,15 +128,15 @@
         opts: PaneOptions = getattr(self, PANE_OPTS)
         if opts.frozen:
             raise FrozenInstanceError(f"cannot assign to field {name!r}")
         super().__setattr__(name, value)
         set_fields: t.Set[str] = getattr(self, PANE_SET_FIELDS)
         set_fields.add(name)
 
-    def __delattr__(self, name: str, value: t.Any) -> None:
+    def __delattr__(self, name: str) -> None:
         raise AttributeError(f"cannot delete field {name!r}")
 
     @classmethod
     def _converter(cls: t.Type[T], *args: t.Type[FromData],
                    annotations: t.Optional[t.Tuple[t.Any, ...]] = None) -> Converter[T]:
         return t.cast(Converter[T], PaneConverter(cls, annotations))
 
@@ -174,130 +178,130 @@
             from yaml import Loader
 
         with open_file(f) as f:
             obj = yaml.load(f, Loader)
         return cls.from_data(obj)
 
     @classmethod
-    def make_unchecked(cls, *args, **kwargs) -> Self:
+    def make_unchecked(cls, *args: t.Any, **kwargs: t.Any) -> Self:
         ...
 
 
-def _make_init(cls, fields: t.Sequence[Field]):
-    params = []
+def _make_init(cls: t.Type[PaneBase], fields: t.Sequence[Field]):
+    params: t.List[Parameter] = []
     for field in fields:
         if field.default is not _MISSING:
             default = field.default
         elif field.default_factory is not None:
             default = field.default_factory()
         else:
             default = Parameter.empty
         kind = Parameter.KEYWORD_ONLY if field.kw_only else Parameter.POSITIONAL_OR_KEYWORD
         annotation = field.type if field.type is not _MISSING else Parameter.empty
         params.append(Parameter(field.name, kind, default=default, annotation=annotation))
 
     sig = Signature(params, return_annotation=None)
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self: PaneBase, *args: t.Any, **kwargs: t.Any):
         checked = kwargs.pop('_pane_checked', True)
         try:
-            args = sig.bind(*args, **kwargs).arguments
+            bound_args = sig.bind(*args, **kwargs).arguments
         except TypeError as e:
             raise TypeError(*e.args) from None
 
-        set_fields = set()
+        set_fields: t.Set[str] = set()
 
         for field in t.cast(t.Sequence[Field], getattr(self, PANE_FIELDS)):
-            if field.name in args:
-                val = args[field.name]
+            if field.name in bound_args:
+                val = bound_args[field.name]
                 if checked:
                     val = convert(val, field.type)  # type: ignore
                 set_fields.add(field.name)
             elif field.default is not _MISSING:
                 val = field.default
             elif field.default_factory is not None:
                 val = field.default_factory()
             else:
-                raise RuntimeError()
+                raise RuntimeError("Mismatch between fields and signature. This shouldn't happen")
             object.__setattr__(self, field.name, val)
 
         object.__setattr__(self, PANE_SET_FIELDS, set_fields)
 
         if hasattr(self, POST_INIT):
             getattr(self, POST_INIT)()
 
-    __init__.__signature__ = sig
+    setattr(__init__, '__signature__', sig)
     setattr(cls, '__init__', __init__)
     setattr(cls, '__signature__', sig)
 
     @classmethod
-    def make_unchecked(cls, *args, **kwargs):
-        return cls(*args, **kwargs, _pane_checked=False)
+    def make_unchecked(cls, *args, **kwargs):  # type: ignore
+        return cls(*args, **kwargs, _pane_checked=False)  # type: ignore
 
     sig2 = Signature([Parameter('cls', Parameter.POSITIONAL_OR_KEYWORD), *params], return_annotation=cls)
-    make_unchecked.__func__.__signature__ = sig2
+    make_unchecked.__func__.__signature__ = sig2  # type: ignore
     setattr(cls, 'make_unchecked', make_unchecked)
 
 
-def _make_eq(cls, fields: t.Sequence[Field]):
+def _make_eq(cls: t.Type[PaneBase], fields: t.Sequence[Field]):
     #eq_fields = list(filter(lambda f: f.eq, fields))
-    def __eq__(self, other: t.Any) -> bool:
+    def __eq__(self: PaneBase, other: t.Any) -> bool:
         if self.__class__ != other.__class__:
             return False
         return all(
             getattr(self, field.name) == getattr(other, field.name)
             for field in fields
         )
 
     setattr(cls, '__eq__', __eq__)
 
 
-def _make_ord(cls, fields: t.Sequence[Field]):
+def _make_ord(cls: t.Type[PaneBase], fields: t.Sequence[Field]):
     #ord_fields = list(filter(lambda f: f.ord, fields))
-    def _pane_ord(self, other: t.Any) -> t.Union[NotImplementedType, t.Literal[-1, 0, 1]]:
+    def _pane_ord(self: PaneBase, other: t.Any) -> t.Union[NotImplementedType, t.Literal[-1, 0, 1]]:
         if self.__class__ != other.__class__:
             return NotImplemented
         for field in fields:
             if getattr(self, field.name) == getattr(other, field.name):
                 continue
             return 1 if getattr(self, field.name) > getattr(other, field.name) else -1
         return 0
 
-    def __lt__(self, other: t.Any):
-        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else o < 0
+    def __lt__(self: PaneBase, other: t.Any) -> t.Union[bool, NotImplementedType]:
+        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else t.cast(int, o) < 0
 
-    def __le__(self, other: t.Any):
-        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else o <= 0
+    def __le__(self: PaneBase, other: t.Any) -> t.Union[bool, NotImplementedType]:
+        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else t.cast(int, o) <= 0
 
-    def __gt__(self, other: t.Any):
-        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else o > 0
+    def __gt__(self: PaneBase, other: t.Any) -> t.Union[bool, NotImplementedType]:
+        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else t.cast(int, o) > 0
 
-    def __ge__(self, other: t.Any):
-        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else o >= 0
+    def __ge__(self: PaneBase, other: t.Any) -> t.Union[bool, NotImplementedType]:
+        return NotImplemented if (o := _pane_ord(self, other)) is NotImplemented else t.cast(int, o) >= 0
 
     setattr(cls, '_pane_ord', _pane_ord)
     setattr(cls, '__lt__', __lt__)
     setattr(cls, '__le__', __le__)
     setattr(cls, '__gt__', __gt__)
     setattr(cls, '__ge__', __ge__)
 
 
-def _process(cls, opts: PaneOptions):
+def _process(cls: t.Type[PaneBase], opts: PaneOptions):
     fields: t.List[Field] = []
 
     specs: t.Dict[str, FieldSpec] = {}
 
     # collect FieldSpecs from base classes
     for base in reversed(cls.__mro__[1:]):
         if not hasattr(base, PANE_SPECS):
             continue  # not a pane dataclass
         cls_specs = getattr(base, PANE_SPECS)
 
         # apply typevar replacements
-        bound_vars = getattr(base, PANE_BOUNDVARS, {})
+        bound_vars = t.cast(t.Mapping[t.Union[t.TypeVar, t.ParamSpec], type], getattr(base, PANE_BOUNDVARS, {}))
         specs.update(cls_specs)
         specs = {k: spec.replace_typevars(bound_vars) for (k, spec) in specs.items()}
 
     annotations = get_type_hints(cls)
     kw_only = opts.kw_only  # current kw_only state
     cls_specs = {}
 
@@ -357,15 +361,15 @@
 class PaneConverter(Converter[PaneBase]):
     def __init__(self, cls: t.Type[PaneBase],
                  annotations: t.Optional[t.Tuple[t.Any, ...]] = None):
         self.cls = cls
         self.name = self.cls.__name__
         self.opts: PaneOptions = getattr(self.cls, PANE_OPTS)
         self.fields: t.Sequence[Field] = getattr(self.cls, PANE_FIELDS)
-        self.field_converters: t.Sequence[Converter] = [make_converter(field.type) for field in self.fields]
+        self.field_converters: t.Sequence[Converter[t.Any]] = [make_converter(field.type) for field in self.fields]
         self.field_map: t.Dict[str, int] = {}
 
         for (i, field) in enumerate(self.fields):
             self.field_map[field.name] = i
             for alias in field.in_names:
                 self.field_map[alias] = i
 
@@ -379,15 +383,15 @@
             raise NotImplementedError()
 
         elif isinstance(val, (dict, t.Mapping)):
             if 'struct' not in self.opts.in_format:
                 raise ParseInterrupt()
 
             values: t.Dict[str, t.Any] = {}
-            for (k, v) in val.items():
+            for (k, v) in t.cast(t.Dict[str, t.Any], val).items():
                 if k not in self.field_map:
                     if not self.opts.allow_extra:
                         raise ParseInterrupt()  # extra key
                     continue
                 field = self.fields[self.field_map[k]]
                 conv = self.field_converters[self.field_map[k]]
 
@@ -401,24 +405,26 @@
 
             return self.cls.make_unchecked(**values)
 
         raise ParseInterrupt()
 
     def collect_errors(self, val: t.Any) -> t.Union[WrongTypeError, ProductErrorNode, None]:
         if isinstance(val, (list, tuple, t.Sequence)):
+            val = t.cast(t.Sequence[t.Any], val)
             if 'tuple' not in self.opts.in_format:
                 return WrongTypeError(f'struct {self.name}', val)
             return WrongTypeError(f'tuple {self.name}', "Not implemented")
         elif isinstance(val, (dict, t.Mapping)):
+            val = t.cast(t.Mapping[str, t.Any], val)
             if 'struct' not in self.opts.out_format:
                 return WrongTypeError(f'tuple {self.name}', val)
 
-            children = {}
-            extra = set()
-            seen = set()
+            children: t.Dict[t.Union[str, int], ErrorNode] = {}
+            extra: t.Set[str] = set()
+            seen: t.Set[str] = set()
             for (k, v) in val.items():
                 if k not in self.field_map:
                     if not self.opts.allow_extra:
                         extra.add(k)  # unknown key
                     continue
 
                 field = self.fields[self.field_map[k]]
@@ -427,22 +433,21 @@
                     children[k] = DuplicateKeyError(k, field.in_names)
                     continue
                 seen.add(field.name)
 
                 if (node := conv.collect_errors(v)) is not None:
                     children[k] = node
 
-            missing = set()
+            missing: t.Set[str] = set()
             for field in self.fields:
                 if field.name not in seen and not field.is_optional():
                     missing.add(field.name)
 
             if len(missing) or len(children) or len(extra):
                 return ProductErrorNode(self.name, children, val, missing, extra)
             return None
         return WrongTypeError(self.name, val)
 
 
-__ALL__ = [
-    DataType, IntoData, FromData, from_data, into_data, convert,
-    Field, PaneOptions, PaneBase, ConvertError
+__all__ = [
+    'PaneBase', 'PaneOptions', 'field', 'Field', 'KW_ONLY',
 ]
```

### Comparing `py-pane-0.2/pane/convert.py` & `py-pane-0.3/pane/converters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,444 +1,438 @@
-from __future__ import annotations
+"""
+Converter types, which do the hard work of recursive validation.
+"""
 
 import abc
-import sys
-from io import StringIO
-import warnings
-import traceback
 import dataclasses
+import traceback
 from itertools import chain
 import typing as t
 
-from .util import list_phrase
-
-
-@t.runtime_checkable
-class HasFromData(t.Protocol):
-    @classmethod
-    def _converter(cls: t.Type[HasFromDataT], *args: t.Type[FromData],
-                   annotations: t.Optional[t.Tuple[t.Any, ...]] = None) -> Converter[HasFromDataT]:
-        ...
+from pane.errors import ErrorNode
 
+from .convert import FromData, IntoConverter, make_converter
+from .util import list_phrase, pluralize
+from .errors import ConvertError, ParseInterrupt, WrongTypeError, ConditionFailedError
+from .errors import ErrorNode, SumErrorNode, ProductErrorNode
 
-@t.runtime_checkable
-class HasIntoData(t.Protocol):
-    def into_data(self) -> DataType:
-        ...
 
-
-DataType = t.Union[str, int, bool, float, complex, None, t.Mapping, t.Sequence]
-FromData = t.Union[DataType, HasFromData]
-IntoData = t.Union[DataType, HasIntoData]
-
-HasFromDataT = t.TypeVar('HasFromDataT', bound=HasFromData)
 T_co = t.TypeVar('T_co', covariant=True)
-TupleT = t.TypeVar('TupleT', bound=tuple)
-T = t.TypeVar('T', bound=FromData)
+T = t.TypeVar('T')
 U = t.TypeVar('U', bound=FromData)
-K = t.TypeVar('K', bound=FromData)
-V = t.TypeVar('V', bound=FromData)
-
-DataTypes = (str, int, bool, float, complex, type(None), t.Mapping, t.Sequence)
-
-
-class ParseInterrupt(Exception):
-    ...
-
-
-class ConvertError(Exception):
-    def __init__(self, tree: ErrorNode):
-        self.tree: ErrorNode = tree
-
-    def __repr__(self) -> str:
-        return f"ConvertError({self.tree!r})"
-
-    def __str__(self) -> str:
-        return str(self.tree)
-
-
-class ErrorNode(abc.ABC):
-    @abc.abstractmethod
-    def print_error(self, indent="", inside_sum=False, file=sys.stdout):
-        ...
-
-    def __str__(self) -> str:
-        buf = StringIO()
-        self.print_error(file=buf)
-        return buf.getvalue().rstrip('\n')
-
-
-@dataclasses.dataclass
-class WrongTypeError(ErrorNode):
-    expected: str
-    actual: t.Any
-    cause: t.Optional[traceback.TracebackException] = None
-
-    def print_error(self, indent="", inside_sum=False, file=sys.stdout):
-        if inside_sum:
-            print(f"{self.expected}", file=file)
-        else:
-            print(f"Expected {self.expected}, instead got `{self.actual}` of type `{type(self.actual).__name__}`", file=file)
-        if self.cause is not None:
-            s = f"{indent}\n".join(self.cause.format())
-            print(f"Caused by exception:\n{indent}{s}", file=file)
-
-
-@dataclasses.dataclass
-class DuplicateKeyError(ErrorNode):
-    key: str
-    aliases: t.Sequence[str]
-
-    def print_error(self, indent="", inside_sum=False, file=sys.stdout):
-        assert not inside_sum
-        print(f"Duplicate key {self.key} (same as {'/'.join(self.aliases)})", file=file)
-
-
-@dataclasses.dataclass
-class ProductErrorNode(ErrorNode):
-    expected: str
-    children: t.Dict[t.Union[int, str], ErrorNode]
-    actual: t.Any
-    missing: t.AbstractSet[t.Union[t.Sequence[str], str]] = dataclasses.field(default_factory=set)
-    extra: t.AbstractSet[str] = dataclasses.field(default_factory=set)
-
-    def print_error(self, indent="", inside_sum=False, file=sys.stdout):
-        # fuse together non-branching productnodes
-        while len(self.children) == 1 and not len(self.missing) and not len(self.extra):
-            field, child = next(iter(self.children.items()))
-            if not isinstance(child, ProductErrorNode):
-                break
-            children: t.Dict[t.Union[str, int], ErrorNode] = {f"{field}.{k}": v for (k, v) in child.children.items()}
-            missing = set(f"{field}.{f}" for f in child.missing)
-            extra = set(f"{field}.{f}" for f in child.extra)
-            self = ProductErrorNode(self.expected, children, self.actual, missing, extra)
-
-        print(f"{'' if inside_sum else 'Expected '}{self.expected}", file=file)
-        for (field, child) in self.children.items():
-            print(f"{indent}While parsing field '{field}':\n{indent}  ", end="", file=file)
-            child.print_error(f"{indent}  ", file=file)
-
-        for field in self.missing:
-            if not isinstance(field, str):
-                field = '/'.join(field)
-            print(f"{indent}  Missing required field '{field}'", file=file)
-
-        for field in self.extra:
-            print(f"{indent}  Unexpected field '{field}'", file=file)
-
-
-@dataclasses.dataclass
-class SumErrorNode(ErrorNode):
-    # sumnodes shouldn't contain sumnodes
-    children: t.List[t.Union[ProductErrorNode, WrongTypeError]]
-
-    def print_error(self, indent="", inside_sum=False, file=sys.stdout):
-        print(f"Expected one of:", file=file)
-        assert len(self.children)
-        actual = None
-        for child in self.children:
-            print(f"{indent}- ", end="", file=file)
-            child.print_error(f"{indent}  ", inside_sum=True, file=file)
-            actual = child.actual
-        print(f"{indent}Instead got `{actual}` of type `{type(actual).__name__}`", file=file)
+FromDataT = t.TypeVar('FromDataT', bound=FromData)
+FromDataK = t.TypeVar('FromDataK', bound=FromData)
+FromDataV = t.TypeVar('FromDataV', bound=FromData)
 
 
 class Converter(abc.ABC, t.Generic[T_co]):
+    """
+    Base class for a converter to a given type ``T_co``.
+    """
+
     def convert(self, val: t.Any) -> T_co:
+        """Convert ``val`` to ``T_co``. Raises a ``ConvertError`` on failure."""
         try:
             return self.try_convert(val)
         except ParseInterrupt:
             pass
         node = self.collect_errors(val)
         if node is None:
             raise RuntimeError("convert() raised but ``collect_errors`` returned ``None``."
                                " This is a bug of the ``Converter`` implementation.")
         raise ConvertError(node)
 
     @abc.abstractmethod
     def expected(self, plural: bool = False) -> str:
+        """Return a descriptive string indicating the value(s) expected."""
         ...
 
     @abc.abstractmethod
     def try_convert(self, val: t.Any) -> T_co:
         """
         Attempt to convert ``val`` to ``T``.
-        Should raise ``ParseInterrupt`` when
-        a given parsing path reaches a dead end.
+        Should raise ``ParseInterrupt`` (and only ``ParseInterrupt``)
+        when a given parsing path reaches a dead end.
         """
         ...
 
     @abc.abstractmethod
     def collect_errors(self, val: t.Any) -> t.Optional[ErrorNode]:
         """
         Return an error tree caused by converting ``val`` to ``T``.
         ``collect_errors`` should return ``None`` iff ``convert`` doesn't raise.
         """
         ...
 
 
 @dataclasses.dataclass
 class AnyConverter(Converter[t.Any]):
+    """Converter for ``t.Any``."""
     def try_convert(self, val: t.Any) -> t.Any:
         return val
 
     def expected(self, plural: bool = False) -> str:
-        return "any value" + ("s" if plural else "")
+        return pluralize("any value", plural)
 
     def collect_errors(self, val: t.Any) -> None:
         return None
 
 
 @dataclasses.dataclass
 class ScalarConverter(Converter[T]):
+    """
+    Converter for a simple scalar type,
+    constructible from a list of allowed types.
+    """
+
     ty: t.Type[T]
+    """Type to convert into."""
     allowed: t.Union[type, t.Tuple[type, ...]]
+    """Type or list of allowed types."""
     expect: t.Optional[str] = None
+    """Singular form of expected value."""
     expect_plural: t.Optional[str] = None
+    """Plural form of expected value."""
 
     def __post_init__(self):
         self.expect = self.expect or self.ty.__name__
         self.expect_plural = self.expect_plural or self.expect
 
     def expected(self, plural: bool = False) -> str:
         return t.cast(str, self.expect_plural if plural else self.expect)
 
-    def try_convert(self, val) -> T:
+    def try_convert(self, val: t.Any) -> T:
         if isinstance(val, self.allowed):
             return self.ty(val)  # type: ignore
         raise ParseInterrupt()
 
-    def collect_errors(self, actual) -> t.Optional[WrongTypeError]:
-        if isinstance(actual, self.allowed):
+    def collect_errors(self, val: t.Any) -> t.Optional[WrongTypeError]:
+        if isinstance(val, self.allowed):
             return None
-        return WrongTypeError(f'{self.expected()}', actual)
+        return WrongTypeError(f'{self.expected()}', val)
 
 
 @dataclasses.dataclass
 class NoneConverter(Converter[None]):
+    """
+    Converter which accepts only ``None``.
+    """
+
     def try_convert(self, val: t.Any) -> None:
         if val is None:
             return val
         raise ParseInterrupt()
 
     def expected(self, plural: bool = False) -> str:
-        return "null value" + ("s" if plural else "")
+        return pluralize("null value", plural)
 
-    def collect_errors(self, val) -> t.Optional[WrongTypeError]:
+    def collect_errors(self, val: t.Any) -> t.Optional[WrongTypeError]:
         if val is None:
             return None
         return WrongTypeError(self.expected(), val)
 
 
 @dataclasses.dataclass
-class LiteralConverter(Converter):
-    vals: t.Sequence[t.Any]
+class LiteralConverter(Converter[T_co]):
+    """
+    Converter which accepts any of a list of literal values.
+    """
 
-    def try_convert(self, val: t.Any) -> t.Any:
+    vals: t.Sequence[T_co]
+
+    def try_convert(self, val: t.Any) -> T_co:
         if val in self.vals:
             return val
         raise ParseInterrupt()
 
     def expected(self, plural: bool = False) -> str:
         l = list_phrase(tuple(map(repr, self.vals)))
         return f"({l})" if plural else l
 
-    def collect_errors(self, val) -> t.Optional[WrongTypeError]:
+    def collect_errors(self, val: t.Any) -> t.Optional[WrongTypeError]:
         if val in self.vals:
             return None
         return WrongTypeError(self.expected(), val)
 
 
 @dataclasses.dataclass(init=False)
 class UnionConverter(Converter[t.Any]):
-    types: t.Tuple[t.Any, ...]
-    converters: t.Tuple[Converter, ...]
+    """
+    Converter which accepts one of a union of subtypes.
+    Unions are always evaluated left-to-right.
+    """
+    types: t.Tuple[IntoConverter, ...]
+    """List of potential types"""
+    converters: t.Tuple[Converter[t.Any], ...]
+    """List of type converters"""
 
     def __init__(self, types: t.Sequence[t.Any]):
         def _flatten_unions(ty: t.Any) -> t.Sequence[t.Any]:
             if t.get_origin(ty) is t.Union:
                 return t.get_args(ty)
             return (ty,)
 
         types = tuple(chain.from_iterable(map(_flatten_unions, types)))
         self.types = types
         self.converters = tuple(map(make_converter, types))
 
     def expected(self, plural: bool = False) -> str:
         return list_phrase(tuple(conv.expected(plural) for conv in self.converters))
 
-    def try_convert(self, val) -> t.Any:
+    def try_convert(self, val: t.Any) -> t.Any:
         for conv in self.converters:
             try:
                 return conv.try_convert(val)
             except ParseInterrupt:
                 pass
         raise ParseInterrupt
 
-    def collect_errors(self, actual) -> t.Optional[SumErrorNode]:
-        failed_children = []
-        for (ty, conv) in zip(self.types, self.converters):
-            node = conv.collect_errors(actual)
+    def collect_errors(self, val: t.Any) -> t.Optional[SumErrorNode]:
+        failed_children: t.List[t.Union[ProductErrorNode, WrongTypeError]] = []
+        for (_, conv) in zip(self.types, self.converters):
+            node = conv.collect_errors(val)
             # if one branch is successful, the whole type is successful
             if node is None:
                 return None
-            failed_children.append(node)
+            failed_children.append(t.cast(t.Union[ProductErrorNode, WrongTypeError], node))
         return SumErrorNode(failed_children)
 
 
 @dataclasses.dataclass
 class StructConverter(Converter[T]):
+    """
+    Converter for a simple, hetereogeneous struct-like type, constructible from a dict.
+    """
+
     ty: t.Type[T]
-    fields: t.Dict[str, t.Any]
+    """Type to convert into. Must be constructible from a dict/mapping."""
+    fields: t.Mapping[str, IntoConverter]
+    """List of fields and their types"""
     name: t.Optional[str] = None
+    """Optional name of struct"""
     opt_fields: t.Set[str] = dataclasses.field(default_factory=set, kw_only=True)
-    field_converters: t.Dict[str, Converter] = dataclasses.field(init=False)
+    """Set of fields which are optional"""
+    field_converters: t.Dict[str, Converter[t.Any]] = dataclasses.field(init=False)
+    """Dict of sub-converters for each field"""
 
     def __post_init__(self):
         self.field_converters = {k: make_converter(v) for (k, v) in self.fields.items()}
 
     def expected(self, plural: bool = False) -> str:
-        p = "s" if plural else ""
         name = f" {self.name}" if self.name is not None else ""
-        return f"struct{p}{name}"
+        return f"{pluralize('struct', plural)}{name}"
 
-    def try_convert(self, val) -> T:
+    def try_convert(self, val: t.Any) -> T:
         if not isinstance(val, (dict, t.Mapping)):
             raise ParseInterrupt()
-        d = {}
+        val = t.cast(t.Dict[str, t.Any], val)
+        d: t.Dict[str, t.Any] = {}
         for (k, v) in val.items():
             if k not in self.fields:
                 raise ParseInterrupt()  # unknown field
             d[k] = self.field_converters[k].try_convert(v)
         missing = set(self.fields.keys()) - set(val.keys()) - self.opt_fields
         if len(missing):
             raise ParseInterrupt()
         return self.ty(d)  # type: ignore
 
-    def collect_errors(self, actual) -> t.Union[WrongTypeError, ProductErrorNode, None]:
-        if not isinstance(actual, (dict, t.Mapping)):
-            return WrongTypeError(self.expected(), actual)
+    def collect_errors(self, val: t.Any) -> t.Union[WrongTypeError, ProductErrorNode, None]:
+        if not isinstance(val, (dict, t.Mapping)):
+            return WrongTypeError(self.expected(), val)
+        val = t.cast(t.Dict[str, t.Any], val)
 
-        children = {}
-        extra = set()
-        for (k, v) in actual.items():
+        children: t.Dict[t.Union[str, int], t.Any] = {}
+        extra: t.Set[str] = set()
+        for (k, v) in val.items():
             if k not in self.fields:
                 extra.add(k)
                 continue
             if (node := self.field_converters[k].collect_errors(v)) is not None:
                 children[k] = node
-        missing = set(self.fields.keys()) - set(actual.keys()) - self.opt_fields
+        missing = set(self.fields.keys()) - set(val.keys()) - self.opt_fields
         if len(children) or len(missing) or len(extra):
-            return ProductErrorNode(self.expected(), children, actual, missing, extra)
+            return ProductErrorNode(self.expected(), children, val, missing, extra)
         return None
 
 
 @dataclasses.dataclass(init=False)
-class TupleConverter(t.Generic[TupleT], Converter[TupleT]):
-    ty: t.Type[TupleT]
-    converters: t.Tuple[Converter, ...]
+class TupleConverter(t.Generic[T], Converter[T]):
+    """Converter for a simple, heterogeneous tuple-like type"""
+    ty: t.Type[T]
+    """Type to convert into. Must be constructible from a sequence/tuple"""
+    converters: t.Tuple[Converter[t.Any], ...]
+    """List of sub-converters for each field"""
 
-    def __init__(self, ty: t.Type[TupleT], types: t.Sequence[t.Type]):
+    def __init__(self, ty: t.Type[T], types: t.Sequence[IntoConverter]):
         self.ty = ty
         self.converters = tuple(map(make_converter, types))
 
-    def try_convert(self, val: t.Any) -> TupleT:
+    def try_convert(self, val: t.Any) -> T:
         if not isinstance(val, t.Sequence):
             raise ParseInterrupt
+        val = t.cast(t.Sequence[t.Any], val)
         if len(val) != len(self.converters):
             raise ParseInterrupt
 
         return self.ty(conv.try_convert(v) for (conv, v) in zip(self.converters, val))
 
     def expected(self, plural: bool = False) -> str:
-        s = "s" if plural else ""
-        return f"tuple{s} of length {len(self.converters)}"
+        return f"{pluralize('tuple', plural)} of length {len(self.converters)}"
 
     def collect_errors(self, val: t.Any) -> t.Union[None, ProductErrorNode, WrongTypeError]:
-        if not isinstance(val, t.Sequence) or len(val) != len(self.converters):
+        if not isinstance(val, t.Sequence) or len(val) != len(self.converters):  # type: ignore
             return WrongTypeError(self.expected(), val)
+        val = t.cast(t.Sequence[t.Any], val)
         children = {}
         for (i, (conv, v)) in enumerate(zip(self.converters, val)):
             node = conv.collect_errors(v)
             if node is not None:
                 children[i] = node
         if len(children) == 0:
             return None
         return ProductErrorNode(self.expected(), children, val)
 
 
 @dataclasses.dataclass(init=False)
-class DictConverter(t.Generic[K, V], Converter[t.Dict[K, V]]):
-    ty: t.Type[t.Dict]
-    k_conv: Converter
-    v_conv: Converter
+class DictConverter(t.Generic[FromDataK, FromDataV], Converter[t.Mapping[FromDataK, FromDataV]]):
+    """Converter for a homogenous dict-like type."""
+    ty: t.Type[t.Mapping[FromDataK, FromDataV]]
+    """Type to convert into. Must be constructible from a dict"""
+    k_conv: Converter[FromDataK]
+    """Sub-converter for keys"""
+    v_conv: Converter[FromDataV]
+    """Sub-converter for values"""
 
-    def __init__(self, ty: t.Type[t.Dict], k: t.Type[K] = t.Any, v: t.Type[V] = t.Any):
-        self.ty: t.Type[t.Dict] = ty
+    def __init__(self, ty: t.Type[t.Dict[t.Any, t.Any]], k: t.Type[FromDataK] = t.Any, v: t.Type[FromDataV] = t.Any):
+        self.ty = ty
         self.k_conv = make_converter(k)
         self.v_conv = make_converter(v)
 
     def expected(self, plural: bool = False) -> str:
-        s = "s" if plural else ""
-        return f"mapping{s} of {self.k_conv.expected(True)} => {self.v_conv.expected(True)}"
+        return f"{pluralize('mapping', plural)} of {self.k_conv.expected(True)} => {self.v_conv.expected(True)}"
 
-    def try_convert(self, val: t.Any) -> t.Dict[K, V]:
+    def try_convert(self, val: t.Any) -> t.Mapping[FromDataK, FromDataV]:
         if not isinstance(val, t.Mapping):
             raise ParseInterrupt()
-        return {self.k_conv.try_convert(k): self.v_conv.try_convert(v) for (k, v) in val.items()}
+        val = t.cast(t.Mapping[t.Any, t.Any], val)
+        d = {self.k_conv.try_convert(k): self.v_conv.try_convert(v) for (k, v) in val.items()}
+        return self.ty(d)  # type: ignore
 
     def collect_errors(self, val: t.Any) -> t.Union[None, WrongTypeError, ProductErrorNode]:
         if not isinstance(val, t.Mapping):
             return WrongTypeError(self.expected(), val)
-        nodes = {}
+        val = t.cast(t.Mapping[t.Any, t.Any], val)
+        nodes: t.Dict[t.Union[str, int], ErrorNode] = {}
         for (k, v) in val.items():
             if (node := self.k_conv.collect_errors(k)) is not None:
-                nodes[k] = node  # TODO split bad fields from bad values
+                nodes[str(k)] = node  # TODO split bad fields from bad values
             if (node := self.v_conv.collect_errors(v)) is not None:
-                nodes[k] = node
+                nodes[str(k)] = node
         if len(nodes):
             return ProductErrorNode(self.expected(), nodes, val)
 
 
 @dataclasses.dataclass(init=False)
-class SequenceConverter(t.Generic[T], Converter[t.Sequence[T]]):
-    ty: t.Type[t.Sequence]
-    v_conv: Converter[T]
+class SequenceConverter(t.Generic[FromDataT], Converter[t.Sequence[FromDataT]]):
+    """Converter for a homogenous sequence-like type"""
+    ty: type
+    """Type to convert into. Must be constructible from a tuple/sequence."""
+    v_conv: Converter[FromDataT]
+    """Sub-converter for values"""
 
-    def __init__(self, ty: t.Type[t.Sequence], v: t.Type[T] = t.Any):
+    def __init__(self, ty: t.Type[t.Sequence[t.Any]], v: t.Type[FromDataT] = t.Any):
         self.ty = ty
         self.v_conv = make_converter(v)
 
     def expected(self, plural: bool = False) -> str:
-        s = "s" if plural else ""
-        return f"sequence{s} of {self.v_conv.expected(True)}"
+        return f"{pluralize('sequence', plural)} of {self.v_conv.expected(True)}"
 
-    def try_convert(self, val: t.Any) -> t.Sequence[T]:
+    def try_convert(self, val: t.Any) -> t.Sequence[FromDataT]:
         if not isinstance(val, t.Sequence) or isinstance(val, str):
             raise ParseInterrupt
         return self.ty(self.v_conv.try_convert(v) for v in val)  # type: ignore
 
     def collect_errors(self, val: t.Any) -> t.Union[None, WrongTypeError, ProductErrorNode]:
         if not isinstance(val, t.Sequence) or isinstance(val, str):
             return WrongTypeError("sequence", val)
+        val = t.cast(t.Sequence[t.Any], val)
         nodes = {}
         for (i, v) in enumerate(val):
             if (node := self.v_conv.collect_errors(v)) is not None:
                 nodes[i] = node
         if len(nodes):
             return ProductErrorNode("sequence", nodes, val)
 
 
 @dataclasses.dataclass
+class ConditionalConverter(t.Generic[FromDataT], Converter[FromDataT]):
+    """
+    Converter which applies an arbitrary pre-condition to the converted value.
+    """
+    inner_type: t.Union[t.Type[FromDataT], Converter[FromDataT]]
+    """Inner type to apply condition to"""
+    condition: t.Callable[[FromDataT], bool]
+    """Function to evaluate condition"""
+    condition_name: str
+    make_expected: t.Callable[[str, bool], str]
+    """Function which takes ``(expected, plural)`` and makes a compound ``expected``."""
+    inner: Converter[FromDataT] = dataclasses.field(init=False)
+    """Inner sub-converter"""
+
+    def __post_init__(self):
+        if isinstance(self.inner_type, Converter):
+            self.inner = self.inner_type
+        else:
+            self.inner = make_converter(t.cast(t.Type[FromDataT], self.inner_type))
+
+    def expected(self, plural: bool = False) -> str:
+        return self.make_expected(self.inner.expected(plural), plural)
+
+    def try_convert(self, val: t.Any) -> FromDataT:
+        val = self.inner.try_convert(val)
+        try:
+            if self.condition(val):
+                return val
+        except Exception:
+            pass
+        raise ParseInterrupt()
+
+    def collect_errors(self, val: t.Any) -> t.Optional[ErrorNode]:
+        try:
+            conv_val = self.inner.try_convert(val)
+        except ParseInterrupt:
+            # TODO with_expected() here
+            return self.inner.collect_errors(val)
+        try:
+            # condition failed
+            if not self.condition(conv_val):
+                return ConditionFailedError(self.expected(), val, self.condition_name)
+        except Exception as e:
+            tb = e.__traceback__.tb_next  # type: ignore
+            tb = traceback.TracebackException(type(e), e, tb)
+            return ConditionFailedError(self.expected(), val, self.condition_name, tb)
+        return None
+
+
+@dataclasses.dataclass
 class DelegateConverter(t.Generic[T, U], Converter[T]):
+    """
+    Converter which delegates to a sub-converter, and then attempts
+    to construct a different type
+    """
     from_type: t.Type[U]
+    """Inner type to convert to"""
     constructor: t.Callable[[U], T]
+    """Constructor for outer type"""
     expect: t.Optional[str] = None
+    """Expected value. Defaults to inner expected value."""
     expect_plural: t.Optional[str] = None
+    """Plural expected value. Defaults to inner expected value."""
     inner: Converter[U] = dataclasses.field(init=False)
+    """Inner sub-converter"""
 
     def __post_init__(self):
         self.inner = make_converter(self.from_type)
         self.expect = self.expect or self.from_type.__name__
         self.expect_plural = self.expect_plural or self.expect
 
     def expected(self, plural: bool = False) -> str:
@@ -449,103 +443,34 @@
         try:
             return self.constructor(val)
         except Exception:
             raise ParseInterrupt from None
 
     def collect_errors(self, val: t.Any) -> t.Optional[ErrorNode]:
         try:
-            val = self.inner.try_convert(val)
+            conv_val = self.inner.try_convert(val)
         except ParseInterrupt:
+            # TODO with_expected() here
             return self.inner.collect_errors(val)
         try:
-            self.constructor(val)
+            self.constructor(conv_val)
         except Exception as e:
             tb = e.__traceback__.tb_next  # type: ignore
             tb = traceback.TracebackException(type(e), e, tb)
             return WrongTypeError(self.expected(), val, tb)
 
 
+# converters for scalar types
 _BASIC_CONVERTERS = {
     str: ScalarConverter(str, str, 'a string', 'strings'),
     int: ScalarConverter(int, int, 'an int', 'ints'),
     float: ScalarConverter(float, (int, float), 'a float', 'floats'),
     complex: ScalarConverter(complex, (int, float, complex), 'a complex float', 'complex floats'),
     type(None): NoneConverter(),
 }
-
-
-def make_converter(ty: t.Type[T]) -> Converter[T]:
-    if ty is t.Any:
-        return AnyConverter()
-    if isinstance(ty, t.TypeVar):
-        warnings.warn(f"Unbound TypeVar '{ty}'. Will be interpreted as Any.")
-        return AnyConverter()
-    if isinstance(ty, (dict, t.Dict)):
-        return StructConverter(type(ty), ty)
-    if isinstance(ty, (tuple, t.Tuple)):
-        return TupleConverter(type(ty), ty)
-    if isinstance(ty, t.ForwardRef) or isinstance(ty, str):
-        raise TypeError(f"Unresolved forward reference '{ty}'")
-
-    base = t.get_origin(ty) or ty
-    args = t.get_args(ty)
-
-    # TODO eat annotation
-
-    # special types
-    if base is t.Union:
-        return UnionConverter(args)
-    if base is t.Literal:
-        return LiteralConverter(args)
-
-    if not isinstance(base, type):
-        raise TypeError(f"Unsupported special type '{base}'")
-
-    if issubclass(base, HasFromData):
-        return base._converter(*args, annotations=None)
-
-    if ty in _BASIC_CONVERTERS:
-        return _BASIC_CONVERTERS[ty]
-
-    if issubclass(base, (tuple, t.Tuple)) and len(args) > 0 and args[-1] != Ellipsis:
-        return TupleConverter(base, args)
-    if issubclass(base, (list, t.Sequence)):
-        return SequenceConverter(base, args[0] if len(args) > 0 else t.Any)  # type: ignore
-    if issubclass(base, (dict, t.Mapping)):
-        return DictConverter(base,  # type: ignore
-                             args[0] if len(args) > 0 else t.Any,
-                             args[1] if len(args) > 1 else t.Any)  # type: ignore
-
-    raise TypeError(f"Can't convert data into type '{ty}'")
-
-
-def into_data(val: IntoData) -> DataType:
-    if isinstance(val, (dict, t.Mapping)):
-        return {into_data(k): into_data(v) for (k, v) in val.items()}
-    if isinstance(val, tuple):
-        return type(val)(map(into_data, val))
-    if isinstance(val, t.Sequence) and not isinstance(val, str):
-        return list(map(into_data, val))
-    if isinstance(val, DataTypes):
-        return val
-    if isinstance(val, IntoData):
-        return val.into_data()
-
-    raise TypeError(f"Can't convert type '{type(val)}' into data.")
-
-
-def from_data(val: DataType, ty: t.Type[T]) -> T:
-    if not isinstance(val, DataTypes):
-        raise TypeError(f"Type {type(val)} is not a valid data interchange type.")
-
-    converter = make_converter(ty)
-    return converter.convert(val)
-
-
-def convert(val: IntoData, ty: t.Type[T]) -> T:
-    data = into_data(val)
-    return from_data(data, ty)
+"""Built-in scalar converters for some basic types"""
 
 __all__ = [
-    'FromData', 'IntoData', 'DataType', 'ConvertError',
-    'from_data', 'into_data', 'make_converter', 'convert',
+    'Converter', 'AnyConverter', 'ScalarConverter', 'NoneConverter', 'LiteralConverter',
+    'UnionConverter', 'StructConverter', 'TupleConverter', 'DictConverter', 'SequenceConverter',
+    'DelegateConverter', 'ConditionalConverter',
 ]
```

### Comparing `py-pane-0.2/pane/field.py` & `py-pane-0.3/pane/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,45 +26,45 @@
     'scream': lambda parts: '_'.join(part.upper() for part in parts),
     'kebab': lambda parts: '-'.join(part.lower() for part in parts),
     'camel': lambda parts: ''.join(part.lower() if i == 0 else part.title() for (i, part) in enumerate(parts)),
     'pascal': lambda parts: ''.join(part.title() for part in parts),
 }
 
 
-def pairwise(it: t.Iterable[T]) -> t.Iterator[t.Tuple[T, T]]:
+def _pairwise(it: t.Iterable[T]) -> t.Iterator[t.Tuple[T, T]]:
     it = iter(it)
     while True:
         try:
             a = next(it)
             b = next(it)
         except StopIteration:
             break
         yield (a, b)
 
 
-def split_field_name(field: str) -> t.Sequence[str]:
+def _split_field_name(field: str) -> t.Sequence[str]:
     parts = re.split(r'[_-]', field)
     if not all(parts):
         raise ValueError(f"Unable to interpret field '{field}' for automatic rename")
 
     def split_case(field: str):
         if field.isupper() or field.islower() or field.istitle():
             yield field
             return
         seps = re.split(r'([A-Z])', field)
         if seps[0] != '':
             yield seps[0]
-        for (s1, s2) in pairwise(seps[1:]):
+        for (s1, s2) in _pairwise(seps[1:]):
             yield s1 + s2
 
     return tuple(itertools.chain.from_iterable(map(split_case, parts)))
 
 
 def rename_field(field: str, style: RenameStyle) -> str:
-    return CONVERT_FNS[style](split_field_name(field))
+    return CONVERT_FNS[style](_split_field_name(field))
 
 
 @dataclass(kw_only=True)
 class Field:
     name: str
     type: type
     in_names: t.Sequence[str]
@@ -98,18 +98,18 @@
     kw_only: bool = False
     ty: t.Union[type, _Missing] = _MISSING
 
     def __post_init__(self):
         if isinstance(self.aliases, str):
             self.aliases = [self.aliases]
 
-    def replace_typevars(self, replacements: t.Mapping[t.Union[t.TypeVar, t.ParamSpec], t.Type]) -> Self:
+    def replace_typevars(self, replacements: t.Mapping[t.Union[t.TypeVar, t.ParamSpec], t.Type[t.Any]]) -> Self:
         if self.ty is _MISSING:
             return replace(self)
-        return replace(self, ty=replace_typevars(self.ty, replacements))
+        return replace(self, ty=replace_typevars(t.cast(type, self.ty), replacements))
 
     def make_field(self, name: str,
                    in_rename: t.Optional[t.Sequence[RenameStyle]] = None,
                    out_rename: t.Optional[RenameStyle] = None) -> Field:
         # out_name
         if self.out_name is not None:
             out_name = self.out_name
@@ -146,8 +146,14 @@
     default: t.Union[T, _Missing] = _MISSING,
     default_factory: t.Optional[t.Callable[[], T]] = None,
     kw_only: bool = False,
 ) -> t.Any:
     return FieldSpec(
         rename=rename, in_names=in_names, aliases=aliases, out_name=out_name,
         init=init, default=default, default_factory=default_factory, kw_only=kw_only
-    )
+    )
+
+
+__all__ = [
+    'Field', 'FieldSpec', 'field',
+    'rename_field',
+]
```

### Comparing `py-pane-0.2/pane/test_field.py` & `py-pane-0.3/pane/test_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import pytest
 
-from .field import split_field_name, rename_field
+from .field import _split_field_name, rename_field
 
 
 @pytest.mark.parametrize(('field', 'out'), [
     ('test', ('test',)),
     ('test_snake_Case', ('test', 'snake', 'Case'),),
     ('test-KEBAB-Case', ('test', 'KEBAB', 'Case'),),
     ('TestPascalCase', ('Test', 'Pascal', 'Case'),),
@@ -13,17 +13,17 @@
     ('TEST_SCREAM_CASE', ('TEST', 'SCREAM', 'CASE'),),
     # conservative for now
     ('__test__', ValueError("Unable to interpret field '__test__' for automatic rename")),
 ])
 def test_split_field(field, out):
     if isinstance(out, ValueError):
         with pytest.raises(ValueError, match=out.args[0]):
-            split_field_name(field)
+            _split_field_name(field)
     else:
-        assert split_field_name(field) == out
+        assert _split_field_name(field) == out
 
 
 @pytest.mark.parametrize(('field', 'style', 'out'), [
     ('toPascalCase', 'pascal', 'ToPascalCase'),
     ('To_CAMEL_case', 'camel', 'toCamelCase'),
     ('ToScream_Case', 'scream', 'TO_SCREAM_CASE'),
     ('To_kebab_Case', 'kebab', 'to-kebab-case'),
```

### Comparing `py-pane-0.2/pane/test_util.py` & `py-pane-0.3/pane/test_util.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.2/py_pane.egg-info/PKG-INFO` & `py-pane-0.3/py_pane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pane
-Version: 0.2
+Version: 0.3
 Summary: A modern dataclass & data conversion library, focused on speed and expressiveness.
 Author-email: Colin Gilgenbach <hexane@mit.edu>
 License: MIT License
         
         Copyright (c) 2023 Colin Gilgenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `py-pane-0.2/tests/test_pane.py` & `py-pane-0.3/tests/test_pane.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 import inspect
-from dataclasses import field, dataclass
 import typing as t
 
 import pytest
 
 import pane
-from pane.convert import ErrorNode, ProductErrorNode, DuplicateKeyError, WrongTypeError
+from pane.errors import ErrorNode, ProductErrorNode, DuplicateKeyError, WrongTypeError
 
 
 def check_ord(obj, other, ordering: t.Literal[-1, 0, 1]):
     assert (obj < other) == (ordering < 0)
     assert (obj > other) == (ordering > 0)
     assert (obj <= other) == (ordering <= 0)
     assert (obj >= other) == (ordering >= 0)
@@ -73,15 +72,15 @@
 
 
 class TestClassInherit2(TestClassInherit):
     w: int = 4
 
 
 class TestClassModifyFields(TestClassInherit):
-    x: float = 9.
+    x: float = 9.  # type: ignore
 
 
 class TestClass2(pane.PaneBase):
     x: int = 1
     z: int = pane.field(default=3, kw_only=True)
     y: int = 2
     _: pane.KW_ONLY
```

