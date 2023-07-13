# Comparing `tmp/grai_schemas-0.2.0a6.tar.gz` & `tmp/grai_schemas-0.2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.2.0a6.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a7.tar", max compression
```

## Comparing `grai_schemas-0.2.0a6.tar` & `grai_schemas-0.2.0a7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3793 2023-05-26 18:12:59.756317 grai_schemas-0.2.0a6/LICENSE
--rw-r--r--   0        0        0      322 2023-05-26 18:12:59.756709 grai_schemas-0.2.0a6/README.md
--rw-r--r--   0        0        0      885 2023-07-13 18:46:06.842419 grai_schemas-0.2.0a6/pyproject.toml
--rw-r--r--   0        0        0      210 2023-07-13 18:46:06.848140 grai_schemas-0.2.0a6/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      848 2023-07-10 15:57:25.736802 grai_schemas-0.2.0a6/src/grai_schemas/base.py
--rw-r--r--   0        0        0     3528 2023-07-13 17:22:30.699125 grai_schemas-0.2.0a6/src/grai_schemas/generics.py
--rw-r--r--   0        0        0    41788 2023-06-14 21:10:34.453210 grai_schemas-0.2.0a6/src/grai_schemas/human_ids.py
--rw-r--r--   0        0        0      175 2023-06-01 16:01:43.271004 grai_schemas-0.2.0a6/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-05-26 18:12:59.757931 grai_schemas-0.2.0a6/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      669 2023-07-10 15:57:25.737338 grai_schemas-0.2.0a6/src/grai_schemas/schema.py
--rw-r--r--   0        0        0     2564 2023-07-10 15:57:25.737534 grai_schemas-0.2.0a6/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      451 2023-07-10 15:57:25.737795 grai_schemas-0.2.0a6/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     3737 2023-07-13 16:32:19.161602 grai_schemas-0.2.0a6/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0      845 2023-07-10 15:57:25.738097 grai_schemas-0.2.0a6/src/grai_schemas/v1/events.py
--rw-r--r--   0        0        0      793 2023-07-10 15:57:25.738417 grai_schemas-0.2.0a6/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0     1738 2023-07-10 15:57:25.738789 grai_schemas-0.2.0a6/src/grai_schemas/v1/merge.py
--rw-r--r--   0        0        0      279 2023-06-15 00:41:57.158195 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     2179 2023-07-10 15:57:25.739070 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      240 2023-07-10 15:57:25.739286 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/generics.py
--rw-r--r--   0        0        0     1009 2023-07-13 18:27:40.465906 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     2228 2023-07-11 00:38:07.412504 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     7034 2023-07-13 18:36:46.290173 grai_schemas-0.2.0a6/src/grai_schemas/v1/mock.py
--rw-r--r--   0        0        0     3727 2023-07-13 16:32:19.172713 grai_schemas-0.2.0a6/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0      940 2023-07-10 15:57:25.740065 grai_schemas-0.2.0a6/src/grai_schemas/v1/organization.py
--rw-r--r--   0        0        0     1203 2023-07-10 15:57:25.740281 grai_schemas-0.2.0a6/src/grai_schemas/v1/source.py
--rw-r--r--   0        0        0     3696 2023-07-10 15:57:25.740372 grai_schemas-0.2.0a6/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a6/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-05-26 18:12:59.756317 grai_schemas-0.2.0a7/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-26 18:12:59.756709 grai_schemas-0.2.0a7/README.md
+-rw-r--r--   0        0        0      885 2023-07-13 19:26:09.667557 grai_schemas-0.2.0a7/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-07-13 19:26:09.672297 grai_schemas-0.2.0a7/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      848 2023-07-10 15:57:25.736802 grai_schemas-0.2.0a7/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3618 2023-07-13 19:24:12.951398 grai_schemas-0.2.0a7/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-14 21:10:34.453210 grai_schemas-0.2.0a7/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-01 16:01:43.271004 grai_schemas-0.2.0a7/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:59.757931 grai_schemas-0.2.0a7/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      669 2023-07-10 15:57:25.737338 grai_schemas-0.2.0a7/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2564 2023-07-10 15:57:25.737534 grai_schemas-0.2.0a7/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      451 2023-07-10 15:57:25.737795 grai_schemas-0.2.0a7/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     3737 2023-07-13 16:32:19.161602 grai_schemas-0.2.0a7/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:57:25.738097 grai_schemas-0.2.0a7/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      793 2023-07-10 15:57:25.738417 grai_schemas-0.2.0a7/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0     1738 2023-07-10 15:57:25.738789 grai_schemas-0.2.0a7/src/grai_schemas/v1/merge.py
+-rw-r--r--   0        0        0      279 2023-06-15 00:41:57.158195 grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2179 2023-07-10 15:57:25.739070 grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      240 2023-07-10 15:57:25.739286 grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0      928 2023-07-13 19:24:12.948758 grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     2228 2023-07-11 00:38:07.412504 grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     7035 2023-07-13 18:46:32.818119 grai_schemas-0.2.0a7/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     3727 2023-07-13 16:32:19.172713 grai_schemas-0.2.0a7/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-07-10 15:57:25.740065 grai_schemas-0.2.0a7/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1203 2023-07-10 15:57:25.740281 grai_schemas-0.2.0a7/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3696 2023-07-10 15:57:25.740372 grai_schemas-0.2.0a7/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a7/PKG-INFO
```

### Comparing `grai_schemas-0.2.0a6/LICENSE` & `grai_schemas-0.2.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/pyproject.toml` & `grai_schemas-0.2.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.2.0-alpha6"
+version = "0.2.0-alpha7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
```

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/base.py` & `grai_schemas-0.2.0a7/src/grai_schemas/base.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/generics.py` & `grai_schemas-0.2.0a7/src/grai_schemas/generics.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,20 @@
         validate_assignment = True
         validate_all = True
 
 
 class Metadata(GraiBaseModel):
     pass
 
+    class Config:
+        """ """
+
+        extra = "allow"
+        allow_mutation = True
+
 
 class MalformedMetadata(GraiBaseModel):
     """ """
 
     malformed_values: Dict = {}
 
     @root_validator(pre=True)
```

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/human_ids.py` & `grai_schemas-0.2.0a7/src/grai_schemas/human_ids.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/schema.py` & `grai_schemas-0.2.0a7/src/grai_schemas/schema.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/utilities.py` & `grai_schemas-0.2.0a7/src/grai_schemas/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/edge.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/edge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/events.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/events.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/merge.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/merge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/edges.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/metadata.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, Optional, Union
+from uuid import UUID
 
 from grai_schemas.generics import GraiBaseModel, MalformedMetadata, Metadata
 from grai_schemas.utilities import merge
 from grai_schemas.v1.metadata import edges, nodes
