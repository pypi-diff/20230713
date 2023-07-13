# Comparing `tmp/opentelemetry_instrumentation_httpx-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_httpx-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_httpx-0.39b0.tar` & `opentelemetry_instrumentation_httpx-0.40b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    20909 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/src/opentelemetry/instrumentation/httpx/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/src/opentelemetry/instrumentation/httpx/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/src/opentelemetry/instrumentation/httpx/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    24756 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/tests/test_httpx_integration.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/LICENSE
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/README.rst
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    20890 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/src/opentelemetry/instrumentation/httpx/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/src/opentelemetry/instrumentation/httpx/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/src/opentelemetry/instrumentation/httpx/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    24746 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/tests/test_httpx_integration.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/LICENSE
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/README.rst
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_httpx-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/src/opentelemetry/instrumentation/httpx/__init__.py` & `opentelemetry_instrumentation_httpx-0.40b0/src/opentelemetry/instrumentation/httpx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 When using the instrumentor, all clients will automatically trace requests.
 
 .. code-block:: python
 
      import httpx
      from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
-     url = "https://httpbin.org/get"
+     url = "https://some.url/get"
      HTTPXClientInstrumentor().instrument()
 
      with httpx.Client() as client:
           response = client.get(url)
 
      async with httpx.AsyncClient() as client:
           response = await client.get(url)
@@ -42,15 +42,15 @@
 
 
 .. code-block:: python
 
     import httpx
     from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
-    url = "https://httpbin.org/get"
+    url = "https://some.url/get"
 
     with httpx.Client(transport=telemetry_transport) as client:
         HTTPXClientInstrumentor.instrument_client(client)
         response = client.get(url)
 
     async with httpx.AsyncClient(transport=telemetry_transport) as client:
         HTTPXClientInstrumentor.instrument_client(client)
@@ -87,15 +87,15 @@
 
     import httpx
     from opentelemetry.instrumentation.httpx import (
         AsyncOpenTelemetryTransport,
         SyncOpenTelemetryTransport,
     )
 
-    url = "https://httpbin.org/get"
+    url = "https://some.url/get"
     transport = httpx.HTTPTransport()
     telemetry_transport = SyncOpenTelemetryTransport(transport)
 
     with httpx.Client(transport=telemetry_transport) as client:
         response = client.get(url)
 
     transport = httpx.AsyncHTTPTransport()
@@ -205,15 +205,15 @@
     status_code: int
     headers: typing.Optional[Headers]
     stream: typing.Iterable[bytes]
     extensions: typing.Optional[dict]
 
 
 def _get_default_span_name(method: str) -> str:
-    return f"HTTP {method.strip()}"
+    return method.strip()
 
 
 def _apply_status_code(span: Span, status_code: int) -> None:
     if not span.is_recording():
         return
 
     span.set_attribute(SpanAttributes.HTTP_STATUS_CODE, status_code)
```

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/src/opentelemetry/instrumentation/httpx/package.py` & `opentelemetry_instrumentation_httpx-0.40b0/src/opentelemetry/instrumentation/httpx/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/src/opentelemetry/instrumentation/httpx/version.py` & `opentelemetry_instrumentation_httpx-0.40b0/src/opentelemetry/instrumentation/httpx/version.py`

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

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/tests/test_httpx_integration.py` & `opentelemetry_instrumentation_httpx-0.40b0/tests/test_httpx_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,24 @@
     loop = asyncio.get_event_loop()
     return loop.run_until_complete(coro)
 
 
 def _response_hook(span, request: "RequestInfo", response: "ResponseInfo"):
     span.set_attribute(
         HTTP_RESPONSE_BODY,
-        response[2].read(),
+        b"".join(response[2]),
     )
 
 
 async def _async_response_hook(
     span: "Span", request: "RequestInfo", response: "ResponseInfo"
 ):
     span.set_attribute(
         HTTP_RESPONSE_BODY,
-        await response[2].aread(),
+        b"".join([part async for part in response[2]]),
     )
 
 
 def _request_hook(span: "Span", request: "RequestInfo"):
     url = httpx.URL(request[1])
     span.update_name("GET" + str(url))
 
