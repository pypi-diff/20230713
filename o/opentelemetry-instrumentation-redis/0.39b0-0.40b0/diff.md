# Comparing `tmp/opentelemetry_instrumentation_redis-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_redis-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_redis-0.39b0.tar` & `opentelemetry_instrumentation_redis-0.40b0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/environment_variables.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/package.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/util.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     7488 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/tests/test_redis.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/LICENSE
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/README.rst
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    12780 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/package.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/util.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/tests/test_redis.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/LICENSE
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/README.rst
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/__init__.py` & `opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
 Instrument `redis`_ to report Redis queries.
 
 There are two options for instrumenting code. The first option is to use the
-``opentelemetry-instrumentation`` executable which will automatically
+``opentelemetry-instrument`` executable which will automatically
 instrument your Redis client. The second is to programmatically enable
 instrumentation via the following code:
 
 .. _redis: https://pypi.org/project/redis/
 
 Usage
 -----
@@ -60,16 +60,14 @@
 
 request_hook (Callable) - a function with extra user-defined logic to be performed before performing the request
 this function signature is:  def request_hook(span: Span, instance: redis.connection.Connection, args, kwargs) -> None
 
 response_hook (Callable) - a function with extra user-defined logic to be performed after performing the request
 this function signature is: def response_hook(span: Span, instance: redis.connection.Connection, response) -> None
 
-sanitize_query (Boolean) - default False, enable the Redis query sanitization
-
 for example:
 
 .. code: python
 
     from opentelemetry.instrumentation.redis import RedisInstrumentor
     import redis
 
@@ -84,45 +82,26 @@
     # Instrument redis with hooks
     RedisInstrumentor().instrument(request_hook=request_hook, response_hook=response_hook)
 
     # This will report a span with the default settings and the custom attributes added from the hooks
     client = redis.StrictRedis(host="localhost", port=6379)
     client.get("my-key")
 
