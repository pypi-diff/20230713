# Comparing `tmp/opentelemetry_instrumentation_botocore-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_botocore-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_botocore-0.39b0.tar` & `opentelemetry_instrumentation_botocore-0.40b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/version.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py
--rw-r--r--   0        0        0    13523 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_dynamodb.py
--rw-r--r--   0        0        0    14026 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_instrumentation.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_lambda.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_messaging.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sns.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sqs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/LICENSE
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/README.rst
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    10416 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/version.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py
+-rw-r--r--   0        0        0    13523 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_dynamodb.py
+-rw-r--r--   0        0        0    14583 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_instrumentation.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_lambda.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_messaging.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_sns.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_sqs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/LICENSE
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/README.rst
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/__init__.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,69 +97,79 @@
 from opentelemetry.instrumentation.botocore.package import _instruments
 from opentelemetry.instrumentation.botocore.version import __version__
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import (
     _SUPPRESS_INSTRUMENTATION_KEY,
     unwrap,
 )
-from opentelemetry.propagate import inject
+from opentelemetry.propagators.aws.aws_xray_propagator import AwsXRayPropagator
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import get_tracer
 from opentelemetry.trace.span import Span
 
 logger = logging.getLogger(__name__)
 
 
-# pylint: disable=unused-argument
-def _patched_endpoint_prepare_request(wrapped, instance, args, kwargs):
-    request = args[0]
-    headers = request.headers
-    inject(headers)
-    return wrapped(*args, **kwargs)
-
-
 class BotocoreInstrumentor(BaseInstrumentor):
     """An instrumentor for Botocore.
 
     See `BaseInstrumentor`
     """
 
     def __init__(self):
         super().__init__()
         self.request_hook = None
         self.response_hook = None
+        self.propagator = AwsXRayPropagator()
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         # pylint: disable=attribute-defined-outside-init
         self._tracer = get_tracer(
             __name__, __version__, kwargs.get("tracer_provider")
         )
 
         self.request_hook = kwargs.get("request_hook")
         self.response_hook = kwargs.get("response_hook")
 
+        propagator = kwargs.get("propagator")
+        if propagator is not None:
+            self.propagator = propagator
+
         wrap_function_wrapper(
             "botocore.client",
             "BaseClient._make_api_call",
             self._patched_api_call,
         )
 
         wrap_function_wrapper(
             "botocore.endpoint",
             "Endpoint.prepare_request",
-            _patched_endpoint_prepare_request,
+            self._patched_endpoint_prepare_request,
         )
 
     def _uninstrument(self, **kwargs):
         unwrap(BaseClient, "_make_api_call")
         unwrap(Endpoint, "prepare_request")
 
+    # pylint: disable=unused-argument
+    def _patched_endpoint_prepare_request(
+        self, wrapped, instance, args, kwargs
+    ):
+        request = args[0]
+        headers = request.headers
+
+        # Only the x-ray header is propagated by AWS services. Using any
+        # other propagator will lose the trace context.
+        self.propagator.inject(headers)
+
+        return wrapped(*args, **kwargs)
+
     # pylint: disable=too-many-branches
     def _patched_api_call(self, original_func, instance, args, kwargs):
         if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
             return original_func(*args, **kwargs)
 
         call_context = _determine_call_context(instance, args)
         if call_context is None:
```

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/package.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/version.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/version.py`

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

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/types.py` & `opentelemetry_instrumentation_botocore-0.40b0/src/opentelemetry/instrumentation/botocore/extensions/types.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_dynamodb.py` & `opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_instrumentation.py` & `opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_instrumentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,19 @@
     attach,
     detach,
     set_value,
 )
 from opentelemetry.instrumentation.botocore import BotocoreInstrumentor
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.propagate import get_global_textmap, set_global_textmap
+from opentelemetry.propagators.aws.aws_xray_propagator import TRACE_HEADER_KEY
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.test.mock_textmap import MockTextMapPropagator
 from opentelemetry.test.test_base import TestBase
+from opentelemetry.trace.span import format_span_id, format_trace_id
 
 _REQUEST_ID_REGEX_MATCH = r"[A-Z0-9]{52}"
 
 
 # pylint:disable=too-many-public-methods
 class TestBotocoreInstrumentor(TestBase):
     """Botocore integration testsuite"""
@@ -221,35 +223,29 @@
 
         kinesis.list_streams()
         self.assertEqual(0, len(self.memory_exporter.get_finished_spans()))
 
     @mock_ec2
     def test_uninstrument_does_not_inject_headers(self):
         headers = {}
-        previous_propagator = get_global_textmap()
-        try:
-            set_global_textmap(MockTextMapPropagator())
 
-            def intercept_headers(**kwargs):
-                headers.update(kwargs["request"].headers)
+        def intercept_headers(**kwargs):
+            headers.update(kwargs["request"].headers)
 
