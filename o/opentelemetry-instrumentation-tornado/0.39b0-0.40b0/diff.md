# Comparing `tmp/opentelemetry_instrumentation_tornado-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_tornado-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_tornado-0.39b0.tar` & `opentelemetry_instrumentation_tornado-0.40b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/__init__.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/client.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    28750 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/tests/test_instrumentation.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/tests/test_metrics_instrumentation.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/tests/tornado_test_app.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/LICENSE
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/README.rst
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    22922 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/__init__.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/client.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    28751 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/tests/test_instrumentation.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/tests/test_metrics_instrumentation.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/tests/tornado_test_app.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/LICENSE
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/README.rst
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_tornado-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/__init__.py` & `opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -450,29 +450,42 @@
             ] = request.connection.context._orig_remote_ip
 
     return extract_attributes_from_object(
         request, _traced_request_attrs, attrs
     )
 
 
-def _get_operation_name(handler, request):
-    full_class_name = type(handler).__name__
-    class_name = full_class_name.rsplit(".")[-1]
-    return f"{class_name}.{request.method.lower()}"
+def _get_default_span_name(request):
+    """
+    Default span name is the HTTP method and URL path, or just the method.
+    https://github.com/open-telemetry/opentelemetry-specification/pull/3165
+    https://opentelemetry.io/docs/reference/specification/trace/semantic_conventions/http/#name
+
+    Args:
+        request: Tornado request object.
+    Returns:
+        Default span name.
+    """
+
+    path = request.path
+    method = request.method
+    if method and path:
+        return f"{method} {path}"
+    return f"{method}"
 
 
 def _get_full_handler_name(handler):
     klass = type(handler)
     return f"{klass.__module__}.{klass.__qualname__}"
 
 
 def _start_span(tracer, handler) -> _TraceContext:
     span, token = _start_internal_or_server_span(
         tracer=tracer,
-        span_name=_get_operation_name(handler, handler.request),
+        span_name=_get_default_span_name(handler.request),
         start_time=time_ns(),
         context_carrier=handler.request.headers,
         context_getter=textmap.default_getter,
     )
 
     if span.is_recording():
         attributes = _get_attributes_from_request(handler.request)
```

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/client.py` & `opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/package.py` & `opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/src/opentelemetry/instrumentation/tornado/version.py` & `opentelemetry_instrumentation_tornado-0.40b0/src/opentelemetry/instrumentation/tornado/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.39b0"
+__version__ = "0.40b0"
```

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/tests/test_instrumentation.py` & `opentelemetry_instrumentation_tornado-0.40b0/tests/test_instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from unittest.mock import Mock, patch
 
+from http_server_mock import HttpServerMock
 from tornado.testing import AsyncHTTPTestCase
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.propagators import (
     TraceResponsePropagator,
     get_global_response_propagator,
     set_global_response_propagator,
@@ -131,15 +132,15 @@
 
         manual, server, client = self.sorted_spans(spans)
 
         self.assertEqual(manual.name, "manual")
         self.assertEqual(manual.parent, server.context)
         self.assertEqual(manual.context.trace_id, client.context.trace_id)
 
-        self.assertEqual(server.name, "MainHandler." + method.lower())
+        self.assertEqual(server.name, f"{method} /")
         self.assertTrue(server.parent.is_remote)
         self.assertNotEqual(server.parent, client.context)
         self.assertEqual(server.parent.span_id, client.context.span_id)
         self.assertEqual(server.context.trace_id, client.context.trace_id)
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
@@ -192,15 +193,15 @@
     def _test_async_handler(self, url, handler_name):
         response = self.fetch(url)
         self.assertEqual(response.code, 201)
         spans = self.get_finished_spans()
         self.assertEqual(len(spans), 5)
 
         client = spans.by_name("GET")
-        server = spans.by_name(handler_name + ".get")
+        server = spans.by_name(f"GET {url}")
         sub_wrapper = spans.by_name("sub-task-wrapper")
 
         sub2 = spans.by_name("sub-task-2")
         self.assertEqual(sub2.name, "sub-task-2")
         self.assertEqual(sub2.parent, sub_wrapper.context)
         self.assertEqual(sub2.context.trace_id, client.context.trace_id)
 
@@ -209,15 +210,15 @@
         self.assertEqual(sub1.parent, sub_wrapper.context)
         self.assertEqual(sub1.context.trace_id, client.context.trace_id)
 
         self.assertEqual(sub_wrapper.name, "sub-task-wrapper")
         self.assertEqual(sub_wrapper.parent, server.context)
         self.assertEqual(sub_wrapper.context.trace_id, client.context.trace_id)
 
-        self.assertEqual(server.name, handler_name + ".get")
+        self.assertEqual(server.name, f"GET {url}")
         self.assertTrue(server.parent.is_remote)
         self.assertNotEqual(server.parent, client.context)
         self.assertEqual(server.parent.span_id, client.context.span_id)
         self.assertEqual(server.context.trace_id, client.context.trace_id)
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
@@ -225,14 +226,15 @@
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_SCHEME: "http",
                 SpanAttributes.HTTP_HOST: "127.0.0.1:"
                 + str(self.get_http_port()),
                 SpanAttributes.HTTP_TARGET: url,
                 SpanAttributes.HTTP_CLIENT_IP: "127.0.0.1",
                 SpanAttributes.HTTP_STATUS_CODE: 201,
+                "tornado.handler": f"tests.tornado_test_app.{handler_name}",
             },
         )
 
         self.assertEqual(client.name, "GET")
         self.assertFalse(client.context.is_remote)
         self.assertIsNone(client.parent)
         self.assertEqual(client.kind, SpanKind.CLIENT)
