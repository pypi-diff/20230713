# Comparing `tmp/grai_schemas-0.2.0a5.tar.gz` & `tmp/grai_schemas-0.2.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.2.0a5.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a6.tar", max compression
```

## Comparing `grai_schemas-0.2.0a5.tar` & `grai_schemas-0.2.0a6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a5/LICENSE
--rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a5/README.md
--rw-r--r--   0        0        0      862 2023-07-11 10:27:21.769257 grai_schemas-0.2.0a5/pyproject.toml
--rw-r--r--   0        0        0      210 2023-07-11 10:27:28.122212 grai_schemas-0.2.0a5/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      848 2023-07-11 08:47:36.928111 grai_schemas-0.2.0a5/src/grai_schemas/base.py
--rw-r--r--   0        0        0     3757 2023-07-11 08:47:36.928239 grai_schemas-0.2.0a5/src/grai_schemas/generics.py
--rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a5/src/grai_schemas/human_ids.py
--rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a5/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a5/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      669 2023-07-11 08:47:36.929249 grai_schemas-0.2.0a5/src/grai_schemas/schema.py
--rw-r--r--   0        0        0     2564 2023-07-11 08:47:36.929380 grai_schemas-0.2.0a5/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      451 2023-07-11 08:47:36.929506 grai_schemas-0.2.0a5/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     2786 2023-07-11 08:47:36.929628 grai_schemas-0.2.0a5/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0      845 2023-07-11 08:47:36.929712 grai_schemas-0.2.0a5/src/grai_schemas/v1/events.py
--rw-r--r--   0        0        0      793 2023-07-11 08:47:36.929837 grai_schemas-0.2.0a5/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0     1738 2023-07-11 08:47:36.929909 grai_schemas-0.2.0a5/src/grai_schemas/v1/merge.py
--rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     2179 2023-07-11 08:47:36.930042 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      240 2023-07-11 08:47:36.930143 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/generics.py
--rw-r--r--   0        0        0      784 2023-07-11 08:47:36.930249 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     2228 2023-07-11 08:47:41.704120 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     6925 2023-07-11 08:47:36.935588 grai_schemas-0.2.0a5/src/grai_schemas/v1/mock.py
--rw-r--r--   0        0        0     2776 2023-07-11 08:47:36.935745 grai_schemas-0.2.0a5/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0      940 2023-07-11 08:47:36.935826 grai_schemas-0.2.0a5/src/grai_schemas/v1/organization.py
--rw-r--r--   0        0        0     1203 2023-07-11 08:47:36.936153 grai_schemas-0.2.0a5/src/grai_schemas/v1/source.py
--rw-r--r--   0        0        0     3696 2023-07-11 08:47:36.936896 grai_schemas-0.2.0a5/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a5/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-05-26 18:12:59.756317 grai_schemas-0.2.0a6/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-26 18:12:59.756709 grai_schemas-0.2.0a6/README.md
+-rw-r--r--   0        0        0      885 2023-07-13 18:46:06.842419 grai_schemas-0.2.0a6/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-07-13 18:46:06.848140 grai_schemas-0.2.0a6/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      848 2023-07-10 15:57:25.736802 grai_schemas-0.2.0a6/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3528 2023-07-13 17:22:30.699125 grai_schemas-0.2.0a6/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-14 21:10:34.453210 grai_schemas-0.2.0a6/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-01 16:01:43.271004 grai_schemas-0.2.0a6/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:59.757931 grai_schemas-0.2.0a6/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      669 2023-07-10 15:57:25.737338 grai_schemas-0.2.0a6/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2564 2023-07-10 15:57:25.737534 grai_schemas-0.2.0a6/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      451 2023-07-10 15:57:25.737795 grai_schemas-0.2.0a6/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     3737 2023-07-13 16:32:19.161602 grai_schemas-0.2.0a6/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:57:25.738097 grai_schemas-0.2.0a6/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      793 2023-07-10 15:57:25.738417 grai_schemas-0.2.0a6/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0     1738 2023-07-10 15:57:25.738789 grai_schemas-0.2.0a6/src/grai_schemas/v1/merge.py
+-rw-r--r--   0        0        0      279 2023-06-15 00:41:57.158195 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2179 2023-07-10 15:57:25.739070 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      240 2023-07-10 15:57:25.739286 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0     1009 2023-07-13 18:27:40.465906 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     2228 2023-07-11 00:38:07.412504 grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     7034 2023-07-13 18:36:46.290173 grai_schemas-0.2.0a6/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     3727 2023-07-13 16:32:19.172713 grai_schemas-0.2.0a6/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-07-10 15:57:25.740065 grai_schemas-0.2.0a6/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1203 2023-07-10 15:57:25.740281 grai_schemas-0.2.0a6/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3696 2023-07-10 15:57:25.740372 grai_schemas-0.2.0a6/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a6/PKG-INFO
```

### Comparing `grai_schemas-0.2.0a5/LICENSE` & `grai_schemas-0.2.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/pyproject.toml` & `grai_schemas-0.2.0a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.2.0-alpha5"
+version = "0.2.0-alpha6"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.4"
 multimethod = "^1.9.1"
