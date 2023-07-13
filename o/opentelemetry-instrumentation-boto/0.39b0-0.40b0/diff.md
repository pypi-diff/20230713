# Comparing `tmp/opentelemetry_instrumentation_boto-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_boto-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_boto-0.39b0.tar` & `opentelemetry_instrumentation_boto-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/src/opentelemetry/instrumentation/boto/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/src/opentelemetry/instrumentation/boto/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/src/opentelemetry/instrumentation/boto/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/tests/conftest.py
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/tests/test_boto_instrumentation.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/LICENSE
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/README.rst
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/src/opentelemetry/instrumentation/boto/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/src/opentelemetry/instrumentation/boto/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/src/opentelemetry/instrumentation/boto/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/tests/conftest.py
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/tests/test_boto_instrumentation.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/LICENSE
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/README.rst
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_boto-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_boto-0.39b0/src/opentelemetry/instrumentation/boto/__init__.py` & `opentelemetry_instrumentation_boto-0.40b0/src/opentelemetry/instrumentation/boto/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_boto-0.39b0/src/opentelemetry/instrumentation/boto/package.py` & `opentelemetry_instrumentation_boto-0.40b0/src/opentelemetry/instrumentation/boto/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_boto-0.39b0/src/opentelemetry/instrumentation/boto/version.py` & `opentelemetry_instrumentation_boto-0.40b0/src/opentelemetry/instrumentation/boto/version.py`

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

### Comparing `opentelemetry_instrumentation_boto-0.39b0/tests/conftest.py` & `opentelemetry_instrumentation_boto-0.40b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_boto-0.39b0/tests/test_boto_instrumentation.py` & `opentelemetry_instrumentation_boto-0.40b0/tests/test_boto_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_boto-0.39b0/LICENSE` & `opentelemetry_instrumentation_boto-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_boto-0.39b0/README.rst` & `opentelemetry_instrumentation_boto-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_boto-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_boto-0.40b0/pyproject.toml`

 * *Files 5% similar despite different names*

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
 ]
 
 [project.optional-dependencies]
 instruments = [
   "boto~=2.0",
 ]
 test = [
   "opentelemetry-instrumentation-boto[instruments]",
   "markupsafe==2.0.1",
   "moto~=2.0",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 boto = "opentelemetry.instrumentation.boto:BotoInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-boto"
```

### Comparing `opentelemetry_instrumentation_boto-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_boto-0.40b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-boto
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Boto instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-boto
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
 Provides-Extra: instruments
 Requires-Dist: boto~=2.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: markupsafe==2.0.1; extra == 'test'
 Requires-Dist: moto~=2.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-boto[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Boto Tracing
 ==========================
 
 |pypi|
```