@@ -93,15 +93,15 @@
 # Using this wrapper class to have a base class for the tests while also not
 # angering pylint or mypy when calling methods not in the class when only
 # subclassing abc.ABC.
 class BaseTestCases:
     class BaseTest(TestBase, metaclass=abc.ABCMeta):
         # pylint: disable=no-member
 
-        URL = "http://httpbin.org/status/200"
+        URL = "http://mock/status/200"
         response_hook = staticmethod(_response_hook)
         request_hook = staticmethod(_request_hook)
         no_update_request_hook = staticmethod(_no_update_request_hook)
 
         # pylint: disable=invalid-name
         def setUp(self):
             super().setUp()
@@ -138,15 +138,15 @@
 
         def test_basic(self):
             result = self.perform_request(self.URL)
             self.assertEqual(result.text, "Hello!")
             span = self.assert_span()
 
             self.assertIs(span.kind, trace.SpanKind.CLIENT)
-            self.assertEqual(span.name, "HTTP GET")
+            self.assertEqual(span.name, "GET")
 
             self.assertEqual(
                 span.attributes,
                 {
                     SpanAttributes.HTTP_METHOD: "GET",
                     SpanAttributes.HTTP_URL: self.URL,
                     SpanAttributes.HTTP_STATUS_CODE: 200,
@@ -161,15 +161,15 @@
 
         def test_basic_multiple(self):
             self.perform_request(self.URL)
             self.perform_request(self.URL)
             self.assert_span(num_spans=2)
 
         def test_not_foundbasic(self):
-            url_404 = "http://httpbin.org/status/404"
+            url_404 = "http://mock/status/404"
 
             with respx.mock:
                 respx.get(url_404).mock(httpx.Response(404))
                 result = self.perform_request(url_404)
 
             self.assertEqual(result.status_code, 404)
             span = self.assert_span()
@@ -254,15 +254,15 @@
 
             with respx.mock, self.assertRaises(httpx.UnsupportedProtocol):
                 respx.post("invalid://nope").pass_through()
                 self.perform_request(url, method="POST")
 
             span = self.assert_span()
 
-            self.assertEqual(span.name, "HTTP POST")
+            self.assertEqual(span.name, "POST")
             self.assertEqual(
                 span.attributes[SpanAttributes.HTTP_METHOD], "POST"
             )
             self.assertEqual(span.attributes[SpanAttributes.HTTP_URL], url)
             self.assertEqual(span.status.status_code, StatusCode.ERROR)
 
         def test_if_headers_equals_none(self):
@@ -346,15 +346,15 @@
                 request_hook=self.no_update_request_hook
             )
             client = self.create_client(transport)
             result = self.perform_request(self.URL, client=client)
 
             self.assertEqual(result.text, "Hello!")
             span = self.assert_span()
-            self.assertEqual(span.name, "HTTP GET")
+            self.assertEqual(span.name, "GET")
 
         def test_not_recording(self):
             with mock.patch("opentelemetry.trace.INVALID_SPAN") as mock_span:
                 transport = self.create_transport(
                     tracer_provider=trace.NoOpTracerProvider()
                 )
                 client = self.create_client(transport)
@@ -440,15 +440,15 @@
                 request_hook=self.no_update_request_hook,
             )
             client = self.create_client()
             result = self.perform_request(self.URL, client=client)
 
             self.assertEqual(result.text, "Hello!")
             span = self.assert_span()
-            self.assertEqual(span.name, "HTTP GET")
+            self.assertEqual(span.name, "GET")
             HTTPXClientInstrumentor().uninstrument()
 
         def test_not_recording(self):
             with mock.patch("opentelemetry.trace.INVALID_SPAN") as mock_span:
                 HTTPXClientInstrumentor().instrument(
                     tracer_provider=trace.NoOpTracerProvider()
                 )
