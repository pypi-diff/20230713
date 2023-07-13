# Comparing `tmp/opentelemetry_instrumentation_fastapi-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_fastapi-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_fastapi-0.39b0.tar` & `opentelemetry_instrumentation_fastapi-0.40b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    33406 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/tests/test_fastapi_instrumentation.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/LICENSE
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/README.rst
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/src/opentelemetry/instrumentation/fastapi/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/src/opentelemetry/instrumentation/fastapi/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/src/opentelemetry/instrumentation/fastapi/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    34236 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/tests/test_fastapi_instrumentation.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/LICENSE
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/README.rst
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/__init__.py` & `opentelemetry_instrumentation_fastapi-0.40b0/src/opentelemetry/instrumentation/fastapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             else:
                 excluded_urls = parse_excluded_urls(excluded_urls)
             meter = get_meter(__name__, __version__, meter_provider)
 
             app.add_middleware(
                 OpenTelemetryMiddleware,
                 excluded_urls=excluded_urls,
-                default_span_details=_get_route_details,
+                default_span_details=_get_default_span_details,
                 server_request_hook=server_request_hook,
                 client_request_hook=client_request_hook,
                 client_response_hook=client_response_hook,
                 tracer_provider=tracer_provider,
                 meter=meter,
             )
             app._is_instrumented_by_opentelemetry = True
@@ -296,15 +296,15 @@
         super().__init__(*args, **kwargs)
         meter = get_meter(
             __name__, __version__, _InstrumentedFastAPI._meter_provider
         )
         self.add_middleware(
             OpenTelemetryMiddleware,
             excluded_urls=_InstrumentedFastAPI._excluded_urls,
-            default_span_details=_get_route_details,
+            default_span_details=_get_default_span_details,
             server_request_hook=_InstrumentedFastAPI._server_request_hook,
             client_request_hook=_InstrumentedFastAPI._client_request_hook,
             client_response_hook=_InstrumentedFastAPI._client_response_hook,
             tracer_provider=_InstrumentedFastAPI._tracer_provider,
             meter=meter,
         )
         self._is_instrumented_by_opentelemetry = True
@@ -312,30 +312,53 @@
 
     def __del__(self):
         if self in _InstrumentedFastAPI._instrumented_fastapi_apps:
             _InstrumentedFastAPI._instrumented_fastapi_apps.remove(self)
 
 
 def _get_route_details(scope):
-    """Callback to retrieve the fastapi route being served.
+    """
+    Function to retrieve Starlette route from scope.
 
     TODO: there is currently no way to retrieve http.route from
     a starlette application from scope.
-
     See: https://github.com/encode/starlette/pull/804