-from uuid import UUID
+
 
 class GraiMetadataV1(Metadata):
     """ """
 
     grai: Union[edges.Metadata, nodes.Metadata]
 
 
@@ -15,21 +16,15 @@
     """"""
 
     sources: Dict[UUID, GraiMetadataV1]
 
 
 class MetadataV1(GraiMetadataV1, SourcesMetadataV1):
     """ """
-
-    class Config:
-        """ """
-
-        extra = "allow"
-        allow_mutation = True
-
+    pass
 
 class GraiMalformedNodeMetadataV1(MalformedMetadata, MetadataV1):
     """ """
 
     grai: nodes.MalformedNodeMetadataV1 = nodes.MalformedNodeMetadataV1()  # type: ignore
     sources: Dict[UUID, GraiMetadataV1] = {}
```

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/metadata/nodes.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/mock.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/mock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import uuid
-from typing import Dict, Type, Any, Generic, TypeVar
+from typing import Any, Dict, Generic, Type, TypeVar
 
+from grai_schemas.generics import DefaultValue
 from grai_schemas.human_ids import get_human_id
 from grai_schemas.v1.edge import EdgeV1
 from grai_schemas.v1.edge import IDSourceSpec as EdgeIDSourceSpec
 from grai_schemas.v1.edge import IDSpec as EdgeIDSpec
 from grai_schemas.v1.edge import NamedSourceSpec as NamedEdgeSourceSpec
 from grai_schemas.v1.edge import NamedSpec as NamedEdgeSpec
 from grai_schemas.v1.edge import SourcedEdgeSpec, SourcedEdgeV1
@@ -17,18 +18,18 @@
     NodeV1,
     SourcedNodeSpec,
     SourcedNodeV1,
 )
 from grai_schemas.v1.organization import OrganisationSpec, OrganisationV1
 from grai_schemas.v1.source import SourceSpec, SourceV1
 from grai_schemas.v1.workspace import WorkspaceSpec, WorkspaceV1
-from polyfactory.factories.pydantic_factory import ModelFactory
 from polyfactory import Ignore, PostGenerated
-from grai_schemas.generics import DefaultValue
 from polyfactory.decorators import post_generated
+from polyfactory.factories.pydantic_factory import ModelFactory
+
 T = TypeVar("T")
 
 
 class DefaultValueFactory(ModelFactory[DefaultValue]):
     __model__ = DefaultValue
     __set_as_default_factory_for_type__ = True
```

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/node.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/node.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/organization.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/organization.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/source.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/source.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/src/grai_schemas/v1/workspace.py` & `grai_schemas-0.2.0a7/src/grai_schemas/v1/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a6/PKG-INFO` & `grai_schemas-0.2.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

