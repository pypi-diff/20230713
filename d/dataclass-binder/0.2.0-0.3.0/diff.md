# Comparing `tmp/dataclass_binder-0.2.0.tar.gz` & `tmp/dataclass_binder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_binder-0.2.0.tar", max compression
+gzip compressed data, was "dataclass_binder-0.3.0.tar", max compression
```

## Comparing `dataclass_binder-0.2.0.tar` & `dataclass_binder-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/LICENSE
--rw-r--r--   0        0        0    15881 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/README.md
--rw-r--r--   0        0        0     2512 2023-06-26 06:28:27.198699 dataclass_binder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/src/dataclass_binder/__init__.py
--rw-r--r--   0        0        0    28033 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/src/dataclass_binder/_impl.py
--rw-r--r--   0        0        0        0 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/src/dataclass_binder/py.typed
--rw-r--r--   0        0        0    17237 1970-01-01 00:00:00.000000 dataclass_binder-0.2.0/setup.py
--rw-r--r--   0        0        0    16797 1970-01-01 00:00:00.000000 dataclass_binder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-13 00:30:40.115385 dataclass_binder-0.3.0/LICENSE
+-rw-r--r--   0        0        0    17494 2023-07-13 00:30:40.115385 dataclass_binder-0.3.0/README.md
+-rw-r--r--   0        0        0     2550 2023-07-13 00:31:03.031852 dataclass_binder-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-13 00:30:40.115385 dataclass_binder-0.3.0/src/dataclass_binder/__init__.py
+-rw-r--r--   0        0        0    33489 2023-07-13 00:30:40.115385 dataclass_binder-0.3.0/src/dataclass_binder/_impl.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:30:40.115385 dataclass_binder-0.3.0/src/dataclass_binder/py.typed
+-rw-r--r--   0        0        0    18878 1970-01-01 00:00:00.000000 dataclass_binder-0.3.0/setup.py
+-rw-r--r--   0        0        0    18410 1970-01-01 00:00:00.000000 dataclass_binder-0.3.0/PKG-INFO
```

### Comparing `dataclass_binder-0.2.0/LICENSE` & `dataclass_binder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_binder-0.2.0/README.md` & `dataclass_binder-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -370,14 +370,30 @@
 
 @dataclass(frozen=True)
 class Config:
     tags: Sequence[str] = ()
     limits: Mapping[str, int]
 ```
 
+### Layered Binding
+
+`Binder` can be instantiated from a dataclass object rather than the dataclass itself.
+The dataclass object will provide new default values when binding data to it.
+This can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:
+
+```py
+config = Config()
+if system_config_path.exists():
+    config = Binder(config).parse_toml(system_config_path)
+if user_config_path.exists():
+    config = Binder(config).parse_toml(user_config_path)
+```
+
+Later layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.
+
 ### Generating a Configuration Template
 
 To provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.
 
 For example, when the following dataclass defines your configuration:
 
 ```py
@@ -389,18 +405,18 @@
     port: int = 12345
     """TCP port on which to accept connections."""
 ```
 
 You can generate a template configuration file using:
 
 ```py
-from dataclass_binder import format_template
+from dataclass_binder import Binder
 
 
-for line in format_template(Config):
+for line in Binder(Config).format_toml_template():
     print(line)
 ```
 
 Which will print:
 
 ```toml
 # The URL of the database to connect to.
@@ -408,23 +424,23 @@
 database-url = '???'
 
 # TCP port on which to accept connections.
 # Default:
 # port = 12345
 ```
 
-It is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_template()`:
+It is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:
 
 ```py
 TEMPLATE = Config(
     database_url="postgresql://<username>:<password>@<hostname>/<database name>",
     port=8080,
 )
 
-for line in format_template(TEMPLATE):
+for line in Binder(TEMPLATE).format_toml_template():
     print(line)
 ```
 
 Which will print:
 
 ```toml
 # The URL of the database to connect to.
@@ -471,14 +487,18 @@
 
 ## Deprecations
 
 ### Binder Specialization
 
 Prior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.
 
+### Template Formatting
+
+In version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.
+
 ## Changelog
 
 ### 0.1.0 - 2023-02-21:
 
 - First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible
 
 ### 0.1.1 - 2023-02-22:
@@ -494,7 +514,15 @@
 - Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))
 
 ### 0.2.0 - 2023-06-26:
 
 - Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))
 - Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))
 - Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))
+
+### 0.3.0 - 2023-07-13:
+
+- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))
+- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))
+- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))
+- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))
+- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))
```

