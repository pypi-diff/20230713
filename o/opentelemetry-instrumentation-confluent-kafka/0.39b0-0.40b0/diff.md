# Comparing `tmp/opentelemetry_instrumentation_confluent_kafka-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_confluent_kafka-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0.tar` & `opentelemetry_instrumentation_confluent_kafka-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/package.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/tests/test_instrumentation.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/LICENSE
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/README.rst
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/package.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/tests/test_instrumentation.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/LICENSE
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/README.rst
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/package.py` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-_instruments = ("confluent-kafka >= 1.8.2, < 2.0.0",)
+_instruments = ("confluent-kafka >= 1.8.2, <= 2.2.0",)
```

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/version.py` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/src/opentelemetry/instrumentation/confluent_kafka/version.py`

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

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/tests/test_instrumentation.py` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/LICENSE` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/README.rst` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 dependencies = [
   "opentelemetry-api ~= 1.12",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
-  "confluent-kafka >= 1.8.2, < 2.0.0",
+  "confluent-kafka >= 1.8.2, <= 2.2.0",
 ]
 test = [
   "opentelemetry-instrumentation-confluent-kafka[instruments]",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 confluent_kafka = "opentelemetry.instrumentation.confluent_kafka:ConfluentKafkaInstrumentor"
```

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_confluent_kafka-0.40b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-confluent-kafka
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Confluent Kafka instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-confluent-kafka
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
-Requires-Dist: confluent-kafka<2.0.0,>=1.8.2; extra == 'instruments'
+Requires-Dist: confluent-kafka<=2.2.0,>=1.8.2; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-confluent-kafka[instruments]; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry confluent-kafka Instrumentation
 =============================================
```

