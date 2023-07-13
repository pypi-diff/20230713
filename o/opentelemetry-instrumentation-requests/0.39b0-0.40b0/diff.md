# Comparing `tmp/opentelemetry_instrumentation_requests-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_requests-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_requests-0.39b0.tar` & `opentelemetry_instrumentation_requests-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    17436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_integration.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_ip_support.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/LICENSE
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/README.rst
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/src/opentelemetry/instrumentation/requests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/src/opentelemetry/instrumentation/requests/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/src/opentelemetry/instrumentation/requests/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    17398 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/tests/test_requests_integration.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/tests/test_requests_ip_support.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/LICENSE
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/README.rst
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/__init__.py` & `opentelemetry_instrumentation_requests-0.40b0/src/opentelemetry/instrumentation/requests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,16 +241,24 @@
         original = instr_func.__wrapped__  # pylint:disable=no-member
         if restore_as_bound_func:
             original = types.MethodType(original, instr_root)
         setattr(instr_root, instr_func_name, original)
 
 
 def get_default_span_name(method):
-    """Default implementation for name_callback, returns HTTP {method_name}."""
-    return f"HTTP {method.strip()}"
+    """
+    Default implementation for name_callback, returns HTTP {method_name}.
+    https://opentelemetry.io/docs/reference/specification/trace/semantic_conventions/http/#name
+
+    Args:
+        method: string representing HTTP method
+    Returns:
+        span name
+    """
+    return method.strip()
 
 
 class RequestsInstrumentor(BaseInstrumentor):
     """An instrumentor for requests
     See `BaseInstrumentor`
     """
```

### Comparing `opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/package.py` & `opentelemetry_instrumentation_requests-0.40b0/src/opentelemetry/instrumentation/requests/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/version.py` & `opentelemetry_instrumentation_requests-0.40b0/src/opentelemetry/instrumentation/requests/version.py`

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

### Comparing `opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_integration.py` & `opentelemetry_instrumentation_requests-0.40b0/tests/test_requests_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.response = {}
 
 
 class RequestsIntegrationTestBase(abc.ABC):
     # pylint: disable=no-member
     # pylint: disable=too-many-public-methods
 
-    URL = "http://httpbin.org/status/200"
+    URL = "http://mock/status/200"
 
     # pylint: disable=invalid-name
     def setUp(self):
         super().setUp()
 
         self.env_patch = mock.patch.dict(
             "os.environ",
@@ -112,15 +112,15 @@
 
     def test_basic(self):
         result = self.perform_request(self.URL)
         self.assertEqual(result.text, "Hello!")
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
@@ -148,15 +148,15 @@
         self.assertEqual(result.text, "Hello!")
         span = self.assert_span()
 
         self.assertEqual(span.name, "name set from hook")
         self.assertEqual(span.attributes["response_hook_attr"], "value")
 
     def test_excluded_urls_explicit(self):
-        url_404 = "http://httpbin.org/status/404"
+        url_404 = "http://mock/status/404"
         httpretty.register_uri(
             httpretty.GET,
             url_404,
             status=404,
         )
 
         RequestsInstrumentor().uninstrument()
@@ -187,18 +187,18 @@
 
         RequestsInstrumentor().uninstrument()
         RequestsInstrumentor().instrument(name_callback=name_callback)
         result = self.perform_request(self.URL)
         self.assertEqual(result.text, "Hello!")
         span = self.assert_span()
 
-        self.assertEqual(span.name, "HTTP GET")
+        self.assertEqual(span.name, "GET")
 
     def test_not_foundbasic(self):
-        url_404 = "http://httpbin.org/status/404"
+        url_404 = "http://mock/status/404"
         httpretty.register_uri(
             httpretty.GET,
             url_404,
             status=404,
         )
         result = self.perform_request(url_404)
         self.assertEqual(result.status_code, 404)
@@ -456,15 +456,15 @@
     @staticmethod
     def perform_request(url: str, session: requests.Session = None):
         if session is None:
             return requests.get(url)
         return session.get(url)
 
     def test_credential_removal(self):
-        new_url = "http://username:password@httpbin.org/status/200"
+        new_url = "http://username:password@mock/status/200"
         self.perform_request(new_url)
         span = self.assert_span()
 
         self.assertEqual(span.attributes[SpanAttributes.HTTP_URL], self.URL)
 
     def test_if_headers_equals_none(self):
         result = requests.get(self.URL, headers=None)
```

### Comparing `opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_ip_support.py` & `opentelemetry_instrumentation_requests-0.40b0/tests/test_requests_ip_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,14 @@
         return span_list
 
     def assert_success_span(self, response: requests.Response):
         self.assertEqual("Hello!", response.text)
 
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

### Comparing `opentelemetry_instrumentation_requests-0.39b0/LICENSE` & `opentelemetry_instrumentation_requests-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.39b0/README.rst` & `opentelemetry_instrumentation_requests-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_requests-0.40b0/pyproject.toml`

 * *Files 7% similar despite different names*

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
-  "opentelemetry-semantic-conventions == 0.39b0",
-  "opentelemetry-util-http == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
+  "opentelemetry-util-http == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "requests ~= 2.0",
 ]
 test = [
   "opentelemetry-instrumentation-requests[instruments]",
   "httpretty ~= 1.0",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 requests = "opentelemetry.instrumentation.requests:RequestsInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests"
```

### Comparing `opentelemetry_instrumentation_requests-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_requests-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-requests
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry requests instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,23 +14,23 @@
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
 Requires-Dist: requests~=2.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: httpretty~=1.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-requests[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Requests Instrumentation
 ======================================
 
 |pypi|
```