+
+    Args:
+        scope: A Starlette scope
+    Returns:
+        A string containing the route or None
     """
     app = scope["app"]
     route = None
+
     for starlette_route in app.routes:
         match, _ = starlette_route.matches(scope)
         if match == Match.FULL:
             route = starlette_route.path
             break
         if match == Match.PARTIAL:
             route = starlette_route.path
-    # method only exists for http, if websocket
-    # leave it blank.
-    span_name = route or scope.get("method", "")
+    return route
+
+
+def _get_default_span_details(scope):
+    """
+    Callback to retrieve span name and attributes from scope.
+
+    Args:
+        scope: A Starlette scope
+    Returns:
+        A tuple of span name and attributes
+    """
+    route = _get_route_details(scope)
+    method = scope.get("method", "")
     attributes = {}
     if route:
         attributes[SpanAttributes.HTTP_ROUTE] = route
+    if method and route:  # http
+        span_name = f"{method} {route}"
+    elif route:  # websocket
+        span_name = route
+    else:  # fallback
+        span_name = method
     return span_name, attributes
```

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/package.py` & `opentelemetry_instrumentation_fastapi-0.40b0/src/opentelemetry/instrumentation/fastapi/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/version.py` & `opentelemetry_instrumentation_fastapi-0.40b0/src/opentelemetry/instrumentation/fastapi/version.py`

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

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/tests/test_fastapi_instrumentation.py` & `opentelemetry_instrumentation_fastapi-0.40b0/tests/test_fastapi_instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,28 @@
     _duration_attrs,
     get_excluded_urls,
 )
 
 _expected_metric_names = [
     "http.server.active_requests",
     "http.server.duration",
+    "http.server.response.size",
+    "http.server.request.size",
 ]
 _recommended_attrs = {
     "http.server.active_requests": _active_requests_count_attrs,
     "http.server.duration": {*_duration_attrs, SpanAttributes.HTTP_TARGET},
+    "http.server.response.size": {
+        *_duration_attrs,
+        SpanAttributes.HTTP_TARGET,
+    },
+    "http.server.request.size": {
+        *_duration_attrs,
+        SpanAttributes.HTTP_TARGET,
+    },
 }
 
 
 class TestFastAPIManualInstrumentation(TestBase):
     def _create_app(self):
         app = self._create_fastapi_app()
         self._instrumentor.instrument_app(
@@ -102,15 +112,15 @@
     def test_instrument_app_with_instrument(self):
         if not isinstance(self, TestAutoInstrumentation):
             self._instrumentor.instrument()
         self._client.get("/foobar")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 3)
         for span in spans:
-            self.assertIn("/foobar", span.name)
+            self.assertIn("GET /foobar", span.name)
 
     def test_uninstrument_app(self):
         self._client.get("/foobar")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 3)
 
         self._instrumentor.uninstrument_app(self._app)
@@ -134,23 +144,23 @@
         self.assertEqual(len(spans), 0)
 
     def test_basic_fastapi_call(self):
         self._client.get("/foobar")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 3)
         for span in spans:
-            self.assertIn("/foobar", span.name)
+            self.assertIn("GET /foobar", span.name)
 
     def test_fastapi_route_attribute_added(self):
         """Ensure that fastapi routes are used as the span name."""
         self._client.get("/user/123")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 3)
         for span in spans:
-            self.assertIn("/user/{username}", span.name)
+            self.assertIn("GET /user/{username}", span.name)
         self.assertEqual(
             spans[-1].attributes[SpanAttributes.HTTP_ROUTE], "/user/{username}"
         )
         # ensure that at least one attribute that is populated by
         # the asgi instrumentation is successfully feeding though.
         self.assertEqual(
             spans[-1].attributes[SpanAttributes.HTTP_FLAVOR], "1.1"
@@ -183,15 +193,15 @@
         metrics_list = self.memory_metrics_reader.get_metrics_data()
         number_data_point_seen = False
         histogram_data_point_seen = False
         self.assertTrue(len(metrics_list.resource_metrics) == 1)
         for resource_metric in metrics_list.resource_metrics:
             self.assertTrue(len(resource_metric.scope_metrics) == 1)
             for scope_metric in resource_metric.scope_metrics:
-                self.assertTrue(len(scope_metric.metrics) == 2)
+                self.assertTrue(len(scope_metric.metrics) == 3)
                 for metric in scope_metric.metrics:
                     self.assertIn(metric.name, _expected_metric_names)
                     data_points = list(metric.data.data_points)
                     self.assertEqual(len(data_points), 1)
                     for point in data_points:
                         if isinstance(point, HistogramDataPoint):
                             self.assertEqual(point.count, 3)
@@ -242,24 +252,34 @@
                         expected_requests_count_attributes,
                         dict(point.attributes),
                     )
                     self.assertEqual(point.value, 0)
 
     def test_basic_post_request_metric_success(self):
         start = default_timer()
-        self._client.post("/foobar")
+        response = self._client.post(
+            "/foobar",
+            json={"foo": "bar"},
+        )
         duration = max(round((default_timer() - start) * 1000), 0)
+        response_size = int(response.headers.get("content-length"))
+        request_size = int(response.request.headers.get("content-length"))
         metrics_list = self.memory_metrics_reader.get_metrics_data()
         for metric in (
             metrics_list.resource_metrics[0].scope_metrics[0].metrics
         ):
             for point in list(metric.data.data_points):
                 if isinstance(point, HistogramDataPoint):
                     self.assertEqual(point.count, 1)
-                    self.assertAlmostEqual(duration, point.sum, delta=30)
+                    if metric.name == "http.server.duration":
+                        self.assertAlmostEqual(duration, point.sum, delta=30)
+                    elif metric.name == "http.server.response.size":
+                        self.assertEqual(response_size, point.sum)
+                    elif metric.name == "http.server.request.size":
+                        self.assertEqual(request_size, point.sum)
                 if isinstance(point, NumberDataPoint):
                     self.assertEqual(point.value, 0)
 
     def test_metric_uninstruemnt_app(self):
         self._client.get("/foobar")
         self._instrumentor.uninstrument_app(self._app)
         self._client.get("/foobar")
```

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/LICENSE` & `opentelemetry_instrumentation_fastapi-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/README.rst` & `opentelemetry_instrumentation_fastapi-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_fastapi-0.40b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -22,27 +22,27 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
-  "opentelemetry-instrumentation-asgi == 0.39b0",
-  "opentelemetry-semantic-conventions == 0.39b0",
-  "opentelemetry-util-http == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-instrumentation-asgi == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
+  "opentelemetry-util-http == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "fastapi ~= 0.58",
 ]
 test = [
   "opentelemetry-instrumentation-fastapi[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "requests ~= 2.23", # needed for testclient
   "httpx ~= 0.22", # needed for testclient
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 fastapi = "opentelemetry.instrumentation.fastapi:FastAPIInstrumentor"
```

### Comparing `opentelemetry_instrumentation_fastapi-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_fastapi-0.40b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-fastapi
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry FastAPI Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-fastapi
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,24 +14,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation-asgi==0.39b0
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
-Requires-Dist: opentelemetry-util-http==0.39b0
+Requires-Dist: opentelemetry-instrumentation-asgi==0.40b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
+Requires-Dist: opentelemetry-util-http==0.40b0
 Provides-Extra: instruments
 Requires-Dist: fastapi~=0.58; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: httpx~=0.22; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-fastapi[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: requests~=2.23; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry FastAPI Instrumentation
 =======================================
 
 |pypi|
```

