# Comparing `tmp/opentelemetry_instrumentation_grpc-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_grpc-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_grpc-0.39b0.tar` & `opentelemetry_instrumentation_grpc-0.40b0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    21061 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/__init__.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_client.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_server.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_client.py
--rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_server.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_utilities.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/version.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/_aio_client.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/_client.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/_server.py
--rw-r--r--   0        0        0    12603 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_filter.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_hooks.py
--rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor_filter.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor.py
--rw-r--r--   0        0        0    23591 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_filter.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_hooks.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_filters.py
--rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor.py
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor_filter.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server.proto
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2_grpc.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/LICENSE
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/README.rst
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    21061 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/__init__.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_aio_client.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_aio_server.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_client.py
+-rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_server.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_utilities.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/version.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/_aio_client.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/_client.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/_server.py
+-rw-r--r--   0        0        0    12603 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_client_interceptor.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_client_interceptor_filter.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_client_interceptor_hooks.py
+-rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_server_interceptor.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_server_interceptor_filter.py
+-rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_client_interceptor.py
+-rw-r--r--   0        0        0    23591 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_client_interceptor_filter.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_client_interceptor_hooks.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_filters.py
+-rw-r--r--   0        0        0    22293 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_server_interceptor.py
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/test_server_interceptor_filter.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/protobuf/test_server.proto
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/protobuf/test_server_pb2.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/tests/protobuf/test_server_pb2_grpc.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/LICENSE
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/README.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/__init__.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_client.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_aio_client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_server.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_aio_server.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_client.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_server.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,32 +246,38 @@
 
         # Split up the peer to keep with how other telemetry sources
         # do it.  This looks like:
         # * ipv6:[::1]:57284
         # * ipv4:127.0.0.1:57284
         # * ipv4:10.2.1.1:57284,127.0.0.1:57284
         #
-        try:
-            ip, port = (
-                context.peer().split(",")[0].split(":", 1)[1].rsplit(":", 1)
-            )
-            ip = unquote(ip)
-            attributes.update(
-                {
-                    SpanAttributes.NET_PEER_IP: ip,
-                    SpanAttributes.NET_PEER_PORT: port,
-                }
-            )
+        if context.peer() != "unix:":
+            try:
+                ip, port = (
+                    context.peer()
+                    .split(",")[0]
+                    .split(":", 1)[1]
+                    .rsplit(":", 1)
+                )
+                ip = unquote(ip)
+                attributes.update(
+                    {
+                        SpanAttributes.NET_PEER_IP: ip,
+                        SpanAttributes.NET_PEER_PORT: port,
+                    }
+                )
 
-            # other telemetry sources add this, so we will too
-            if ip in ("[::1]", "127.0.0.1"):
-                attributes[SpanAttributes.NET_PEER_NAME] = "localhost"
+                # other telemetry sources add this, so we will too
+                if ip in ("[::1]", "127.0.0.1"):
+                    attributes[SpanAttributes.NET_PEER_NAME] = "localhost"
 
-        except IndexError:
-            logger.warning("Failed to parse peer address '%s'", context.peer())
+            except IndexError:
+                logger.warning(
+                    "Failed to parse peer address '%s'", context.peer()
+                )
 
         return self._tracer.start_as_current_span(
             name=handler_call_details.method,
             kind=trace.SpanKind.SERVER,
             attributes=attributes,
             set_status_on_exception=set_status_on_exception,
         )
```

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_utilities.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/_utilities.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/package.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/version.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/version.py`

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

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py` & `opentelemetry_instrumentation_grpc-0.40b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/__init__.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/_aio_client.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/_aio_client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/_client.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/_client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/_server.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/_server.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_client_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_hooks.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_client_interceptor_hooks.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_server_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_aio_server_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_client_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_hooks.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_client_interceptor_hooks.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_filters.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_server_interceptor.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=unused-argument
 # pylint:disable=no-self-use
 
+import contextlib
+import tempfile
 import threading
 from concurrent import futures
 
 import grpc
 
 import opentelemetry.instrumentation.grpc
 from opentelemetry import trace
@@ -74,31 +76,40 @@
             yield Response(
                 server_id=request.client_id,
                 response_data=data,
             )
 
 
 class TestOpenTelemetryServerInterceptor(TestBase):