+polyfactory = "^2.6.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pre-commit = "^2.21.0"
 pytest = "^7.2.0"
 mypy = "^0.991"
```

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/base.py` & `grai_schemas-0.2.0a6/src/grai_schemas/base.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/generics.py` & `grai_schemas-0.2.0a6/src/grai_schemas/generics.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,19 +91,14 @@
         Raises:
 
         """
         if isinstance(values, dict):
             has_default_value = values.get("has_default_value", None)
             data_type = values.get("data_type", None)
             default_value = values.get("default_value", None)
-        # elif isinstance(values, DefaultValue):
-        #     breakpoint()
-        #     has_default_value = values.has_default_value
-        #     data_type = values.data_type
-        #     default_value = values.default_value
         else:
             raise NotImplementedError(f"No available implementation to produce a DefaultValue from a {type(values)}")
 
         if has_default_value is None or has_default_value is False:
             assert data_type is None, "Cannot set a data_type when `has_default_value` is not True"
             assert default_value is None, "Cannot set a default_value when `has_default_value` is not True"
         else:
```

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/human_ids.py` & `grai_schemas-0.2.0a6/src/grai_schemas/human_ids.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/schema.py` & `grai_schemas-0.2.0a6/src/grai_schemas/schema.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/utilities.py` & `grai_schemas-0.2.0a6/src/grai_schemas/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/edge.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/edge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable, Dict, List, Literal, Optional, Type, Union
 from uuid import UUID
 
 from grai_schemas.v1.generics import GraiBaseModel, NamedID, UuidID
 from grai_schemas.v1.metadata.edges import GenericEdgeMetadataV1, Metadata
-from grai_schemas.v1.metadata.metadata import MetadataV1
+from grai_schemas.v1.metadata.metadata import GraiMetadataV1, MetadataV1
 from grai_schemas.v1.node import NodeIdTypes
 from grai_schemas.v1.source import DataSourceMixin, DataSourcesMixin
 from pydantic import validator
 
 
 class EdgeNamedID(NamedID):
     """ """
@@ -28,38 +28,41 @@
     """ """
 
     display_name: Optional[str]
     source: NodeIdTypes
     destination: NodeIdTypes
     is_active: Optional[bool] = True
     workspace: Optional[UUID]
-    metadata: MetadataV1 = MetadataV1(grai=GenericEdgeMetadataV1(edge_type="Generic"))
 
     def __str__(self):
         return f"Edge[Node({self.source}) -> Node({self.destination})]"
 
+
+class SourcedEdgeSpecMetadataMixin(GraiBaseModel):
+    metadata: GraiMetadataV1 = GraiMetadataV1(grai=GenericEdgeMetadataV1(edge_type="Generic"))
+
     @validator("metadata", always=True, pre=True)
-    def validate_metadata(cls, v: Optional[Union[Dict, MetadataV1]]) -> MetadataV1:
-        if isinstance(v, MetadataV1):
+    def validate_metadata(cls, v: Optional[Union[Dict, GraiMetadataV1]]) -> GraiMetadataV1:
+        if isinstance(v, GraiMetadataV1):
             return v
         elif isinstance(v, dict):
             v.setdefault("grai", GenericEdgeMetadataV1(edge_type="Generic"))
-            return MetadataV1(**v)
+            return GraiMetadataV1(**v)
         elif v is None:
-            return MetadataV1(grai=GenericEdgeMetadataV1(edge_type="Generic"))
+            return GraiMetadataV1(grai=GenericEdgeMetadataV1(edge_type="Generic"))
         raise ValueError(f"Invalid metadata: {v}. Expected either None, a dict, or a MetadataV1 instance.")
 
 