@@ -249,17 +251,17 @@
         response = self.fetch("/error")
         self.assertEqual(response.code, 500)
 
         spans = self.get_finished_spans()
         self.assertEqual(len(spans), 2)
 
         client = spans.by_name("GET")
-        server = spans.by_name("BadHandler.get")
+        server = spans.by_name("GET /error")
 
-        self.assertEqual(server.name, "BadHandler.get")
+        self.assertEqual(server.name, "GET /error")
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_SCHEME: "http",
                 SpanAttributes.HTTP_HOST: "127.0.0.1:"
@@ -286,15 +288,15 @@
         response = self.fetch("/missing-url")
         self.assertEqual(response.code, 404)
 
         spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
         self.assertEqual(len(spans), 2)
         server, client = spans
 
-        self.assertEqual(server.name, "ErrorHandler.get")
+        self.assertEqual(server.name, "GET /missing-url")
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_SCHEME: "http",
                 SpanAttributes.HTTP_HOST: "127.0.0.1:"
@@ -321,15 +323,15 @@
         response = self.fetch("/raise_403")
         self.assertEqual(response.code, 403)
 
         spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
         self.assertEqual(len(spans), 2)
         server, client = spans
 
-        self.assertEqual(server.name, "RaiseHTTPErrorHandler.get")
+        self.assertEqual(server.name, "GET /raise_403")
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_SCHEME: "http",
                 SpanAttributes.HTTP_HOST: "127.0.0.1:"
@@ -362,15 +364,15 @@
         response = self.fetch("/dyna")
         self.assertEqual(response.code, 202)
 
         spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
         self.assertEqual(len(spans), 2)
         server, client = spans
 
-        self.assertEqual(server.name, "DynamicHandler.get")
+        self.assertEqual(server.name, "GET /dyna")
         self.assertTrue(server.parent.is_remote)
         self.assertNotEqual(server.parent, client.context)
         self.assertEqual(server.parent.span_id, client.context.span_id)
         self.assertEqual(server.context.trace_id, client.context.trace_id)
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
@@ -403,15 +405,15 @@
         response = self.fetch("/on_finish")
         self.assertEqual(response.code, 200)
 
         spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
         self.assertEqual(len(spans), 3)
         auditor, server, client = spans
 