-    def test_instrumentor(self):
-        def handler(request, context):
-            return b""
-
-        grpc_server_instrumentor = GrpcInstrumentorServer()
-        grpc_server_instrumentor.instrument()
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
+    net_peer_span_attributes = {
+        SpanAttributes.NET_PEER_IP: "[::1]",
+        SpanAttributes.NET_PEER_NAME: "localhost",
+    }
+
+    @contextlib.contextmanager
+    def server(self, max_workers=1, interceptors=None):
+        with futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             server = grpc.server(
                 executor,
                 options=(("grpc.so_reuseport", 0),),
+                interceptors=interceptors or [],
             )
 
-            server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
-
             port = server.add_insecure_port("[::]:0")
             channel = grpc.insecure_channel(f"localhost:{port:d}")
+            yield server, channel
+
+    def test_instrumentor(self):
+        def handler(request, context):
+            return b""
 
+        grpc_server_instrumentor = GrpcInstrumentorServer()
+        grpc_server_instrumentor.instrument()
+        with self.server(max_workers=1) as (server, channel):
+            server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
             rpc_call = "TestServicer/handler"
             try:
                 server.start()
                 channel.unary_unary(rpc_call)(b"test")
             finally:
                 server.stop(None)
 
@@ -113,16 +124,15 @@
                 span, opentelemetry.instrumentation.grpc
             )
 
             # Check attributes
             self.assertSpanHasAttributes(
                 span,
                 {
-                    SpanAttributes.NET_PEER_IP: "[::1]",
-                    SpanAttributes.NET_PEER_NAME: "localhost",
+                    **self.net_peer_span_attributes,
                     SpanAttributes.RPC_METHOD: "handler",
                     SpanAttributes.RPC_SERVICE: "TestServicer",
                     SpanAttributes.RPC_SYSTEM: "grpc",
                     SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                         0
                     ],
                 },
@@ -133,25 +143,16 @@
     def test_uninstrument(self):
         def handler(request, context):
             return b""
 
         grpc_server_instrumentor = GrpcInstrumentorServer()
         grpc_server_instrumentor.instrument()
         grpc_server_instrumentor.uninstrument()
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-            )
-
+        with self.server(max_workers=1) as (server, channel):
             server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
-
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
-
             rpc_call = "TestServicer/test"
             try:
                 server.start()
                 channel.unary_unary(rpc_call)(b"test")
             finally:
                 server.stop(None)
 
@@ -160,23 +161,19 @@
 
     def test_create_span(self):
         """Check that the interceptor wraps calls with spans server-side."""
 
         # Intercept gRPC calls...
         interceptor = server_interceptor()
 
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             add_GRPCTestServerServicer_to_server(Servicer(), server)
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
 
             rpc_call = "/GRPCTestServer/SimpleMethod"
             request = Request(client_id=1, request_data="test")
             msg = request.SerializeToString()
             try:
                 server.start()
                 channel.unary_unary(rpc_call)(msg)
@@ -195,16 +192,15 @@
             span, opentelemetry.instrumentation.grpc
         )
 
         # Check attributes
         self.assertSpanHasAttributes(
             span,
             {
-                SpanAttributes.NET_PEER_IP: "[::1]",
-                SpanAttributes.NET_PEER_NAME: "localhost",
+                **self.net_peer_span_attributes,
                 SpanAttributes.RPC_METHOD: "SimpleMethod",
                 SpanAttributes.RPC_SERVICE: "GRPCTestServer",
                 SpanAttributes.RPC_SYSTEM: "grpc",
                 SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                     0
                 ],
             },
@@ -227,23 +223,19 @@
                     response_data=request.request_data,
                 )
 
         # Intercept gRPC calls...
         interceptor = server_interceptor()
 
         # setup the server
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             add_GRPCTestServerServicer_to_server(TwoSpanServicer(), server)
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
 
             # setup the RPC
             rpc_call = "/GRPCTestServer/SimpleMethod"
             request = Request(client_id=1, request_data="test")
             msg = request.SerializeToString()
             try:
                 server.start()
@@ -264,16 +256,15 @@
             parent_span, opentelemetry.instrumentation.grpc
         )
 
         # Check attributes
         self.assertSpanHasAttributes(
             parent_span,
             {
-                SpanAttributes.NET_PEER_IP: "[::1]",
-                SpanAttributes.NET_PEER_NAME: "localhost",
+                **self.net_peer_span_attributes,
                 SpanAttributes.RPC_METHOD: "SimpleMethod",
                 SpanAttributes.RPC_SERVICE: "GRPCTestServer",
                 SpanAttributes.RPC_SYSTEM: "grpc",
                 SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                     0
                 ],
             },
