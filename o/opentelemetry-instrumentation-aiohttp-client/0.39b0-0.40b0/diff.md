# Comparing `tmp/opentelemetry_instrumentation_aiohttp_client-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_aiohttp_client-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0.tar` & `opentelemetry_instrumentation_aiohttp_client-0.40b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/src/opentelemetry/instrumentation/aiohttp_client/__init__.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/src/opentelemetry/instrumentation/aiohttp_client/package.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/src/opentelemetry/instrumentation/aiohttp_client/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    20412 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/tests/test_aiohttp_client_integration.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/LICENSE
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/README.rst
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/src/opentelemetry/instrumentation/aiohttp_client/__init__.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/src/opentelemetry/instrumentation/aiohttp_client/package.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/src/opentelemetry/instrumentation/aiohttp_client/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    20749 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/tests/test_aiohttp_client_integration.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/LICENSE
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/README.rst
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aiohttp_client-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/src/opentelemetry/instrumentation/aiohttp_client/__init__.py` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/src/opentelemetry/instrumentation/aiohttp_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         params: aiohttp.TraceRequestStartParams,
     ):
         if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
             trace_config_ctx.span = None
             return
 
         http_method = params.method.upper()
-        request_span_name = f"HTTP {http_method}"
+        request_span_name = f"{http_method}"
         request_url = (
             remove_url_credentials(trace_config_ctx.url_filter(params.url))
             if callable(trace_config_ctx.url_filter)
             else remove_url_credentials(str(params.url))
         )
 
         span_attributes = {
```

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/src/opentelemetry/instrumentation/aiohttp_client/package.py` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/src/opentelemetry/instrumentation/aiohttp_client/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/src/opentelemetry/instrumentation/aiohttp_client/version.py` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/src/opentelemetry/instrumentation/aiohttp_client/version.py`

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

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/tests/test_aiohttp_client_integration.py` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/tests/test_aiohttp_client_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import urllib.parse
 from http import HTTPStatus
 from unittest import mock
 
 import aiohttp
 import aiohttp.test_utils
 import yarl
