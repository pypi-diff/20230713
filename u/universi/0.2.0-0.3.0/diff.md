# Comparing `tmp/universi-0.2.0.tar.gz` & `tmp/universi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universi-0.2.0.tar", max compression
+gzip compressed data, was "universi-0.3.0.tar", max compression
```

## Comparing `universi-0.2.0.tar` & `universi-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.2.0/LICENSE
--rw-r--r--   0        0        0      921 2023-07-02 16:05:32.636241 universi-0.2.0/README.md
--rw-r--r--   0        0        0     3983 2023-07-11 00:08:58.759192 universi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      374 2023-07-09 10:59:39.112133 universi-0.2.0/universi/__init__.py
--rw-r--r--   0        0        0     1954 2023-07-08 11:43:06.920139 universi-0.2.0/universi/_utils.py
--rw-r--r--   0        0        0    16364 2023-07-10 23:30:12.755289 universi-0.2.0/universi/codegen.py
--rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.2.0/universi/exceptions.py
--rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.2.0/universi/fields.py
--rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.2.0/universi/header.py
--rw-r--r--   0        0        0     6281 2023-07-07 14:40:35.153712 universi-0.2.0/universi/linting.py
--rw-r--r--   0        0        0        1 2023-07-03 05:47:19.541761 universi-0.2.0/universi/migration.py
--rw-r--r--   0        0        0    11138 2023-07-10 23:30:24.881889 universi-0.2.0/universi/routing.py
--rw-r--r--   0        0        0      396 2023-07-08 11:43:06.913473 universi-0.2.0/universi/structure/__init__.py
--rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.2.0/universi/structure/common.py
--rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.2.0/universi/structure/endpoints.py
--rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.2.0/universi/structure/enums.py
--rw-r--r--   0        0        0     1392 2023-07-08 11:43:06.916806 universi-0.2.0/universi/structure/responses.py
--rw-r--r--   0        0        0     4208 2023-07-08 06:21:22.326331 universi-0.2.0/universi/structure/schemas.py
--rw-r--r--   0        0        0     8741 2023-07-10 23:59:45.108897 universi-0.2.0/universi/structure/versions.py
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 universi-0.2.0/setup.py
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 universi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1111 2023-07-13 19:54:24.646654 universi-0.3.0/README.md
+-rw-r--r--   0        0        0     4059 2023-07-12 23:05:34.016074 universi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.3.0/universi/__init__.py
+-rw-r--r--   0        0        0     2007 2023-07-13 07:28:53.287286 universi-0.3.0/universi/_utils.py
+-rw-r--r--   0        0        0    16536 2023-07-12 19:34:22.676522 universi-0.3.0/universi/codegen.py
+-rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.3.0/universi/exceptions.py
+-rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.3.0/universi/fields.py
+-rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.3.0/universi/header.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.3.0/universi/py.typed
+-rw-r--r--   0        0        0    11467 2023-07-12 19:38:06.375294 universi-0.3.0/universi/routing.py
+-rw-r--r--   0        0        0      396 2023-07-08 11:43:06.913473 universi-0.3.0/universi/structure/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.3.0/universi/structure/common.py
+-rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.3.0/universi/structure/endpoints.py
+-rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.3.0/universi/structure/enums.py
+-rw-r--r--   0        0        0     1239 2023-07-12 19:32:07.873928 universi-0.3.0/universi/structure/responses.py
+-rw-r--r--   0        0        0     4199 2023-07-11 01:53:10.755842 universi-0.3.0/universi/structure/schemas.py
+-rw-r--r--   0        0        0     8670 2023-07-12 19:32:07.877261 universi-0.3.0/universi/structure/versions.py
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 universi-0.3.0/setup.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 universi-0.3.0/PKG-INFO
```

### Comparing `universi-0.2.0/LICENSE` & `universi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universi-0.2.0/README.md` & `universi-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -20,7 +20,12 @@
 </p>
 
 ## Installation
 
 ```bash
 pip install universi
 ```
+
+<!---
+# TODO: Note that we don't handle "from .schemas import Schema as OtherSchema" case
+# TODO: Need to validate that the user doesn't use versioned schemas instead of the latest ones
+-->
```

### Comparing `universi-0.2.0/pyproject.toml` & `universi-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "universi"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/universi"
 
 [tool.poetry.dependencies]