### Comparing `dataclass_binder-0.2.0/pyproject.toml` & `dataclass_binder-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-binder"
-version = "0.2.0"
+version = "0.3.0"
 description = "Library to bind TOML data to Python dataclasses in a type-safe way."
 authors = [
     "Maarten ter Huurne <maarten.terhuurne@protix.eu>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ProtixIT/dataclass-binder"
@@ -42,22 +42,23 @@
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 src = ["src"]
 select = [
     "F", "E", "W", "I", "N", "UP", "ANN0", "ANN2", "FBT", "B", "A", "C4", "FA",
-    "ISC", "ICN", "G", "INP", "PIE", "T20", "PT", "Q", "RSE", "RET", "SLF", "SIM",
+    "ISC", "ICN", "G", "INP", "PIE", "T20", "PT", "Q", "RSE", "RET", "SIM",
     "ARG", "ERA", "PGH", "PLC", "PLE", "PLW", "TRY", "FLY", "RUF",
 ]
 ignore = [
     "PT007",  # not using tuples for single argument helps readability
     "RET505", "RET506",  # not sure following that style improves readability
     "PLW2901",  # overwriting the loop variable is sometimes useful
     "TRY003",  # maybe in the future
+    "TRY301",  # alternatives might be worse
 ]
 
 [tool.mypy]
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
```

### Comparing `dataclass_binder-0.2.0/src/dataclass_binder/_impl.py` & `dataclass_binder-0.3.0/src/dataclass_binder/_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from __future__ import annotations
 
 import ast
 import operator
 import re
 import sys
-from collections.abc import Collection, Iterable, Iterator, Mapping, MutableMapping, MutableSequence, Sequence
-from dataclasses import MISSING, Field, fields, is_dataclass
+from collections.abc import Callable, Collection, Iterable, Iterator, Mapping, MutableMapping, MutableSequence, Sequence
+from dataclasses import MISSING, asdict, dataclass, fields, is_dataclass, replace
 from datetime import date, datetime, time, timedelta
 from functools import reduce
 from importlib import import_module
 from inspect import cleandoc, get_annotations, getmodule, getsource, isabstract
 from pathlib import Path
 from textwrap import dedent
 from types import MappingProxyType, ModuleType, NoneType, UnionType
-from typing import TYPE_CHECKING, Any, BinaryIO, Generic, TypeVar, Union, cast, get_args, get_origin
+from typing import TYPE_CHECKING, Any, BinaryIO, ClassVar, Generic, TypeVar, Union, cast, get_args, get_origin, overload
 from weakref import WeakKeyDictionary
 
 if sys.version_info < (3, 11):
     import tomli as tomllib  # pragma: no cover
 else:
     import tomllib  # pragma: no cover
 
@@ -160,19 +160,19 @@
     Iterates through all the fields in a dataclass.
 
     This includes fields inherited from superclasses.
     """
 
     fields_by_name = {field.name: field for field in fields(cls)}
 
-    # Note: getmodule() can return None, but the end result is still fine.
-    cls_globals = getattr(getmodule(cls), "__dict__", {})
-    cls_locals = vars(cls)
-
     for field_container in reversed(cls.__mro__):
+        # Note: getmodule() can return None, but the end result is still fine.
+        cls_globals = getattr(getmodule(field_container), "__dict__", {})
+        cls_locals = vars(field_container)
+
         for name, annotation in get_annotations(field_container).items():
             field = fields_by_name[name]
             if not field.init:
                 continue
             if isinstance(annotation, str):
                 try:
                     annotation = eval(annotation, cls_globals, cls_locals)  # noqa: PGH001
@@ -182,62 +182,95 @@
 
 
 _TIMEDELTA_SUFFIXES = {"days", "seconds", "microseconds", "milliseconds", "minutes", "hours", "weeks"}
 
 T = TypeVar("T")
 
 
-class _BinderCache(type, Generic[T]):
-    """
-    Cache that returns a dedicated `Binder` instance for each dataclass.
-    """
+@dataclass(slots=True)
+class _ClassInfo(Generic[T]):
+
+    _cache: ClassVar[MutableMapping[type[Any], _ClassInfo[Any]]] = WeakKeyDictionary()
 
-    _cache: MutableMapping[T, Binder[T]] = WeakKeyDictionary()
+    dataclass: type[T]
+    field_types: Mapping[str, type | Binder[Any]]
+    _field_docstrings: Mapping[str, str] | None = None
 
-    def __call__(cls, dataclass: T) -> Binder[T]:
+    @classmethod
+    def get(cls, dataclass: type[T]) -> _ClassInfo[T]:
         try:
             return cls._cache[dataclass]
         except KeyError:
-            pass
+            info = cls(
+                dataclass,
+                {
+                    field_name: _collect_type(field_type, f"{dataclass.__name__}.{field_name}")
+                    for field_name, field_type in _get_fields(dataclass)
+                },
+            )
+            cls._cache[dataclass] = info
+            return info
 
-        instance: Binder[T] = super().__call__(dataclass)
-        cls._cache[dataclass] = instance
-        return instance
+    @property
+    def class_docstring(self) -> str | None:
+        class_docstring = self.dataclass.__doc__
+        if class_docstring is None:
+            # No coverage because of the undocumented feature described below.
+            return None  # pragma: no cover
+        if class_docstring.startswith(f"{self.dataclass.__name__}("):
+            # As an undocumented feature, the dataclass implementation will auto-generate docstrings.
+            # Those only contain redundant information, so we don't want to use them.
+            return None
+        return cleandoc(class_docstring)
+
+    @property
+    def field_docstrings(self) -> Mapping[str, str]:
+        field_docstrings = self._field_docstrings
+        if field_docstrings is None:
+            self._field_docstrings = field_docstrings = get_field_docstrings(self.dataclass)
+        return field_docstrings
 
 
-class Binder(Generic[T], metaclass=_BinderCache):
+class Binder(Generic[T]):
     """
     Binds TOML data to a specific dataclass.
     """
 
-    __slots__ = ("_dataclass", "_field_types")
+    __slots__ = ("_dataclass", "_instance", "_class_info")
     _dataclass: type[T]
-    _field_types: Mapping[str, type | Binder[Any]]
+    _instance: T | None
+    _class_info: _ClassInfo[T]
 
     def __class_getitem__(cls: type[Binder[T]], dataclass: type[T]) -> Binder[T]:
         """Deprecated: use `Binder(MyDataClass)` instead."""
         return cls(dataclass)
 
-    def __init__(self, dataclass: type[T]) -> None:
-        self._dataclass = dataclass
-        self._field_types = {
-            field_name: _collect_type(field_type, f"{dataclass.__name__}.{field_name}")
-            for field_name, field_type in _get_fields(dataclass)
-        }
+    @overload
+    def __init__(self, class_or_instance: type[T]) -> None:
+        ...
+
+    @overload
+    def __init__(self, class_or_instance: T) -> None:
+        ...
+
+    def __init__(self, class_or_instance: type[T] | T) -> None:
+        if isinstance(class_or_instance, type):
+            self._dataclass = dataclass = class_or_instance
+            self._instance = None
+        else:
+            self._dataclass = dataclass = class_or_instance.__class__
+            self._instance = class_or_instance
+        self._class_info = _ClassInfo.get(dataclass)
 
-    def _bind_to_single_type(self, value: object, field_type: type | Binder[Any], context: str) -> object:
+    def _bind_to_single_type(self, value: object, field_type: type, context: str) -> object:
         """
         Convert a TOML value to a singular (non-union) field type.
 
         Raises TypeError if the TOML value's type doesn't match the field type.
         """
-        if isinstance(field_type, Binder):
-            if not isinstance(value, dict):
-                raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected table")
-            return field_type._bind_to_class(value, context)  # noqa: SLF001
         origin = get_origin(field_type)
         if origin is None:
             if field_type is ModuleType:
                 if not isinstance(value, str):
                     raise TypeError(
                         f"Expected TOML string for Python reference '{context}', got '{type(value).__name__}'"
                     )
@@ -258,38 +291,40 @@
                 type(value) is not bool or field_type is bool or field_type is object
             ):
                 return value
         elif issubclass(origin, Mapping):
             if not isinstance(value, dict):
                 raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected table")
             key_type, elem_type = get_args(field_type)
-            mapping = {key: self._bind_to_field(elem, elem_type, f'{context}["{key}"]') for key, elem in value.items()}
+            mapping = {
+                key: self._bind_to_field(elem, elem_type, None, f'{context}["{key}"]') for key, elem in value.items()
+            }
             return (
                 (mapping if isinstance(origin, MutableMapping) else MappingProxyType(mapping))
                 if isabstract(origin)
                 else field_type(mapping)
             )
         elif issubclass(origin, Iterable):
             if not isinstance(value, list):
                 raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected array")
             type_args = get_args(field_type)
             if issubclass(origin, tuple):
                 if len(type_args) == len(value):
                     return tuple(
-                        self._bind_to_field(elem, elem_type, f"{context}[{index}]")
+                        self._bind_to_field(elem, elem_type, None, f"{context}[{index}]")
                         for index, (elem, elem_type) in enumerate(zip(value, type_args, strict=True))
                     )
                 else:
                     raise TypeError(f"Expected {len(type_args)} elements for '{context}', got {len(value)}")
             (elem_type,) = type_args
             container_class = (
                 (list if isinstance(origin, MutableSequence) else tuple) if isabstract(origin) else field_type
             )
             return container_class(
-                self._bind_to_field(elem, elem_type, f"{context}[{index}]") for index, elem in enumerate(value)
+                self._bind_to_field(elem, elem_type, None, f"{context}[{index}]") for index, elem in enumerate(value)
             )
         elif origin is type:
             if not isinstance(value, str):
                 raise TypeError(f"Expected TOML string for Python reference '{context}', got '{type(value).__name__}'")
             obj = _find_object_by_name(value, context)
             if not isinstance(obj, type):
                 raise TypeError(f"Value for '{context}' has type '{type(obj).__name__}', expected class")
@@ -303,36 +338,40 @@
                 )
         else:
             # This is currently unreachable because we reject unsupported generic types in _collect_type().
             raise AssertionError(origin)
 
         raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected '{field_type.__name__}'")
 
-    def _bind_to_field(self, value: object, field_type: type | Binder[Any], context: str) -> object:
+    def _bind_to_field(self, value: object, field_type: type | Binder[Any], instance: T | None, context: str) -> object:
         """
         Convert a TOML value to a field type which is possibly a union type.
 
         Raises TypeError if the TOML value's type doesn't match the field type.
         """
-        if get_origin(field_type) is UnionType:
-            for arg in get_args(field_type):
-                try:
-                    return self._bind_to_single_type(value, arg, context)
-                except TypeError:
-                    # TODO: This is inefficient: we format and then discard the error string.
-                    #       Union types are not used a lot though, so it's fine for now.
-                    # TODO: When the union contains multiple custom classes, we pick the first that succeeds.
-                    #       It would be cleaner to limit custom classes to one at collection time.
-                    pass
-            raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected '{field_type}'")
-        else:
-            return self._bind_to_single_type(value, field_type, context)
+        target_types = get_args(field_type) if get_origin(field_type) is UnionType else (field_type,)
+        for target_type in target_types:
+            try:
+                if isinstance(field_type, Binder):
+                    if not isinstance(value, dict):
+                        raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected table")
+                    return field_type._bind_to_class(value, instance, context)
+                else:
+                    return self._bind_to_single_type(value, target_type, context)
+            except TypeError:
+                if len(target_types) == 1:
+                    raise
+                # TODO: This is inefficient: we format and then discard the error string.
+                #       Union types are not used a lot though, so it's fine for now.
+                # TODO: When the union contains multiple custom classes, we pick the first that succeeds.
+                #       It would be cleaner to limit custom classes to one at collection time.
+        raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected '{field_type}'")
 
-    def _bind_to_class(self, toml_dict: Mapping[str, Any], context: str) -> T:
-        field_types = self._field_types
+    def _bind_to_class(self, toml_dict: Mapping[str, Any], instance: T | None, context: str) -> T:
+        field_types = self._class_info.field_types
         parsed = {}
         for key, value in toml_dict.items():
             if "_" in key:
                 raise ValueError(f"Underscore found in TOML key '{key}'")
             field_name = key.replace("-", "_")
             try:
                 field_name, suffix = _find_field(field_name, field_types)
@@ -346,25 +385,128 @@
                         value = timedelta(**{suffix: value})
                     else:
                         raise TypeError(
                             f"Value for '{context}.{field_name}' with suffix '{suffix}' "
                             f"has type '{type(value).__name__}', expected number"
                         )
                 else:
-                    type_name = (
-                        field_type._dataclass if isinstance(field_type, Binder) else field_type  # noqa: SLF001
-                    ).__name__
+                    type_name = (field_type._dataclass if isinstance(field_type, Binder) else field_type).__name__
                     raise ValueError(
                         f"Field '{context}.{field_name}' has type '{type_name}', "
                         f"which does not support suffix '{suffix}'"
                     )
 
-            parsed[field_name] = self._bind_to_field(value, field_type, f"{context}.{field_name}")
+            parsed[field_name] = self._bind_to_field(
+                value,
+                field_type,
+                None if instance is None else getattr(instance, field_name),
+                f"{context}.{field_name}",
+            )
+
+        if instance is None:
+            return self._dataclass(**parsed)
+        else:
+            return replace(instance, **parsed)  # type: ignore[type-var]
 
-        return self._dataclass(**parsed)
+    def format_toml_template(self) -> Iterator[str]:
+        """
+        Yield lines of TOML text as a template for populating the dataclass or object that we are binding to.
+
+        A template in this case means it is suitable as a starting point for a user to fill in;
+        the template is not guaranteed to be parseable as-is.
+
+        If we are binding to an object, values from that object will be used to populate the template.
+        If we are binding to a class, example values will be derived from the field types.
+        """
+
+        queue: list[Table[Any]] = [Table(self, "", self._instance, None)]
+
+        def defer(table: Table[Any]) -> None:
+            queue.append(table.prefix_context(context))
+
+        skip_empty = True
+        while queue:
+            table = queue.pop(0)
+            context = table.key_fmt
+            for line in table.format_table(defer):
+                if not line and skip_empty:
+                    skip_empty = False
+                    continue
+                yield line
+
+    def _format_toml_table(self, instance: T | None, defer: Callable[[Table[Any]], None]) -> Iterator[str]:
+        dataclass = self._dataclass
+        field_types = self._class_info.field_types
+        docstrings = self._class_info.field_docstrings
+
+        for field in fields(dataclass):  # type: ignore[arg-type]
+            if not field.init:
+                continue
+
+            key = field.name.replace("_", "-")
+            # Most Python names are valid as bare keys, but not if they contain non-ASCII characters.
+            key_fmt = "".join(_iter_format_key(key))
+            value = None if instance is None else getattr(instance, field.name)
+            docstring = docstrings.get(field.name)
+
+            field_type = field_types[field.name]
+            if isinstance(field_type, Binder):
+                defer(Table(field_type, key_fmt, value, docstring, field.default is not MISSING))
+                continue
+            origin = get_origin(field_type)
+            if origin is not None:
+                if issubclass(origin, Mapping):
+                    key_type, value_type = get_args(field_type)
+                    if isinstance(value_type, Binder):
+                        if value is None:
+                            nested_map = {f"{key_fmt}.<name>": None}
+                        else:
+                            nested_map = {
+                                f"{key_fmt}.{''.join(_iter_format_key(nested_key))}": nested_value
+                                for nested_key, nested_value in value.items()
+                            }
+                        for nested_key_fmt, nested_value in nested_map.items():
+                            defer(Table(value_type, nested_key_fmt, nested_value, docstring))
+                        continue
+                    if value_type is object:  # Any
+                        defer(Table(None, key_fmt, value, docstring, field.default is not MISSING))
+                        continue
+                elif issubclass(origin, Sequence):
+                    (value_type,) = get_args(field_type)
+                    binder = value_type if isinstance(value_type, Binder) else None
+                    if binder is not None or (
+                        value_type is object  # Any
+                        and (value is None or all(isinstance(item, Mapping) or is_dataclass(item) for item in value))
+                    ):
+                        nested_key_fmt = f"[{key_fmt}]"
+                        optional = field.default is not MISSING
+                        for nested_value in [None] if value is None else value:
+                            defer(Table(binder, nested_key_fmt, nested_value, docstring, optional))
+                        continue
+
+            yield ""
+
+            comments = [docstring]
+            default = field.default
+            if value == default:
+                value = None
+            if default is MISSING or default is None:
+                comments.append("Optional." if default is None else "Mandatory.")
+            else:
+                comments.append(f"Default:\n{format_toml_pair(key, default)}")
+            yield from _format_comments(*comments)
+
+            if value is None:
+                if default is MISSING or default is None:
+                    comment = "# " if default is None else ""
+                    key_fmt = "".join(_iter_format_key(key))
+                    value_fmt = _format_value_for_type(field_type)
+                    yield f"{comment}{key_fmt} = {value_fmt}"
+            else:
+                yield f"{format_toml_pair(key, value)}"
 
     if TYPE_CHECKING:
         # These definitions exist to support the deprecated `Binder[DC]` syntax in mypy.
 
         @classmethod
         def bind(cls, data: Mapping[str, Any]) -> T:
             ...
@@ -372,26 +514,73 @@
         @classmethod
         def parse_toml(cls, file: BinaryIO | str | Path) -> T:
             ...
 
     else:
 
         def bind(self, data: Mapping[str, Any]) -> T:
-            return self._bind_to_class(data, self._dataclass.__name__)
+            return self._bind_to_class(data, self._instance, self._dataclass.__name__)
 
         def parse_toml(self, file: BinaryIO | str | Path) -> T:
             match file:
                 case Path() | str():
                     with open(file, "rb") as stream:
                         data = tomllib.load(stream)
                 case _:
                     data = tomllib.load(file)
             return self.bind(data)
 
 
+@dataclass
+class Table(Generic[T]):
+    """The information to format a TOML table."""
+
+    binder: Binder[T] | None
+    key_fmt: str
+    value: T | None
+    field_docstring: str | None
+    optional: bool = False
+
+    @property
+    def class_docstring(self) -> str | None:
+        binder = self.binder
+        return None if binder is None else binder._class_info.class_docstring
+
+    def prefix_context(self, context: str) -> Table[T]:
+        return replace(self, key_fmt=f"{context}.{self.key_fmt}" if context else self.key_fmt)
+
+    def format_table(self, defer: Callable[[Table[Any]], None]) -> Iterator[str]:
+        if (binder := self.binder) is None:
+            match self.value:
+                case Mapping() as mapping:
+                    content = [format_toml_pair(k, v) for k, v in mapping.items()]
+                case dc if is_dataclass(dc):
+                    content = [format_toml_pair(k, v) for k, v in asdict(dc).items()]  # type: ignore[arg-type]
+                case _:
+                    content = []
+        else:
+            content = list(binder._format_toml_table(self.value, defer))
+            if not content:
+                return
+
+        if self.key_fmt:
+            yield from self.format_header()
+
+        yield from content
+
+    def format_header(self) -> Iterator[str]:
+        yield ""
+        yield from _format_comments(
+            self.class_docstring,
+            self.field_docstring,
+            "Optional table." if self.optional else None,
+        )
+        yield f"[{self.key_fmt}]"
+
+
 def format_toml_pair(key: str, value: object) -> str:
     """Format a key/value pair as TOML text."""
     suffix, data = _to_toml_pair(value)
     if suffix is not None:
         key += suffix
     return "".join(_iter_format_key_value(key, data))
 
@@ -447,14 +636,16 @@
                 array.append(dd_val)
             return None, array
         case type():
             return None, f"{value.__module__}.{value.__name__}"
         case _ if is_dataclass(value):
             table = {}
             for field in fields(value):
+                if not field.init:
+                    continue
                 name = field.name
                 sub_value = getattr(value, name)
                 if sub_value is None:
                     assert field.default is None
                     continue
                 key = name.replace("_", "-")
                 suffix, data = _to_toml_pair(sub_value)
@@ -535,14 +726,28 @@
                     yield ", "
                 yield from _iter_format_value(elem)
             yield "]"
         case _:
             raise TypeError(type(value).__name__)
 
 
+def _format_comments(*comments: str | None) -> Iterator[str]:
+    separator = False
+    for comment in comments:
+        if comment:
+            contains_empty = False
+            for line in comment.split("\n"):
+                if separator:
+                    yield "#"
+                    separator = False
+                yield f"# {line}".rstrip()
+                contains_empty |= not line
+            separator = contains_empty
+
+
 def get_field_docstrings(dataclass: type[Any]) -> Mapping[str, str]:
     """
     Return a mapping of field name to the docstring for that field.
 
     Attribute docstrings are not supported by the Python runtime, therefore we must read them from the source code.
     If the source code cannot be found, an empty mapping is returned.
     """
@@ -571,93 +776,19 @@
                     pass
                 else:
                     docstrings[scope] = cleandoc(docstring)
     return docstrings
 
 
 def format_template(class_or_instance: Any) -> Iterator[str]:
-    """
-    Yield lines of TOML text as a template for populating the given data class or instance.
-
-    If an instance is provided, values from that instance will be used to populate the template.
-    If a class is provided, values will be derived from the field types.
-    """
-
-    if isinstance(class_or_instance, type):
-        dataclass = class_or_instance
-        instance = None
-    else:
-        dataclass = class_or_instance.__class__
-        instance = class_or_instance
-
-    docstrings = get_field_docstrings(dataclass)
-
-    first = True
-    for field in fields(dataclass):
-        if not field.init:
-            continue
-
-        if first:
-            first = False
-        else:
-            yield ""
-
-        docstring = docstrings.get(field.name)
-        lines = docstring.split("\n") if docstring else []
-        # End with an empty line if the docstring contains multiple paragraphs.
-        if "" in lines:
-            lines.append("")
-
-        for line in lines:
-            yield f"# {line}".rstrip()
-
-        key = field.name.replace("_", "-")
-        value = None if instance is None else getattr(instance, field.name)
-        default = field.default
-        if value == default:
-            value = None
-        if default is MISSING or default is None:
-            if default is None:
-                yield "# Optional."
-            else:
-                yield "# Mandatory."
-            if value is None:
-                comment = "# " if default is None else ""
-                key_fmt = "".join(_iter_format_key(key))
-                value_fmt = _format_value_for_field(dataclass, field)
-                yield f"{comment}{key_fmt} = {value_fmt}"
-        else:
-            yield "# Default:"
-            yield f"# {format_toml_pair(key, default)}"
-        if value is not None:
-            yield f"{format_toml_pair(key, value)}"
-
-
-def _format_value_for_field(dataclass: type[Any], field: Field) -> str:
-    """Format an example value or placeholder for a value depending on the given field's type."""
-
-    annotated_type: type[Any] | str | None = field.type
-    if isinstance(annotated_type, str):
-        module_locals = {}
-        module = getmodule(dataclass)
-        if module is not None:
-            for name in dir(module):
-                module_locals[name] = getattr(module, name)
-        try:
-            evaluated_type = eval(annotated_type, globals(), module_locals)  # noqa: PGH001
-        except Exception:
-            return "???"
-    else:
-        evaluated_type = annotated_type
+    """Deprecated: use `Binder.format_toml_template()` instead."""
+    yield from Binder(class_or_instance).format_toml_template()
 
-    field_type = _collect_type(evaluated_type, f"{dataclass.__name__}.{field.name}")
-    return _format_value_for_type(field_type)
 
-
-def _format_value_for_type(field_type: type[Any] | Binder[Any]) -> str:
+def _format_value_for_type(field_type: type[Any]) -> str:
     origin = get_origin(field_type)
     if origin is None:
         if field_type is str:
             return "'???'"
         elif field_type is bool:
             return "true | false"
         elif field_type is int:
@@ -668,37 +799,21 @@
             return "'fully.qualified.module.name'"
         elif field_type is datetime:
             return "2020-01-01 00:00:00+01:00"
         elif field_type is date:
             return "2020-01-01"
         elif field_type is time or field_type is timedelta:
             return "00:00:00"
-        elif isinstance(field_type, Binder):
-            return "".join(_format_fields_inline(field_type._dataclass))  # noqa: SLF001
         else:
             # We have handled all the non-generic types supported by _collect_type().
             raise AssertionError(field_type)
     elif origin in (UnionType, Union):
         return " | ".join(_format_value_for_type(arg) for arg in get_args(field_type))
     elif issubclass(origin, Mapping):
         return "{}"
     elif issubclass(origin, Iterable):
         return "[]"
     elif origin is type:
         return "'fully.qualified.class.name'"
     else:
         # This is currently unreachable because we reject unsupported generic types in _collect_type().
         raise AssertionError(origin)
-
-
-def _format_fields_inline(dataclass: type[Any]) -> Iterable[str]:
-    yield "{"
-    first = True
-    for field in fields(dataclass):
-        if first:
-            first = False
-        else:
-            yield ", "
-        yield from _iter_format_key(field.name.replace("_", "-"))
-        yield " = "
-        yield _format_value_for_field(dataclass, field)
-    yield "}"
```

### Comparing `dataclass_binder-0.2.0/setup.py` & `dataclass_binder-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'dataclass-binder',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Library to bind TOML data to Python dataclasses in a type-safe way.',
-    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import format_template\n\n\nfor line in format_template(Config):\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in format_template(TEMPLATE):\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n',
+    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Layered Binding\n\n`Binder` can be instantiated from a dataclass object rather than the dataclass itself.\nThe dataclass object will provide new default values when binding data to it.\nThis can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:\n\n```py\nconfig = Config()\nif system_config_path.exists():\n    config = Binder(config).parse_toml(system_config_path)\nif user_config_path.exists():\n    config = Binder(config).parse_toml(user_config_path)\n```\n\nLater layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import Binder\n\n\nfor line in Binder(Config).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in Binder(TEMPLATE).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n### Template Formatting\n\nIn version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n\n### 0.3.0 - 2023-07-13:\n\n- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))\n- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))\n- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))\n- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))\n- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))\n',
     'author': 'Maarten ter Huurne',
     'author_email': 'maarten.terhuurne@protix.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ProtixIT/dataclass-binder',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `dataclass_binder-0.2.0/PKG-INFO` & `dataclass_binder-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-binder
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library to bind TOML data to Python dataclasses in a type-safe way.
 Home-page: https://github.com/ProtixIT/dataclass-binder
 License: MIT
 Keywords: dataclass,toml,bind,binding
 Author: Maarten ter Huurne
 Author-email: maarten.terhuurne@protix.eu
 Requires-Python: >=3.10,<4.0
@@ -391,14 +391,30 @@
 
 @dataclass(frozen=True)
 class Config:
     tags: Sequence[str] = ()
     limits: Mapping[str, int]
 ```
 
+### Layered Binding
+
+`Binder` can be instantiated from a dataclass object rather than the dataclass itself.
+The dataclass object will provide new default values when binding data to it.
+This can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:
+
+```py
+config = Config()
+if system_config_path.exists():
+    config = Binder(config).parse_toml(system_config_path)
+if user_config_path.exists():
+    config = Binder(config).parse_toml(user_config_path)
+```
+
+Later layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.
+
 ### Generating a Configuration Template
 
 To provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.
 
 For example, when the following dataclass defines your configuration:
 
 ```py
@@ -410,18 +426,18 @@
     port: int = 12345
     """TCP port on which to accept connections."""
 ```
 
 You can generate a template configuration file using:
 
 ```py
-from dataclass_binder import format_template
+from dataclass_binder import Binder
 
 
-for line in format_template(Config):
+for line in Binder(Config).format_toml_template():
     print(line)
 ```
 
 Which will print:
 
 ```toml
 # The URL of the database to connect to.
@@ -429,23 +445,23 @@
 database-url = '???'
 
 # TCP port on which to accept connections.
 # Default:
 # port = 12345
 ```
 
-It is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_template()`:
+It is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:
 
 ```py
 TEMPLATE = Config(
     database_url="postgresql://<username>:<password>@<hostname>/<database name>",
     port=8080,
 )
 
-for line in format_template(TEMPLATE):
+for line in Binder(TEMPLATE).format_toml_template():
     print(line)
 ```
 
 Which will print:
 
 ```toml
 # The URL of the database to connect to.
@@ -492,14 +508,18 @@
 
 ## Deprecations
 
 ### Binder Specialization
 
 Prior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.
 
+### Template Formatting
+
+In version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.
+
 ## Changelog
 
 ### 0.1.0 - 2023-02-21:
 
 - First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible
 
 ### 0.1.1 - 2023-02-22:
@@ -516,7 +536,15 @@
 
 ### 0.2.0 - 2023-06-26:
 
 - Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))
 - Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))
 - Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))
 
+### 0.3.0 - 2023-07-13:
+
+- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))
+- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))
+- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))
+- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))
+- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))
+
```

