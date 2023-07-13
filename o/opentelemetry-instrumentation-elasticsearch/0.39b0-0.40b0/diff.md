# Comparing `tmp/opentelemetry_instrumentation_elasticsearch-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_elasticsearch-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0.tar` & `opentelemetry_instrumentation_elasticsearch-0.40b0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/package.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es2.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es5.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es6.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es7.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/sanitization_queries.py
--rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/test_elasticsearch.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/LICENSE
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/README.rst
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/package.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es2.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es5.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es6.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es7.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es8.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/sanitization_queries.py
+-rw-r--r--   0        0        0    17044 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/tests/test_elasticsearch.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/LICENSE
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/README.rst
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,14 +94,20 @@
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import unwrap
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import SpanKind, get_tracer
 
 from .utils import sanitize_body
 
+# Split of elasticsearch and elastic_transport in 8.0.0+
+# https://www.elastic.co/guide/en/elasticsearch/client/python-api/master/release-notes.html#rn-8-0-0
+es_transport_split = elasticsearch.VERSION[0] > 7
+if es_transport_split:
+    import elastic_transport
+
 logger = getLogger(__name__)
 
 
 # Values to add as tags from the actual
 # payload returned by Elasticsearch, if any.
 _ATTRIBUTES_FROM_RESULT = [
     "found",
@@ -133,24 +139,36 @@
         """
         Instruments Elasticsearch module
         """
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
         request_hook = kwargs.get("request_hook")
         response_hook = kwargs.get("response_hook")
-        _wrap(
-            elasticsearch,
-            "Transport.perform_request",
-            _wrap_perform_request(
-                tracer,
-                self._span_name_prefix,
-                request_hook,
-                response_hook,
-            ),
-        )
+        if es_transport_split:
+            _wrap(
+                elastic_transport,
+                "Transport.perform_request",
+                _wrap_perform_request(
+                    tracer,
+                    self._span_name_prefix,
+                    request_hook,
+                    response_hook,
+                ),
+            )
+        else:
+            _wrap(
+                elasticsearch,
+                "Transport.perform_request",
+                _wrap_perform_request(
+                    tracer,
+                    self._span_name_prefix,
+                    request_hook,
+                    response_hook,
+                ),
+            )
 
     def _uninstrument(self, **kwargs):
         unwrap(elasticsearch.Transport, "perform_request")
 
 
 _regex_doc_url = re.compile(r"/_doc/([^/]+)")
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/package.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/utils.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
 
 sanitized_keys = (
     "message",
     "should",
     "filter",
     "query",
     "queries",
@@ -47,14 +48,17 @@
                 d[key] = {}
             d = d[key]
         d[keys[-1]] = v
     return res
 
 
 def sanitize_body(body) -> str:
+    if isinstance(body, str):
+        body = json.loads(body)
+
     flatten_body = _flatten_dict(body)
 
     for key in flatten_body:
         if key.endswith(sanitized_keys):
             flatten_body[key] = sanitized_value
 
     return str(_unflatten_dict(flatten_body))
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/version.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/src/opentelemetry/instrumentation/elasticsearch/version.py`

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

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es2.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es5.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es5.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es6.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es6.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es7.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/tests/helpers_es7.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/sanitization_queries.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/tests/sanitization_queries.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/test_elasticsearch.py` & `opentelemetry_instrumentation_elasticsearch-0.40b0/tests/test_elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 from opentelemetry.test.test_base import TestBase
 from opentelemetry.trace import StatusCode
 
 from . import sanitization_queries  # pylint: disable=no-name-in-module
 
 major_version = elasticsearch.VERSION[0]
 
-if major_version == 7:
+if major_version == 8:
+    from . import helpers_es8 as helpers  # pylint: disable=no-name-in-module
+elif major_version == 7:
     from . import helpers_es7 as helpers  # pylint: disable=no-name-in-module
 elif major_version == 6:
     from . import helpers_es6 as helpers  # pylint: disable=no-name-in-module
 elif major_version == 5:
     from . import helpers_es5 as helpers  # pylint: disable=no-name-in-module
 else:
     from . import helpers_es2 as helpers  # pylint: disable=no-name-in-module
@@ -475,7 +477,11 @@
             sanitize_body(sanitization_queries.match_query),
             str(sanitization_queries.match_query_sanitized),
         )
         self.assertEqual(
             sanitize_body(sanitization_queries.filter_query),
             str(sanitization_queries.filter_query_sanitized),
         )
+        self.assertEqual(
+            sanitize_body(json.dumps(sanitization_queries.interval_query)),
+            str(sanitization_queries.interval_query_sanitized),
+        )
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/LICENSE` & `opentelemetry_instrumentation_elasticsearch-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/README.rst` & `opentelemetry_instrumentation_elasticsearch-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_elasticsearch-0.40b0/pyproject.toml`

 * *Files 12% similar despite different names*

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
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "elasticsearch >= 2.0",
 ]
 test = [
   "opentelemetry-instrumentation-elasticsearch[instruments]",
   "elasticsearch-dsl >= 2.0",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 elasticsearch = "opentelemetry.instrumentation.elasticsearch:ElasticsearchInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-elasticsearch"
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_elasticsearch-0.40b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-elasticsearch
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry elasticsearch instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-elasticsearch
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
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: elasticsearch>=2.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: elasticsearch-dsl>=2.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-elasticsearch[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry elasticsearch Integration
 ========================================
 
 |pypi|
```

