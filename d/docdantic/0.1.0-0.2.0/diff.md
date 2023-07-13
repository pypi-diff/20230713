# Comparing `tmp/docdantic-0.1.0-py3-none-any.whl.zip` & `tmp/docdantic-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5480 bytes, number of entries: 6
--rw-r--r--  2.0 unx     7290 b- defN 80-Jan-01 00:00 docdantic/__init__.py
+Zip file size: 5759 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     7844 b- defN 80-Jan-01 00:00 docdantic/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 docdantic/py.typed
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 docdantic-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3040 b- defN 80-Jan-01 00:00 docdantic-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 docdantic-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      452 b- defN 16-Jan-01 00:00 docdantic-0.1.0.dist-info/RECORD
-6 files, 11936 bytes uncompressed, 4664 bytes compressed:  60.9%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 docdantic-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3467 b- defN 80-Jan-01 00:00 docdantic-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 docdantic-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      452 b- defN 16-Jan-01 00:00 docdantic-0.2.0.dist-info/RECORD
+6 files, 12917 bytes uncompressed, 4943 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: docdantic/__init__.py
 Comment: 
 
 Filename: docdantic/py.typed
 Comment: 
 
-Filename: docdantic-0.1.0.dist-info/LICENSE
+Filename: docdantic-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: docdantic-0.1.0.dist-info/METADATA
+Filename: docdantic-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: docdantic-0.1.0.dist-info/WHEEL
+Filename: docdantic-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: docdantic-0.1.0.dist-info/RECORD
+Filename: docdantic-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docdantic/__init__.py

```diff
@@ -1,20 +1,30 @@
 import re
 import tabulate
-import json
 import importlib
+import json
 from importlib.metadata import version
 from collections import namedtuple
-from pydantic import BaseModel
-from pydantic.fields import FieldInfo
-from pydantic_core import PydanticUndefined
 from markdown import Markdown
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
-from typing import Type, Any
+from pydantic.version import VERSION as PYDANTIC_VERSION
+from pydantic import BaseModel
+from typing import Any, Type
+
+if PYDANTIC_VERSION.startswith("1."):
+    from pydantic.fields import Undefined as PydanticUndefined  # type: ignore
+    _model_dump = lambda model, *args, **kwargs: model.dict(*args, **kwargs)
+    _get_field_annotation = lambda field: field.type_
+    _get_required = lambda field: field.required
+else:
+    from pydantic_core import PydanticUndefined  # type: ignore
+    _model_dump = lambda model, *args, **kwargs: model.model_dump(*args, **kwargs)
+    _get_field_annotation = lambda field: field.annotation
+    _get_required = lambda field: field.is_required()
 
 __version__ = version(__package__)
 ModelFieldInfo = namedtuple("ModelFieldInfo", "name type required default")
 
 
 def is_pydantic_model(obj: Type | None) -> bool:
     """
@@ -28,43 +38,14 @@
     if isinstance(obj, (list, tuple)):
         return any(is_pydantic_model(o) for o in obj)
     if isinstance(obj, type) and issubclass(obj, BaseModel):
         return True
     return False
 
 
-def get_default_string(field: FieldInfo):
-    """
-    Get a string representation of the default value of a field.
-
-    :param field: Field to process.
-    :return: String representation of the default value.
-    """
-    if field.default == PydanticUndefined:
-        return "..."
-    elif field.default is not None and is_pydantic_model(field.default):
-        return str(field.default.model_dump())
-    elif field.default is not None:
-        return str(field.default)
-    else:
-        return ""
-
-def get_annotation_string(field: FieldInfo):
-    """
-    Get a string representation of the field's type annotation.
-
-    :param field: Field to process.
-    :return: String representation of the field's annotation.
-    """
-    if field.annotation is None:
-        return "None"
-
-    return str(field.annotation.__name__)
-
-
 def submodel_link(sub_model: str):
     """
     Create a Markdown link to the given submodel.
 
     :param sub_model: Name of the submodel.
     :return: Markdown link to the submodel.
     """
@@ -99,50 +80,14 @@
         module = importlib.import_module(module_name)
     except ModuleNotFoundError:
         return None
 
     return getattr(module, class_name, None)
 
 
-def get_field_info(model: Any, config: dict = {}, models: dict | None = None):
-    """
-    Get information about the fields of a model.
-
-    :param model: The model to inspect.
-    :param config: Configuration for the inspection.
-    :param models: Already inspected models to avoid circular references.
-    :return: A dictionary with the model's field information.
-    """
-    if models is None:
-        models = {}
-
-    fields: list[ModelFieldInfo] = []
-    model_name = model.__name__
-    models[model_name] = fields
-
-    for name, field in model.__fields__.items():
-        if model_name in config.get("exclude", {}) and name in config["exclude"][model_name]:
-            # Skip fields that are explicitly excluded
-            continue
-
-        annotation = get_annotation_string(field)
-        default = get_default_string(field)
-        required = str(field.is_required())
-
-        if is_pydantic_model(field.annotation):
-            annotation = submodel_link(annotation)
-            get_field_info(field.annotation, config, models)
-
-        fields.append(
-            ModelFieldInfo(highlight_name(name), annotation, required, default)
-        )
-
-    return models
-
-
 def extract_configuration(index, lines):
     """
     Extract configuration from the lines.
 
     :param index: Current index in the lines.
     :param lines: All lines of the document.
     :return: Configuration and new index.
@@ -169,14 +114,80 @@
         except json.JSONDecodeError:
             index += 1  # Continue if the JSON is not yet fully extracted
             continue  # If the current JSON string is not valid, ignore it and continue
 
     return config, index
 
 
+def get_default_string(default: Any):
+    """
+    Get a string representation of the default value of a field.
+
+    :param field: Field to process.
+    :return: String representation of the default value.
+    """
+    if default == PydanticUndefined:
+        return "..."
+    elif default is not None and is_pydantic_model(default):
+        return str(_model_dump(default))
+    elif default is not None:
+        return str(default)
+    else:
+        return ""
+
+def get_annotation_string(annotation: Any):
+    """
+    Get a string representation of the annotation of a field.
+
+    :param annotation: Annotation to process.
+    :return: String representation of the annotation.
+    """
+    if annotation is None:
+        return "None"
+
+    return str(annotation.__name__)
+
+
+def get_field_info(model: Any, config: dict = {}, models: dict | None = None):
+    """
+    Get information about the fields of a model.
+
+    :param model: The model to inspect.
+    :param config: Configuration for the inspection.
+    :param models: Already inspected models to avoid circular references.
+    :return: A dictionary with the model's field information.
+    """
+    if models is None:
+        models = {}
+
+    fields: list[ModelFieldInfo] = []
+    model_name = model.__name__
+    models[model_name] = fields
+
+    for name, field in model.__fields__.items():
+        if model_name in config.get("exclude", {}) and name in config["exclude"][model_name]:
+            # Skip fields that are explicitly excluded
+            continue
+
+        annotation = _get_field_annotation(field)
+        annotation_str = get_annotation_string(annotation)
+        default = get_default_string(field.default)
+        required = str(_get_required(field))
+
+        if is_pydantic_model(annotation):
+            annotation_str = submodel_link(annotation_str)
+            get_field_info(annotation, config, models)
+
+        fields.append(
+            ModelFieldInfo(highlight_name(name), annotation_str, required, default)
+        )
+
+    return models
+
+
 def render_table(model_path: str, config: dict) -> str:
     """
     Render a table with the fields of a model.
 
     :param model_path: Full path to the model.
     :param config: Configuration for the generation.
     :return: Rendered table or an empty string if the model was not found.
```

