# Comparing `tmp/opentelemetry_instrumentation_aio_pika-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_aio_pika-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_aio_pika-0.39b0.tar` & `opentelemetry_instrumentation_aio_pika-0.40b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/aio_pika_instrumentor.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/callback_decorator.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/package.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/publish_decorator.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/span_builder.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/tests/consts.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_aio_pika_instrumentation.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_callback_decorator.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_publish_decorator.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_span_builder.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/LICENSE
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/README.rst
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/aio_pika_instrumentor.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/callback_decorator.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/package.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/publish_decorator.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/span_builder.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/tests/consts.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_aio_pika_instrumentation.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_callback_decorator.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_publish_decorator.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_span_builder.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/LICENSE
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/README.rst
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aio_pika-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/__init__.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/aio_pika_instrumentor.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/aio_pika_instrumentor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/callback_decorator.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/callback_decorator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/package.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/publish_decorator.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/publish_decorator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/span_builder.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/span_builder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/src/opentelemetry/instrumentation/aio_pika/version.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/src/opentelemetry/instrumentation/aio_pika/version.py`

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

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/tests/consts.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_aio_pika_instrumentation.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_aio_pika_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_callback_decorator.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_callback_decorator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_publish_decorator.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_publish_decorator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/tests/test_span_builder.py` & `opentelemetry_instrumentation_aio_pika-0.40b0/tests/test_span_builder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/LICENSE` & `opentelemetry_instrumentation_aio_pika-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/README.rst` & `opentelemetry_instrumentation_aio_pika-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_aio_pika-0.40b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [project.optional-dependencies]
 instruments = [
   "aio_pika >= 7.2.0, < 10.0.0",
 ]
 test = [
   "opentelemetry-instrumentation-aio-pika[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "pytest",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 aio-pika = "opentelemetry.instrumentation.aio_pika:AioPikaInstrumentor"
```

### Comparing `opentelemetry_instrumentation_aio_pika-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_aio_pika-0.40b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-aio-pika
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Aio-pika instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aio-pika
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.5
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: aio-pika<10.0.0,>=7.2.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-aio-pika[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: wrapt<2.0.0,>=1.0.0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Aio-pika Instrumentation
 ======================================
```