@@ -288,23 +279,19 @@
     def test_create_span_streaming(self):
         """Check that the interceptor wraps calls with spans server-side, on a
         streaming call."""
 
         # Intercept gRPC calls...
         interceptor = server_interceptor()
 
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             add_GRPCTestServerServicer_to_server(Servicer(), server)
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
 
             # setup the RPC
             rpc_call = "/GRPCTestServer/ServerStreamingMethod"
             request = Request(client_id=1, request_data="test")
             msg = request.SerializeToString()
             try:
                 server.start()
@@ -324,16 +311,15 @@
             span, opentelemetry.instrumentation.grpc
         )
 
         # Check attributes
         self.assertSpanHasAttributes(
             span,
             {
-                SpanAttributes.NET_PEER_IP: "[::1]",
-                SpanAttributes.NET_PEER_NAME: "localhost",
+                **self.net_peer_span_attributes,
                 SpanAttributes.RPC_METHOD: "ServerStreamingMethod",
                 SpanAttributes.RPC_SERVICE: "GRPCTestServer",
                 SpanAttributes.RPC_SYSTEM: "grpc",
                 SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                     0
                 ],
             },
@@ -356,23 +342,19 @@
                         server_id=request.client_id,
                         response_data=data,
                     )
 
         # Intercept gRPC calls...
         interceptor = server_interceptor()
 
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             add_GRPCTestServerServicer_to_server(TwoSpanServicer(), server)
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
 
             # setup the RPC
             rpc_call = "/GRPCTestServer/ServerStreamingMethod"
             request = Request(client_id=1, request_data="test")
             msg = request.SerializeToString()
             try:
                 server.start()
@@ -393,16 +375,15 @@
             parent_span, opentelemetry.instrumentation.grpc
         )
 
         # Check attributes
         self.assertSpanHasAttributes(
             parent_span,
             {
-                SpanAttributes.NET_PEER_IP: "[::1]",
-                SpanAttributes.NET_PEER_NAME: "localhost",
+                **self.net_peer_span_attributes,
                 SpanAttributes.RPC_METHOD: "ServerStreamingMethod",
                 SpanAttributes.RPC_SERVICE: "GRPCTestServer",
                 SpanAttributes.RPC_SYSTEM: "grpc",
                 SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                     0
                 ],
             },
@@ -423,25 +404,20 @@
         active_span_in_handler = None
 
         def handler(request, context):
             nonlocal active_span_in_handler
             active_span_in_handler = trace.get_current_span()
             return b""
 
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
 
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
-
             active_span_before_call = trace.get_current_span()
             try:
                 server.start()
                 channel.unary_unary("TestServicer/handler")(b"")
             finally:
                 server.stop(None)
         active_span_after_call = trace.get_current_span()
@@ -459,25 +435,20 @@
         # Capture the currently active span in each thread
         active_spans_in_handler = []
 
         def handler(request, context):
             active_spans_in_handler.append(trace.get_current_span())
             return b""
 
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
 
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
-
             try:
                 server.start()
                 channel.unary_unary("TestServicer/handler")(b"")
                 channel.unary_unary("TestServicer/handler")(b"")
             finally:
                 server.stop(None)
 
@@ -492,16 +463,15 @@
             # each should be a root span
             self.assertIsNone(span2.parent)
 
             # check attributes
             self.assertSpanHasAttributes(
                 span,
                 {
-                    SpanAttributes.NET_PEER_IP: "[::1]",
-                    SpanAttributes.NET_PEER_NAME: "localhost",
+                    **self.net_peer_span_attributes,
                     SpanAttributes.RPC_METHOD: "handler",
                     SpanAttributes.RPC_SERVICE: "TestServicer",
                     SpanAttributes.RPC_SYSTEM: "grpc",
                     SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                         0
                     ],
                 },
@@ -523,25 +493,20 @@
         latch = get_latch(2)
 
         def handler(request, context):
             latch()
             active_spans_in_handler.append(trace.get_current_span())
             return b""
 
