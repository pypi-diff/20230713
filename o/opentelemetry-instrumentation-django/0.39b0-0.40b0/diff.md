# Comparing `tmp/opentelemetry_instrumentation_django-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_django-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_django-0.39b0.tar` & `opentelemetry_instrumentation_django-0.40b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    14520 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/environment_variables.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/__init__.py
--rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    24755 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/test_middleware.py
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/test_middleware_asgi.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/test_sqlcommenter.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/views.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/README.rst
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    14520 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/environment_variables.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/middleware/__init__.py
+-rw-r--r--   0        0        0    14612 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    24931 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/tests/test_middleware.py
+-rw-r--r--   0        0        0    20602 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/tests/test_middleware_asgi.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/tests/test_sqlcommenter.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/tests/views.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/README.rst
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/__init__.py` & `opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/environment_variables.py` & `opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/package.py` & `opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/version.py` & `opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/version.py`

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

### Comparing `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py` & `opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,27 +168,24 @@
     def _get_span_name(request):
         try:
             if getattr(request, "resolver_match"):
                 match = request.resolver_match
             else:
                 match = resolve(request.path)
 
-            if hasattr(match, "route"):
-                return match.route
+            if hasattr(match, "route") and match.route:
+                return f"{request.method} {match.route}"
 
-            # Instead of using `view_name`, better to use `_func_name` as some applications can use similar
-            # view names in different modules
-            if hasattr(match, "_func_name"):
-                return match._func_name  # pylint: disable=protected-access
+            if hasattr(match, "url_name") and match.url_name:
+                return f"{request.method} {match.url_name}"
 
-            # Fallback for safety as `_func_name` private field
-            return match.view_name
+            return request.method
 
         except Resolver404:
-            return f"HTTP {request.method}"
+            return request.method
 
     # pylint: disable=too-many-locals
     def process_request(self, request):
         # request.META is a dictionary containing all available HTTP headers
         # Read more about request.META here:
         # https://docs.djangoproject.com/en/3.0/ref/request-response/#django.http.HttpRequest.META
```

### Comparing `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py` & `opentelemetry_instrumentation_django-0.40b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/tests/test_middleware.py` & `opentelemetry_instrumentation_django-0.40b0/tests/test_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,32 @@
 )
 
 DJANGO_2_0 = VERSION >= (2, 0)
 DJANGO_2_2 = VERSION >= (2, 2)
 DJANGO_3_0 = VERSION >= (3, 0)
 
 if DJANGO_2_0:
-    from django.urls import re_path
+    from django.urls import path, re_path
 else:
     from django.conf.urls import url as re_path
 
+    def path(path_argument, *args, **kwargs):
+        return re_path(rf"^{path_argument}$", *args, **kwargs)
+
+
 urlpatterns = [
     re_path(r"^traced/", traced),
     re_path(r"^traced_custom_header/", response_with_custom_header),
     re_path(r"^route/(?P<year>[0-9]{4})/template/$", traced_template),
     re_path(r"^error/", error),
     re_path(r"^excluded_arg/", excluded),
     re_path(r"^excluded_noarg/", excluded_noarg),
     re_path(r"^excluded_noarg2/", excluded_noarg2),
     re_path(r"^span_name/([0-9]{4})/$", route_span_name),
+    path("", traced, name="empty"),
 ]
 _django_instrumentor = DjangoInstrumentor()
 
 
 # pylint: disable=too-many-public-methods
 class TestMiddleware(WsgiTestBase):
     @classmethod
@@ -146,17 +151,17 @@
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
         self.assertEqual(
             span.name,
-            "^route/(?P<year>[0-9]{4})/template/$"
+            "GET ^route/(?P<year>[0-9]{4})/template/$"
             if DJANGO_2_2
-            else "tests.views.traced_template",
+            else "GET",
         )
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "GET")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://testserver/route/2020/template/",
@@ -173,17 +178,15 @@
         Client().get("/traced/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(
-            span.name, "^traced/" if DJANGO_2_2 else "tests.views.traced"
-        )
+        self.assertEqual(span.name, "GET ^traced/" if DJANGO_2_2 else "GET")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "GET")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://testserver/traced/",
         )
@@ -203,25 +206,33 @@
             tracer.return_value = mock_tracer
             Client().get("/traced/")
             self.assertFalse(mock_span.is_recording())
             self.assertTrue(mock_span.is_recording.called)
             self.assertFalse(mock_span.set_attribute.called)
             self.assertFalse(mock_span.set_status.called)
 
+    def test_empty_path(self):
+        Client().get("/")
+
+        spans = self.memory_exporter.get_finished_spans()
+        self.assertEqual(len(spans), 1)
+
+        span = spans[0]
+
+        self.assertEqual(span.name, "GET empty")
+
     def test_traced_post(self):
         Client().post("/traced/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(
-            span.name, "^traced/" if DJANGO_2_2 else "tests.views.traced"
-        )
+        self.assertEqual(span.name, "POST ^traced/" if DJANGO_2_2 else "POST")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "POST")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://testserver/traced/",
         )
@@ -237,17 +248,15 @@
             Client().get("/error/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(
-            span.name, "^error/" if DJANGO_2_2 else "tests.views.error"
-        )
+        self.assertEqual(span.name, "GET ^error/" if DJANGO_2_2 else "GET")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.ERROR)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "GET")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://testserver/error/",
         )