@@ -21,14 +21,18 @@
 pytest-cov = ">=4.0.0"
 httpx = ">=0.23.0"
 uvicorn = "*"
 devtools = "*"
 pdbpp = "^0.10.3"
 pytest-pretty = "^1.2.0"
 notebook = "^6.5.4"
+pytest-asyncio = "^0.21.0"
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
 
 [tool.coverage.report]
 fail_under = 100
 skip_covered = true
 skip_empty = true
 # Taken from https://coverage.readthedocs.io/en/7.1.0/excluding.html#advanced-exclusion
 exclude_lines = [
```

### Comparing `universi-0.2.0/universi/codegen.py` & `universi-0.3.0/universi/codegen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import ast
 import importlib
 import inspect
-import json
 import os
-import pprint
 import shutil
 import sys
 from collections.abc import Sequence
 from copy import deepcopy
 from datetime import date
 from enum import Enum, auto
 from pathlib import Path
 from types import GenericAlias, LambdaType, ModuleType
-from typing import Any, TypeAlias, get_args, get_origin
+from typing import (
+    Any,
+    TypeAlias,
+    _BaseGenericAlias,  # pyright: ignore[reportGeneralTypeIssues]
+    get_args,
+    get_origin,
+)
 
 from pydantic import BaseConfig, BaseModel
+from pydantic.fields import FieldInfo as PydanticFieldInfo
 from pydantic.fields import ModelField
+from pydantic.typing import convert_generics
 from typing_extensions import assert_never
-from pydantic.fields import FieldInfo as PydanticFieldInfo
 
-from ._utils import Sentinel
-from .exceptions import CodeGenerationError, InvalidGenerationInstructionError
-from .fields import FieldInfo
 from universi.structure.enums import AlterEnumSubInstruction, EnumDidntHaveMembersInstruction, EnumHadMembersInstruction
 from universi.structure.schemas import (
     AlterSchemaInstruction,
     OldSchemaDidntHaveField,
     OldSchemaFieldWas,
     OldSchemaHadField,
 )
 from universi.structure.versions import Version, Versions
-from pydantic.typing import convert_generics
 
+from ._utils import Sentinel
+from .exceptions import CodeGenerationError, InvalidGenerationInstructionError
+from .fields import FieldInfo
+
+LambdaFunctionName = (lambda: None).__name__  # pragma: no branch
 FieldNameT: TypeAlias = str
 dict_of_empty_field_info = {k: getattr(PydanticFieldInfo(), k) for k in PydanticFieldInfo.__slots__}
 
 
 # TODO: Add enum alteration here
 def regenerate_dir_to_all_versions(template_module: ModuleType, versions: Versions):
     schemas = {k: (v, _get_fields_for_model(v)) for k, v in deepcopy(versions.versioned_schemas).items()}
@@ -43,18 +49,18 @@
 
     for version in versions.versions:
         # NOTE: You'll have to use relative imports
 
         _generate_versioned_directory(template_module, schemas, enums, version.date)
         _apply_migrations(version, schemas, enums)
 
-    base_package = template_module.__name__.split(".")[0]
-    for module_name, module_value in sys.modules.copy().items():
-        if module_name.startswith(base_package) and module_name in sys.modules:
-            importlib.reload(module_value)
+    current_package = template_module.__name__
+    while current_package != "":
+        importlib.reload(sys.modules[current_package])
+        current_package = ".".join(current_package.split(".")[:-1])
 
 
 def _apply_migrations(
     version: Version,
     schemas: dict[
         str,
         tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
@@ -83,29 +89,29 @@
 
             elif isinstance(field_change, OldSchemaFieldWas):
                 # TODO: Add a check that field actually exists (it's very necessary!)
                 model_field = field_name_to_field_model[field_change.field_name][1]
                 if field_change.type is not Sentinel:
                     if model_field.annotation == field_change.type:
                         raise InvalidGenerationInstructionError(
-                            f"You tried to change the type of field '{field_change.field_name}' to '{field_change.type}' in {schema.__name__} but it already has type '{model_field.annotation}'"
+                            f"You tried to change the type of field '{field_change.field_name}' to '{field_change.type}' in {schema.__name__} but it already has type '{model_field.annotation}'",
                         )
-                    setattr(model_field, "annotation", field_change.type)
-                    setattr(model_field, "type_", convert_generics(field_change.type))
-                    setattr(model_field, "outer_type_", field_change.type)
+                    model_field.annotation = field_change.type
+                    model_field.type_ = convert_generics(field_change.type)
+                    model_field.outer_type_ = field_change.type
                 field_info = model_field.field_info
 
                 if not isinstance(field_info, FieldInfo):
                     dict_of_field_info = {k: getattr(field_info, k) for k in field_info.__slots__}
                     if dict_of_field_info == dict_of_empty_field_info:
                         field_info = FieldInfo()
                         model_field.field_info = field_info
                     else:
                         raise InvalidGenerationInstructionError(
-                            f"You have defined a Field using pydantic.fields.Field but you must use universi.Field in {schema.__name__}"
+                            f"You have defined a Field using pydantic.fields.Field but you must use universi.Field in {schema.__name__}",
                         )
                 for attr_name in field_change.field_changes.__dataclass_fields__:
                     attr_value = getattr(field_change.field_changes, attr_name)
                     if attr_value is not Sentinel:
                         setattr(field_info, attr_name, attr_value)
                         field_info._universi_field_names.add(attr_name)
             elif isinstance(field_change, OldSchemaHadField):
@@ -131,15 +137,15 @@
         enum = alter_enum_instruction.enum
         enum_path = enum.__module__ + enum.__name__
         enum_member_to_value = enums[enum_path]
         if isinstance(alter_enum_instruction, EnumDidntHaveMembersInstruction):
             for member in alter_enum_instruction.members:
                 if member not in enum_member_to_value[1]:
                     raise InvalidGenerationInstructionError(
-                        f"Enum member '{member}' was not found in enum '{enum_path}'"
+                        f"Enum member '{member}' was not found in enum '{enum_path}'",
                     )
                 enum_member_to_value[1].pop(member)
         elif isinstance(alter_enum_instruction, EnumHadMembersInstruction):
             for member, member_value in alter_enum_instruction.members.items():
                 if member in enum_member_to_value[1] and enum_member_to_value[1][member] == member_value:
                     raise InvalidGenerationInstructionError(
                         f"Enum member '{member}' already exists in enum '{enum_path}' with the same value",
@@ -243,15 +249,18 @@
         raise CodeGenerationError("Failed to get source code for module") from e  # pragma: no cover
 
     if module.__name__.endswith(".__init__"):
         module_name = module.__name__.removesuffix(".__init__")
     else:
         module_name = module.__name__
     body = ast.Module(
-        [ast.ImportFrom(module="universi", names=[ast.alias(name="Field")], level=0)]
+        [
+            ast.ImportFrom(module="universi", names=[ast.alias(name="Field")], level=0),
+            ast.Import(names=[ast.alias(name="typing")], level=0),
+        ]
         + [
             _modify_cls(n, module_name, modified_schemas, modified_enums) if isinstance(n, ast.ClassDef) else n
             for n in parsed_file.body
         ],
         [],
     )
 
@@ -339,29 +348,28 @@
     else:
         return []
 
 
 # The following is based on by Samuel Colvin's devtools
 
 
-# TODO: Fully cover this with tests
 def custom_repr(value: Any) -> Any:
     if isinstance(value, list | tuple | set | frozenset):
         return PlainRepr(value.__class__(map(custom_repr, value)))
     if isinstance(value, dict):
         return PlainRepr(value.__class__((custom_repr(k), custom_repr(v)) for k, v in value.items()))
-    if isinstance(value, GenericAlias):
+    if isinstance(value, _BaseGenericAlias | GenericAlias):
         return f"{custom_repr(get_origin(value))}[{', '.join(custom_repr(a) for a in get_args(value))}]"
     if isinstance(value, type):
         return value.__name__
     if isinstance(value, Enum):
         return PlainRepr(f"{value.__class__.__name__}.{value.name}")
     if isinstance(value, auto):
         return PlainRepr("auto()")
-    if isinstance(value, LambdaType):
+    if isinstance(value, LambdaType) and LambdaFunctionName == value.__name__:
         return _find_a_lambda(inspect.getsource(value).strip())
     if inspect.isfunction(value):
         return PlainRepr(value.__name__)
     else:
         return PlainRepr(repr(value))
 
 
@@ -380,11 +388,11 @@
         if isinstance(node, ast.keyword) and node.arg == "default_factory" and isinstance(node.value, ast.Lambda):
             found_lambdas.append(node.value)
     if len(found_lambdas) == 1:
         return ast.unparse(found_lambdas[0])
     # These two errors are really hard to cover. Not sure if even possible, honestly :)
     elif len(found_lambdas) == 0:  # pragma: no cover
         raise InvalidGenerationInstructionError(
-            f"No lambda found in default_factory even though one was passed: {source}"
+            f"No lambda found in default_factory even though one was passed: {source}",
         )
     else:  # pragma: no cover
         raise InvalidGenerationInstructionError("More than one lambda found in default_factory. This is not supported.")
```

### Comparing `universi-0.2.0/universi/fields.py` & `universi-0.3.0/universi/fields.py`

 * *Files identical despite different names*

### Comparing `universi-0.2.0/universi/header.py` & `universi-0.3.0/universi/header.py`

 * *Files identical despite different names*

### Comparing `universi-0.2.0/universi/routing.py` & `universi-0.3.0/universi/routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 import datetime
+import functools
+import inspect
 from collections.abc import Callable
 from copy import deepcopy
 from enum import Enum
-import functools
-import inspect
 from pathlib import Path
-from types import GenericAlias, MappingProxyType, ModuleType
-from starlette.routing import request_response
+from threading import Lock
+from types import FunctionType, GenericAlias, MappingProxyType, ModuleType
 from typing import (
-    _SpecialForm,
-    Annotated,
     Any,
-    Collection,
-    ParamSpec,
     TypeVar,
+    _BaseGenericAlias,  # pyright: ignore
     cast,
     get_args,
     get_origin,
-    get_type_hints,
 )
-from typing_extensions import assert_never
+
 import fastapi.routing
-from fastapi.dependencies.utils import get_dependant, get_body_field, get_parameterless_sub_dependant
+from fastapi.dependencies.utils import get_body_field, get_dependant, get_parameterless_sub_dependant
+from fastapi.params import Depends
 from fastapi.routing import APIRoute
 from pydantic import BaseModel
 from starlette._utils import is_async_callable
 from starlette.routing import (
     BaseRoute,
+    request_response,
 )
 from starlette.routing import Mount as Mount  # noqa
-from typing_extensions import Self
+from typing_extensions import Self, assert_never
 
 from universi._utils import Sentinel, get_another_version_of_cls
 from universi.codegen import _get_versioned_schema_dir_name
-from universi.exceptions import RouterGenerationError, UniversiError
+from universi.exceptions import RouterGenerationError
 from universi.structure.common import Endpoint
 from universi.structure.endpoints import (
     EndpointDidntExistInstruction,
     EndpointExistedInstruction,
     EndpointHadInstruction,
 )
 from universi.structure.versions import Versions
-from fastapi.params import Depends
-from threading import Lock
-from typing import _BaseGenericAlias  # pyright: ignore
 
 _T = TypeVar("_T", bound=Callable[..., Any])
 annotation_resolution_lock = Lock()
 
 
 def same_definition_as_in(t: _T) -> Callable[[Callable], _T]:
     def decorator(f: Callable) -> _T:
@@ -91,36 +86,40 @@
         router = self
         for route in router.routes + router._deleted_routes:
             if isinstance(route, APIRoute):
                 if not is_async_callable(route.endpoint):
                     raise TypeError(
                         "All versioned endpoints must be asynchronous.",
                     )
-                route.endpoint = versions.versioned(route.endpoint)
+                route.endpoint = versions.versioned()(route.endpoint)
         routers = {}
         for version in versions.versions:
             if latest_schemas_module:
                 version_dir = _get_versioned_schema_dir_name(latest_schemas_module, version.date)
                 if not version_dir.is_dir():
                     raise RouterGenerationError(f"Versioned schema directory '{version_dir}' does not exist.")
                 for route in router.routes:
                     if isinstance(route, APIRoute):
                         if route.response_model is not None:
                             route.response_model = _change_versions_of_all_annotations(
-                                route.response_model, version_dir
+                                route.response_model,
+                                version_dir,
                             )
+                        # TODO: Write a test for this line
+                        route.dependencies = _change_versions_of_all_annotations(route.dependencies, version_dir)
                         route.endpoint = _change_versions_of_all_annotations(route.endpoint, version_dir)
                         route.dependant = get_dependant(path=route.path_format, call=route.endpoint)
                         route.body_field = get_body_field(dependant=route.dependant, name=route.unique_id)
                         for depends in route.dependencies[::-1]:
                             route.dependant.dependencies.insert(
                                 0,
                                 get_parameterless_sub_dependant(depends=depends, path=route.path_format),
                             )
                         route.app = request_response(route.get_route_handler())
+
             routers[version.date] = router
             router = deepcopy(router)
             for version_change in version.version_changes:
                 for instruction in version_change.alter_endpoint_instructions:
                     original_route_index = _get_route_index(
                         router.routes,
                         instruction.endpoint,
@@ -130,31 +129,31 @@
                             raise RouterGenerationError(
                                 f"Endpoint '{instruction.endpoint.__name__}' you tried to delete in '{version_change.__name__}' doesn't exist in new version",
                             )
                         router.routes.pop(original_route_index)
                     elif isinstance(instruction, EndpointExistedInstruction):
                         if original_route_index is not None:
                             raise RouterGenerationError(
-                                f"Endpoint '{instruction.endpoint.__name__}' you tried to re-create in '{version_change.__name__}' already existed in newer versions"
+                                f"Endpoint '{instruction.endpoint.__name__}' you tried to re-create in '{version_change.__name__}' already existed in newer versions",
                             )
                         deleted_route_index = _get_route_index(
                             router._deleted_routes,
                             instruction.endpoint,
                         )
                         if deleted_route_index is None:
                             raise RouterGenerationError(
-                                f"Endpoint '{instruction.endpoint.__name__}' you tried to re-create in '{version_change.__name__}' wasn't among the deleted routes"
+                                f"Endpoint '{instruction.endpoint.__name__}' you tried to re-create in '{version_change.__name__}' wasn't among the deleted routes",
                             )
                         router.routes.append(
                             router._deleted_routes.pop(deleted_route_index),
                         )
                     elif isinstance(instruction, EndpointHadInstruction):
                         if original_route_index is None:
                             raise RouterGenerationError(
-                                f"Endpoint '{instruction.endpoint.__name__}' you tried to delete in '{version_change.__name__}' doesn't exist in new version"
+                                f"Endpoint '{instruction.endpoint.__name__}' you tried to delete in '{version_change.__name__}' doesn't exist in new version",
                             )
                         route = router.routes[original_route_index]
                         for attr_name in instruction.attributes.__dataclass_fields__:
                             attr = getattr(instruction.attributes, attr_name)
                             if attr is not Sentinel:
                                 assert getattr(route, attr_name) != attr
                                 setattr(route, attr_name, attr)
@@ -163,59 +162,70 @@
         return routers
 
 
 def _change_versions_of_all_annotations(annotation: Any, version_dir: Path) -> Any:
     if isinstance(annotation, dict):
         return {
             _change_versions_of_all_annotations(key, version_dir): _change_versions_of_all_annotations(
-                value, version_dir
+                value,
+                version_dir,
             )
             for key, value in annotation.items()
         }
 
-    elif isinstance(annotation, (list, tuple)):
+    elif isinstance(annotation, list | tuple):
         return type(annotation)(_change_versions_of_all_annotations(v, version_dir) for v in annotation)
     else:
         return _memoized_change_versions_of_all_annotations(annotation, version_dir)
 
 
 # This cache is not here for speeding things up. It's for preventing the creation of copies of the same object
 # because such copies could produce weird behaviors at runtime, especially if you/fastapi do any comparisons.
 @functools.cache
 def _memoized_change_versions_of_all_annotations(annotation: Any, version_dir: Path) -> Any:
-    if isinstance(annotation, (_BaseGenericAlias, GenericAlias)):
+    if isinstance(annotation, _BaseGenericAlias | GenericAlias):
         return _change_versions_of_all_annotations(get_origin(annotation), version_dir)[
             tuple(_change_versions_of_all_annotations(arg, version_dir) for arg in get_args(annotation))
         ]
     elif isinstance(annotation, Depends):
         return Depends(
-            _change_versions_of_all_annotations(annotation.dependency, version_dir), use_cache=annotation.use_cache
+            _change_versions_of_all_annotations(annotation.dependency, version_dir),
+            use_cache=annotation.use_cache,
         )
     elif isinstance(annotation, type):
-        if issubclass(annotation, (BaseModel, Enum)):
+        if issubclass(annotation, BaseModel | Enum):
             return get_another_version_of_cls(annotation, version_dir)
         else:
             return annotation
-    # TODO: We need memoization for callables. Otherwise we're gonna get in trouble
-    elif getattr(annotation, "__call__", None) is not None:
+    elif callable(annotation):
         if inspect.iscoroutinefunction(annotation):
 
             @functools.wraps(annotation)
-            async def new_callable(*args: Any, **kwargs: Any) -> Any:
+            async def new_callable(  # pyright: ignore[reportGeneralTypeIssues]
+                *args: Any,
+                **kwargs: Any,
+            ) -> Any:
                 return await annotation(*args, **kwargs)
 
         else:
 
             @functools.wraps(annotation)
-            def new_callable(*args: Any, **kwargs: Any) -> Any:
+            def new_callable(  # pyright: ignore[reportGeneralTypeIssues]
+                *args: Any,
+                **kwargs: Any,
+            ) -> Any:
                 return annotation(*args, **kwargs)
 
+        # Otherwise it will have the same signature as __wrapped__
         del new_callable.__wrapped__
         old_params = inspect.signature(annotation).parameters
-        new_callable.__annotations__ = _change_versions_of_all_annotations(new_callable.__annotations__, version_dir)
+        callable_annotations = new_callable.__annotations__
+
+        new_callable: Any = cast(Any, new_callable)
+        new_callable.__annotations__ = _change_versions_of_all_annotations(callable_annotations, version_dir)
         new_callable.__defaults__ = _change_versions_of_all_annotations(
             tuple(p.default for p in old_params.values() if p.default is not inspect.Signature.empty),
             version_dir=version_dir,
         )
         new_callable.__signature__ = _generate_signature(new_callable, old_params)
         return new_callable
     else:
@@ -233,15 +243,15 @@
             default = inspect.Signature.empty
         parameters.append(
             inspect.Parameter(
                 param.name,
                 param.kind,
                 default=default,
                 annotation=new_callable.__annotations__.get(param.name, inspect.Signature.empty),
-            )
+            ),
         )
     return inspect.Signature(
         parameters=parameters,
         return_annotation=new_callable.__annotations__.get("return", inspect.Signature.empty),
     )
```

### Comparing `universi-0.2.0/universi/structure/endpoints.py` & `universi-0.3.0/universi/structure/endpoints.py`

 * *Files identical despite different names*

### Comparing `universi-0.2.0/universi/structure/enums.py` & `universi-0.3.0/universi/structure/enums.py`

 * *Files identical despite different names*

### Comparing `universi-0.2.0/universi/structure/responses.py` & `universi-0.3.0/universi/structure/responses.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,29 @@
 @dataclass
 class AlterResponseInstruction:
     endpoints: tuple[Endpoint, ...]
     method: Callable[[type, dict[str, Any]], None]
     owner: type = field(init=False)
 
     def __post_init__(self):
-        assert inspect.signature(self.method).return_annotation is None
-        assert (
-            len(inspect.signature(self.method).parameters) == 2
-        ), f"Method {self.method.__name__} must have 2 parameters: cls and data"
-        annotation = inspect.signature(self.method).parameters["data"].annotation
-        assert annotation == dict[str, Any], annotation
+        signature = inspect.signature(self.method)
+        if list(signature.parameters) != ["cls", "data"]:
+            raise ValueError(f"Method '{self.method.__name__}' must have 2 parameters: cls and data")
 
         functools.update_wrapper(self, self.method)
 
     def __set_name__(self, owner, name):
         self.owner = owner
 
     def __call__(self, data: dict[str, Any]) -> None:
         return self.method(self.owner, data)
 
 
 def convert_response_to_previous_version_for(
-    first_endpoint: Endpoint, /, *other_endpoints: Endpoint,
+    first_endpoint: Endpoint,
+    /,
+    *other_endpoints: Endpoint,
 ) -> "type[classmethod[Any, _P, None]]":
     def decorator(method: Callable[[object, dict[str, Any]], None]) -> Any:
         return AlterResponseInstruction((first_endpoint, *other_endpoints), method)
 
     return decorator  # pyright: ignore[reportGeneralTypeIssues]
```

### Comparing `universi-0.2.0/universi/structure/schemas.py` & `universi-0.3.0/universi/structure/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     type: type
     field: FieldInfo
 
 
 @dataclass(slots=True)
 class AlterSchemaSubInstructionFactory:
     name: str
-    # TODO: Add a validation to linter to check that field actually changed
+    # TODO: Add a validation  to check that field actually changed
 
     def had(
         self,
         *,
         type: Any = Sentinel,
         default: Any = Sentinel,
         default_factory: Callable = Sentinel,
```

### Comparing `universi-0.2.0/universi/structure/versions.py` & `universi-0.3.0/universi/structure/versions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,59 @@
-from contextvars import ContextVar
 import datetime
 import functools
 from collections.abc import Callable, Sequence
+from contextvars import ContextVar
 from enum import Enum
-from typing import Any, ClassVar, ParamSpec, TypeAlias, TypeVar, overload
+from typing import Any, ClassVar, ParamSpec, TypeAlias, TypeVar
 
 from fastapi.routing import _prepare_response_content
-from universi.exceptions import UniversiStructureError
 
+from universi.exceptions import UniversiStructureError
 from universi.header import api_version_var
 from universi.structure.endpoints import AlterEndpointSubInstruction
 from universi.structure.enums import AlterEnumSubInstruction
 
 from .._utils import Sentinel
 from .common import Endpoint, VersionedModel
 from .responses import AlterResponseInstruction
 from .schemas import AlterSchemaInstruction
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 VersionDate: TypeAlias = datetime.date
+PossibleInstructions: TypeAlias = AlterSchemaInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
 
 
 class AbstractVersionChange:
     side_effects: ClassVar[bool] = False
     description: ClassVar[str] = Sentinel
-    instructions_to_migrate_to_previous_version: ClassVar[
-        Sequence[AlterSchemaInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction]
-    ] = Sentinel
+    instructions_to_migrate_to_previous_version: ClassVar[Sequence[PossibleInstructions]] = Sentinel
     alter_schema_instructions: ClassVar[Sequence[AlterSchemaInstruction]] = Sentinel
     alter_enum_instructions: ClassVar[Sequence[AlterEnumSubInstruction]] = Sentinel
     alter_endpoint_instructions: ClassVar[Sequence[AlterEndpointSubInstruction]] = Sentinel
     alter_response_instructions: ClassVar[dict[Endpoint, AlterResponseInstruction]] = Sentinel
 
     def __init_subclass__(cls) -> None:
-        assert isinstance(cls.side_effects, bool)
+        if not isinstance(cls.side_effects, bool):
+            raise UniversiStructureError(f"Side effects must be bool. Found: {type(cls.side_effects)}")
         if cls.description is Sentinel:
             raise UniversiStructureError(f"Version change description is not set on '{cls.__name__}' but is required.")
         if cls.instructions_to_migrate_to_previous_version is Sentinel:
             raise UniversiStructureError(
                 f"Attribute 'instructions_to_migrate_to_previous_version' is not set on '{cls.__name__}' but is required.",
             )
         if not isinstance(cls.instructions_to_migrate_to_previous_version, Sequence):
             raise UniversiStructureError(
                 f"Attribute 'instructions_to_migrate_to_previous_version' must be a sequence in '{cls.__name__}'.",
             )
+        for instruction in cls.instructions_to_migrate_to_previous_version:
+            if not isinstance(instruction, PossibleInstructions):
+                raise UniversiStructureError(
+                    f"Instruction '{instruction}' is not allowed. Please, use the correct instruction types",
+                )
         for attr_name, attr_value in cls.__dict__.items():
             if not isinstance(attr_value, AlterResponseInstruction) and attr_name not in {
                 "description",
                 "side_effects",
                 "instructions_to_migrate_to_previous_version",
                 "__module__",
                 "__doc__",
@@ -71,17 +76,19 @@
             endpoint: instruction
             for instruction in cls.__dict__.values()
             if isinstance(instruction, AlterResponseInstruction)
             for endpoint in instruction.endpoints
         }
         repetitions = set()
         for alter_instruction in cls.alter_schema_instructions:
-            assert (
-                alter_instruction.schema not in repetitions
-            ), f"Model {alter_instruction.schema} got repeated. Please, merge these instructions."
+            if alter_instruction.schema in repetitions:
+                raise UniversiStructureError(
+                    f"'{alter_instruction.schema.__name__}' got repeated in multiple instructions. "
+                    "Please, merge these instructions.",
+                )
             repetitions.add(alter_instruction.schema)
 
         if cls.mro() != [cls, AbstractVersionChange, object]:
             raise TypeError(
                 f"Can't subclass {cls.__name__} as it was never meant to be subclassed.",
             )
 
@@ -131,15 +138,15 @@
     @functools.cached_property
     def _version_changes_to_version_mapping(self) -> dict[type[AbstractVersionChange], VersionDate]:
         return {version_change: version.date for version in self.versions for version_change in version.version_changes}
 
     def is_active(self, version_change: type[AbstractVersionChange]) -> bool:
         api_version = self.api_version_var.get()
         if api_version is None:
-            return False
+            return True
         return self._version_changes_to_version_mapping[version_change] <= api_version
 
     # TODO: It might need caching for iteration to speed it up
     def data_to_version(
         self,
         endpoint: Endpoint,
         data: dict[str, Any],
@@ -149,63 +156,41 @@
             if v.date <= version:
                 break
             for version_change in v.version_changes:
                 if endpoint in version_change.alter_response_instructions:
                     version_change.alter_response_instructions[endpoint](data)
         return data
 
-    @overload
-    def versioned(self, endpoint: Endpoint[_P, _R]) -> Endpoint[_P, _R]:
-        ...
-
-    @overload
-    def versioned(
-        self,
-        endpoint: None = None,
-    ) -> Callable[[Endpoint[_P, _R]], Endpoint[_P, _R]]:
-        ...
-
     def versioned(
         self,
         endpoint: Endpoint | None = None,
-    ) -> Callable[[Endpoint[_P, _R]], Endpoint[_P, _R]] | Endpoint[_P, _R]:
-        if endpoint is not None:
-
-            @functools.wraps(endpoint)
-            async def decorator(*args: _P.args, **kwargs: _P.kwargs) -> _R:
-                return await self._convert_endpoint_response_to_version(
-                    endpoint,
-                    args,
-                    kwargs,
-                )
-
-            decorator.func = endpoint  # pyright: ignore[reportGeneralTypeIssues]
-            return decorator
-
-        def wrapper(endpoint: Endpoint[_P, _R]) -> Endpoint[_P, _R]:
-            @functools.wraps(endpoint)
+    ) -> Callable[[Endpoint[_P, _R]], Endpoint[_P, _R]]:
+        def wrapper(func: Endpoint[_P, _R]) -> Endpoint[_P, _R]:
+            @functools.wraps(func)
             async def decorator(*args: _P.args, **kwargs: _P.kwargs) -> _R:
                 return await self._convert_endpoint_response_to_version(
-                    endpoint,
+                    func,
+                    endpoint or func,
                     args,
                     kwargs,
                 )
 
-            decorator.func = endpoint  # pyright: ignore[reportGeneralTypeIssues]
+            decorator.func = func  # pyright: ignore[reportGeneralTypeIssues]
             return decorator
 
         return wrapper
 
     async def _convert_endpoint_response_to_version(
         self,
+        func_to_get_response_from: Endpoint,
         endpoint: Endpoint,
         args: tuple[Any, ...],
         kwargs: dict[str, Any],
     ) -> Any:
-        response = await endpoint(*args, **kwargs)
+        response = await func_to_get_response_from(*args, **kwargs)
         api_version = self.api_version_var.get()
         if api_version is None:
             return response
         # TODO We probably need to call this in the same way as in fastapi instead of hardcoding exclude_unset.
         # We have such an ability if we force passing the route into this wrapper. Or maybe not... Important!
         response = _prepare_response_content(response, exclude_unset=False)
         return self.data_to_version(endpoint, response, api_version)
```

### Comparing `universi-0.2.0/setup.py` & `universi-0.3.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['fastapi>=0.96.1',
  'type-inspector>=1.2.2,<2.0.0',
  'typer[all]',
  'typing-extensions']
 
 setup_kwargs = {
     'name': 'universi',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
-    'long_description': '# universi\n\nPackage description\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n',
+    'long_description': '# universi\n\nPackage description\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n\n<!---\n# TODO: Note that we don\'t handle "from .schemas import Schema as OtherSchema" case\n# TODO: Need to validate that the user doesn\'t use versioned schemas instead of the latest ones\n-->',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ovsyanka83/universi',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['universi',
 'universi.structure'] package_data = \ {'': ['*']} install_requires = \
 ['fastapi>=0.96.1', 'type-inspector>=1.2.2,<2.0.0', 'typer[all]', 'typing-
-extensions'] setup_kwargs = { 'name': 'universi', 'version': '0.2.0',
+extensions'] setup_kwargs = { 'name': 'universi', 'version': '0.3.0',
 'description': '', 'long_description': '# universi\n\nPackage description\n\n--
 -\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
-\n\n## Installation\n\n```bash\npip install universi\n```\n', 'author':
+\n\n## Installation\n\n```bash\npip install universi\n```\n\n', 'author':
 'Stanislav Zmiev', 'author_email': 'szmiev2000@gmail.com', 'maintainer':
 'None', 'maintainer_email': 'None', 'url': 'https://github.com/ovsyanka83/
 universi', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
 (**setup_kwargs)
```

