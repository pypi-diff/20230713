# Comparing `tmp/opentelemetry_instrumentation_urllib-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_urllib-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_urllib-0.39b0.tar` & `opentelemetry_instrumentation_urllib-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/__init__.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/package.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/tests/test_metrics_instrumentation.py
--rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/tests/test_urllib_integration.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/LICENSE
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/README.rst
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/src/opentelemetry/instrumentation/urllib/__init__.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/src/opentelemetry/instrumentation/urllib/package.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/src/opentelemetry/instrumentation/urllib/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/tests/test_metrics_instrumentation.py
+-rw-r--r--   0        0        0    14073 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/tests/test_urllib_integration.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/LICENSE
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/README.rst
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/__init__.py` & `opentelemetry_instrumentation_urllib-0.40b0/src/opentelemetry/instrumentation/urllib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
         url = request.full_url
         if excluded_urls and excluded_urls.url_disabled(url):
             return call_wrapped()
 
         method = request.get_method().upper()
 
-        span_name = f"HTTP {method}".strip()
+        span_name = method.strip()
 
         url = remove_url_credentials(url)
 
         labels = {
             SpanAttributes.HTTP_METHOD: method,
             SpanAttributes.HTTP_URL: url,
         }
```

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/package.py` & `opentelemetry_instrumentation_urllib-0.40b0/src/opentelemetry/instrumentation/urllib/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/version.py` & `opentelemetry_instrumentation_urllib-0.40b0/src/opentelemetry/instrumentation/urllib/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.39b0"
+__version__ = "0.40b0"
 
 _instruments = tuple()
```

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/tests/test_metrics_instrumentation.py` & `opentelemetry_instrumentation_urllib-0.40b0/tests/test_metrics_instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     URLLibInstrumentor,
 )
 from opentelemetry.semconv.metrics import MetricInstruments
 from opentelemetry.test.test_base import TestBase
 
 
 class TestUrllibMetricsInstrumentation(TestBase):
