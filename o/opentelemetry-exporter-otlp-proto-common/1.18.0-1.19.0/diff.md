# Comparing `tmp/opentelemetry_exporter_otlp_proto_common-1.18.0.tar.gz` & `tmp/opentelemetry_exporter_otlp_proto_common-1.19.0.tar.gz`

## Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0.tar` & `opentelemetry_exporter_otlp_proto_common-1.19.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/py.typed
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/version.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py
--rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/tests/test_log_encoder.py
--rw-r--r--   0        0        0    39051 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/tests/test_metrics_encoder.py
--rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/tests/test_trace_encoder.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/LICENSE
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/README.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/pyproject.toml
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.18.0/PKG-INFO
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/py.typed
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/version.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py
+-rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py
+-rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/tests/test_log_encoder.py
+-rw-r--r--   0        0        0    38631 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/tests/test_metrics_encoder.py
+-rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/tests/test_trace_encoder.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/LICENSE
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/README.rst
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/pyproject.toml
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 opentelemetry_exporter_otlp_proto_common-1.19.0/PKG-INFO
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_log_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/metrics_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/trace_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/version.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.18.0"
+__version__ = "1.19.0"
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/_log_encoder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         time_unix_nano=log_data.log_record.timestamp,
         span_id=_encode_span_id(log_data.log_record.span_id),
         trace_id=_encode_trace_id(log_data.log_record.trace_id),
         flags=int(log_data.log_record.trace_flags),
         body=_encode_value(log_data.log_record.body),
         severity_text=log_data.log_record.severity_text,
         attributes=_encode_attributes(log_data.log_record.attributes),
+        dropped_attributes_count=log_data.log_record.dropped_attributes,
         severity_number=log_data.log_record.severity_number.value,
     )
 
 
 def _encode_resource_logs(batch: Sequence[LogData]) -> List[ResourceLogs]:
     sdk_resource_logs = defaultdict(lambda: defaultdict(list))
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/metrics_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/src/opentelemetry/exporter/otlp/proto/common/_internal/trace_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/tests/test_log_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/tests/test_log_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,26 +35,39 @@
 from opentelemetry.proto.logs.v1.logs_pb2 import (
     ResourceLogs as PB2ResourceLogs,
 )
 from opentelemetry.proto.logs.v1.logs_pb2 import ScopeLogs as PB2ScopeLogs
 from opentelemetry.proto.resource.v1.resource_pb2 import (
     Resource as PB2Resource,
 )
-from opentelemetry.sdk._logs import LogData
+from opentelemetry.sdk._logs import LogData, LogLimits
 from opentelemetry.sdk._logs import LogRecord as SDKLogRecord
 from opentelemetry.sdk.resources import Resource as SDKResource
 from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 from opentelemetry.trace import TraceFlags
 
 
 class TestOTLPLogEncoder(unittest.TestCase):
     def test_encode(self):
         sdk_logs, expected_encoding = self.get_test_logs()
         self.assertEqual(encode_logs(sdk_logs), expected_encoding)
 
+    def test_dropped_attributes_count(self):
+        sdk_logs = self._get_test_logs_dropped_attributes()
+        encoded_logs = encode_logs(sdk_logs)
+        self.assertTrue(hasattr(sdk_logs[0].log_record, "dropped_attributes"))
+        self.assertEqual(
+            # pylint:disable=no-member
+            encoded_logs.resource_logs[0]
+            .scope_logs[0]
+            .log_records[0]
+            .dropped_attributes_count,
+            2,
+        )
+
     @staticmethod
     def _get_sdk_log_data() -> List[LogData]:
         log1 = LogData(
             log_record=SDKLogRecord(
                 timestamp=1644650195189786880,
                 trace_id=89564621134313219400156819398935297684,
                 span_id=1312458408527513268,
@@ -247,7 +260,46 @@
                         ),
                     ],
                 ),
             ]
         )
 
         return sdk_logs, pb2_service_request
