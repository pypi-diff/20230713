# Comparing `tmp/opentelemetry_instrumentation_falcon-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_falcon-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_falcon-0.39b0.tar` & `opentelemetry_instrumentation_falcon-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    20375 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/__init__.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/tests/app.py
--rw-r--r--   0        0        0    23387 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/tests/test_falcon.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/LICENSE
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/README.rst
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    20785 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/src/opentelemetry/instrumentation/falcon/__init__.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/src/opentelemetry/instrumentation/falcon/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/src/opentelemetry/instrumentation/falcon/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/tests/app.py
+-rw-r--r--   0        0        0    24416 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/tests/test_falcon.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/LICENSE
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/README.rst
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/__init__.py` & `opentelemetry_instrumentation_falcon-0.40b0/src/opentelemetry/instrumentation/falcon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     _start_internal_or_server_span,
     extract_attributes_from_object,
     http_status_to_status_code,
 )
 from opentelemetry.metrics import get_meter
 from opentelemetry.semconv.metrics import MetricInstruments
 from opentelemetry.semconv.trace import SpanAttributes
-from opentelemetry.trace.status import Status
+from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.util.http import get_excluded_urls, get_traced_request_attrs
 
 _logger = getLogger(__name__)
 
 _ENVIRON_STARTTIME_KEY = "opentelemetry-falcon.starttime_key"
 _ENVIRON_SPAN_KEY = "opentelemetry-falcon.span_key"
 _ENVIRON_ACTIVATION_KEY = "opentelemetry-falcon.activation_key"
@@ -424,15 +424,14 @@
     def process_resource(self, req, resp, resource, params):
         span = req.env.get(_ENVIRON_SPAN_KEY)
         if not span or not span.is_recording():
             return
 
         resource_name = resource.__class__.__name__
         span.set_attribute("falcon.resource", resource_name)
-        span.update_name(f"{resource_name}.on_{req.method.lower()}")
 
     def process_response(
         self, req, resp, resource, req_succeeded=None
     ):  # pylint:disable=R0201,R0912
         span = req.env.get(_ENVIRON_SPAN_KEY)
 
         if not span or not span.is_recording():
@@ -457,30 +456,42 @@
                     status = "500"
                     reason = f"{exc_type.__name__}: {exc}"
 
         status = status.split(" ")[0]
         try:
             status_code = int(status)
             span.set_attribute(SpanAttributes.HTTP_STATUS_CODE, status_code)
+            otel_status_code = http_status_to_status_code(
+                status_code, server_span=True
+            )
+
+            # set the description only when the status code is ERROR
+            if otel_status_code is not StatusCode.ERROR:
+                reason = None
+
             span.set_status(
                 Status(
-                    status_code=http_status_to_status_code(
-                        status_code, server_span=True
-                    ),
+                    status_code=otel_status_code,
                     description=reason,
                 )
             )
 
             # Falcon 1 does not support response headers. So
             # send an empty dict.
             response_headers = {}
             if _falcon_version > 1:
                 response_headers = resp.headers
 
             if span.is_recording() and span.kind == trace.SpanKind.SERVER:
+                # Check if low-cardinality route is available as per semantic-conventions
+                if req.uri_template:
+                    span.update_name(f"{req.method} {req.uri_template}")
+                else:
+                    span.update_name(f"{req.method}")
+
                 custom_attributes = (
                     otel_wsgi.collect_custom_response_headers_attributes(
                         response_headers.items()
                     )
                 )
                 if len(custom_attributes) > 0:
                     span.set_attributes(custom_attributes)
```

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/package.py` & `opentelemetry_instrumentation_falcon-0.40b0/src/opentelemetry/instrumentation/falcon/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/version.py` & `opentelemetry_instrumentation_falcon-0.40b0/src/opentelemetry/instrumentation/falcon/version.py`

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

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/tests/app.py` & `opentelemetry_instrumentation_falcon-0.40b0/tests/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,14 +57,21 @@
         resp.set_header(
             "My-Custom-Regex-Header-2",
             "my-custom-regex-value-3,my-custom-regex-value-4",
         )
         resp.set_header("my-secret-header", "my-secret-value")
 
 
+class UserResource:
+    def on_get(self, req, resp, user_id):
+        # pylint: disable=no-member
+        resp.status = falcon.HTTP_200
+        resp.body = f"Hello user {user_id}"
+
+
 def make_app():
     _parsed_falcon_version = package_version.parse(falcon.__version__)
     if _parsed_falcon_version < package_version.parse("3.0.0"):
         # Falcon 1 and Falcon 2
         app = falcon.API()
     else:
         # Falcon 3
@@ -72,8 +79,10 @@
 
     app.add_route("/hello", HelloWorldResource())
     app.add_route("/ping", HelloWorldResource())
     app.add_route("/error", ErrorResource())
     app.add_route(
         "/test_custom_response_headers", CustomResponseHeaderResource()
     )
