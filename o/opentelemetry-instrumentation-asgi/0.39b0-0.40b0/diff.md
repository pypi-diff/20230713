# Comparing `tmp/opentelemetry_instrumentation_asgi-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_asgi-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_asgi-0.39b0.tar` & `opentelemetry_instrumentation_asgi-0.40b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    24887 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_custom_headers.py
--rw-r--r--   0        0        0    30123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_middleware.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/test_getter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/LICENSE
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/README.rst
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    26670 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/src/opentelemetry/instrumentation/asgi/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/src/opentelemetry/instrumentation/asgi/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/src/opentelemetry/instrumentation/asgi/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/tests/test_asgi_custom_headers.py
+-rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/tests/test_asgi_middleware.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/tests/test_getter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/LICENSE
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/README.rst
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/__init__.py` & `opentelemetry_instrumentation_asgi-0.40b0/src/opentelemetry/instrumentation/asgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,26 +411,31 @@
         span.set_attribute(SpanAttributes.HTTP_STATUS_CODE, status_code)
         span.set_status(
             Status(http_status_to_status_code(status_code, server_span=True))
         )
 
 
 def get_default_span_details(scope: dict) -> Tuple[str, dict]:
-    """Default implementation for get_default_span_details
+    """
+    Default span name is the HTTP method and URL path, or just the method.
+    https://github.com/open-telemetry/opentelemetry-specification/pull/3165
+    https://opentelemetry.io/docs/reference/specification/trace/semantic_conventions/http/#name
+
     Args:
         scope: the ASGI scope dictionary
     Returns:
         a tuple of the span name, and any attributes to attach to the span.
     """
-    span_name = (
-        scope.get("path", "").strip()
-        or f"HTTP {scope.get('method', '').strip()}"
-    )
-
-    return span_name, {}
+    path = scope.get("path", "").strip()
+    method = scope.get("method", "").strip()
+    if method and path:  # http
+        return f"{method} {path}", {}
+    if path:  # websocket
+        return path, {}
+    return method, {}  # http with no path
 
 
 def _collect_target_attribute(
     scope: typing.Dict[str, typing.Any]
 ) -> typing.Optional[str]:
     """
     Returns the target path as defined by the Semantic Conventions.
@@ -497,26 +502,37 @@
             else meter
         )
         self.duration_histogram = self.meter.create_histogram(
             name=MetricInstruments.HTTP_SERVER_DURATION,
             unit="ms",
             description="measures the duration of the inbound HTTP request",
         )
+        self.server_response_size_histogram = self.meter.create_histogram(
+            name=MetricInstruments.HTTP_SERVER_RESPONSE_SIZE,
+            unit="By",
+            description="measures the size of HTTP response messages (compressed).",
+        )
+        self.server_request_size_histogram = self.meter.create_histogram(
+            name=MetricInstruments.HTTP_SERVER_REQUEST_SIZE,
+            unit="By",
+            description="Measures the size of HTTP request messages (compressed).",
+        )
         self.active_requests_counter = self.meter.create_up_down_counter(
             name=MetricInstruments.HTTP_SERVER_ACTIVE_REQUESTS,
             unit="requests",
             description="measures the number of concurrent HTTP requests that are currently in-flight",
         )
         self.excluded_urls = excluded_urls
         self.default_span_details = (
             default_span_details or get_default_span_details
         )
         self.server_request_hook = server_request_hook
         self.client_request_hook = client_request_hook
         self.client_response_hook = client_response_hook
