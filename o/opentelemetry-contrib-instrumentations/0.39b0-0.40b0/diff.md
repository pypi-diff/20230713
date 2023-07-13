# Comparing `tmp/opentelemetry_contrib_instrumentations-0.39b0.tar.gz` & `tmp/opentelemetry_contrib_instrumentations-0.40b0.tar.gz`

## Comparing `opentelemetry_contrib_instrumentations-0.39b0.tar` & `opentelemetry_contrib_instrumentations-0.40b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.39b0/src/opentelemetry/contrib-instrumentations/version.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.39b0/LICENSE
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.39b0/README.rst
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.40b0/src/opentelemetry/contrib-instrumentations/version.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.40b0/LICENSE
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.40b0/README.rst
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_contrib_instrumentations-0.39b0/src/opentelemetry/contrib-instrumentations/version.py` & `opentelemetry_contrib_instrumentations-0.40b0/src/opentelemetry/contrib-instrumentations/version.py`

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

### Comparing `opentelemetry_contrib_instrumentations-0.39b0/LICENSE` & `opentelemetry_contrib_instrumentations-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_contrib_instrumentations-0.39b0/README.rst` & `opentelemetry_contrib_instrumentations-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_contrib_instrumentations-0.39b0/pyproject.toml` & `opentelemetry_contrib_instrumentations-0.40b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,56 +25,57 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "opentelemetry-instrumentation-aio-pika==0.39b0",
-    "opentelemetry-instrumentation-aiohttp-client==0.39b0",
-    "opentelemetry-instrumentation-aiopg==0.39b0",
-    "opentelemetry-instrumentation-asgi==0.39b0",
-    "opentelemetry-instrumentation-asyncpg==0.39b0",
-    "opentelemetry-instrumentation-aws-lambda==0.39b0",
-    "opentelemetry-instrumentation-boto==0.39b0",
-    "opentelemetry-instrumentation-boto3sqs==0.39b0",
-    "opentelemetry-instrumentation-botocore==0.39b0",
-    "opentelemetry-instrumentation-celery==0.39b0",
-    "opentelemetry-instrumentation-confluent-kafka==0.39b0",
-    "opentelemetry-instrumentation-dbapi==0.39b0",
-    "opentelemetry-instrumentation-django==0.39b0",
-    "opentelemetry-instrumentation-elasticsearch==0.39b0",
-    "opentelemetry-instrumentation-falcon==0.39b0",
-    "opentelemetry-instrumentation-fastapi==0.39b0",
-    "opentelemetry-instrumentation-flask==0.39b0",
-    "opentelemetry-instrumentation-grpc==0.39b0",
-    "opentelemetry-instrumentation-httpx==0.39b0",
-    "opentelemetry-instrumentation-jinja2==0.39b0",
-    "opentelemetry-instrumentation-kafka-python==0.39b0",
-    "opentelemetry-instrumentation-logging==0.39b0",
-    "opentelemetry-instrumentation-mysql==0.39b0",
-    "opentelemetry-instrumentation-pika==0.39b0",
-    "opentelemetry-instrumentation-psycopg2==0.39b0",
-    "opentelemetry-instrumentation-pymemcache==0.39b0",
-    "opentelemetry-instrumentation-pymongo==0.39b0",
-    "opentelemetry-instrumentation-pymysql==0.39b0",
-    "opentelemetry-instrumentation-pyramid==0.39b0",
-    "opentelemetry-instrumentation-redis==0.39b0",
-    "opentelemetry-instrumentation-remoulade==0.39b0",
-    "opentelemetry-instrumentation-requests==0.39b0",
-    "opentelemetry-instrumentation-sklearn==0.39b0",
-    "opentelemetry-instrumentation-sqlalchemy==0.39b0",
-    "opentelemetry-instrumentation-sqlite3==0.39b0",
-    "opentelemetry-instrumentation-starlette==0.39b0",
-    "opentelemetry-instrumentation-system-metrics==0.39b0",
-    "opentelemetry-instrumentation-tornado==0.39b0",
-    "opentelemetry-instrumentation-tortoiseorm==0.39b0",
-    "opentelemetry-instrumentation-urllib==0.39b0",
-    "opentelemetry-instrumentation-urllib3==0.39b0",
-    "opentelemetry-instrumentation-wsgi==0.39b0",
+    "opentelemetry-instrumentation-aio-pika==0.40b0",
+    "opentelemetry-instrumentation-aiohttp-client==0.40b0",
+    "opentelemetry-instrumentation-aiopg==0.40b0",
+    "opentelemetry-instrumentation-asgi==0.40b0",
+    "opentelemetry-instrumentation-asyncpg==0.40b0",
+    "opentelemetry-instrumentation-aws-lambda==0.40b0",
+    "opentelemetry-instrumentation-boto==0.40b0",
+    "opentelemetry-instrumentation-boto3sqs==0.40b0",
+    "opentelemetry-instrumentation-botocore==0.40b0",
+    "opentelemetry-instrumentation-celery==0.40b0",
+    "opentelemetry-instrumentation-confluent-kafka==0.40b0",
+    "opentelemetry-instrumentation-dbapi==0.40b0",
+    "opentelemetry-instrumentation-django==0.40b0",
+    "opentelemetry-instrumentation-elasticsearch==0.40b0",
+    "opentelemetry-instrumentation-falcon==0.40b0",
+    "opentelemetry-instrumentation-fastapi==0.40b0",
+    "opentelemetry-instrumentation-flask==0.40b0",
+    "opentelemetry-instrumentation-grpc==0.40b0",
+    "opentelemetry-instrumentation-httpx==0.40b0",
+    "opentelemetry-instrumentation-jinja2==0.40b0",
+    "opentelemetry-instrumentation-kafka-python==0.40b0",
+    "opentelemetry-instrumentation-logging==0.40b0",
+    "opentelemetry-instrumentation-mysql==0.40b0",
+    "opentelemetry-instrumentation-mysqlclient==0.40b0",
+    "opentelemetry-instrumentation-pika==0.40b0",
+    "opentelemetry-instrumentation-psycopg2==0.40b0",
+    "opentelemetry-instrumentation-pymemcache==0.40b0",
+    "opentelemetry-instrumentation-pymongo==0.40b0",
+    "opentelemetry-instrumentation-pymysql==0.40b0",
+    "opentelemetry-instrumentation-pyramid==0.40b0",
+    "opentelemetry-instrumentation-redis==0.40b0",
+    "opentelemetry-instrumentation-remoulade==0.40b0",
+    "opentelemetry-instrumentation-requests==0.40b0",
+    "opentelemetry-instrumentation-sklearn==0.40b0",
+    "opentelemetry-instrumentation-sqlalchemy==0.40b0",
+    "opentelemetry-instrumentation-sqlite3==0.40b0",
+    "opentelemetry-instrumentation-starlette==0.40b0",
+    "opentelemetry-instrumentation-system-metrics==0.40b0",
+    "opentelemetry-instrumentation-tornado==0.40b0",
+    "opentelemetry-instrumentation-tortoiseorm==0.40b0",
+    "opentelemetry-instrumentation-urllib==0.40b0",
+    "opentelemetry-instrumentation-urllib3==0.40b0",
+    "opentelemetry-instrumentation-wsgi==0.40b0",
 ]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/opentelemetry-contrib-instrumentations"