-    URL = "http://httpbin.org/status/200"
-    URL_POST = "http://httpbin.org/post"
+    URL = "http://mock/status/200"
+    URL_POST = "http://mock/post"
 
     def setUp(self):
         super().setUp()
         URLLibInstrumentor().instrument()
         httpretty.enable()
         httpretty.register_uri(httpretty.GET, self.URL, body=b"Hello!")
         httpretty.register_uri(
```

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/tests/test_urllib_integration.py` & `opentelemetry_instrumentation_urllib-0.40b0/tests/test_urllib_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 
 # pylint: disable=too-many-public-methods
 
 
 class RequestsIntegrationTestBase(abc.ABC):
     # pylint: disable=no-member
 
-    URL = "http://httpbin.org/status/200"
-    URL_TIMEOUT = "http://httpbin.org/timeout/0"
-    URL_EXCEPTION = "http://httpbin.org/exception/0"
+    URL = "http://mock/status/200"
+    URL_TIMEOUT = "http://mock/timeout/0"
+    URL_EXCEPTION = "http://mock/exception/0"
 
     # pylint: disable=invalid-name
     def setUp(self):
         super().setUp()
 
         self.env_patch = mock.patch.dict(
             "os.environ",
@@ -79,15 +79,15 @@
         httpretty.register_uri(
             httpretty.GET,
             self.URL_EXCEPTION,
             body=self.base_exception_callback,
         )
         httpretty.register_uri(
             httpretty.GET,
-            "http://httpbin.org/status/500",
+            "http://mock/status/500",
             status=500,
         )
 
     # pylint: disable=invalid-name
     def tearDown(self):
         super().tearDown()
         URLLibInstrumentor().uninstrument()
@@ -120,15 +120,15 @@
     def test_basic(self):
         result = self.perform_request(self.URL)
 
         self.assertEqual(result.read(), b"Hello!")
         span = self.assert_span()
 
         self.assertIs(span.kind, trace.SpanKind.CLIENT)
-        self.assertEqual(span.name, "HTTP GET")
+        self.assertEqual(span.name, "GET")
 
         self.assertEqual(
             span.attributes,
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_URL: self.URL,
                 SpanAttributes.HTTP_STATUS_CODE: 200,
@@ -138,15 +138,15 @@
         self.assertIs(span.status.status_code, trace.StatusCode.UNSET)
 
         self.assertEqualSpanInstrumentationInfo(
             span, opentelemetry.instrumentation.urllib
         )
 
     def test_excluded_urls_explicit(self):
-        url_201 = "http://httpbin.org/status/201"
+        url_201 = "http://mock/status/201"
         httpretty.register_uri(
             httpretty.GET,
             url_201,
             status=201,
         )
 
         URLLibInstrumentor().uninstrument()
@@ -168,15 +168,15 @@
         URLLibInstrumentor().instrument()
         self.perform_request(self.URL)
         self.perform_request(url)
 
         self.assert_span(num_spans=1)
 
     def test_not_foundbasic(self):
-        url_404 = "http://httpbin.org/status/404/"
+        url_404 = "http://mock/status/404/"
         httpretty.register_uri(
             httpretty.GET,
             url_404,
             status=404,
         )
         exception = None
         try:
@@ -205,15 +205,15 @@
     def test_response_code_none(self):
         result = self.perform_request(self.URL)
 
         self.assertEqual(result.read(), b"Hello!")
         span = self.assert_span()
 
         self.assertIs(span.kind, trace.SpanKind.CLIENT)
-        self.assertEqual(span.name, "HTTP GET")
+        self.assertEqual(span.name, "GET")
 
         self.assertEqual(
             span.attributes,
             {
                 SpanAttributes.HTTP_METHOD: "GET",
                 SpanAttributes.HTTP_URL: self.URL,
             },
@@ -332,22 +332,22 @@
         self.assertEqual(result.read(), b"Hello!")
 
         span = self.assert_span(exporter=exporter)
         self.assertIs(span.resource, resource)
 
     def test_requests_exception_with_response(self, *_, **__):
         with self.assertRaises(HTTPError):
-            self.perform_request("http://httpbin.org/status/500")
+            self.perform_request("http://mock/status/500")
 
         span = self.assert_span()
         self.assertEqual(
             dict(span.attributes),
             {
                 SpanAttributes.HTTP_METHOD: "GET",
-                SpanAttributes.HTTP_URL: "http://httpbin.org/status/500",
+                SpanAttributes.HTTP_URL: "http://mock/status/500",
                 SpanAttributes.HTTP_STATUS_CODE: 500,
             },
         )
         self.assertEqual(span.status.status_code, StatusCode.ERROR)
 
     def test_requests_basic_exception(self, *_, **__):
         with self.assertRaises(Exception):
@@ -361,15 +361,15 @@
             opener = urllib.request.build_opener()
             opener.open(self.URL_TIMEOUT, timeout=0.0001)
 
         span = self.assert_span()
         self.assertEqual(span.status.status_code, StatusCode.ERROR)
 
     def test_credential_removal(self):
-        url = "http://username:password@httpbin.org/status/200"
+        url = "http://username:password@mock/status/200"
 
         with self.assertRaises(Exception):
             self.perform_request(url)
 
         span = self.assert_span()
         self.assertEqual(span.attributes[SpanAttributes.HTTP_URL], self.URL)
```

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/LICENSE` & `opentelemetry_instrumentation_urllib-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/README.rst` & `opentelemetry_instrumentation_urllib-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_urllib-0.40b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,24 @@
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
   "httpretty ~= 1.0",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 urllib = "opentelemetry.instrumentation.urllib:URLLibInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib"
```

### Comparing `opentelemetry_instrumentation_urllib-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_urllib-0.40b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-urllib
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry urllib instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,21 @@
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
 Requires-Dist: httpretty~=1.0; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry urllib Instrumentation
 ====================================
 
 |pypi|
```