+from http_server_mock import HttpServerMock
 from pkg_resources import iter_entry_points
 
 from opentelemetry import context
 from opentelemetry import trace as trace_api
 from opentelemetry.instrumentation import aiohttp_client
 from opentelemetry.instrumentation.aiohttp_client import (
     AioHttpClientInstrumentor,
@@ -114,15 +115,15 @@
                     url="/test-path?query=param#foobar",
                     status_code=status_code,
                 )
 
                 self.assert_spans(
                     [
                         (
-                            "HTTP GET",
+                            "GET",
                             (span_status, None),
                             {
                                 SpanAttributes.HTTP_METHOD: "GET",
                                 SpanAttributes.HTTP_URL: f"http://{host}:{port}/test-path#foobar",
                                 SpanAttributes.HTTP_STATUS_CODE: int(
                                     status_code
                                 ),
@@ -208,15 +209,15 @@
             url="/some/path?query=param&other=param2",
             status_code=HTTPStatus.OK,
         )
 
         self.assert_spans(
             [
                 (
-                    "HTTP GET",
+                    "GET",
                     (StatusCode.UNSET, None),
                     {
                         SpanAttributes.HTTP_METHOD: "GET",
                         SpanAttributes.HTTP_URL: f"http://{host}:{port}/some/path",
                         SpanAttributes.HTTP_STATUS_CODE: int(HTTPStatus.OK),
                     },
                 )
@@ -242,15 +243,15 @@
                 loop = asyncio.get_event_loop()
                 with self.assertRaises(aiohttp.ClientConnectorError):
                     loop.run_until_complete(do_request(url))
 
             self.assert_spans(
                 [
                     (
-                        "HTTP GET",
+                        "GET",
                         (expected_status, None),
                         {
                             SpanAttributes.HTTP_METHOD: "GET",
                             SpanAttributes.HTTP_URL: url,
                         },
                     )
                 ]
@@ -269,15 +270,15 @@
             request_handler=request_handler,
             timeout=aiohttp.ClientTimeout(sock_read=0.01),
         )
 
         self.assert_spans(
             [
                 (
-                    "HTTP GET",
+                    "GET",
                     (StatusCode.ERROR, None),
                     {
                         SpanAttributes.HTTP_METHOD: "GET",
                         SpanAttributes.HTTP_URL: f"http://{host}:{port}/test_timeout",
                     },
                 )
             ]
@@ -296,48 +297,58 @@
             request_handler=request_handler,
             max_redirects=2,
         )
 
         self.assert_spans(
             [
                 (
-                    "HTTP GET",
+                    "GET",
                     (StatusCode.ERROR, None),
                     {
                         SpanAttributes.HTTP_METHOD: "GET",
                         SpanAttributes.HTTP_URL: f"http://{host}:{port}/test_too_many_redirects",
                     },
                 )
             ]
         )
 
     def test_credential_removal(self):
         trace_configs = [aiohttp_client.create_trace_config()]
 
-        url = "http://username:password@httpbin.org/status/200"
-        with self.subTest(url=url):
+        app = HttpServerMock("test_credential_removal")
 
-            async def do_request(url):
-                async with aiohttp.ClientSession(
-                    trace_configs=trace_configs,
-                ) as session:
-                    async with session.get(url):
-                        pass
+        @app.route("/status/200")
+        def index():
+            return "hello"
 
-            loop = asyncio.get_event_loop()
-            loop.run_until_complete(do_request(url))
+        url = "http://username:password@localhost:5000/status/200"
+
+        with app.run("localhost", 5000):
+            with self.subTest(url=url):
+
+                async def do_request(url):
+                    async with aiohttp.ClientSession(
+                        trace_configs=trace_configs,
+                    ) as session:
+                        async with session.get(url):
+                            pass
+
+                loop = asyncio.get_event_loop()
+                loop.run_until_complete(do_request(url))
 
         self.assert_spans(
             [
                 (
-                    "HTTP GET",
+                    "GET",
                     (StatusCode.UNSET, None),
                     {
                         SpanAttributes.HTTP_METHOD: "GET",
-                        SpanAttributes.HTTP_URL: "http://httpbin.org/status/200",
+                        SpanAttributes.HTTP_URL: (
+                            "http://localhost:5000/status/200"
+                        ),
                         SpanAttributes.HTTP_STATUS_CODE: int(HTTPStatus.OK),
                     },
                 )
             ]
         )
         self.memory_exporter.clear()
 
@@ -376,14 +387,15 @@
         return finished_spans
 
     def test_instrument(self):
         host, port = run_with_test_server(
             self.get_default_request(), self.URL, self.default_handler
         )
         span = self.assert_spans(1)
+        self.assertEqual("GET", span.name)
         self.assertEqual("GET", span.attributes[SpanAttributes.HTTP_METHOD])
         self.assertEqual(
             f"http://{host}:{port}/test-path",
             span.attributes[SpanAttributes.HTTP_URL],
         )
         self.assertEqual(200, span.attributes[SpanAttributes.HTTP_STATUS_CODE])
```

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/LICENSE` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/README.rst` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -22,26 +22,27 @@
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
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "aiohttp ~= 3.0",
 ]
 test = [
   "opentelemetry-instrumentation-aiohttp-client[instruments]",
+  "http-server-mock"
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 aiohttp-client = "opentelemetry.instrumentation.aiohttp_client:AioHttpClientInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aiohttp-client"
```

### Comparing `opentelemetry_instrumentation_aiohttp_client-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_aiohttp_client-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-aiohttp-client
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry aiohttp client instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aiohttp-client
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,22 @@
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
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: aiohttp~=3.0; extra == 'instruments'
 Provides-Extra: test
+Requires-Dist: http-server-mock; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-aiohttp-client[instruments]; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry aiohttp client Integration
 ========================================
 
 |pypi|
```

