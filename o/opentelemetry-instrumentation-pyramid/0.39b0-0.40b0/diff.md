# Comparing `tmp/opentelemetry_instrumentation_pyramid-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_pyramid-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_pyramid-0.39b0.tar` & `opentelemetry_instrumentation_pyramid-0.40b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/__init__.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/callbacks.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/tests/pyramid_base_test.py
--rw-r--r--   0        0        0    18044 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/tests/test_automatic.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/tests/test_programmatic.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/LICENSE
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/README.rst
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/__init__.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/callbacks.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/tests/pyramid_base_test.py
+-rw-r--r--   0        0        0    18044 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/tests/test_automatic.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/tests/test_programmatic.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/LICENSE
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/README.rst
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pyramid-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/__init__.py` & `opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/callbacks.py` & `opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/callbacks.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/package.py` & `opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/src/opentelemetry/instrumentation/pyramid/version.py` & `opentelemetry_instrumentation_pyramid-0.40b0/src/opentelemetry/instrumentation/pyramid/version.py`

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

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/tests/pyramid_base_test.py` & `opentelemetry_instrumentation_pyramid-0.40b0/tests/pyramid_base_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pyramid.httpexceptions as exc
 from pyramid.response import Response
 from werkzeug.test import Client
-from werkzeug.wrappers import BaseResponse
+
+# opentelemetry-instrumentation-pyramid uses werkzeug==0.16.1 which has
+# werkzeug.wrappers.BaseResponse. This is not the case for newer versions of
+# werkzeug like the one lint uses.
+from werkzeug.wrappers import BaseResponse  # pylint: disable=no-name-in-module
 
 
 class InstrumentationTest:
     @staticmethod
     def _hello_endpoint(request):
         helloid = int(request.matchdict["helloid"])
         if helloid == 500:
```

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/tests/test_automatic.py` & `opentelemetry_instrumentation_pyramid-0.40b0/tests/test_automatic.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/tests/test_programmatic.py` & `opentelemetry_instrumentation_pyramid-0.40b0/tests/test_programmatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         )
 
         resp = self.client.post("/bye")
         self.assertEqual(404, resp.status_code)
         resp.close()
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
-        self.assertEqual(span_list[0].name, "HTTP POST")
+        self.assertEqual(span_list[0].name, "POST /bye")
         self.assertEqual(span_list[0].kind, trace.SpanKind.SERVER)
         self.assertEqual(span_list[0].attributes, expected_attrs)
 
     def test_internal_error(self):
         expected_attrs = expected_attributes(
             {
                 SpanAttributes.HTTP_TARGET: "/hello/500",
```

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/LICENSE` & `opentelemetry_instrumentation_pyramid-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/README.rst` & `opentelemetry_instrumentation_pyramid-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_pyramid-0.40b0/pyproject.toml`

 * *Files 7% similar despite different names*

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
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "pyramid >= 1.7",
 ]
 test = [
   "opentelemetry-instrumentation-pyramid[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "werkzeug == 0.16.1",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 pyramid = "opentelemetry.instrumentation.pyramid:PyramidInstrumentor"
 
 [project.urls]
```

### Comparing `opentelemetry_instrumentation_pyramid-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_pyramid-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-pyramid
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Pyramid instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-pyramid
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
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: pyramid>=1.7; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-pyramid[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: werkzeug==0.16.1; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Pyramid Instrumentation
 =====================================
 
 |pypi|
```