@@ -303,42 +312,38 @@
         Client().get("/span_name/1234/")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
         self.assertEqual(
             span.name,
-            "^span_name/([0-9]{4})/$"
-            if DJANGO_2_2
-            else "tests.views.route_span_name",
+            "GET ^span_name/([0-9]{4})/$" if DJANGO_2_2 else "GET",
         )
 
     def test_span_name_for_query_string(self):
         """
         request not have query string
         """
         Client().get("/span_name/1234/?query=test")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
         self.assertEqual(
             span.name,
-            "^span_name/([0-9]{4})/$"
-            if DJANGO_2_2
-            else "tests.views.route_span_name",
+            "GET ^span_name/([0-9]{4})/$" if DJANGO_2_2 else "GET",
         )
 
     def test_span_name_404(self):
         Client().get("/span_name/1234567890/")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
-        self.assertEqual(span.name, "HTTP GET")
+        self.assertEqual(span.name, "GET")
 
     def test_traced_request_attrs(self):
         Client().get("/span_name/1234/", CONTENT_TYPE="test/ct")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
```

### Comparing `opentelemetry_instrumentation_django-0.39b0/tests/test_middleware_asgi.py` & `opentelemetry_instrumentation_django-0.40b0/tests/test_middleware_asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         await self.async_client.get("/route/2020/template/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(span.name, "^route/(?P<year>[0-9]{4})/template/$")
+        self.assertEqual(span.name, "GET ^route/(?P<year>[0-9]{4})/template/$")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "GET")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://127.0.0.1/route/2020/template/",
         )
@@ -156,15 +156,15 @@
         await self.async_client.get("/traced/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(span.name, "^traced/")
+        self.assertEqual(span.name, "GET ^traced/")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "GET")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://127.0.0.1/traced/",
         )
@@ -191,15 +191,15 @@
         await self.async_client.post("/traced/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(span.name, "^traced/")
+        self.assertEqual(span.name, "POST ^traced/")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.UNSET)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "POST")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://127.0.0.1/traced/",
         )
@@ -214,15 +214,15 @@
             await self.async_client.get("/error/")
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
 
         span = spans[0]
 
-        self.assertEqual(span.name, "^error/")
+        self.assertEqual(span.name, "GET ^error/")
         self.assertEqual(span.kind, SpanKind.SERVER)
         self.assertEqual(span.status.status_code, StatusCode.ERROR)
         self.assertEqual(span.attributes[SpanAttributes.HTTP_METHOD], "GET")
         self.assertEqual(
             span.attributes[SpanAttributes.HTTP_URL],
             "http://127.0.0.1/error/",
         )
@@ -260,34 +260,34 @@
     async def test_span_name(self):
         # test no query_string
         await self.async_client.get("/span_name/1234/")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
-        self.assertEqual(span.name, "^span_name/([0-9]{4})/$")
+        self.assertEqual(span.name, "GET ^span_name/([0-9]{4})/$")
 
     async def test_span_name_for_query_string(self):
         """
         request not have query string
         """
         await self.async_client.get("/span_name/1234/?query=test")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
-        self.assertEqual(span.name, "^span_name/([0-9]{4})/$")
+        self.assertEqual(span.name, "GET ^span_name/([0-9]{4})/$")
 
     async def test_span_name_404(self):
         await self.async_client.get("/span_name/1234567890/")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
-        self.assertEqual(span.name, "HTTP GET")
+        self.assertEqual(span.name, "GET")
 
     async def test_traced_request_attrs(self):
         await self.async_client.get("/span_name/1234/", CONTENT_TYPE="test/ct")
         span_list = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(span_list), 1)
 
         span = span_list[0]
```

### Comparing `opentelemetry_instrumentation_django-0.39b0/tests/test_sqlcommenter.py` & `opentelemetry_instrumentation_django-0.40b0/tests/test_sqlcommenter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/tests/views.py` & `opentelemetry_instrumentation_django-0.40b0/tests/views.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/LICENSE` & `opentelemetry_instrumentation_django-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/README.rst` & `opentelemetry_instrumentation_django-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_django-0.40b0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -22,30 +22,30 @@
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
 ]
 
 [project.optional-dependencies]
 asgi = [
-  "opentelemetry-instrumentation-asgi == 0.39b0",
+  "opentelemetry-instrumentation-asgi == 0.40b0",
 ]
 instruments = [
   "django >= 1.10",
 ]
 test = [
   "opentelemetry-instrumentation-django[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 django = "opentelemetry.instrumentation.django:DjangoInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django"
```

### Comparing `opentelemetry_instrumentation_django-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_django-0.40b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-django
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Instrumentation for Django
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,25 +14,25 @@
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
 Provides-Extra: asgi
-Requires-Dist: opentelemetry-instrumentation-asgi==0.39b0; extra == 'asgi'
+Requires-Dist: opentelemetry-instrumentation-asgi==0.40b0; extra == 'asgi'
 Provides-Extra: instruments
 Requires-Dist: django>=1.10; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-django[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Django Tracing
 ============================
 
 |pypi|
```

