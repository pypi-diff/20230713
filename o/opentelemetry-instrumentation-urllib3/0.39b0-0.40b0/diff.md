# Comparing `tmp/opentelemetry_instrumentation_urllib3-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_urllib3-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_urllib3-0.39b0.tar` & `opentelemetry_instrumentation_urllib3-0.40b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/__init__.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_integration.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_ip_support.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_metrics.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/LICENSE
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/README.rst
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    12317 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/src/opentelemetry/instrumentation/urllib3/__init__.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/src/opentelemetry/instrumentation/urllib3/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/src/opentelemetry/instrumentation/urllib3/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    13686 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/tests/test_urllib3_integration.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/tests/test_urllib3_ip_support.py
+-rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/tests/test_urllib3_metrics.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/LICENSE
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/README.rst
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/__init__.py` & `opentelemetry_instrumentation_urllib3-0.40b0/src/opentelemetry/instrumentation/urllib3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         pass
 
     # `request` is an instance of urllib3.connectionpool.HTTPConnectionPool
     # `response` is an instance of urllib3.response.HTTPResponse
     def response_hook(span, request, response):
         pass
 
-    URLLib3Instrumentor.instrument(
-        request_hook=request_hook, response_hook=response_hook)
+    URLLib3Instrumentor().instrument(
+        request_hook=request_hook, response_hook=response_hook
     )
 
 Exclude lists
 *************
 
 To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB3_EXCLUDED_URLS``
 (or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
@@ -221,15 +221,15 @@
         if excluded_urls and excluded_urls.url_disabled(url):
             return wrapped(*args, **kwargs)
 
         method = _get_url_open_arg("method", args, kwargs).upper()
         headers = _prepare_headers(kwargs)
         body = _get_url_open_arg("body", args, kwargs)
 
-        span_name = f"HTTP {method.strip()}"
+        span_name = method.strip()
         span_attributes = {
             SpanAttributes.HTTP_METHOD: method,
             SpanAttributes.HTTP_URL: url,
         }
 
         with tracer.start_as_current_span(
             span_name, kind=SpanKind.CLIENT, attributes=span_attributes
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/package.py` & `opentelemetry_instrumentation_urllib3-0.40b0/src/opentelemetry/instrumentation/urllib3/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-_instruments = ("urllib3 >= 1.0.0, < 2.0.0",)
+_instruments = ("urllib3 >= 1.0.0, < 3.0.0",)
 
 _supports_metrics = True
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/version.py` & `opentelemetry_instrumentation_urllib3-0.40b0/src/opentelemetry/instrumentation/urllib3/version.py`

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

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_integration.py` & `opentelemetry_instrumentation_urllib3-0.40b0/tests/test_urllib3_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from opentelemetry.test.test_base import TestBase
 from opentelemetry.util.http import get_excluded_urls
 
 # pylint: disable=too-many-public-methods
 
 
 class TestURLLib3Instrumentor(TestBase):
-    HTTP_URL = "http://httpbin.org/status/200"
-    HTTPS_URL = "https://httpbin.org/status/200"
+    HTTP_URL = "http://mock/status/200"
+    HTTPS_URL = "https://mock/status/200"
 
     def setUp(self):
         super().setUp()
 
         self.env_patch = mock.patch.dict(
             "os.environ",
             {
@@ -83,15 +83,15 @@
     def assert_success_span(
         self, response: urllib3.response.HTTPResponse, url: str
     ):
         self.assertEqual(b"Hello!", response.data)
 
         span = self.assert_span()
         self.assertIs(trace.SpanKind.CLIENT, span.kind)
-        self.assertEqual("HTTP GET", span.name)
+        self.assertEqual("GET", span.name)
 
         attributes = {
             SpanAttributes.HTTP_METHOD: "GET",
             SpanAttributes.HTTP_URL: url,
             SpanAttributes.HTTP_STATUS_CODE: 200,
         }
         self.assertEqual(attributes, span.attributes)
@@ -119,67 +119,67 @@
         return pool.request("GET", url, headers=headers, retries=retries)
 
     def test_basic_http_success(self):
         response = self.perform_request(self.HTTP_URL)
         self.assert_success_span(response, self.HTTP_URL)
 
     def test_basic_http_success_using_connection_pool(self):
-        pool = urllib3.HTTPConnectionPool("httpbin.org")
+        pool = urllib3.HTTPConnectionPool("mock")
         response = pool.request("GET", "/status/200")
 
         self.assert_success_span(response, self.HTTP_URL)
 
     def test_basic_https_success(self):
         response = self.perform_request(self.HTTPS_URL)
         self.assert_success_span(response, self.HTTPS_URL)
 
     def test_basic_https_success_using_connection_pool(self):
-        pool = urllib3.HTTPSConnectionPool("httpbin.org")
+        pool = urllib3.HTTPSConnectionPool("mock")
         response = pool.request("GET", "/status/200")
 
         self.assert_success_span(response, self.HTTPS_URL)
 
     def test_basic_not_found(self):
-        url_404 = "http://httpbin.org/status/404"
+        url_404 = "http://mock/status/404"
         httpretty.register_uri(httpretty.GET, url_404, status=404)
 
         response = self.perform_request(url_404)
         self.assertEqual(404, response.status)
 
         span = self.assert_span()
         self.assertEqual(
             404, span.attributes.get(SpanAttributes.HTTP_STATUS_CODE)
         )
         self.assertIs(trace.status.StatusCode.ERROR, span.status.status_code)
 
     def test_basic_http_non_default_port(self):
-        url = "http://httpbin.org:666/status/200"
+        url = "http://mock:666/status/200"
         httpretty.register_uri(httpretty.GET, url, body="Hello!")
 
         response = self.perform_request(url)
         self.assert_success_span(response, url)
 
     def test_basic_http_absolute_url(self):
-        url = "http://httpbin.org:666/status/200"
+        url = "http://mock:666/status/200"
         httpretty.register_uri(httpretty.GET, url, body="Hello!")
-        pool = urllib3.HTTPConnectionPool("httpbin.org", port=666)
+        pool = urllib3.HTTPConnectionPool("mock", port=666)
         response = pool.request("GET", url)
 
         self.assert_success_span(response, url)
 
     def test_url_open_explicit_arg_parameters(self):
-        url = "http://httpbin.org:666/status/200"
+        url = "http://mock:666/status/200"
         httpretty.register_uri(httpretty.GET, url, body="Hello!")
-        pool = urllib3.HTTPConnectionPool("httpbin.org", port=666)
+        pool = urllib3.HTTPConnectionPool("mock", port=666)
         response = pool.urlopen(method="GET", url="/status/200")
 
         self.assert_success_span(response, url)
 
     def test_excluded_urls_explicit(self):
-        url_201 = "http://httpbin.org/status/201"
+        url_201 = "http://mock/status/201"
         httpretty.register_uri(
             httpretty.GET,
             url_201,
             status=201,
         )
 
         URLLib3Instrumentor().uninstrument()
@@ -297,15 +297,15 @@
         URLLib3Instrumentor().uninstrument()
         URLLib3Instrumentor().instrument(url_filter=url_filter)
 
         response = self.perform_request(self.HTTP_URL + "?e=mcc")
         self.assert_success_span(response, self.HTTP_URL)
 
     def test_credential_removal(self):
-        url = "http://username:password@httpbin.org/status/200"
+        url = "http://username:password@mock/status/200"
 
         response = self.perform_request(url)
         self.assert_success_span(response, self.HTTP_URL)
 
     def test_hooks(self):
         def request_hook(span, request, body, headers):
             span.update_name("name set from hook")
@@ -324,26 +324,28 @@
 
         self.assertEqual(span.name, "name set from hook")
         self.assertIn("response_hook_attr", span.attributes)
         self.assertEqual(span.attributes["response_hook_attr"], "value")
 
     def test_request_hook_params(self):
         def request_hook(span, request, headers, body):
-            span.set_attribute("request_hook_headers", json.dumps(headers))
+            span.set_attribute(
+                "request_hook_headers", json.dumps(dict(headers))
+            )
             span.set_attribute("request_hook_body", body)
 
         URLLib3Instrumentor().uninstrument()
         URLLib3Instrumentor().instrument(
             request_hook=request_hook,
         )
 
         headers = {"header1": "value1", "header2": "value2"}
         body = "param1=1&param2=2"
 
-        pool = urllib3.HTTPConnectionPool("httpbin.org")
+        pool = urllib3.HTTPConnectionPool("mock")
         response = pool.request(
             "POST", "/status/200", body=body, headers=headers
         )
 
         self.assertEqual(b"Hello!", response.data)
 
         span = self.assert_span()
@@ -362,15 +364,15 @@
         URLLib3Instrumentor().uninstrument()
         URLLib3Instrumentor().instrument(
             request_hook=request_hook,
         )
 
         body = "param1=1&param2=2"
 
-        pool = urllib3.HTTPConnectionPool("httpbin.org")
+        pool = urllib3.HTTPConnectionPool("mock")
         response = pool.urlopen("POST", "/status/200", body)
 
         self.assertEqual(b"Hello!", response.data)
 
         span = self.assert_span()
 
         self.assertIn("request_hook_body", span.attributes)
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_ip_support.py` & `opentelemetry_instrumentation_urllib3-0.40b0/tests/test_urllib3_ip_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,14 @@
     def assert_success_span(
         self, response: urllib3.response.HTTPResponse, url: str
     ):
         self.assertEqual(b"Hello!", response.data)
 
         span = self.assert_span()
         self.assertIs(trace.SpanKind.CLIENT, span.kind)
-        self.assertEqual("HTTP GET", span.name)
+        self.assertEqual("GET", span.name)
 
         attributes = {
             "http.status_code": 200,
             "net.peer.ip": self.assert_ip,
         }
         self.assertGreaterEqual(span.attributes.items(), attributes.items())
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_metrics.py` & `opentelemetry_instrumentation_urllib3-0.40b0/tests/test_urllib3_metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 import io
 from timeit import default_timer
 
 import httpretty
 import urllib3
 import urllib3.exceptions
-from urllib3.request import encode_multipart_formdata
+from urllib3 import encode_multipart_formdata
 
 from opentelemetry.instrumentation.urllib3 import URLLib3Instrumentor
 from opentelemetry.test.httptest import HttpTestBase
 from opentelemetry.test.test_base import TestBase
 
 
 class TestURLLib3InstrumentorMetric(HttpTestBase, TestBase):
-    HTTP_URL = "http://httpbin.org/status/200"
+    HTTP_URL = "http://mock/status/200"
 
     def setUp(self):
         super().setUp()
         URLLib3Instrumentor().instrument()
         httpretty.enable(allow_net_connect=False)
         httpretty.register_uri(httpretty.GET, self.HTTP_URL, body="Hello!")
         httpretty.register_uri(httpretty.POST, self.HTTP_URL, body="Hello!")
@@ -64,19 +64,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=client_duration_estimated,
                     max_data_point=client_duration_estimated,
                     min_data_point=client_duration_estimated,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "GET",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
             est_value_delta=200,
         )
 
@@ -87,19 +87,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=0,
                     max_data_point=0,
                     min_data_point=0,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "GET",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
         )
 
         expected_size = len(response.data)
@@ -112,19 +112,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=expected_size,
                     max_data_point=expected_size,
                     min_data_point=expected_size,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "GET",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
         )
 
     def test_str_request_body_size_metrics(self):
@@ -140,19 +140,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=6,
                     max_data_point=6,
                     min_data_point=6,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "POST",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
         )
 
     def test_bytes_request_body_size_metrics(self):
@@ -168,19 +168,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=6,
                     max_data_point=6,
                     min_data_point=6,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "POST",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
         )
 
     def test_fields_request_body_size_metrics(self):
@@ -197,19 +197,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=expected_value,
                     max_data_point=expected_value,
                     min_data_point=expected_value,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "POST",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
         )
 
     def test_bytesio_request_body_size_metrics(self):
@@ -225,19 +225,19 @@
                 self.create_histogram_data_point(
                     count=1,
                     sum_data_point=6,
                     max_data_point=6,
                     min_data_point=6,
                     attributes={
                         "http.flavor": "1.1",
-                        "http.host": "httpbin.org",
+                        "http.host": "mock",
                         "http.method": "POST",
                         "http.scheme": "http",
                         "http.status_code": 200,
-                        "net.peer.name": "httpbin.org",
+                        "net.peer.name": "mock",
                         "net.peer.port": 80,
                     },
                 )
             ],
         )
 
     def test_generator_request_body_size_metrics(self):
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/LICENSE` & `opentelemetry_instrumentation_urllib3-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/README.rst` & `opentelemetry_instrumentation_urllib3-0.40b0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         pass
 
     # `request` is an instance of urllib3.connectionpool.HTTPConnectionPool
     # `response` is an instance of urllib3.response.HTTPResponse
     def response_hook(span, request, response):
         pass
 
-    URLLib3Instrumentor.instrument(
-        request_hook=request_hook, response_hook=response_hook)
+    URLLib3Instrumentor().instrument(
+        request_hook=request_hook, response_hook=response_hook
     )
 
 Exclude lists
 *************
 
 To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB3_EXCLUDED_URLS``
 (or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_urllib3-0.40b0/pyproject.toml`

 * *Files 4% similar despite different names*

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
-  "opentelemetry-semantic-conventions == 0.39b0",
-  "opentelemetry-util-http == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
+  "opentelemetry-util-http == 0.40b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
-  "urllib3 >= 1.0.0, < 2.0.0",
+  "urllib3 >= 1.0.0, < 3.0.0",
 ]
 test = [
   "opentelemetry-instrumentation-urllib3[instruments]",
   "httpretty ~= 1.0",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 urllib3 = "opentelemetry.instrumentation.urllib3:URLLib3Instrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3"
```

### Comparing `opentelemetry_instrumentation_urllib3-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_urllib3-0.40b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-urllib3
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry urllib3 instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3
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
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
-Requires-Dist: opentelemetry-util-http==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
+Requires-Dist: opentelemetry-util-http==0.40b0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
-Requires-Dist: urllib3<2.0.0,>=1.0.0; extra == 'instruments'
+Requires-Dist: urllib3<3.0.0,>=1.0.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: httpretty~=1.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-urllib3[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry urllib3 Instrumentation
 ======================================
 
 |pypi|
 
@@ -66,16 +66,16 @@
         pass
 
     # `request` is an instance of urllib3.connectionpool.HTTPConnectionPool
     # `response` is an instance of urllib3.response.HTTPResponse
     def response_hook(span, request, response):
         pass
 
-    URLLib3Instrumentor.instrument(
-        request_hook=request_hook, response_hook=response_hook)
+    URLLib3Instrumentor().instrument(
+        request_hook=request_hook, response_hook=response_hook
     )
 
 Exclude lists
 *************
 
 To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB3_EXCLUDED_URLS``
 (or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
```

