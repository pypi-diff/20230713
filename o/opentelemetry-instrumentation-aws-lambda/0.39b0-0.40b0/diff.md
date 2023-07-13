# Comparing `tmp/opentelemetry_instrumentation_aws_lambda-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_aws_lambda-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0.tar` & `opentelemetry_instrumentation_aws_lambda-0.40b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation.py
--rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation_manual.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_http_api_event.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_proxy_event.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/lambda_function.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/LICENSE
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/README.rst
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    18033 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/src/opentelemetry/instrumentation/aws_lambda/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/src/opentelemetry/instrumentation/aws_lambda/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/tests/test_aws_lambda_instrumentation.py
+-rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/tests/test_aws_lambda_instrumentation_manual.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/tests/mocks/api_gateway_http_api_event.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/tests/mocks/api_gateway_proxy_event.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/tests/mocks/lambda_function.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/LICENSE
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/README.rst
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,79 +197,87 @@
 
     More info:
     https://docs.aws.amazon.com/apigateway/latest/developerguide/set-up-lambda-proxy-integrations.html#api-gateway-simple-proxy-for-lambda-input-format
     """
     span.set_attribute(
         SpanAttributes.HTTP_METHOD, lambda_event.get("httpMethod")
     )
-    span.set_attribute(SpanAttributes.HTTP_ROUTE, lambda_event.get("resource"))
 
     if lambda_event.get("headers"):
-        span.set_attribute(
-            SpanAttributes.HTTP_USER_AGENT,
-            lambda_event["headers"].get("User-Agent"),
-        )
-        span.set_attribute(
-            SpanAttributes.HTTP_SCHEME,
-            lambda_event["headers"].get("X-Forwarded-Proto"),
-        )
-        span.set_attribute(
-            SpanAttributes.NET_HOST_NAME, lambda_event["headers"].get("Host")
-        )
+        if "User-Agent" in lambda_event["headers"]:
+            span.set_attribute(
+                SpanAttributes.HTTP_USER_AGENT,
+                lambda_event["headers"]["User-Agent"],
+            )
+        if "X-Forwarded-Proto" in lambda_event["headers"]:
+            span.set_attribute(
+                SpanAttributes.HTTP_SCHEME,
+                lambda_event["headers"]["X-Forwarded-Proto"],
+            )
+        if "Host" in lambda_event["headers"]:
+            span.set_attribute(
+                SpanAttributes.NET_HOST_NAME,
+                lambda_event["headers"]["Host"],
+            )
+    if "resource" in lambda_event:
+        span.set_attribute(SpanAttributes.HTTP_ROUTE, lambda_event["resource"])
 
-    if lambda_event.get("queryStringParameters"):
-        span.set_attribute(
-            SpanAttributes.HTTP_TARGET,
-            f"{lambda_event.get('resource')}?{urlencode(lambda_event.get('queryStringParameters'))}",
-        )
-    else:
-        span.set_attribute(
-            SpanAttributes.HTTP_TARGET, lambda_event.get("resource")
-        )
+        if lambda_event.get("queryStringParameters"):
+            span.set_attribute(
+                SpanAttributes.HTTP_TARGET,
+                f"{lambda_event['resource']}?{urlencode(lambda_event['queryStringParameters'])}",
+            )
+        else:
+            span.set_attribute(
+                SpanAttributes.HTTP_TARGET, lambda_event["resource"]
+            )
 
     return span
 
 
 def _set_api_gateway_v2_proxy_attributes(
     lambda_event: Any, span: Span
 ) -> Span:
     """Sets HTTP attributes for v2 HTTP APIs
 
     More info:
     https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-lambda.html
     """
-    span.set_attribute(
-        SpanAttributes.NET_HOST_NAME,
-        lambda_event["requestContext"].get("domainName"),
-    )
-
-    if lambda_event["requestContext"].get("http"):
-        span.set_attribute(
-            SpanAttributes.HTTP_METHOD,
-            lambda_event["requestContext"]["http"].get("method"),
-        )
-        span.set_attribute(
-            SpanAttributes.HTTP_USER_AGENT,
-            lambda_event["requestContext"]["http"].get("userAgent"),
-        )
+    if "domainName" in lambda_event["requestContext"]:
         span.set_attribute(
-            SpanAttributes.HTTP_ROUTE,
-            lambda_event["requestContext"]["http"].get("path"),
+            SpanAttributes.NET_HOST_NAME,
+            lambda_event["requestContext"]["domainName"],
         )
 
-        if lambda_event.get("rawQueryString"):
+    if lambda_event["requestContext"].get("http"):
+        if "method" in lambda_event["requestContext"]["http"]:
             span.set_attribute(
-                SpanAttributes.HTTP_TARGET,
-                f"{lambda_event['requestContext']['http'].get('path')}?{lambda_event.get('rawQueryString')}",
+                SpanAttributes.HTTP_METHOD,
+                lambda_event["requestContext"]["http"]["method"],
             )
-        else:
+        if "userAgent" in lambda_event["requestContext"]["http"]:
             span.set_attribute(
-                SpanAttributes.HTTP_TARGET,
-                lambda_event["requestContext"]["http"].get("path"),
+                SpanAttributes.HTTP_USER_AGENT,
+                lambda_event["requestContext"]["http"]["userAgent"],
+            )
+        if "path" in lambda_event["requestContext"]["http"]:
+            span.set_attribute(
+                SpanAttributes.HTTP_ROUTE,
+                lambda_event["requestContext"]["http"]["path"],
             )
+            if lambda_event.get("rawQueryString"):
+                span.set_attribute(
+                    SpanAttributes.HTTP_TARGET,
+                    f"{lambda_event['requestContext']['http']['path']}?{lambda_event['rawQueryString']}",
+                )
+            else:
+                span.set_attribute(
+                    SpanAttributes.HTTP_TARGET,
+                    lambda_event["requestContext"]["http"]["path"],
+                )
 
     return span
 
 
 def _instrument(
     wrapped_module_name,
     wrapped_function_name,
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/package.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/src/opentelemetry/instrumentation/aws_lambda/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/version.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/src/opentelemetry/instrumentation/aws_lambda/version.py`

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

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/tests/test_aws_lambda_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation_manual.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/tests/test_aws_lambda_instrumentation_manual.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_http_api_event.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/tests/mocks/api_gateway_http_api_event.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_proxy_event.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/tests/mocks/api_gateway_proxy_event.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/lambda_function.py` & `opentelemetry_instrumentation_aws_lambda-0.40b0/tests/mocks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/LICENSE` & `opentelemetry_instrumentation_aws_lambda-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/README.rst` & `opentelemetry_instrumentation_aws_lambda-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_aws_lambda-0.40b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
-  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
   "opentelemetry-propagator-aws-xray == 1.0.1",
-  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = []
 test = [
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aws-lambda"
 
 [tool.hatch.version]
 path = "src/opentelemetry/instrumentation/aws_lambda/version.py"
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_aws_lambda-0.40b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-aws-lambda
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry AWS Lambda instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aws-lambda
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
-Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
 Requires-Dist: opentelemetry-propagator-aws-xray==1.0.1
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Provides-Extra: instruments
 Provides-Extra: test
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry AWS Lambda Tracing
 ================================
 
 |pypi|
```

