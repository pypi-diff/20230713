# Comparing `tmp/pythogen-0.2.4.tar.gz` & `tmp/pythogen-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.4.tar", max compression
+gzip compressed data, was "pythogen-0.2.5.tar", max compression
```

## Comparing `pythogen-0.2.4.tar` & `pythogen-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-07-12 09:47:38.443211 pythogen-0.2.4/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-12 09:47:38.443211 pythogen-0.2.4/README.md
--rw-r--r--   0        0        0     1567 2023-07-12 09:47:38.447211 pythogen-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7531 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/models.py
--rw-r--r--   0        0        0     2329 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/response.py
--rw-r--r--   0        0        0    17663 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0    10011 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/settings.py
--rw-r--r--   0        0        0     5149 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0    11127 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-13 08:24:12.427281 pythogen-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-13 08:24:12.427281 pythogen-0.2.5/README.md
+-rw-r--r--   0        0        0     1567 2023-07-13 08:24:12.427281 pythogen-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 08:24:12.427281 pythogen-0.2.5/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7660 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/models.py
+-rw-r--r--   0        0        0     2329 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    17663 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10011 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/settings.py
+-rw-r--r--   0        0        0     5149 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0    11016 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.5/PKG-INFO
```

### Comparing `pythogen-0.2.4/LICENSE` & `pythogen-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/README.md` & `pythogen-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pyproject.toml` & `pythogen-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.4"
+version = "0.2.5"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.2.4/pythogen/entrypoint.py` & `pythogen-0.2.5/pythogen/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/models.py` & `pythogen-0.2.5/pythogen/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     info: InfoObject
     paths: dict[str, PathItemObject]
     parameters: dict[str, ParameterObject]
     schemas: dict[str, SchemaObject]
 
     discriminator_base_class_schemas: list[DiscriminatorBaseClassSchema]
 
-    def _build_sorted_schemas(self, keys):
+    def _build_sorted_schemas(self, keys: list[str], exclude_enums: bool = False):
         sorted: list[str] = []
         key_for_processing = set(keys)
         while keys:
             key = keys.pop()
             if key in sorted:
                 index = sorted.index(key)
             else:
@@ -285,24 +285,28 @@
                     elif property.schema.items.id in self.schemas:
                         sorted.insert(index, property.schema.items.id)
 
         sorted_schemas = []
         for key in sorted:
             if self.schemas[key] not in sorted_schemas:
                 sorted_schemas.append(self.schemas[key])
+
+        if exclude_enums:
+            sorted_schemas = [s for s in sorted_schemas if s.enum is None]
+
         return sorted_schemas
 
     @property
     def sorted_schemas(self) -> list[SchemaObject]:
-        schema_keys = list(filter(lambda x: self.schemas[x].enum is None, self.schemas.keys()))
-        return self._build_sorted_schemas(schema_keys)
+        keys = [key for key, schema in self.schemas.items() if schema.enum is None]
+        return self._build_sorted_schemas(keys, exclude_enums=True)
 
     @property
     def sorted_enums(self) -> list[SchemaObject]:
-        enum_keys = list(filter(lambda x: self.schemas[x].enum is not None, self.schemas.keys()))
-        return self._build_sorted_schemas(enum_keys)
+        keys = [key for key, schema in self.schemas.items() if schema.enum is not None]
+        return self._build_sorted_schemas(keys)
 
 
 @dataclass
 class DiscriminatorBaseClassSchema:
     name: str
     attr: str