-Configuration
--------------
-
-Query sanitization
-******************
-To enable query sanitization with an environment variable, set
-``OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS`` to "true".
-
-For example,
-
-::
-
-    export OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS="true"
-
-will result in traced queries like "SET ? ?".
 
 API
 ---
 """
 import typing
-from os import environ
 from typing import Any, Collection
 
 import redis
 from wrapt import wrap_function_wrapper
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
-from opentelemetry.instrumentation.redis.environment_variables import (
-    OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS,
-)
 from opentelemetry.instrumentation.redis.package import _instruments
 from opentelemetry.instrumentation.redis.util import (
     _extract_conn_attributes,
     _format_command_args,
 )
 from opentelemetry.instrumentation.redis.version import __version__
 from opentelemetry.instrumentation.utils import unwrap
@@ -153,27 +132,60 @@
         return
     for key, value in _extract_conn_attributes(
         conn.connection_pool.connection_kwargs
     ).items():
         span.set_attribute(key, value)
 
 
+def _build_span_name(instance, cmd_args):
+    if len(cmd_args) > 0 and cmd_args[0]:
+        name = cmd_args[0]
+    else:
+        name = instance.connection_pool.connection_kwargs.get("db", 0)
+    return name
+
+
+def _build_span_meta_data_for_pipeline(instance):
+    try:
+        command_stack = (
+            instance.command_stack
+            if hasattr(instance, "command_stack")
+            else instance._command_stack
+        )
+
+        cmds = [
+            _format_command_args(c.args if hasattr(c, "args") else c[0])
+            for c in command_stack
+        ]
+        resource = "\n".join(cmds)
+
+        span_name = " ".join(
+            [
+                (c.args[0] if hasattr(c, "args") else c[0][0])
+                for c in command_stack
+            ]
+        )
+    except (AttributeError, IndexError):
+        command_stack = []
+        resource = ""
+        span_name = ""
+
+    return command_stack, resource, span_name
+
+
+# pylint: disable=R0915
 def _instrument(
     tracer,
     request_hook: _RequestHookT = None,
     response_hook: _ResponseHookT = None,
-    sanitize_query: bool = False,
 ):
     def _traced_execute_command(func, instance, args, kwargs):
-        query = _format_command_args(args, sanitize_query)
+        query = _format_command_args(args)
+        name = _build_span_name(instance, args)
 
-        if len(args) > 0 and args[0]:
-            name = args[0]
-        else:
-            name = instance.connection_pool.connection_kwargs.get("db", 0)
         with tracer.start_as_current_span(
             name, kind=trace.SpanKind.CLIENT
         ) as span:
             if span.is_recording():
                 span.set_attribute(SpanAttributes.DB_STATEMENT, query)
                 _set_connection_attributes(span, instance)
                 span.set_attribute("db.redis.args_length", len(args))
@@ -181,39 +193,19 @@
                 request_hook(span, instance, args, kwargs)
             response = func(*args, **kwargs)
             if callable(response_hook):
                 response_hook(span, instance, response)
             return response
 
     def _traced_execute_pipeline(func, instance, args, kwargs):
-        try:
-            command_stack = (
-                instance.command_stack
-                if hasattr(instance, "command_stack")
-                else instance._command_stack
-            )
-
-            cmds = [
-                _format_command_args(
-                    c.args if hasattr(c, "args") else c[0], sanitize_query
-                )
-                for c in command_stack
-            ]
-            resource = "\n".join(cmds)
-
-            span_name = " ".join(
-                [
-                    (c.args[0] if hasattr(c, "args") else c[0][0])
-                    for c in command_stack
-                ]
-            )
-        except (AttributeError, IndexError):
-            command_stack = []
-            resource = ""
-            span_name = ""
+        (
+            command_stack,
+            resource,
+            span_name,
+        ) = _build_span_meta_data_for_pipeline(instance)
 
         with tracer.start_as_current_span(
             span_name, kind=trace.SpanKind.CLIENT
         ) as span:
             if span.is_recording():
                 span.set_attribute(SpanAttributes.DB_STATEMENT, resource)
                 _set_connection_attributes(span, instance)
@@ -250,40 +242,80 @@
             _traced_execute_command,
         )
         wrap_function_wrapper(
             "redis.cluster",
             "ClusterPipeline.execute",
             _traced_execute_pipeline,
         )
+
+    async def _async_traced_execute_command(func, instance, args, kwargs):
+        query = _format_command_args(args)
+        name = _build_span_name(instance, args)
+
+        with tracer.start_as_current_span(
+            name, kind=trace.SpanKind.CLIENT
+        ) as span:
+            if span.is_recording():
+                span.set_attribute(SpanAttributes.DB_STATEMENT, query)
+                _set_connection_attributes(span, instance)
+                span.set_attribute("db.redis.args_length", len(args))
+            if callable(request_hook):
+                request_hook(span, instance, args, kwargs)
+            response = await func(*args, **kwargs)
+            if callable(response_hook):
+                response_hook(span, instance, response)
+            return response
+
+    async def _async_traced_execute_pipeline(func, instance, args, kwargs):
+        (
+            command_stack,
+            resource,
+            span_name,
+        ) = _build_span_meta_data_for_pipeline(instance)
+
+        with tracer.start_as_current_span(
+            span_name, kind=trace.SpanKind.CLIENT
+        ) as span:
+            if span.is_recording():
+                span.set_attribute(SpanAttributes.DB_STATEMENT, resource)
+                _set_connection_attributes(span, instance)
+                span.set_attribute(
+                    "db.redis.pipeline_length", len(command_stack)
+                )
+            response = await func(*args, **kwargs)
+            if callable(response_hook):
+                response_hook(span, instance, response)
+            return response
+
     if redis.VERSION >= _REDIS_ASYNCIO_VERSION:
         wrap_function_wrapper(
             "redis.asyncio",
             f"{redis_class}.execute_command",
-            _traced_execute_command,
+            _async_traced_execute_command,
         )
         wrap_function_wrapper(
             "redis.asyncio.client",
             f"{pipeline_class}.execute",
-            _traced_execute_pipeline,
+            _async_traced_execute_pipeline,
         )
         wrap_function_wrapper(
             "redis.asyncio.client",
             f"{pipeline_class}.immediate_execute_command",
-            _traced_execute_command,
+            _async_traced_execute_command,
         )
     if redis.VERSION >= _REDIS_ASYNCIO_CLUSTER_VERSION:
         wrap_function_wrapper(
             "redis.asyncio.cluster",
             "RedisCluster.execute_command",
-            _traced_execute_command,
+            _async_traced_execute_command,
         )
         wrap_function_wrapper(
             "redis.asyncio.cluster",
             "ClusterPipeline.execute",
-            _traced_execute_pipeline,
+            _async_traced_execute_pipeline,
         )
 
 
 class RedisInstrumentor(BaseInstrumentor):
     """An instrumentor for Redis
     See `BaseInstrumentor`
     """
@@ -303,23 +335,14 @@
         tracer = trace.get_tracer(
             __name__, __version__, tracer_provider=tracer_provider
         )
         _instrument(
             tracer,
             request_hook=kwargs.get("request_hook"),
             response_hook=kwargs.get("response_hook"),
-            sanitize_query=kwargs.get(
-                "sanitize_query",
-                environ.get(
-                    OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS, "false"
-                )
-                .lower()
-                .strip()
-                == "true",
-            ),
         )
 
     def _uninstrument(self, **kwargs):
         if redis.VERSION < (3, 0, 0):
             unwrap(redis.StrictRedis, "execute_command")
             unwrap(redis.StrictRedis, "pipeline")
             unwrap(redis.Redis, "pipeline")
```

### Comparing `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/environment_variables.py` & `opentelemetry_instrumentation_redis-0.40b0/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,11 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS = (
-    "OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS"
-)
```

### Comparing `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/package.py` & `opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/util.py` & `opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,45 +44,27 @@
         attributes[
             SpanAttributes.NET_TRANSPORT
         ] = NetTransportValues.UNIX.value
 
     return attributes
 
 
-def _format_command_args(args, sanitize_query):
+def _format_command_args(args):
     """Format and sanitize command arguments, and trim them as needed"""
     cmd_max_len = 1000
     value_too_long_mark = "..."
-    if sanitize_query:
-        # Sanitized query format: "COMMAND ? ?"
-        args_length = len(args)
-        if args_length > 0:
-            out = [str(args[0])] + ["?"] * (args_length - 1)
-            out_str = " ".join(out)
-
-            if len(out_str) > cmd_max_len:
-                out_str = (
-                    out_str[: cmd_max_len - len(value_too_long_mark)]
-                    + value_too_long_mark
-                )
-        else:
-            out_str = ""
-        return out_str
-
-    value_max_len = 100
-    length = 0
-    out = []
-    for arg in args:
-        cmd = str(arg)
-
-        if len(cmd) > value_max_len:
-            cmd = cmd[:value_max_len] + value_too_long_mark
-
-        if length + len(cmd) > cmd_max_len:
-            prefix = cmd[: cmd_max_len - length]
-            out.append(f"{prefix}{value_too_long_mark}")
-            break
 
-        out.append(cmd)
-        length += len(cmd)
+    # Sanitized query format: "COMMAND ? ?"
+    args_length = len(args)
+    if args_length > 0:
+        out = [str(args[0])] + ["?"] * (args_length - 1)
+        out_str = " ".join(out)
+
+        if len(out_str) > cmd_max_len:
+            out_str = (
+                out_str[: cmd_max_len - len(value_too_long_mark)]
+                + value_too_long_mark
+            )
+    else:
+        out_str = ""
 
-    return " ".join(out)
+    return out_str
```

### Comparing `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/version.py` & `opentelemetry_instrumentation_redis-0.40b0/src/opentelemetry/instrumentation/redis/version.py`

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

### Comparing `opentelemetry_instrumentation_redis-0.39b0/tests/test_redis.py` & `opentelemetry_instrumentation_redis-0.40b0/tests/test_redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,44 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import asyncio
 from unittest import mock
 
 import redis
+import redis.asyncio
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.redis import RedisInstrumentor
 from opentelemetry.test.test_base import TestBase
 from opentelemetry.trace import SpanKind
 
 
+class AsyncMock:
+    """A sufficient async mock implementation.
+
+    Python 3.7 doesn't have an inbuilt async mock class, so this is used.
+    """
+
+    def __init__(self):
+        self.mock = mock.Mock()
+
+    async def __call__(self, *args, **kwargs):
+        future = asyncio.Future()
+        future.set_result("random")
+        return future
+
+    def __getattr__(self, item):
+        return AsyncMock()
+
+
 class TestRedis(TestBase):
     def setUp(self):
         super().setUp()
         RedisInstrumentor().instrument(tracer_provider=self.tracer_provider)
 
     def tearDown(self):
         super().tearDown()
@@ -83,14 +103,43 @@
 
         with mock.patch.object(redis_client, "connection"):
             redis_client.get("key")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
+    def test_instrument_uninstrument_async_client_command(self):
+        redis_client = redis.asyncio.Redis()
+
+        with mock.patch.object(redis_client, "connection", AsyncMock()):
+            asyncio.run(redis_client.get("key"))
+
+        spans = self.memory_exporter.get_finished_spans()
+        self.assertEqual(len(spans), 1)
+        self.memory_exporter.clear()
+
+        # Test uninstrument
+        RedisInstrumentor().uninstrument()
+
+        with mock.patch.object(redis_client, "connection", AsyncMock()):
+            asyncio.run(redis_client.get("key"))
+
+        spans = self.memory_exporter.get_finished_spans()
+        self.assertEqual(len(spans), 0)
+        self.memory_exporter.clear()
+
+        # Test instrument again
+        RedisInstrumentor().instrument()
+
+        with mock.patch.object(redis_client, "connection", AsyncMock()):
+            asyncio.run(redis_client.get("key"))
+
+        spans = self.memory_exporter.get_finished_spans()
+        self.assertEqual(len(spans), 1)
+
     def test_response_hook(self):
         redis_client = redis.Redis()
         connection = redis.connection.Connection()
         redis_client.connection = connection
 
         response_attribute_name = "db.redis.response"
 
@@ -164,53 +213,27 @@
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
         self.assertEqual(span.attributes.get("db.statement"), "SET ? ?")
 
-    def test_query_sanitizer_enabled_env(self):
+    def test_query_sanitizer(self):
         redis_client = redis.Redis()
         connection = redis.connection.Connection()
         redis_client.connection = connection
 
-        RedisInstrumentor().uninstrument()
-
-        env_patch = mock.patch.dict(
-            "os.environ",
-            {"OTEL_PYTHON_INSTRUMENTATION_SANITIZE_REDIS": "true"},
-        )
-        env_patch.start()
-        RedisInstrumentor().instrument(
-            tracer_provider=self.tracer_provider,
-        )
-
         with mock.patch.object(redis_client, "connection"):
             redis_client.set("key", "value")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
         self.assertEqual(span.attributes.get("db.statement"), "SET ? ?")
-        env_patch.stop()
-
-    def test_query_sanitizer_disabled(self):
-        redis_client = redis.Redis()
-        connection = redis.connection.Connection()
-        redis_client.connection = connection
-
-        with mock.patch.object(redis_client, "connection"):
-            redis_client.set("key", "value")
-
-        spans = self.memory_exporter.get_finished_spans()
-        self.assertEqual(len(spans), 1)
-
-        span = spans[0]
-        self.assertEqual(span.attributes.get("db.statement"), "SET key value")
 
     def test_no_op_tracer_provider(self):
         RedisInstrumentor().uninstrument()
         tracer_provider = trace.NoOpTracerProvider()
         RedisInstrumentor().instrument(tracer_provider=tracer_provider)
 
         redis_client = redis.Redis()
```

### Comparing `opentelemetry_instrumentation_redis-0.39b0/LICENSE` & `opentelemetry_instrumentation_redis-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.39b0/README.rst` & `opentelemetry_instrumentation_redis-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_redis-0.40b0/pyproject.toml`

 * *Files 6% similar despite different names*

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
   "wrapt >= 1.12.1",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "redis >= 2.6",
 ]
 test = [
   "opentelemetry-instrumentation-redis[instruments]",
   "opentelemetry-sdk ~= 1.3",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 redis = "opentelemetry.instrumentation.redis:RedisInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-redis"
```

### Comparing `opentelemetry_instrumentation_redis-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_redis-0.40b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-redis
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Redis instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-redis
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
 Requires-Dist: wrapt>=1.12.1
 Provides-Extra: instruments
 Requires-Dist: redis>=2.6; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-redis[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.3; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Redis Instrumentation
 ===================================
 
 |pypi|
```