-class NamedSourceSpec(EdgeNamedID, BaseSpec, DataSourceMixin):
+class NamedSourceSpec(EdgeNamedID, BaseSpec, SourcedEdgeSpecMetadataMixin, DataSourceMixin):
     """ """
 
     pass
 
 
-class IDSourceSpec(EdgeUuidID, BaseSpec, DataSourceMixin):
+class IDSourceSpec(EdgeUuidID, BaseSpec, SourcedEdgeSpecMetadataMixin, DataSourceMixin):
     """ """
 
     pass
 
 
 SourcedEdgeSpec = Union[IDSourceSpec, NamedSourceSpec]
 
@@ -83,21 +86,37 @@
         """
         return cls(version="v1", type="SourceEdge", spec=spec_dict)
 
     def __hash__(self):
         return hash(self.spec)
 
 
-class NamedSpec(EdgeNamedID, BaseSpec, DataSourcesMixin):
+class EdgeSpecMetadataMixin(GraiBaseModel):
+    metadata: MetadataV1 = MetadataV1(grai=GenericEdgeMetadataV1(edge_type="Generic"), sources={})
+
+    @validator("metadata", always=True, pre=True)
+    def validate_metadata(cls, v: Optional[Union[Dict, MetadataV1]]) -> MetadataV1:
+        if isinstance(v, MetadataV1):
+            return v
+        elif isinstance(v, dict):
+            v.setdefault("grai", GenericEdgeMetadataV1(edge_type="Generic"))
+            v.setdefault("sources", {})
+            return MetadataV1(**v)
+        elif v is None:
+            return MetadataV1(grai=GenericEdgeMetadataV1(edge_type="Generic"), sources={})
+        raise ValueError(f"Invalid metadata: {v}. Expected either None, a dict, or a MetadataV1 instance.")
+
+
+class NamedSpec(EdgeNamedID, BaseSpec, EdgeSpecMetadataMixin, DataSourcesMixin):
     """ """
 
     pass
 
 
-class IDSpec(EdgeUuidID, BaseSpec, DataSourcesMixin):
+class IDSpec(EdgeUuidID, BaseSpec, EdgeSpecMetadataMixin, DataSourcesMixin):
     """ """
 
     pass
 
 
 EdgeSpec = Union[IDSpec, NamedSpec]
```

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/events.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/events.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/merge.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/merge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/edges.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/metadata.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,41 @@
-from typing import Any, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from grai_schemas.generics import GraiBaseModel, MalformedMetadata, Metadata
 from grai_schemas.utilities import merge
 from grai_schemas.v1.metadata import edges, nodes
-
+from uuid import UUID
 
 class GraiMetadataV1(Metadata):
     """ """
 
     grai: Union[edges.Metadata, nodes.Metadata]
 
 
-class MetadataV1(GraiMetadataV1):
+class SourcesMetadataV1(Metadata):
+    """"""
+
+    sources: Dict[UUID, GraiMetadataV1]
+
+
+class MetadataV1(GraiMetadataV1, SourcesMetadataV1):
     """ """
 
     class Config:
         """ """
 
         extra = "allow"
         allow_mutation = True
 
 
 class GraiMalformedNodeMetadataV1(MalformedMetadata, MetadataV1):
     """ """
 
     grai: nodes.MalformedNodeMetadataV1 = nodes.MalformedNodeMetadataV1()  # type: ignore
+    sources: Dict[UUID, GraiMetadataV1] = {}
 
 
 class GraiMalformedEdgeMetadataV1(MalformedMetadata, MetadataV1):
     """ """
 
     grai: edges.MalformedEdgeMetadataV1 = edges.MalformedEdgeMetadataV1()  # type: ignore
+    sources: Dict[UUID, GraiMetadataV1] = {}
```

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/metadata/nodes.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/node.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Literal, Optional, Union
 from uuid import UUID
 
 from grai_schemas.generics import GraiBaseModel
 from grai_schemas.v1.generics import ID, BaseID, NamedID, UuidID
-from grai_schemas.v1.metadata.metadata import MetadataV1
+from grai_schemas.v1.metadata.metadata import GraiMetadataV1, MetadataV1
 from grai_schemas.v1.metadata.nodes import GenericNodeMetadataV1
 from grai_schemas.v1.source import DataSourceMixin, DataSourcesMixin
 from pydantic import Field, validator
 
 
 class NodeNamedID(NamedID):
     """ """
@@ -26,35 +26,38 @@
 
 class BaseSpec(GraiBaseModel):
     """ """
 
     is_active: Optional[bool] = True
     display_name: Optional[str]
     workspace: Optional[UUID]
-    metadata: MetadataV1 = MetadataV1(grai=GenericNodeMetadataV1(node_type="Generic"))
+
+
+class SourcedNodeSpecMetadataMixin(GraiBaseModel):
+    metadata: GraiMetadataV1 = GraiMetadataV1(grai=GenericNodeMetadataV1(node_type="Generic"))
 
     @validator("metadata", always=True, pre=True)
-    def validate_metadata(cls, v: Optional[Union[Dict, MetadataV1]]) -> MetadataV1:
-        if isinstance(v, MetadataV1):
+    def validate_metadata(cls, v: Optional[Union[Dict, GraiMetadataV1]]) -> GraiMetadataV1:
+        if isinstance(v, GraiMetadataV1):
             return v
         elif isinstance(v, dict):
             v.setdefault("grai", GenericNodeMetadataV1(node_type="Generic"))
-            return MetadataV1(**v)
+            return GraiMetadataV1(**v)
         elif v is None:
-            return MetadataV1(grai=GenericNodeMetadataV1(node_type="Generic"))
+            return GraiMetadataV1(grai=GenericNodeMetadataV1(node_type="Generic"))
         raise ValueError(f"Invalid metadata: {v}. Expected either None, a dict, or a MetadataV1 instance.")
 
 
-class NamedSourceSpec(NodeNamedID, BaseSpec, DataSourceMixin):
+class NamedSourceSpec(NodeNamedID, BaseSpec, SourcedNodeSpecMetadataMixin, DataSourceMixin):
     """ """
 
     pass
 
 
-class IDSourceSpec(NodeUuidID, BaseSpec, DataSourceMixin):
+class IDSourceSpec(NodeUuidID, BaseSpec, SourcedNodeSpecMetadataMixin, DataSourceMixin):
     """ """
 
     pass
 
 
 SourcedNodeSpec = Union[IDSourceSpec, NamedSourceSpec]
 
@@ -78,21 +81,37 @@
         """
         return cls(version="v1", type="SourceNode", spec=spec_dict)
 
     def __hash__(self):
         return hash(self.spec)
 
 