+        self.content_length_header = None
 
     async def __call__(self, scope, receive, send):
         """The ASGI application
 
         Args:
             scope: An ASGI environment.
             receive: An awaitable callable yielding dictionaries
@@ -584,14 +600,28 @@
                 if target:
                     duration_attrs[SpanAttributes.HTTP_TARGET] = target
                 duration = max(round((default_timer() - start) * 1000), 0)
                 self.duration_histogram.record(duration, duration_attrs)
                 self.active_requests_counter.add(
                     -1, active_requests_count_attrs
                 )
+                if self.content_length_header:
+                    self.server_response_size_histogram.record(
+                        self.content_length_header, duration_attrs
+                    )
+                request_size = asgi_getter.get(scope, "content-length")
+                if request_size:
+                    try:
+                        request_size_amount = int(request_size[0])
+                    except ValueError:
+                        pass
+                    else:
+                        self.server_request_size_histogram.record(
+                            request_size_amount, duration_attrs
+                        )
             if token:
                 context.detach(token)
 
     # pylint: enable=too-many-branches
 
     def _get_otel_receive(self, server_span_name, scope, receive):
         @wraps(receive)
@@ -651,10 +681,17 @@
                         message,
                         context=set_span_in_context(
                             server_span, trace.context_api.Context()
                         ),
                         setter=asgi_setter,
                     )
 
+                content_length = asgi_getter.get(message, "content-length")
+                if content_length:
+                    try:
+                        self.content_length_header = int(content_length[0])
+                    except ValueError:
+                        pass
+
                 await send(message)
 
         return otel_send
```

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/package.py` & `opentelemetry_instrumentation_asgi-0.40b0/src/opentelemetry/instrumentation/asgi/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/version.py` & `opentelemetry_instrumentation_asgi-0.40b0/src/opentelemetry/instrumentation/asgi/version.py`

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

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_custom_headers.py` & `opentelemetry_instrumentation_asgi-0.40b0/tests/test_asgi_custom_headers.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_middleware.py` & `opentelemetry_instrumentation_asgi-0.40b0/tests/test_asgi_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,30 +42,38 @@
     _active_requests_count_attrs,
     _duration_attrs,
 )
 
 _expected_metric_names = [
     "http.server.active_requests",
     "http.server.duration",
+    "http.server.response.size",
+    "http.server.request.size",
 ]
 _recommended_attrs = {
     "http.server.active_requests": _active_requests_count_attrs,
     "http.server.duration": _duration_attrs,
+    "http.server.response.size": _duration_attrs,
+    "http.server.request.size": _duration_attrs,
 }
 
 
 async def http_app(scope, receive, send):
     message = await receive()
+    scope["headers"] = [(b"content-length", b"128")]
     assert scope["type"] == "http"
     if message.get("type") == "http.request":
         await send(
             {
                 "type": "http.response.start",
                 "status": 200,
-                "headers": [[b"Content-Type", b"text/plain"]],
+                "headers": [
+                    [b"Content-Type", b"text/plain"],
+                    [b"content-length", b"1024"],
+                ],
             }
         )
         await send({"type": "http.response.body", "body": b"*"})
 
 
 async def websocket_app(scope, receive, send):
     assert scope["type"] == "websocket"
@@ -90,24 +98,28 @@
         await websocket_app(scope, receive, send)
 
 
 async def error_asgi(scope, receive, send):
     assert isinstance(scope, dict)
     assert scope["type"] == "http"
     message = await receive()
+    scope["headers"] = [(b"content-length", b"128")]
     if message.get("type") == "http.request":
         try:
             raise ValueError
         except ValueError:
             scope["hack_exc_info"] = sys.exc_info()
         await send(
             {
                 "type": "http.response.start",
                 "status": 200,
-                "headers": [[b"Content-Type", b"text/plain"]],
+                "headers": [
+                    [b"Content-Type", b"text/plain"],
+                    [b"content-length", b"1024"],
+                ],
             }
         )
         await send({"type": "http.response.body", "body": b"*"})
 
 
 class TestAsgiApplication(AsgiTestBase):
     def validate_outputs(self, outputs, error=None, modifiers=None):
@@ -122,15 +134,16 @@
 
         # Check http response body
         self.assertEqual(response_body["body"], b"*")
 
         # Check http response start
         self.assertEqual(response_start["status"], 200)
         self.assertEqual(
-            response_start["headers"], [[b"Content-Type", b"text/plain"]]
+            response_start["headers"],
+            [[b"Content-Type", b"text/plain"], [b"content-length", b"1024"]],
         )
 
         exc_info = self.scope.get("hack_exc_info")
         if error:
             self.assertIs(exc_info[0], error)
             self.assertIsInstance(exc_info[1], error)
             self.assertIsNotNone(exc_info[2])
@@ -138,33 +151,33 @@
             self.assertIsNone(exc_info)
 
         # Check spans
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 4)
         expected = [
             {
-                "name": "/ http receive",
+                "name": "GET / http receive",
                 "kind": trace_api.SpanKind.INTERNAL,
                 "attributes": {"type": "http.request"},
             },
             {
-                "name": "/ http send",
+                "name": "GET / http send",
                 "kind": trace_api.SpanKind.INTERNAL,
                 "attributes": {
                     SpanAttributes.HTTP_STATUS_CODE: 200,
                     "type": "http.response.start",
                 },
             },
             {
-                "name": "/ http send",
+                "name": "GET / http send",
                 "kind": trace_api.SpanKind.INTERNAL,
                 "attributes": {"type": "http.response.body"},
             },
             {
-                "name": "/",
+                "name": "GET /",
                 "kind": trace_api.SpanKind.SERVER,
                 "attributes": {
                     SpanAttributes.HTTP_METHOD: "GET",
                     SpanAttributes.HTTP_SCHEME: "http",
                     SpanAttributes.NET_HOST_PORT: 80,
                     SpanAttributes.HTTP_HOST: "127.0.0.1",
                     SpanAttributes.HTTP_FLAVOR: "1.0",
@@ -227,15 +240,15 @@
 
         def update_expected_span_name(expected):
             for entry in expected:
                 if entry["kind"] == trace_api.SpanKind.SERVER:
                     entry["name"] = span_name
                 else:
                     entry["name"] = " ".join(
-                        [span_name] + entry["name"].split(" ")[1:]
+                        [span_name] + entry["name"].split(" ")[2:]
                     )
             return expected
 
         app = otel_asgi.OpenTelemetryMiddleware(
             simple_asgi, default_span_details=get_predefined_span_details
         )
         self.seed_app(app)
@@ -348,14 +361,15 @@
         span_id = format_span_id(span.get_span_context().span_id)
         traceresponse = f"00-{trace_id}-{span_id}-01"
 
         self.assertListEqual(
             response_start["headers"],
             [
                 [b"Content-Type", b"text/plain"],
+                [b"content-length", b"1024"],
                 [b"traceresponse", f"{traceresponse}".encode()],
                 [b"access-control-expose-headers", b"traceresponse"],
             ],
         )
 
         set_global_response_propagator(orig)
 
@@ -489,17 +503,17 @@
         def client_response_hook(send_span, response):
             send_span.set_attribute("attr-from-hook", "value")
 
         def update_expected_hook_results(expected):
             for entry in expected:
                 if entry["kind"] == trace_api.SpanKind.SERVER:
                     entry["name"] = "name from server hook"
-                elif entry["name"] == "/ http receive":
+                elif entry["name"] == "GET / http receive":
                     entry["name"] = "name from client request hook"
-                elif entry["name"] == "/ http send":
+                elif entry["name"] == "GET / http send":
                     entry["attributes"].update({"attr-from-hook": "value"})
             return expected
 
         app = otel_asgi.OpenTelemetryMiddleware(
             simple_asgi,
             server_request_hook=server_request_hook,
             client_request_hook=client_request_hook,
@@ -561,27 +575,33 @@
         expected_requests_count_attributes = {
             "http.method": "GET",
             "http.host": "127.0.0.1",
             "http.scheme": "http",
             "http.flavor": "1.0",
         }
         metrics_list = self.memory_metrics_reader.get_metrics_data()
+        # pylint: disable=too-many-nested-blocks
         for resource_metric in metrics_list.resource_metrics:
             for scope_metrics in resource_metric.scope_metrics:
                 for metric in scope_metrics.metrics:
                     for point in list(metric.data.data_points):
                         if isinstance(point, HistogramDataPoint):
                             self.assertDictEqual(
                                 expected_duration_attributes,
                                 dict(point.attributes),
                             )
                             self.assertEqual(point.count, 1)
-                            self.assertAlmostEqual(
-                                duration, point.sum, delta=5
-                            )
+                            if metric.name == "http.server.duration":
+                                self.assertAlmostEqual(
+                                    duration, point.sum, delta=5
+                                )
+                            elif metric.name == "http.server.response.size":
+                                self.assertEqual(1024, point.sum)
+                            elif metric.name == "http.server.request.size":
+                                self.assertEqual(128, point.sum)
                         elif isinstance(point, NumberDataPoint):
                             self.assertDictEqual(
                                 expected_requests_count_attributes,
                                 dict(point.attributes),
                             )
                             self.assertEqual(point.value, 0)
 
@@ -598,30 +618,29 @@
                 scope["route"] = TestRoute()
             else:
                 raise ValueError("websockets not supported")
 
         app = otel_asgi.OpenTelemetryMiddleware(target_asgi)
         self.seed_app(app)
         self.send_default_request()
-
         metrics_list = self.memory_metrics_reader.get_metrics_data()
         assertions = 0
         for resource_metric in metrics_list.resource_metrics:
             for scope_metrics in resource_metric.scope_metrics:
                 for metric in scope_metrics.metrics:
-                    if metric.name != "http.server.duration":
+                    if metric.name == "http.server.active_requests":
                         continue
                     for point in metric.data.data_points:
                         if isinstance(point, HistogramDataPoint):
                             self.assertEqual(
                                 point.attributes["http.target"],
                                 expected_target,
                             )
                             assertions += 1
-        self.assertEqual(assertions, 1)
+        self.assertEqual(assertions, 3)
 
     def test_no_metric_for_websockets(self):
         self.scope = {
             "type": "websocket",
             "http_version": "1.1",
             "scheme": "ws",
             "path": "/",
@@ -701,19 +720,19 @@
         self.span.set_attribute.assert_has_calls(expected, any_order=True)
 
     def test_response_attributes_invalid_status_code(self):
         otel_asgi.set_status_code(self.span, "Invalid Status Code")
         self.assertEqual(self.span.set_status.call_count, 1)
 
     def test_credential_removal(self):
-        self.scope["server"] = ("username:password@httpbin.org", 80)
+        self.scope["server"] = ("username:password@mock", 80)
         self.scope["path"] = "/status/200"
         attrs = otel_asgi.collect_request_attributes(self.scope)
         self.assertEqual(
-            attrs[SpanAttributes.HTTP_URL], "http://httpbin.org/status/200"
+            attrs[SpanAttributes.HTTP_URL], "http://mock/status/200"
         )
 
     def test_collect_target_attribute_missing(self):
         self.assertIsNone(otel_asgi._collect_target_attribute(self.scope))
 
     def test_collect_target_attribute_fastapi(self):
         class TestRoute:
```

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/tests/test_getter.py` & `opentelemetry_instrumentation_asgi-0.40b0/tests/test_getter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/LICENSE` & `opentelemetry_instrumentation_asgi-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/README.rst` & `opentelemetry_instrumentation_asgi-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_asgi-0.40b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,26 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "asgiref ~= 3.0",
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
   "asgiref ~= 3.0",
 ]
 test = [
   "opentelemetry-instrumentation-asgi[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-asgi"
 
 [tool.hatch.version]
 path = "src/opentelemetry/instrumentation/asgi/version.py"
```

### Comparing `opentelemetry_instrumentation_asgi-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_asgi-0.40b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-asgi
-Version: 0.39b0
+Version: 0.40b0
 Summary: ASGI instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-asgi
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,22 +15,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: asgiref~=3.0
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
-Requires-Dist: opentelemetry-util-http==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
+Requires-Dist: opentelemetry-util-http==0.40b0
 Provides-Extra: instruments
 Requires-Dist: asgiref~=3.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-asgi[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry ASGI Instrumentation
 ==================================
 
 |pypi|
```

