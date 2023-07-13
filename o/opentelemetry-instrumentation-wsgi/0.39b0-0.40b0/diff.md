# Comparing `tmp/opentelemetry_instrumentation_wsgi-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_wsgi-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_wsgi-0.39b0.tar` & `opentelemetry_instrumentation_wsgi-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/src/opentelemetry/instrumentation/wsgi/__init__.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/src/opentelemetry/instrumentation/wsgi/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/src/opentelemetry/instrumentation/wsgi/version.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/tests/test_getter.py
--rw-r--r--   0        0        0    26416 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/tests/test_wsgi_middleware.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/LICENSE
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/README.rst
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    21375 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/src/opentelemetry/instrumentation/wsgi/__init__.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/src/opentelemetry/instrumentation/wsgi/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/src/opentelemetry/instrumentation/wsgi/version.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/tests/test_getter.py
+-rw-r--r--   0        0        0    26427 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/tests/test_wsgi_middleware.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/LICENSE
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/README.rst
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_wsgi-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/src/opentelemetry/instrumentation/wsgi/__init__.py` & `opentelemetry_instrumentation_wsgi-0.40b0/src/opentelemetry/instrumentation/wsgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,16 +436,29 @@
         span.set_attribute(SpanAttributes.HTTP_STATUS_CODE, status_code)
         span.set_status(
             Status(http_status_to_status_code(status_code, server_span=True))
         )
 
 
 def get_default_span_name(environ):
-    """Default implementation for name_callback, returns HTTP {METHOD_NAME}."""
-    return f"HTTP {environ.get('REQUEST_METHOD', '')}".strip()
+    """
+    Default span name is the HTTP method and URL path, or just the method.
+    https://github.com/open-telemetry/opentelemetry-specification/pull/3165
+    https://opentelemetry.io/docs/reference/specification/trace/semantic_conventions/http/#name
+
+    Args:
+        environ: The WSGI environ object.
+    Returns:
+        The span name.
+    """
+    method = environ.get("REQUEST_METHOD", "").strip()
+    path = environ.get("PATH_INFO", "").strip()
+    if method and path:
+        return f"{method} {path}"
+    return method
 
 
 class OpenTelemetryMiddleware:
     """The WSGI application middleware.
 
     This class is a PEP 3333 conforming WSGI middleware that starts and
     annotates spans for any requests it is invoked with.
```

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/src/opentelemetry/instrumentation/wsgi/package.py` & `opentelemetry_instrumentation_wsgi-0.40b0/src/opentelemetry/instrumentation/wsgi/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/src/opentelemetry/instrumentation/wsgi/version.py` & `opentelemetry_instrumentation_wsgi-0.40b0/src/opentelemetry/instrumentation/wsgi/version.py`

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

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/tests/__init__.py` & `opentelemetry_instrumentation_wsgi-0.40b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/tests/test_getter.py` & `opentelemetry_instrumentation_wsgi-0.40b0/tests/test_getter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/tests/test_wsgi_middleware.py` & `opentelemetry_instrumentation_wsgi-0.40b0/tests/test_wsgi_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 
 class TestWsgiApplication(WsgiTestBase):
     def validate_response(
         self,
         response,
         error=None,
-        span_name="HTTP GET",
+        span_name="GET /",
         http_method="GET",
         span_attributes=None,
         response_headers=None,
     ):
         while True:
             try:
                 value = next(response)
@@ -280,20 +280,21 @@
                             number_data_point_seen = True
                         for attr in point.attributes:
                             self.assertIn(
                                 attr, _recommended_attrs[metric.name]
                             )
         self.assertTrue(number_data_point_seen and histogram_data_point_seen)
 
-    def test_default_span_name_missing_request_method(self):
-        """Test that default span_names with missing request method."""
-        self.environ.pop("REQUEST_METHOD")
+    def test_default_span_name_missing_path_info(self):
+        """Test that default span_names with missing path info."""
+        self.environ.pop("PATH_INFO")
+        method = self.environ.get("REQUEST_METHOD", "").strip()
         app = otel_wsgi.OpenTelemetryMiddleware(simple_wsgi)
         response = app(self.environ, self.start_response)
-        self.validate_response(response, span_name="HTTP", http_method=None)
+        self.validate_response(response, span_name=method)
 
 
 class TestWsgiAttributes(unittest.TestCase):
     def setUp(self):
         self.environ = {}
         wsgiref_util.setup_testing_defaults(self.environ)
         self.span = mock.create_autospec(trace_api.Span, spec_set=True)
@@ -433,33 +434,33 @@
     def test_response_attributes(self):
         otel_wsgi.add_response_attributes(self.span, "404 Not Found", {})
         expected = (mock.call(SpanAttributes.HTTP_STATUS_CODE, 404),)
         self.assertEqual(self.span.set_attribute.call_count, len(expected))
         self.span.set_attribute.assert_has_calls(expected, any_order=True)
 
     def test_credential_removal(self):
-        self.environ["HTTP_HOST"] = "username:password@httpbin.com"
+        self.environ["HTTP_HOST"] = "username:password@mock"
         self.environ["PATH_INFO"] = "/status/200"
         expected = {
-            SpanAttributes.HTTP_URL: "http://httpbin.com/status/200",
+            SpanAttributes.HTTP_URL: "http://mock/status/200",
             SpanAttributes.NET_HOST_PORT: 80,
         }
         self.assertGreaterEqual(
             otel_wsgi.collect_request_attributes(self.environ).items(),
             expected.items(),
         )
 
 
 class TestWsgiMiddlewareWithTracerProvider(WsgiTestBase):
     def validate_response(
         self,
         response,
         exporter,
         error=None,
-        span_name="HTTP GET",
+        span_name="GET /",
         http_method="GET",
     ):
         while True:
             try:
                 value = next(response)
                 self.assertEqual(value, b"*")
             except StopIteration:
```

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/LICENSE` & `opentelemetry_instrumentation_wsgi-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/README.rst` & `opentelemetry_instrumentation_wsgi-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_wsgi-0.40b0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -22,23 +22,23 @@
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
 instruments = []
 test = [
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-wsgi"
 
 [tool.hatch.version]
 path = "src/opentelemetry/instrumentation/wsgi/version.py"
```

### Comparing `opentelemetry_instrumentation_wsgi-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_wsgi-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-wsgi
-Version: 0.39b0
+Version: 0.40b0
 Summary: WSGI Middleware for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-wsgi
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,20 @@
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
 Provides-Extra: test
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry WSGI Middleware
 =============================
 
 |pypi|
```