```

### Comparing `pythogen-0.2.4/pythogen/packager.py` & `pythogen-0.2.5/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/document.py` & `pythogen-0.2.5/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.5/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/operations.py` & `pythogen-0.2.5/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/parameters.py` & `pythogen-0.2.5/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/paths.py` & `pythogen-0.2.5/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/references.py` & `pythogen-0.2.5/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/request_body.py` & `pythogen-0.2.5/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/response.py` & `pythogen-0.2.5/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/parsers/schemas.py` & `pythogen-0.2.5/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/renderer.py` & `pythogen-0.2.5/pythogen/renderer.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.5/pythogen/templates/client/httpx-method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.5/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.4/pythogen/templates/httpx.j2` & `pythogen-0.2.5/pythogen/templates/httpx.j2`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from typing import Union
 from typing import Callable
 from typing import get_type_hints
 from typing import Mapping
 from typing import Sequence
 from typing import IO
 from typing import cast
+from typing import Protocol
 
 {%- if metrics %}
 from prometheus_client import Counter
 from prometheus_client import Histogram
 {%- endif %}
 import httpx
 from pydantic import BaseModel
@@ -51,33 +52,33 @@
 # backward compatibility for httpx<0.18.2
 try:
     DEFAULT_AUTH = httpx.USE_CLIENT_DEFAULT
 except AttributeError:
     DEFAULT_AUTH = None
 
 {%- if metrics %}
-class BaseMetricsIntegration(abc.ABC):
+class MetricsIntegration(Protocol):
     def __init__(
         self,
         client_response_time_histogram: Histogram | None = None,
         client_non_http_errors_counter: Counter | None = None,
         shadow_path: bool = True,
     ):
         self._client_response_time_histogram = client_response_time_histogram
         self._client_non_http_errors_counter = client_non_http_errors_counter
         self.shadow_path = shadow_path
 
-    @abc.abstractmethod
-    def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str) -> None: ...
+    def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str) -> None:
+        ...
 
-    @abc.abstractmethod
-    def on_request_success(self, client_name: str, response, http_method: str, http_target: str) -> None: ...
+    def on_request_success(self, client_name: str, response, http_method: str, http_target: str) -> None:
+        ...
 
 
-class DefaultMetricsIntegration(BaseMetricsIntegration):
+class DefaultMetricsIntegration:
     def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str) -> None:
         self._client_non_http_errors_counter.labels(
             client_name=client_name,
             http_method=http_method,
             http_target=http_target,
             exception=error.__class__.__name__,
         ).inc(1)
@@ -104,26 +105,26 @@
 
 
 @dataclass
 class ResponseBox:
     status_code: int
 
 
-class BaseLogsIntegration(abc.ABC):
-    @abc.abstractmethod
-    def log_extra(self, **kwargs: Any) -> dict[str, Any]: ...
+class LogsIntegration(Protocol):
+    def log_extra(self, **kwargs: Any) -> dict[str, Any]:
+        ...
 
-    @abc.abstractmethod
-    def log_error(self, req: RequestBox, resp: ResponseBox) -> None: ...
+    def log_error(self, req: RequestBox, resp: ResponseBox) -> None:
+        ...
 
-    @abc.abstractmethod
-    def get_log_error_level(self, req: RequestBox, resp: ResponseBox) -> int: ...
+    def get_log_error_level(self, req: RequestBox, resp: ResponseBox) -> int:
+        ...
 
 
-class DefaultLogsIntegration(BaseLogsIntegration):
+class DefaultLogsIntegration:
     def log_extra(self, **kwargs: Any) -> dict[str, Any]:
         return {'props': {'data': kwargs}}
 
     def log_error(self, req: RequestBox, resp: ResponseBox) -> None:
         msg = f"request error"
         msg += f" | client={req.client_name}"
         msg += f" | method={req.method}"
@@ -268,17 +269,17 @@
         {%- if sync %}
         client: httpx.Client | None = None,
         {%- else %}
         client: httpx.AsyncClient | None = None,
         {%- endif %}
         headers: dict[str, str] | None = None,
         {%- if metrics %}
-        metrics_integration: BaseMetricsIntegration | None = None,
+        metrics_integration: MetricsIntegration | None = None,
         {%- endif %}
-        logs_integration: BaseLogsIntegration | None = DefaultLogsIntegration(),
+        logs_integration: LogsIntegration | None = DefaultLogsIntegration(),
     ):
         {%- if sync %}
         self.client = client or httpx.Client(timeout=Timeout(timeout))
         {%- else %}
         self.client = client or httpx.AsyncClient(timeout=Timeout(timeout))
         {%- endif %}
         self.base_url = base_url
```

### Comparing `pythogen-0.2.4/PKG-INFO` & `pythogen-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

