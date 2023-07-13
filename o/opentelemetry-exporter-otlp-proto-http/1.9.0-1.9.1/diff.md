# Comparing `tmp/opentelemetry-exporter-otlp-proto-http-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-otlp-proto-http-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-otlp-proto-http-1.9.0.tar", last modified: Wed Jan 26 18:29:17 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-otlp-proto-http-1.9.1.tar", last modified: Mon Jan 31 10:09:50 2022, max compression
```

## Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0.tar` & `opentelemetry-exporter-otlp-proto-http-1.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/encoder/
--rw-r--r--   0 runner    (1001) docker     (121)    10449 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/tests/test_proto_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)    17493 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-http-1.9.0/tests/test_protobuf_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/
+-rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/
+-rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/encoder/
+-rw-r--r--   0 runner    (1001) docker     (121)    10164 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/tests/test_proto_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17055 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-http-1.9.1/tests/test_protobuf_encoder.py
```

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/LICENSE` & `opentelemetry-exporter-otlp-proto-http-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/PKG-INFO` & `opentelemetry-exporter-otlp-proto-http-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp-proto-http
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Collector Protobuf over HTTP Exporter
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-http
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/README.rst` & `opentelemetry-exporter-otlp-proto-http-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/setup.cfg` & `opentelemetry-exporter-otlp-proto-http-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	=src
 packages = find_namespace:
 install_requires = 
 	requests ~= 2.7
 	googleapis-common-protos ~= 1.52
 	opentelemetry-api ~= 1.3
 	opentelemetry-sdk ~= 1.3
-	opentelemetry-proto == 1.9.0
+	opentelemetry-proto == 1.9.1
 	backoff ~= 1.10.0
 
 [options.extras_require]
 test = 
 
 [options.packages.find]
 where = src
```

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/setup.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/__init__.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/__init__.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/encoder/__init__.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/trace_exporter/encoder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 from opentelemetry.sdk.trace import Event
 from opentelemetry.sdk.util.instrumentation import InstrumentationInfo
 from opentelemetry.sdk.trace import Resource
 from opentelemetry.sdk.trace import Span as SDKSpan
 from opentelemetry.trace import Link
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.span import SpanContext, TraceState, Status
-from opentelemetry.trace.status import StatusCode
 from opentelemetry.util.types import Attributes
 
 # pylint: disable=E1101
 _SPAN_KIND_MAP = {
     SpanKind.INTERNAL: PB2SPan.SpanKind.SPAN_KIND_INTERNAL,
     SpanKind.SERVER: PB2SPan.SpanKind.SPAN_KIND_SERVER,
     SpanKind.CLIENT: PB2SPan.SpanKind.SPAN_KIND_CLIENT,
@@ -192,19 +191,15 @@
             pb2_links.append(encoded_link)
     return pb2_links
 
 
 def _encode_status(status: Status) -> Optional[PB2Status]:
     pb2_status = None
     if status is not None:
-        deprecated_code = PB2Status.DEPRECATED_STATUS_CODE_OK
-        if status.status_code is StatusCode.ERROR:
-            deprecated_code = PB2Status.DEPRECATED_STATUS_CODE_UNKNOWN_ERROR
         pb2_status = PB2Status(
-            deprecated_code=deprecated_code,
             code=status.status_code.value,
             message=status.description,
         )
     return pb2_status
 
 
 def _encode_trace_state(trace_state: TraceState) -> Optional[str]:
```

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry/exporter/otlp/proto/http/version.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry/exporter/otlp/proto/http/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/PKG-INFO` & `opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp-proto-http
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Collector Protobuf over HTTP Exporter
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-http
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/src/opentelemetry_exporter_otlp_proto_http.egg-info/SOURCES.txt` & `opentelemetry-exporter-otlp-proto-http-1.9.1/src/opentelemetry_exporter_otlp_proto_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/tests/test_proto_span_exporter.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/tests/test_proto_span_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-http-1.9.0/tests/test_protobuf_encoder.py` & `opentelemetry-exporter-otlp-proto-http-1.9.1/tests/test_protobuf_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,14 @@
                                                         bool_value=True
                                                     ),
                                                 ),
                                             ],
                                         )
                                     ],
                                     status=PB2Status(
-                                        deprecated_code=PB2Status.DEPRECATED_STATUS_CODE_UNKNOWN_ERROR,  # pylint: disable=no-member
                                         code=SDKStatusCode.ERROR.value,
                                         message="Example description",
                                     ),
                                 )
                             ],
                         ),
                         PB2InstrumentationLibrarySpans(
@@ -370,27 +369,24 @@
 
         return otel_spans, pb2_service_request
 
     def test_encode_status_code_translations(self):
         self.assertEqual(
             _encode_status(SDKStatus(status_code=SDKStatusCode.UNSET)),
             PB2Status(
-                deprecated_code=PB2Status.DEPRECATED_STATUS_CODE_OK,  # pylint: disable=no-member
                 code=SDKStatusCode.UNSET.value,
             ),
         )
 
         self.assertEqual(
             _encode_status(SDKStatus(status_code=SDKStatusCode.OK)),
             PB2Status(
-                deprecated_code=PB2Status.DEPRECATED_STATUS_CODE_OK,  # pylint: disable=no-member
                 code=SDKStatusCode.OK.value,
             ),
         )
 
         self.assertEqual(
             _encode_status(SDKStatus(status_code=SDKStatusCode.ERROR)),
             PB2Status(
-                deprecated_code=PB2Status.DEPRECATED_STATUS_CODE_UNKNOWN_ERROR,  # pylint: disable=no-member
                 code=SDKStatusCode.ERROR.value,
             ),
         )
```

