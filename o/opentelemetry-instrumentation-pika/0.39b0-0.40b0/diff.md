# Comparing `tmp/opentelemetry_instrumentation_pika-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_pika-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_pika-0.39b0.tar` & `opentelemetry_instrumentation_pika-0.40b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/package.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/pika_instrumentor.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/tests/test_getter.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/tests/test_pika_instrumentation.py
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/tests/test_utils.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/LICENSE
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/README.rst
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/package.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/pika_instrumentor.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/tests/test_getter.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/tests/test_pika_instrumentation.py
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/tests/test_utils.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/LICENSE
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/README.rst
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_pika-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/__init__.py` & `opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/package.py` & `opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/pika_instrumentor.py` & `opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/pika_instrumentor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/utils.py` & `opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/src/opentelemetry/instrumentation/pika/version.py` & `opentelemetry_instrumentation_pika-0.40b0/src/opentelemetry/instrumentation/pika/version.py`

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

### Comparing `opentelemetry_instrumentation_pika-0.39b0/tests/test_getter.py` & `opentelemetry_instrumentation_pika-0.40b0/tests/test_getter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/tests/test_pika_instrumentation.py` & `opentelemetry_instrumentation_pika-0.40b0/tests/test_pika_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/tests/test_utils.py` & `opentelemetry_instrumentation_pika-0.40b0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/LICENSE` & `opentelemetry_instrumentation_pika-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/README.rst` & `opentelemetry_instrumentation_pika-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pika-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_pika-0.40b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 [project.optional-dependencies]
 instruments = [
   "pika >= 0.12.0",
 ]
 test = [
   "opentelemetry-instrumentation-pika[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "pytest",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 pika = "opentelemetry.instrumentation.pika:PikaInstrumentor"
```

### Comparing `opentelemetry_instrumentation_pika-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_pika-0.40b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-pika
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry pika instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-pika
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Requires-Dist: opentelemetry-api~=1.5
 Requires-Dist: packaging>=20.0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: pika>=0.12.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-pika[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: wrapt<2.0.0,>=1.0.0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry pika Instrumentation
 ==================================
```