```

### Comparing `opentelemetry_contrib_instrumentations-0.39b0/PKG-INFO` & `opentelemetry_contrib_instrumentations-0.40b0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-contrib-instrumentations
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Contrib Instrumentation Packages
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/opentelemetry-contrib-instrumentations
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,56 +13,57 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: opentelemetry-instrumentation-aio-pika==0.39b0
-Requires-Dist: opentelemetry-instrumentation-aiohttp-client==0.39b0
-Requires-Dist: opentelemetry-instrumentation-aiopg==0.39b0
-Requires-Dist: opentelemetry-instrumentation-asgi==0.39b0
-Requires-Dist: opentelemetry-instrumentation-asyncpg==0.39b0
-Requires-Dist: opentelemetry-instrumentation-aws-lambda==0.39b0
-Requires-Dist: opentelemetry-instrumentation-boto3sqs==0.39b0
-Requires-Dist: opentelemetry-instrumentation-boto==0.39b0
-Requires-Dist: opentelemetry-instrumentation-botocore==0.39b0
-Requires-Dist: opentelemetry-instrumentation-celery==0.39b0
-Requires-Dist: opentelemetry-instrumentation-confluent-kafka==0.39b0
-Requires-Dist: opentelemetry-instrumentation-dbapi==0.39b0
-Requires-Dist: opentelemetry-instrumentation-django==0.39b0
-Requires-Dist: opentelemetry-instrumentation-elasticsearch==0.39b0
-Requires-Dist: opentelemetry-instrumentation-falcon==0.39b0
-Requires-Dist: opentelemetry-instrumentation-fastapi==0.39b0
-Requires-Dist: opentelemetry-instrumentation-flask==0.39b0
-Requires-Dist: opentelemetry-instrumentation-grpc==0.39b0
-Requires-Dist: opentelemetry-instrumentation-httpx==0.39b0
-Requires-Dist: opentelemetry-instrumentation-jinja2==0.39b0
-Requires-Dist: opentelemetry-instrumentation-kafka-python==0.39b0
-Requires-Dist: opentelemetry-instrumentation-logging==0.39b0
-Requires-Dist: opentelemetry-instrumentation-mysql==0.39b0
-Requires-Dist: opentelemetry-instrumentation-pika==0.39b0
-Requires-Dist: opentelemetry-instrumentation-psycopg2==0.39b0
-Requires-Dist: opentelemetry-instrumentation-pymemcache==0.39b0
-Requires-Dist: opentelemetry-instrumentation-pymongo==0.39b0
-Requires-Dist: opentelemetry-instrumentation-pymysql==0.39b0
-Requires-Dist: opentelemetry-instrumentation-pyramid==0.39b0
-Requires-Dist: opentelemetry-instrumentation-redis==0.39b0
-Requires-Dist: opentelemetry-instrumentation-remoulade==0.39b0
-Requires-Dist: opentelemetry-instrumentation-requests==0.39b0
-Requires-Dist: opentelemetry-instrumentation-sklearn==0.39b0
-Requires-Dist: opentelemetry-instrumentation-sqlalchemy==0.39b0
-Requires-Dist: opentelemetry-instrumentation-sqlite3==0.39b0
-Requires-Dist: opentelemetry-instrumentation-starlette==0.39b0
-Requires-Dist: opentelemetry-instrumentation-system-metrics==0.39b0
-Requires-Dist: opentelemetry-instrumentation-tornado==0.39b0
-Requires-Dist: opentelemetry-instrumentation-tortoiseorm==0.39b0
-Requires-Dist: opentelemetry-instrumentation-urllib3==0.39b0
-Requires-Dist: opentelemetry-instrumentation-urllib==0.39b0
-Requires-Dist: opentelemetry-instrumentation-wsgi==0.39b0
+Requires-Dist: opentelemetry-instrumentation-aio-pika==0.40b0
+Requires-Dist: opentelemetry-instrumentation-aiohttp-client==0.40b0
+Requires-Dist: opentelemetry-instrumentation-aiopg==0.40b0
+Requires-Dist: opentelemetry-instrumentation-asgi==0.40b0
+Requires-Dist: opentelemetry-instrumentation-asyncpg==0.40b0
+Requires-Dist: opentelemetry-instrumentation-aws-lambda==0.40b0
+Requires-Dist: opentelemetry-instrumentation-boto3sqs==0.40b0
+Requires-Dist: opentelemetry-instrumentation-boto==0.40b0
+Requires-Dist: opentelemetry-instrumentation-botocore==0.40b0
+Requires-Dist: opentelemetry-instrumentation-celery==0.40b0
+Requires-Dist: opentelemetry-instrumentation-confluent-kafka==0.40b0
+Requires-Dist: opentelemetry-instrumentation-dbapi==0.40b0
+Requires-Dist: opentelemetry-instrumentation-django==0.40b0
+Requires-Dist: opentelemetry-instrumentation-elasticsearch==0.40b0
+Requires-Dist: opentelemetry-instrumentation-falcon==0.40b0
+Requires-Dist: opentelemetry-instrumentation-fastapi==0.40b0
+Requires-Dist: opentelemetry-instrumentation-flask==0.40b0
+Requires-Dist: opentelemetry-instrumentation-grpc==0.40b0
+Requires-Dist: opentelemetry-instrumentation-httpx==0.40b0
+Requires-Dist: opentelemetry-instrumentation-jinja2==0.40b0
+Requires-Dist: opentelemetry-instrumentation-kafka-python==0.40b0
+Requires-Dist: opentelemetry-instrumentation-logging==0.40b0
+Requires-Dist: opentelemetry-instrumentation-mysql==0.40b0
+Requires-Dist: opentelemetry-instrumentation-mysqlclient==0.40b0
+Requires-Dist: opentelemetry-instrumentation-pika==0.40b0
+Requires-Dist: opentelemetry-instrumentation-psycopg2==0.40b0
+Requires-Dist: opentelemetry-instrumentation-pymemcache==0.40b0
+Requires-Dist: opentelemetry-instrumentation-pymongo==0.40b0
+Requires-Dist: opentelemetry-instrumentation-pymysql==0.40b0
+Requires-Dist: opentelemetry-instrumentation-pyramid==0.40b0
+Requires-Dist: opentelemetry-instrumentation-redis==0.40b0
+Requires-Dist: opentelemetry-instrumentation-remoulade==0.40b0
+Requires-Dist: opentelemetry-instrumentation-requests==0.40b0
+Requires-Dist: opentelemetry-instrumentation-sklearn==0.40b0
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy==0.40b0
+Requires-Dist: opentelemetry-instrumentation-sqlite3==0.40b0
+Requires-Dist: opentelemetry-instrumentation-starlette==0.40b0
+Requires-Dist: opentelemetry-instrumentation-system-metrics==0.40b0
+Requires-Dist: opentelemetry-instrumentation-tornado==0.40b0
+Requires-Dist: opentelemetry-instrumentation-tortoiseorm==0.40b0
+Requires-Dist: opentelemetry-instrumentation-urllib3==0.40b0
+Requires-Dist: opentelemetry-instrumentation-urllib==0.40b0
+Requires-Dist: opentelemetry-instrumentation-wsgi==0.40b0
 Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Instrumentation
 =============================
 
 |pypi|
```