+
+    @staticmethod
+    def _get_test_logs_dropped_attributes() -> List[LogData]:
+        log1 = LogData(
+            log_record=SDKLogRecord(
+                timestamp=1644650195189786880,
+                trace_id=89564621134313219400156819398935297684,
+                span_id=1312458408527513268,
+                trace_flags=TraceFlags(0x01),
+                severity_text="WARN",
+                severity_number=SeverityNumber.WARN,
+                body="Do not go gentle into that good night. Rage, rage against the dying of the light",
+                resource=SDKResource({"first_resource": "value"}),
+                attributes={"a": 1, "b": "c", "user_id": "B121092"},
+                limits=LogLimits(max_attributes=1),
+            ),
+            instrumentation_scope=InstrumentationScope(
+                "first_name", "first_version"
+            ),
+        )
+
+        log2 = LogData(
+            log_record=SDKLogRecord(
+                timestamp=1644650249738562048,
+                trace_id=0,
+                span_id=0,
+                trace_flags=TraceFlags.DEFAULT,
+                severity_text="WARN",
+                severity_number=SeverityNumber.WARN,
+                body="Cooper, this is no time for caution!",
+                resource=SDKResource({"second_resource": "CASE"}),
+                attributes={},
+            ),
+            instrumentation_scope=InstrumentationScope(
+                "second_name", "second_version"
+            ),
+        )
+
+        return [log1, log2]
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/tests/test_metrics_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/tests/test_metrics_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,14 @@
                                                 start_time_unix_nano=1641946016139533244,
                                                 time_unix_nano=1641946016139533244,
                                                 count=5,
                                                 sum=67,
                                                 bucket_counts=[1, 4],
                                                 explicit_bounds=[10.0, 20.0],
                                                 exemplars=[],
-                                                flags=pb2.DataPointFlags.FLAG_NONE,
                                                 max=18.0,
                                                 min=8.0,
                                             )
                                         ],
                                         aggregation_temporality=AggregationTemporality.DELTA,
                                     ),
                                 )
@@ -550,15 +549,14 @@
                                                 start_time_unix_nano=1641946016139533244,
                                                 time_unix_nano=1641946016139533244,
                                                 count=5,
                                                 sum=67,
                                                 bucket_counts=[1, 4],
                                                 explicit_bounds=[10.0, 20.0],
                                                 exemplars=[],
-                                                flags=pb2.DataPointFlags.FLAG_NONE,
                                                 max=18.0,
                                                 min=8.0,
                                             )
                                         ],
                                         aggregation_temporality=AggregationTemporality.DELTA,
                                     ),
                                 ),
@@ -586,15 +584,14 @@
                                                 start_time_unix_nano=1641946016139533244,
                                                 time_unix_nano=1641946016139533244,
                                                 count=5,
                                                 sum=67,
                                                 bucket_counts=[1, 4],
                                                 explicit_bounds=[10.0, 20.0],
                                                 exemplars=[],
-                                                flags=pb2.DataPointFlags.FLAG_NONE,
                                                 max=18.0,
                                                 min=8.0,
                                             )
                                         ],
                                         aggregation_temporality=AggregationTemporality.DELTA,
                                     ),
                                 ),
@@ -629,15 +626,14 @@
                                                 start_time_unix_nano=1641946016139533244,
                                                 time_unix_nano=1641946016139533244,
                                                 count=5,
                                                 sum=67,
                                                 bucket_counts=[1, 4],
                                                 explicit_bounds=[10.0, 20.0],
                                                 exemplars=[],
-                                                flags=pb2.DataPointFlags.FLAG_NONE,
                                                 max=18.0,
                                                 min=8.0,
                                             )
                                         ],
                                         aggregation_temporality=AggregationTemporality.DELTA,
                                     ),
                                 )
@@ -672,15 +668,14 @@
                                                 start_time_unix_nano=1641946016139533244,
                                                 time_unix_nano=1641946016139533244,
                                                 count=5,
                                                 sum=67,
                                                 bucket_counts=[1, 4],
                                                 explicit_bounds=[10.0, 20.0],
                                                 exemplars=[],
-                                                flags=pb2.DataPointFlags.FLAG_NONE,
                                                 max=18.0,
                                                 min=8.0,
                                             )
                                         ],
                                         aggregation_temporality=AggregationTemporality.DELTA,
                                     ),
                                 )
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/tests/test_trace_encoder.py` & `opentelemetry_exporter_otlp_proto_common-1.19.0/tests/test_trace_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/.gitignore` & `opentelemetry_exporter_otlp_proto_common-1.19.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/LICENSE` & `opentelemetry_exporter_otlp_proto_common-1.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/README.rst` & `opentelemetry_exporter_otlp_proto_common-1.19.0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/pyproject.toml` & `opentelemetry_exporter_otlp_proto_common-1.19.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-  "opentelemetry-proto == 1.18.0",
+  "opentelemetry-proto == 1.19.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-common"
 
 [tool.hatch.version]
 path = "src/opentelemetry/exporter/otlp/proto/common/version.py"
```

### Comparing `opentelemetry_exporter_otlp_proto_common-1.18.0/PKG-INFO` & `opentelemetry_exporter_otlp_proto_common-1.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp-proto-common
-Version: 1.18.0
+Version: 1.19.0
 Summary: OpenTelemetry Protobuf encoding
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-common
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: opentelemetry-proto==1.18.0
+Requires-Dist: opentelemetry-proto==1.19.0
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Protobuf Encoding
 ===============================
 
 |pypi|
```

