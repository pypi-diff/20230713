# Comparing `tmp/opentelemetry_instrumentation_flask-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_flask-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_flask-0.39b0.tar` & `opentelemetry_instrumentation_flask-0.40b0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    24568 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/base_test.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_automatic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_multithreading.py
--rw-r--r--   0        0        0    26898 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_programmatic.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_sqlcommenter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/LICENSE
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/README.rst
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    25021 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/src/opentelemetry/instrumentation/flask/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/src/opentelemetry/instrumentation/flask/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/src/opentelemetry/instrumentation/flask/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/base_test.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/test_automatic.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/test_copy_context.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/test_multithreading.py
+-rw-r--r--   0        0        0    26898 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/test_programmatic.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/tests/test_sqlcommenter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/LICENSE
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/README.rst
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/__init__.py` & `opentelemetry_instrumentation_flask-0.40b0/src/opentelemetry/instrumentation/flask/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,21 +234,22 @@
 
 Note:
     The environment variable names used to capture HTTP headers are still experimental, and thus are subject to change.
 
 API
 ---
 """
+import weakref
 from logging import getLogger
-from threading import get_ident
 from time import time_ns
 from timeit import default_timer
 from typing import Collection
 
 import flask
+from packaging import version as package_version
 
 import opentelemetry.instrumentation.wsgi as otel_wsgi
 from opentelemetry import context, trace
 from opentelemetry.instrumentation.flask.package import _instruments
 from opentelemetry.instrumentation.flask.version import __version__
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.propagators import (
@@ -261,19 +262,29 @@
 from opentelemetry.util.http import get_excluded_urls, parse_excluded_urls
 
 _logger = getLogger(__name__)
 
 _ENVIRON_STARTTIME_KEY = "opentelemetry-flask.starttime_key"
 _ENVIRON_SPAN_KEY = "opentelemetry-flask.span_key"
 _ENVIRON_ACTIVATION_KEY = "opentelemetry-flask.activation_key"
-_ENVIRON_THREAD_ID_KEY = "opentelemetry-flask.thread_id_key"
+_ENVIRON_REQCTX_REF_KEY = "opentelemetry-flask.reqctx_ref_key"
 _ENVIRON_TOKEN = "opentelemetry-flask.token"
 
 _excluded_urls_from_env = get_excluded_urls("FLASK")
 
+if package_version.parse(flask.__version__) >= package_version.parse("2.2.0"):
+
+    def _request_ctx_ref() -> weakref.ReferenceType:
+        return weakref.ref(flask.globals.request_ctx._get_current_object())
+
+else:
+
+    def _request_ctx_ref() -> weakref.ReferenceType:
+        return weakref.ref(flask._request_ctx_stack.top)
+
 
 def get_default_span_name():
     try:
         span_name = flask.request.url_rule.rule
     except AttributeError:
         span_name = otel_wsgi.get_default_span_name(flask.request.environ)
     return span_name
@@ -360,50 +371,49 @@
 ):
     def _before_request():
         if excluded_urls and excluded_urls.url_disabled(flask.request.url):
             return
         flask_request_environ = flask.request.environ
         span_name = get_default_span_name()
 
+        attributes = otel_wsgi.collect_request_attributes(
+            flask_request_environ
+        )
+        if flask.request.url_rule:
+            # For 404 that result from no route found, etc, we
+            # don't have a url_rule.
+            attributes[SpanAttributes.HTTP_ROUTE] = flask.request.url_rule.rule
         span, token = _start_internal_or_server_span(
             tracer=tracer,
             span_name=span_name,
             start_time=flask_request_environ.get(_ENVIRON_STARTTIME_KEY),
             context_carrier=flask_request_environ,
             context_getter=otel_wsgi.wsgi_getter,
+            attributes=attributes,
         )
 
         if request_hook:
             request_hook(span, flask_request_environ)
 
         if span.is_recording():
-            attributes = otel_wsgi.collect_request_attributes(
-                flask_request_environ
-            )
-            if flask.request.url_rule:
-                # For 404 that result from no route found, etc, we
-                # don't have a url_rule.
-                attributes[
-                    SpanAttributes.HTTP_ROUTE
-                ] = flask.request.url_rule.rule
             for key, value in attributes.items():
                 span.set_attribute(key, value)
             if span.is_recording() and span.kind == trace.SpanKind.SERVER:
                 custom_attributes = (
                     otel_wsgi.collect_custom_request_headers_attributes(
                         flask_request_environ
                     )
                 )
                 if len(custom_attributes) > 0:
                     span.set_attributes(custom_attributes)
 
         activation = trace.use_span(span, end_on_exit=True)
         activation.__enter__()  # pylint: disable=E1101
         flask_request_environ[_ENVIRON_ACTIVATION_KEY] = activation
-        flask_request_environ[_ENVIRON_THREAD_ID_KEY] = get_ident()
+        flask_request_environ[_ENVIRON_REQCTX_REF_KEY] = _request_ctx_ref()
         flask_request_environ[_ENVIRON_SPAN_KEY] = span
         flask_request_environ[_ENVIRON_TOKEN] = token
 
         if enable_commenter:
             current_context = context.get_current()
             flask_info = {}
 
@@ -435,25 +445,30 @@
 ):
     def _teardown_request(exc):
         # pylint: disable=E1101
         if excluded_urls and excluded_urls.url_disabled(flask.request.url):
             return
 
         activation = flask.request.environ.get(_ENVIRON_ACTIVATION_KEY)
-        thread_id = flask.request.environ.get(_ENVIRON_THREAD_ID_KEY)
-        if not activation or thread_id != get_ident():
+
+        original_reqctx_ref = flask.request.environ.get(
+            _ENVIRON_REQCTX_REF_KEY
+        )
+        current_reqctx_ref = _request_ctx_ref()
+        if not activation or original_reqctx_ref != current_reqctx_ref:
             # This request didn't start a span, maybe because it was created in
             # a way that doesn't run `before_request`, like when it is created
             # with `app.test_request_context`.
             #
-            # Similarly, check the thread_id against the current thread to ensure
-            # tear down only happens on the original thread. This situation can
-            # arise if the original thread handling the request spawn children
-            # threads and then uses something like copy_current_request_context
-            # to copy the request context.
+            # Similarly, check that the request_ctx that created the span
+            # matches the current request_ctx, and only tear down if they match.
+            # This situation can arise if the original request_ctx handling
+            # the request calls functions that push new request_ctx's,
+            # like any decorated with `flask.copy_current_request_context`.
+
             return
         if exc is None:
             activation.__exit__(None, None, None)
         else:
             activation.__exit__(
                 type(exc), exc, getattr(exc, "__traceback__", None)
             )
```

### Comparing `opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/package.py` & `opentelemetry_instrumentation_flask-0.40b0/src/opentelemetry/instrumentation/flask/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/version.py` & `opentelemetry_instrumentation_flask-0.40b0/src/opentelemetry/instrumentation/flask/version.py`

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

### Comparing `opentelemetry_instrumentation_flask-0.39b0/tests/base_test.py` & `opentelemetry_instrumentation_flask-0.40b0/tests/base_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from random import randint
 
 import flask
 from werkzeug.test import Client
 from werkzeug.wrappers import Response
 
-from opentelemetry import context
+from opentelemetry import context, trace
 
 
 class InstrumentationTest:
     @staticmethod
     def _hello_endpoint(helloid):
         if helloid == 500:
             raise ValueError(":-(")
@@ -34,14 +34,29 @@
         current_context = context.get_current()
         sqlcommenter_flask_values = current_context.get(
             "SQLCOMMENTER_ORM_TAGS_AND_VALUES", {}
         )
         return sqlcommenter_flask_values
 
     @staticmethod
+    def _copy_context_endpoint():
+        @flask.copy_current_request_context
+        def _extract_header():
+            return flask.request.headers["x-req"]
+
+        # Despite `_extract_header` copying the request context,
+        # calling it shouldn't detach the parent Flask span's contextvar
+        request_header = _extract_header()
+
+        return {
+            "span_name": trace.get_current_span().name,
+            "request_header": request_header,
+        }
+
+    @staticmethod
     def _multithreaded_endpoint(count):
         def do_random_stuff():
             @flask.copy_current_request_context
             def inner():
                 return randint(0, 100)
 
             return inner
@@ -80,14 +95,15 @@
         def excluded2_endpoint():
             return "excluded2"
 
         # pylint: disable=no-member
         self.app.route("/hello/<int:helloid>")(self._hello_endpoint)
         self.app.route("/sqlcommenter")(self._sqlcommenter_endpoint)
         self.app.route("/multithreaded")(self._multithreaded_endpoint)
+        self.app.route("/copy_context")(self._copy_context_endpoint)
         self.app.route("/excluded/<int:helloid>")(self._hello_endpoint)
         self.app.route("/excluded")(excluded_endpoint)
         self.app.route("/excluded2")(excluded2_endpoint)
         self.app.route("/test_custom_response_headers")(
             self._custom_response_headers
         )
```

### Comparing `opentelemetry_instrumentation_flask-0.39b0/tests/test_automatic.py` & `opentelemetry_instrumentation_flask-0.40b0/tests/test_automatic.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.39b0/tests/test_multithreading.py` & `opentelemetry_instrumentation_flask-0.40b0/tests/test_multithreading.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.39b0/tests/test_programmatic.py` & `opentelemetry_instrumentation_flask-0.40b0/tests/test_programmatic.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
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

### Comparing `opentelemetry_instrumentation_flask-0.39b0/tests/test_sqlcommenter.py` & `opentelemetry_instrumentation_flask-0.40b0/tests/test_sqlcommenter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.39b0/LICENSE` & `opentelemetry_instrumentation_flask-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.39b0/README.rst` & `opentelemetry_instrumentation_flask-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_flask-0.40b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,28 +22,29 @@
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
+  "packaging >= 21.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "flask >= 1.0, < 3.0",
 ]
 test = [
   "opentelemetry-instrumentation-flask[instruments]",
-  "markupsafe==2.0.1",
-  "opentelemetry-test-utils == 0.39b0",
+  "markupsafe==2.1.2",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 flask = "opentelemetry.instrumentation.flask:FlaskInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask"
```

### Comparing `opentelemetry_instrumentation_flask-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_flask-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-flask
-Version: 0.39b0
+Version: 0.40b0
 Summary: Flask instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,24 +14,25 @@
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
+Requires-Dist: packaging>=21.0
 Provides-Extra: instruments
 Requires-Dist: flask<3.0,>=1.0; extra == 'instruments'
 Provides-Extra: test
-Requires-Dist: markupsafe==2.0.1; extra == 'test'
+Requires-Dist: markupsafe==2.1.2; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-flask[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Flask Tracing
 ===========================
 
 |pypi|
```

