# Comparing `tmp/opentelemetry_instrumentation_system_metrics-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_system_metrics-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_system_metrics-0.39b0.tar` & `opentelemetry_instrumentation_system_metrics-0.40b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/__init__.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    26038 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/tests/test_system_metrics.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/LICENSE
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/README.rst
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/src/opentelemetry/instrumentation/system_metrics/__init__.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/src/opentelemetry/instrumentation/system_metrics/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/src/opentelemetry/instrumentation/system_metrics/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    26038 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/tests/test_system_metrics.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/LICENSE
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/README.rst
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/__init__.py` & `opentelemetry_instrumentation_system_metrics-0.40b0/src/opentelemetry/instrumentation/system_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/package.py` & `opentelemetry_instrumentation_system_metrics-0.40b0/src/opentelemetry/instrumentation/system_metrics/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/version.py` & `opentelemetry_instrumentation_system_metrics-0.40b0/src/opentelemetry/instrumentation/system_metrics/version.py`

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

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/tests/test_system_metrics.py` & `opentelemetry_instrumentation_system_metrics-0.40b0/tests/test_system_metrics.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/LICENSE` & `opentelemetry_instrumentation_system_metrics-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/README.rst` & `opentelemetry_instrumentation_system_metrics-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_system_metrics-0.40b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 [project.optional-dependencies]
 instruments = [
   "psutil >= 5",
 ]
 test = [
   "opentelemetry-instrumentation-system-metrics[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 system_metrics = "opentelemetry.instrumentation.system_metrics:SystemMetricsInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-system-metrics"
```

### Comparing `opentelemetry_instrumentation_system_metrics-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_system_metrics-0.40b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-system-metrics
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry System Metrics Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-system-metrics
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Requires-Dist: opentelemetry-api~=1.11
 Requires-Dist: opentelemetry-sdk~=1.11
 Requires-Dist: psutil~=5.9
 Provides-Extra: instruments
 Requires-Dist: psutil>=5; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-system-metrics[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry System Metrics Instrumentation
 ============================================
 
 |pypi|
```

