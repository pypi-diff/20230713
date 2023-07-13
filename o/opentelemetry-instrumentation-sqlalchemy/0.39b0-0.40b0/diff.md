# Comparing `tmp/opentelemetry_instrumentation_sqlalchemy-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_sqlalchemy-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0.tar` & `opentelemetry_instrumentation_sqlalchemy-0.40b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    10828 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy_metrics.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlcommenter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/LICENSE
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/README.rst
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11425 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/test_sqlalchemy_metrics.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/test_sqlcommenter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/LICENSE
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/README.rst
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,14 +130,17 @@
         if passed as an argument.
 
         Args:
             **kwargs: Optional arguments
                 ``engine``: a SQLAlchemy engine instance
                 ``engines``: a list of SQLAlchemy engine instances
                 ``tracer_provider``: a TracerProvider, defaults to global
+                ``meter_provider``: a MeterProvider, defaults to global
+                ``enable_commenter``: bool to enable sqlcommenter, defaults to False
+                ``commenter_options``: dict of sqlcommenter config, defaults to None
 
         Returns:
             An instrumented engine if passed in as an argument or list of instrumented engines, None otherwise.
         """
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
 
@@ -147,36 +150,44 @@
         connections_usage = meter.create_up_down_counter(
             name=MetricInstruments.DB_CLIENT_CONNECTIONS_USAGE,
             unit="connections",
             description="The number of connections that are currently in state described by the state attribute.",
         )
 
         enable_commenter = kwargs.get("enable_commenter", False)
+        commenter_options = kwargs.get("commenter_options", {})
 
         _w(
             "sqlalchemy",
             "create_engine",
-            _wrap_create_engine(tracer, connections_usage, enable_commenter),
+            _wrap_create_engine(
+                tracer, connections_usage, enable_commenter, commenter_options
+            ),
         )
         _w(
             "sqlalchemy.engine",
             "create_engine",
-            _wrap_create_engine(tracer, connections_usage, enable_commenter),
+            _wrap_create_engine(
+                tracer, connections_usage, enable_commenter, commenter_options
+            ),
         )
         _w(
             "sqlalchemy.engine.base",
             "Engine.connect",
             _wrap_connect(tracer),
         )
         if parse_version(sqlalchemy.__version__).release >= (1, 4):
             _w(
                 "sqlalchemy.ext.asyncio",
                 "create_async_engine",
                 _wrap_create_async_engine(
-                    tracer, connections_usage, enable_commenter
+                    tracer,
+                    connections_usage,
+                    enable_commenter,
+                    commenter_options,
                 ),
             )
         if kwargs.get("engine") is not None:
             return EngineTracer(
                 tracer,
                 kwargs.get("engine"),
                 connections_usage,
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
+import weakref
 
 from sqlalchemy.event import (  # pylint: disable=no-name-in-module
     listen,
     remove,
 )
 
 from opentelemetry import trace
@@ -38,37 +39,49 @@
     if "postgres" in vendor or vendor == "psycopg2":
         return "postgresql"
 
     return vendor
 
 
 def _wrap_create_async_engine(
-    tracer, connections_usage, enable_commenter=False
+    tracer, connections_usage, enable_commenter=False, commenter_options=None
 ):
     # pylint: disable=unused-argument
     def _wrap_create_async_engine_internal(func, module, args, kwargs):
         """Trace the SQLAlchemy engine, creating an `EngineTracer`
         object that will listen to SQLAlchemy events.
         """
         engine = func(*args, **kwargs)
         EngineTracer(
-            tracer, engine.sync_engine, connections_usage, enable_commenter
+            tracer,
+            engine.sync_engine,
+            connections_usage,
+            enable_commenter,
+            commenter_options,
         )
         return engine
 
     return _wrap_create_async_engine_internal
 
 
-def _wrap_create_engine(tracer, connections_usage, enable_commenter=False):
+def _wrap_create_engine(
+    tracer, connections_usage, enable_commenter=False, commenter_options=None
+):
     def _wrap_create_engine_internal(func, _module, args, kwargs):
         """Trace the SQLAlchemy engine, creating an `EngineTracer`
         object that will listen to SQLAlchemy events.
         """
         engine = func(*args, **kwargs)
-        EngineTracer(tracer, engine, connections_usage, enable_commenter)
+        EngineTracer(
+            tracer,
+            engine,
+            connections_usage,
+            enable_commenter,
+            commenter_options,
+        )
         return engine
 
     return _wrap_create_engine_internal
 
 
 def _wrap_connect(tracer):
     # pylint: disable=unused-argument
@@ -95,59 +108,47 @@
         tracer,
         engine,
         connections_usage,
         enable_commenter=False,
         commenter_options=None,
     ):
         self.tracer = tracer
-        self.engine = engine
         self.connections_usage = connections_usage
         self.vendor = _normalize_vendor(engine.name)
         self.enable_commenter = enable_commenter
         self.commenter_options = commenter_options if commenter_options else {}
+        self._engine_attrs = _get_attributes_from_engine(engine)
         self._leading_comment_remover = re.compile(r"^/\*.*?\*/")
 
         self._register_event_listener(
             engine, "before_cursor_execute", self._before_cur_exec, retval=True
         )
         self._register_event_listener(
             engine, "after_cursor_execute", _after_cur_exec
         )
         self._register_event_listener(engine, "handle_error", _handle_error)
         self._register_event_listener(engine, "connect", self._pool_connect)
         self._register_event_listener(engine, "close", self._pool_close)
         self._register_event_listener(engine, "checkin", self._pool_checkin)
         self._register_event_listener(engine, "checkout", self._pool_checkout)
 
-    def _get_connection_string(self):
-        drivername = self.engine.url.drivername or ""
-        host = self.engine.url.host or ""
-        port = self.engine.url.port or ""
-        database = self.engine.url.database or ""
-        return f"{drivername}://{host}:{port}/{database}"
-
-    def _get_pool_name(self):
-        if self.engine.pool.logging_name is not None:
-            return self.engine.pool.logging_name
-        return self._get_connection_string()
-
     def _add_idle_to_connection_usage(self, value):
         self.connections_usage.add(
             value,
             attributes={
-                "pool.name": self._get_pool_name(),
+                **self._engine_attrs,
                 "state": "idle",
             },
         )
 
     def _add_used_to_connection_usage(self, value):
         self.connections_usage.add(
             value,
             attributes={
-                "pool.name": self._get_pool_name(),
+                **self._engine_attrs,
                 "state": "used",
             },
         )
 
     def _pool_connect(self, _dbapi_connection, _connection_record):
         self._add_idle_to_connection_usage(1)
 
@@ -165,20 +166,29 @@
     ):
         self._add_idle_to_connection_usage(-1)
         self._add_used_to_connection_usage(1)
 
     @classmethod
     def _register_event_listener(cls, target, identifier, func, *args, **kw):
         listen(target, identifier, func, *args, **kw)
-        cls._remove_event_listener_params.append((target, identifier, func))
+        cls._remove_event_listener_params.append(
+            (weakref.ref(target), identifier, func)
+        )
 
     @classmethod
     def remove_all_event_listeners(cls):
-        for remove_params in cls._remove_event_listener_params:
-            remove(*remove_params)
+        for (
+            weak_ref_target,
+            identifier,
+            func,
+        ) in cls._remove_event_listener_params:
+            # Remove an event listener only if saved weak reference points to an object
+            # which has not been garbage collected
+            if weak_ref_target() is not None:
+                remove(weak_ref_target(), identifier, func)
         cls._remove_event_listener_params.clear()
 
     def _operation_name(self, db_name, statement):
         parts = []
         if isinstance(statement, str):
             # otel spec recommends against parsing SQL queries. We are not trying to parse SQL
             # but simply truncating the statement to the first word. This covers probably >95%
@@ -296,7 +306,26 @@
             attrs[
                 SpanAttributes.NET_TRANSPORT
             ] = NetTransportValues.IP_TCP.value
             attrs[SpanAttributes.NET_PEER_NAME] = info.host
             if info.port:
                 attrs[SpanAttributes.NET_PEER_PORT] = int(info.port)
     return attrs
+
+
+def _get_connection_string(engine):
+    drivername = engine.url.drivername or ""
+    host = engine.url.host or ""
+    port = engine.url.port or ""
+    database = engine.url.database or ""
+    return f"{drivername}://{host}:{port}/{database}"
+
+
+def _get_attributes_from_engine(engine):
+    """Set metadata attributes of the database engine"""
+    attrs = {}
+
+    attrs["pool.name"] = getattr(
+        getattr(engine, "pool", None), "logging_name", None
+    ) or _get_connection_string(engine)
+
+    return attrs
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/package.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/version.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/src/opentelemetry/instrumentation/sqlalchemy/version.py`

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

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/__init__.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy_metrics.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/test_sqlalchemy_metrics.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlcommenter.py` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/tests/test_sqlcommenter.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,14 +52,32 @@
         cnx = engine.connect()
         cnx.execute("SELECT  1;").fetchall()
         self.assertRegex(
             self.caplog.records[-2].getMessage(),
             r"SELECT  1 /\*db_driver='(.*)',traceparent='\d{1,2}-[a-zA-Z0-9_]{32}-[a-zA-Z0-9_]{16}-\d{1,2}'\*/;",
         )
 
+    def test_sqlcommenter_enabled_otel_values_false(self):
+        engine = create_engine("sqlite:///:memory:")
+        SQLAlchemyInstrumentor().instrument(
+            engine=engine,
+            tracer_provider=self.tracer_provider,
+            enable_commenter=True,
+            commenter_options={
+                "db_framework": False,
+                "opentelemetry_values": False,
+            },
+        )
+        cnx = engine.connect()
+        cnx.execute("SELECT  1;").fetchall()
+        self.assertRegex(
+            self.caplog.records[-2].getMessage(),
+            r"SELECT  1 /\*db_driver='(.*)'\*/;",
+        )
+
     def test_sqlcommenter_flask_integration(self):
         engine = create_engine("sqlite:///:memory:")
         SQLAlchemyInstrumentor().instrument(
             engine=engine,
             tracer_provider=self.tracer_provider,
             enable_commenter=True,
             commenter_options={"db_framework": False},
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/LICENSE` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/README.rst` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
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
   "packaging >= 21.0",
   "wrapt >= 1.11.2",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "sqlalchemy",
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_sqlalchemy-0.40b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-sqlalchemy
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry SQLAlchemy instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-sqlalchemy
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,16 +14,16 @@
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
 Requires-Dist: packaging>=21.0
 Requires-Dist: wrapt>=1.11.2
 Provides-Extra: instruments
 Requires-Dist: sqlalchemy; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.12; extra == 'test'
```