-        self.assertEqual(server.name, "FinishedHandler.get")
+        self.assertEqual(server.name, "GET /on_finish")
         self.assertTrue(server.parent.is_remote)
         self.assertNotEqual(server.parent, client.context)
         self.assertEqual(server.parent.span_id, client.context.span_id)
         self.assertEqual(server.context.trace_id, client.context.trace_id)
         self.assertEqual(server.kind, SpanKind.SERVER)
         self.assertSpanHasAttributes(
             server,
@@ -490,52 +492,55 @@
         spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
         self.assertEqual(len(spans), 3)
         self.assertTraceResponseHeaderMatchesSpan(response.headers, spans[1])
 
         self.memory_exporter.clear()
         set_global_response_propagator(orig)
 
-    # todo(srikanthccv): fix this test
-    # this test is making request to real httpbin.org/status/200 which
-    # is not a good idea as it can fail due to availability of the
-    # service.
-    # def test_credential_removal(self):
-    #     response = self.fetch(
-    #         "http://username:password@httpbin.org/status/200"
-    #     )
-    #     self.assertEqual(response.code, 200)
-
-    #     spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
-    #     self.assertEqual(len(spans), 1)
-    #     client = spans[0]
-
-    #     self.assertEqual(client.name, "GET")
-    #     self.assertEqual(client.kind, SpanKind.CLIENT)
-    #     self.assertSpanHasAttributes(
-    #         client,
-    #         {
-    #             SpanAttributes.HTTP_URL: "http://httpbin.org/status/200",
-    #             SpanAttributes.HTTP_METHOD: "GET",
-    #             SpanAttributes.HTTP_STATUS_CODE: 200,
-    #         },
-    #     )
+    def test_credential_removal(self):
+        app = HttpServerMock("test_credential_removal")
 
-    #     self.memory_exporter.clear()
+        @app.route("/status/200")
+        def index():
+            return "hello"
+
+        with app.run("localhost", 5000):
+            response = self.fetch(
+                "http://username:password@localhost:5000/status/200"
+            )
+        self.assertEqual(response.code, 200)
+
+        spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
+        self.assertEqual(len(spans), 1)
+        client = spans[0]
+
+        self.assertEqual(client.name, "GET")
+        self.assertEqual(client.kind, SpanKind.CLIENT)
+        self.assertSpanHasAttributes(
+            client,
+            {
+                SpanAttributes.HTTP_URL: "http://localhost:5000/status/200",
+                SpanAttributes.HTTP_METHOD: "GET",
+                SpanAttributes.HTTP_STATUS_CODE: 200,
+            },
+        )
+
+        self.memory_exporter.clear()
 
 
 class TestTornadoInstrumentationWithXHeaders(TornadoTest):
     def get_httpserver_options(self):
         return {"xheaders": True}
 
     def test_xheaders(self):
         response = self.fetch("/", headers={"X-Forwarded-For": "12.34.56.78"})
         self.assertEqual(response.code, 201)
         spans = self.get_finished_spans()
         self.assertSpanHasAttributes(
-            spans.by_name("MainHandler.get"),
+            spans.by_name("GET /"),
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_SCHEME: "http",
                 SpanAttributes.HTTP_HOST: "127.0.0.1:"
                 + str(self.get_http_port()),
                 SpanAttributes.HTTP_TARGET: "/",
                 SpanAttributes.HTTP_CLIENT_IP: "12.34.56.78",
@@ -601,15 +606,15 @@
     def test_uninstrument(self):
         response = self.fetch("/")
         self.assertEqual(response.code, 201)
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 3)
         manual, server, client = self.sorted_spans(spans)
         self.assertEqual(manual.name, "manual")
-        self.assertEqual(server.name, "MainHandler.get")
+        self.assertEqual(server.name, "GET /")
         self.assertEqual(client.name, "GET")
         self.memory_exporter.clear()
 
         TornadoInstrumentor().uninstrument()
 
         response = self.fetch("/")
         self.assertEqual(response.code, 201)
```

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/tests/test_metrics_instrumentation.py` & `opentelemetry_instrumentation_tornado-0.40b0/tests/test_metrics_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/tests/tornado_test_app.py` & `opentelemetry_instrumentation_tornado-0.40b0/tests/tornado_test_app.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/LICENSE` & `opentelemetry_instrumentation_tornado-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/README.rst` & `opentelemetry_instrumentation_tornado-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_tornado-0.40b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,27 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
-  "opentelemetry-semantic-conventions == 0.39b0",
-  "opentelemetry-util-http == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
+  "opentelemetry-util-http == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "tornado >= 5.1.1",
 ]
 test = [
   "opentelemetry-instrumentation-tornado[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
+  "http-server-mock"
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 tornado = "opentelemetry.instrumentation.tornado:TornadoInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-tornado"
```

### Comparing `opentelemetry_instrumentation_tornado-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_tornado-0.40b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-tornado
-Version: 0.39b0
+Version: 0.40b0
 Summary: Tornado instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-tornado
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,22 +13,23 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
-Requires-Dist: opentelemetry-util-http==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
+Requires-Dist: opentelemetry-util-http==0.40b0
 Provides-Extra: instruments
 Requires-Dist: tornado>=5.1.1; extra == 'instruments'
 Provides-Extra: test
+Requires-Dist: http-server-mock; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-tornado[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Tornado Instrumentation
 ======================================
 
 |pypi|
```