-        with futures.ThreadPoolExecutor(max_workers=2) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
+        with self.server(
+            max_workers=2,
+            interceptors=[interceptor],
+        ) as (server, channel):
             server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
 
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
-
             try:
                 server.start()
                 # Interleave calls so spans are active on each thread at the same
                 # time
                 with futures.ThreadPoolExecutor(max_workers=2) as tpe:
                     f1 = tpe.submit(
                         channel.unary_unary("TestServicer/handler"), b""
@@ -564,16 +529,15 @@
             # each should be a root span
             self.assertIsNone(span2.parent)
 
             # check attributes
             self.assertSpanHasAttributes(
                 span,
                 {
-                    SpanAttributes.NET_PEER_IP: "[::1]",
-                    SpanAttributes.NET_PEER_NAME: "localhost",
+                    **self.net_peer_span_attributes,
                     SpanAttributes.RPC_METHOD: "handler",
                     SpanAttributes.RPC_SERVICE: "TestServicer",
                     SpanAttributes.RPC_SYSTEM: "grpc",
                     SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[
                         0
                     ],
                 },
@@ -588,26 +552,19 @@
         # our detailed failure message
         failure_message = "This is a test failure"
 
         # aborting RPC handler
         def handler(request, context):
             context.abort(grpc.StatusCode.FAILED_PRECONDITION, failure_message)
 
-        with futures.ThreadPoolExecutor(max_workers=1) as executor:
-            server = grpc.server(
-                executor,
-                options=(("grpc.so_reuseport", 0),),
-                interceptors=[interceptor],
-            )
-
+        with self.server(
+            max_workers=1,
+            interceptors=[interceptor],
+        ) as (server, channel):
             server.add_generic_rpc_handlers((UnaryUnaryRpcHandler(handler),))
-
-            port = server.add_insecure_port("[::]:0")
-            channel = grpc.insecure_channel(f"localhost:{port:d}")
-
             rpc_call = "TestServicer/handler"
 
             server.start()
             # unfortunately, these are just bare exceptions in grpc...
             with self.assertRaises(Exception):
                 channel.unary_unary(rpc_call)(b"")
             server.stop(None)
@@ -631,26 +588,47 @@
             f"{grpc.StatusCode.FAILED_PRECONDITION}:{failure_message}",
         )
 
         # Check attributes
         self.assertSpanHasAttributes(
             span,
             {
-                SpanAttributes.NET_PEER_IP: "[::1]",
-                SpanAttributes.NET_PEER_NAME: "localhost",
+                **self.net_peer_span_attributes,
                 SpanAttributes.RPC_METHOD: "handler",
                 SpanAttributes.RPC_SERVICE: "TestServicer",
                 SpanAttributes.RPC_SYSTEM: "grpc",
                 SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.FAILED_PRECONDITION.value[
                     0
                 ],
             },
         )
 
 
+class TestOpenTelemetryServerInterceptorUnix(
+    TestOpenTelemetryServerInterceptor,
+):
+    net_peer_span_attributes = {}
+
+    @contextlib.contextmanager
+    def server(self, max_workers=1, interceptors=None):
+        with futures.ThreadPoolExecutor(
+            max_workers=max_workers
+        ) as executor, tempfile.TemporaryDirectory() as tmp:
+            server = grpc.server(
+                executor,
+                options=(("grpc.so_reuseport", 0),),
+                interceptors=interceptors or [],
+            )
+
+            sock = f"unix://{tmp}/grpc.sock"
+            server.add_insecure_port(sock)
+            channel = grpc.insecure_channel(sock)
+            yield server, channel
+
+
 def get_latch(num):
     """Get a countdown latch function for use in n threads."""
     cv = threading.Condition()
     count = 0
 
     def countdown_latch():
         """Block until n-1 other threads have called."""
```

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/test_server_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server.proto` & `opentelemetry_instrumentation_grpc-0.40b0/tests/protobuf/test_server.proto`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/protobuf/test_server_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2_grpc.py` & `opentelemetry_instrumentation_grpc-0.40b0/tests/protobuf/test_server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/LICENSE` & `opentelemetry_instrumentation_grpc-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/README.rst` & `opentelemetry_instrumentation_grpc-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_grpc-0.40b0/pyproject.toml`

 * *Files 6% similar despite different names*

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
+  "opentelemetry-instrumentation == 0.40b0",
   "opentelemetry-sdk ~= 1.12",
-  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "grpcio ~= 1.27",
 ]
 test = [
   "opentelemetry-instrumentation-grpc[instruments]",
   "opentelemetry-sdk ~= 1.12",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "protobuf ~= 3.13",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 grpc_client = "opentelemetry.instrumentation.grpc:GrpcInstrumentorClient"
 grpc_server = "opentelemetry.instrumentation.grpc:GrpcInstrumentorServer"
 grpc_aio_client = "opentelemetry.instrumentation.grpc:GrpcAioInstrumentorClient"
```

### Comparing `opentelemetry_instrumentation_grpc-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_grpc-0.40b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-grpc
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry gRPC instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-grpc
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
+Requires-Dist: opentelemetry-instrumentation==0.40b0
 Requires-Dist: opentelemetry-sdk~=1.12
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: grpcio~=1.27; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-grpc[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.12; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: protobuf~=3.13; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry gRPC Integration
 ==============================
 
 |pypi|
```