-class NamedSpec(NodeNamedID, BaseSpec, DataSourcesMixin):
+class NodeSpecMetadataMixin(GraiBaseModel):
+    metadata: MetadataV1 = MetadataV1(grai=GenericNodeMetadataV1(node_type="Generic"), sources={})
+
+    @validator("metadata", always=True, pre=True)
+    def validate_metadata(cls, v: Optional[Union[Dict, MetadataV1]]) -> MetadataV1:
+        if isinstance(v, MetadataV1):
+            return v
+        elif isinstance(v, dict):
+            v.setdefault("grai", GenericNodeMetadataV1(node_type="Generic"))
+            v.setdefault("sources", {})
+            return MetadataV1(**v)
+        elif v is None:
+            return MetadataV1(grai=GenericNodeMetadataV1(node_type="Generic"), sources={})
+        raise ValueError(f"Invalid metadata: {v}. Expected either None, a dict, or a MetadataV1 instance.")
+
+
+class NamedSpec(NodeNamedID, BaseSpec, NodeSpecMetadataMixin, DataSourcesMixin):
     """ """
 
     pass
 
 
-class IDSpec(NodeUuidID, BaseSpec, DataSourcesMixin):
+class IDSpec(NodeUuidID, BaseSpec, NodeSpecMetadataMixin, DataSourcesMixin):
     """ """
 
     pass
 
 
 NodeSpec = Union[IDSpec, NamedSpec]
```

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/organization.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/organization.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/source.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/source.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/src/grai_schemas/v1/workspace.py` & `grai_schemas-0.2.0a6/src/grai_schemas/v1/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a5/PKG-INFO` & `grai_schemas-0.2.0a6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.2.0a5
+Version: 0.2.0a6
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: multimethod (>=1.9.1,<2.0.0)
+Requires-Dist: polyfactory (>=2.6.1,<3.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-schemas
 Description-Content-Type: text/markdown
 
 # Grai Schemas
```