```

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/LICENSE` & `opentelemetry_instrumentation_httpx-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/README.rst` & `opentelemetry_instrumentation_httpx-0.40b0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 When using the instrumentor, all clients will automatically trace requests.
 
 .. code-block:: python
 
      import httpx
      from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
-     url = "https://httpbin.org/get"
+     url = "https://some.url/get"
      HTTPXClientInstrumentor().instrument()
 
      with httpx.Client() as client:
           response = client.get(url)
 
      async with httpx.AsyncClient() as client:
           response = await client.get(url)
@@ -47,15 +47,15 @@
 
 
 .. code-block:: python
 
     import httpx
     from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
-    url = "https://httpbin.org/get"
+    url = "https://some.url/get"
 
     with httpx.Client(transport=telemetry_transport) as client:
         HTTPXClientInstrumentor.instrument_client(client)
         response = client.get(url)
 
     async with httpx.AsyncClient(transport=telemetry_transport) as client:
         HTTPXClientInstrumentor.instrument_client(client)
@@ -92,15 +92,15 @@
 
     import httpx
     from opentelemetry.instrumentation.httpx import (
         AsyncOpenTelemetryTransport,
         SyncOpenTelemetryTransport,
     )
 
-    url = "https://httpbin.org/get"
+    url = "https://some.url/get"
     transport = httpx.HTTPTransport()
     telemetry_transport = SyncOpenTelemetryTransport(transport)
 
     with httpx.Client(transport=telemetry_transport) as client:
         response = client.get(url)
 
     transport = httpx.AsyncHTTPTransport()
```

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_httpx-0.40b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,26 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
-  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
-  "httpx >= 0.18.0, <= 0.23.0",
+  "httpx >= 0.18.0",
 ]
 test = [
   "opentelemetry-instrumentation-httpx[instruments]",
   "opentelemetry-sdk ~= 1.12",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 httpx = "opentelemetry.instrumentation.httpx:HTTPXClientInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-httpx"
```

### Comparing `opentelemetry_instrumentation_httpx-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_httpx-0.40b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-httpx
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry HTTPX Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-httpx
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Provides-Extra: instruments
-Requires-Dist: httpx<=0.23.0,>=0.18.0; extra == 'instruments'
+Requires-Dist: httpx>=0.18.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-httpx[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.12; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry HTTPX Instrumentation
 ===================================
 
 |pypi|
 
@@ -56,15 +56,15 @@
 When using the instrumentor, all clients will automatically trace requests.
 
 .. code-block:: python
 
      import httpx
      from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
-     url = "https://httpbin.org/get"
+     url = "https://some.url/get"
      HTTPXClientInstrumentor().instrument()
 
      with httpx.Client() as client:
           response = client.get(url)
 
      async with httpx.AsyncClient() as client:
           response = await client.get(url)
@@ -77,15 +77,15 @@
 
 
 .. code-block:: python
 
     import httpx
     from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
-    url = "https://httpbin.org/get"
+    url = "https://some.url/get"
 
     with httpx.Client(transport=telemetry_transport) as client:
         HTTPXClientInstrumentor.instrument_client(client)
         response = client.get(url)
 
     async with httpx.AsyncClient(transport=telemetry_transport) as client:
         HTTPXClientInstrumentor.instrument_client(client)
@@ -122,15 +122,15 @@
 
     import httpx
     from opentelemetry.instrumentation.httpx import (
         AsyncOpenTelemetryTransport,
         SyncOpenTelemetryTransport,
     )
 
-    url = "https://httpbin.org/get"
+    url = "https://some.url/get"
     transport = httpx.HTTPTransport()
     telemetry_transport = SyncOpenTelemetryTransport(transport)
 
     with httpx.Client(transport=telemetry_transport) as client:
         response = client.get(url)
 
     transport = httpx.AsyncHTTPTransport()
```