+    app.add_route("/user/{user_id}", UserResource())
+
     return app
```

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/tests/test_falcon.py` & `opentelemetry_instrumentation_falcon-0.40b0/tests/test_falcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         self._test_method("HEAD")
 
     def _test_method(self, method):
         self.client().simulate_request(method=method, path="/hello")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
         span = spans[0]
-        self.assertEqual(span.name, f"HelloWorldResource.on_{method.lower()}")
+        self.assertEqual(span.name, f"{method} /hello")
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(
             span.status.description,
             None,
         )
         self.assertSpanHasAttributes(
             span,
@@ -141,15 +141,15 @@
         self.memory_exporter.clear()
 
     def test_404(self):
         self.client().simulate_get("/does-not-exist")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
         span = spans[0]
-        self.assertEqual(span.name, "HTTP GET")
+        self.assertEqual(span.name, "GET")
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertSpanHasAttributes(
             span,
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_SERVER_NAME: "falconframework.org",
                 SpanAttributes.HTTP_SCHEME: "http",
@@ -173,15 +173,15 @@
         try:
             self.client().simulate_get("/error")
         except NameError:
             pass
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
         span = spans[0]
-        self.assertEqual(span.name, "ErrorResource.on_get")
+        self.assertEqual(span.name, "GET /error")
         self.assertFalse(span.status.is_ok)
         self.assertEqual(span.status.status_code, StatusCode.ERROR)
         self.assertEqual(
             span.status.description,
             "NameError: name 'non_existent_var' is not defined",
         )
         self.assertSpanHasAttributes(
@@ -202,14 +202,41 @@
         # In falcon>3, NET_PEER_IP is not set to anything by default to
         # https://github.com/falconry/falcon/blob/5233d0abed977d9dab78ebadf305f5abe2eef07c/falcon/testing/helpers.py#L1168-L1172 # noqa
         if SpanAttributes.NET_PEER_IP in span.attributes:
             self.assertEqual(
                 span.attributes[SpanAttributes.NET_PEER_IP], "127.0.0.1"
             )
 
+    def test_url_template(self):
+        self.client().simulate_get("/user/123")
+        spans = self.memory_exporter.get_finished_spans()
+        self.assertEqual(len(spans), 1)
+        span = spans[0]
+        self.assertEqual(span.name, "GET /user/{user_id}")
+        self.assertEqual(span.status.status_code, StatusCode.UNSET)
+        self.assertEqual(
+            span.status.description,
+            None,
+        )
+        self.assertSpanHasAttributes(
+            span,
+            {
+                SpanAttributes.HTTP_METHOD: "GET",
+                SpanAttributes.HTTP_SERVER_NAME: "falconframework.org",
+                SpanAttributes.HTTP_SCHEME: "http",
+                SpanAttributes.NET_HOST_PORT: 80,
+                SpanAttributes.HTTP_HOST: "falconframework.org",
+                SpanAttributes.HTTP_TARGET: "/",
+                SpanAttributes.NET_PEER_PORT: "65133",
+                SpanAttributes.HTTP_FLAVOR: "1.1",
+                "falcon.resource": "UserResource",
+                SpanAttributes.HTTP_STATUS_CODE: 200,
+            },
+        )
+
     def test_uninstrument(self):
         self.client().simulate_get(path="/hello")
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         self.memory_exporter.clear()
```

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/LICENSE` & `opentelemetry_instrumentation_falcon-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/README.rst` & `opentelemetry_instrumentation_falcon-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_falcon-0.40b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,28 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
-  "opentelemetry-instrumentation-wsgi == 0.39b0",
-  "opentelemetry-semantic-conventions == 0.39b0",
-  "opentelemetry-util-http == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-instrumentation-wsgi == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
+  "opentelemetry-util-http == 0.40b0",
   "packaging >= 20.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "falcon >= 1.4.1, < 4.0.0",
 ]
 test = [
   "opentelemetry-instrumentation-falcon[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "parameterized == 0.7.4",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 falcon = "opentelemetry.instrumentation.falcon:FalconInstrumentor"
 
 [project.urls]
```

### Comparing `opentelemetry_instrumentation_falcon-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_falcon-0.40b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-falcon
-Version: 0.39b0
+Version: 0.40b0
 Summary: Falcon instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-falcon
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
-Requires-Dist: opentelemetry-instrumentation-wsgi==0.39b0
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
-Requires-Dist: opentelemetry-util-http==0.39b0
+Requires-Dist: opentelemetry-instrumentation-wsgi==0.40b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
+Requires-Dist: opentelemetry-util-http==0.40b0
 Requires-Dist: packaging>=20.0
 Provides-Extra: instruments
 Requires-Dist: falcon<4.0.0,>=1.4.1; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-falcon[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: parameterized==0.7.4; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Falcon Tracing
 ============================
 
 |pypi|
```