## Comparing `docdantic-0.1.0.dist-info/LICENSE` & `docdantic-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `docdantic-0.1.0.dist-info/METADATA` & `docdantic-0.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: docdantic
-Version: 0.1.0
+Version: 0.2.0
 Summary: A markdown plugin for generating docs from Pydantic models
 Home-page: https://gitlab.com/emergentmethods/docdantic
 License: MIT
 Author: Tim Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: markdown (==3.3.7)
-Requires-Dist: pydantic (==2.0.2)
+Requires-Dist: markdown (>=3.3.7,<4.0.0)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://gitlab.com/emergentmethods/docdantic
 Description-Content-Type: text/markdown
 
 # Docdantic
 
+![Gitlab code coverage (specific job)](https://img.shields.io/gitlab/pipeline-coverage/emergentmethods/docdantic?branch=main&job_name=unit-tests&style=flat-square)
+![GitLab Release (latest by SemVer)](https://img.shields.io/gitlab/v/release/emergentmethods/docdantic?style=flat-square)
+![GitLab](https://img.shields.io/gitlab/license/emergentmethods/docdantic?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docdantic?style=flat-square)
 
-Docdantic is a Python library that enables the automatic generation of Markdown documentation from Pydantic v2 models. It works as an extension of the Markdown package, extracting model details and creating neat tables with model fields and their properties.
+Docdantic is a Python library that enables the automatic generation of Markdown documentation from Pydantic models. It works as an extension of the Markdown package, extracting model details and creating neat tables with model fields and their properties.
 
 
 ## Features
 
-* Automatically generate tables of Pydantic v2 model fields with their details (name, type, required, default).
-* Supports nested Pydantic v2 models.
+* Supports both Pydantic V1 and V2 models.
+* Automatically generate tables of Pydantic model fields with their details (name, type, required, default).
+* Supports nested Pydantic models.
 * Configurable exclusion of specific fields from the documentation.
 
 
 ## Installation
 
 ```bash
 pip install docdantic
```