-            ec2 = self._make_client("ec2")
+        ec2 = self._make_client("ec2")
 
-            BotocoreInstrumentor().uninstrument()
+        BotocoreInstrumentor().uninstrument()
 
-            ec2.meta.events.register_first(
-                "before-send.ec2.DescribeInstances", intercept_headers
-            )
-            with self.tracer_provider.get_tracer("test").start_span("parent"):
-                ec2.describe_instances()
+        ec2.meta.events.register_first(
+            "before-send.ec2.DescribeInstances", intercept_headers
+        )
+        with self.tracer_provider.get_tracer("test").start_span("parent"):
+            ec2.describe_instances()
 
-            self.assertNotIn(MockTextMapPropagator.TRACE_ID_KEY, headers)
-            self.assertNotIn(MockTextMapPropagator.SPAN_ID_KEY, headers)
-        finally:
-            set_global_textmap(previous_propagator)
+        self.assertNotIn(TRACE_HEADER_KEY, headers)
 
     @mock_sqs
     def test_double_patch(self):
         sqs = self._make_client("sqs")
 
         BotocoreInstrumentor().instrument()
         BotocoreInstrumentor().instrument()
@@ -302,28 +298,50 @@
             ec2.describe_instances()
 
             request_id = "fdcdcab1-ae5c-489e-9c33-4637c5dda355"
             span = self.assert_span(
                 "EC2", "DescribeInstances", request_id=request_id
             )
 
-            self.assertIn(MockTextMapPropagator.TRACE_ID_KEY, headers)
-            self.assertEqual(
-                str(span.get_span_context().trace_id),
-                headers[MockTextMapPropagator.TRACE_ID_KEY],
+            # only x-ray propagation is used in HTTP requests
+            self.assertIn(TRACE_HEADER_KEY, headers)
+            xray_context = headers[TRACE_HEADER_KEY]
+            formated_trace_id = format_trace_id(
+                span.get_span_context().trace_id
             )
-            self.assertIn(MockTextMapPropagator.SPAN_ID_KEY, headers)
-            self.assertEqual(
-                str(span.get_span_context().span_id),
-                headers[MockTextMapPropagator.SPAN_ID_KEY],
+            formated_trace_id = (
+                formated_trace_id[:8] + "-" + formated_trace_id[8:]
             )
 
+            self.assertEqual(
+                xray_context.lower(),
+                f"root=1-{formated_trace_id};parent={format_span_id(span.get_span_context().span_id)};sampled=1".lower(),
+            )
         finally:
             set_global_textmap(previous_propagator)
 
+    @mock_ec2
+    def test_override_xray_propagator_injects_into_request(self):
+        headers = {}
+
+        def check_headers(**kwargs):
+            nonlocal headers
+            headers = kwargs["request"].headers
+
+        BotocoreInstrumentor().instrument()
+
+        ec2 = self._make_client("ec2")
+        ec2.meta.events.register_first(
+            "before-send.ec2.DescribeInstances", check_headers
+        )
+        ec2.describe_instances()
+
+        self.assertNotIn(MockTextMapPropagator.TRACE_ID_KEY, headers)
+        self.assertNotIn(MockTextMapPropagator.SPAN_ID_KEY, headers)
+
     @mock_xray
     def test_suppress_instrumentation_xray_client(self):
         xray_client = self._make_client("xray")
         token = attach(set_value(_SUPPRESS_INSTRUMENTATION_KEY, True))
         try:
             xray_client.put_trace_segments(TraceSegmentDocuments=["str1"])
             xray_client.put_trace_segments(TraceSegmentDocuments=["str2"])
```

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_lambda.py` & `opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_lambda.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_messaging.py` & `opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_messaging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sns.py` & `opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_sns.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sqs.py` & `opentelemetry_instrumentation_botocore-0.40b0/tests/test_botocore_sqs.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/LICENSE` & `opentelemetry_instrumentation_botocore-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/README.rst` & `opentelemetry_instrumentation_botocore-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_botocore-0.40b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,28 @@
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
+  "opentelemetry-propagator-aws-xray == 1.0.1",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "botocore ~= 1.0",
 ]
 test = [
   "opentelemetry-instrumentation-botocore[instruments]",
   "markupsafe==2.0.1",
   "moto[all] ~= 2.2.6",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 botocore = "opentelemetry.instrumentation.botocore:BotocoreInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-botocore"
```

### Comparing `opentelemetry_instrumentation_botocore-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_botocore-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-botocore
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Botocore instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-botocore
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,23 +14,24 @@
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
+Requires-Dist: opentelemetry-propagator-aws-xray==1.0.1
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Provides-Extra: instruments
 Requires-Dist: botocore~=1.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: markupsafe==2.0.1; extra == 'test'
 Requires-Dist: moto[all]~=2.2.6; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-botocore[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Botocore Tracing
 ==============================
 
 |pypi|
```

