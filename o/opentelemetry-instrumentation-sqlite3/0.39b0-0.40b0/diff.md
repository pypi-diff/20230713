# Comparing `tmp/opentelemetry_instrumentation_sqlite3-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_sqlite3-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_sqlite3-0.39b0.tar` & `opentelemetry_instrumentation_sqlite3-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/src/opentelemetry/instrumentation/sqlite3/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/src/opentelemetry/instrumentation/sqlite3/package.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/src/opentelemetry/instrumentation/sqlite3/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/tests/test_sqlite3.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/tests/testdb
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/README.rst
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/src/opentelemetry/instrumentation/sqlite3/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/src/opentelemetry/instrumentation/sqlite3/package.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/src/opentelemetry/instrumentation/sqlite3/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/tests/test_sqlite3.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/tests/testdb
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/README.rst
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlite3-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/src/opentelemetry/instrumentation/sqlite3/__init__.py` & `opentelemetry_instrumentation_sqlite3-0.40b0/src/opentelemetry/instrumentation/sqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/src/opentelemetry/instrumentation/sqlite3/package.py` & `opentelemetry_instrumentation_sqlite3-0.40b0/src/opentelemetry/instrumentation/sqlite3/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/src/opentelemetry/instrumentation/sqlite3/version.py` & `opentelemetry_instrumentation_sqlite3-0.40b0/src/opentelemetry/instrumentation/sqlite3/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.39b0"
+__version__ = "0.40b0"
 
 _instruments = tuple()
```

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/tests/test_sqlite3.py` & `opentelemetry_instrumentation_sqlite3-0.40b0/tests/test_sqlite3.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/tests/testdb` & `opentelemetry_instrumentation_sqlite3-0.40b0/tests/testdb`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/LICENSE` & `opentelemetry_instrumentation_sqlite3-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/README.rst` & `opentelemetry_instrumentation_sqlite3-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_sqlite3-0.40b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
-  "opentelemetry-instrumentation-dbapi == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-instrumentation-dbapi == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = []
 test = [
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 sqlite3 = "opentelemetry.instrumentation.sqlite3:SQLite3Instrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-sqlite3"
```

### Comparing `opentelemetry_instrumentation_sqlite3-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_sqlite3-0.40b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-sqlite3
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry SQLite3 instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-sqlite3
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation-dbapi==0.39b0
-Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-instrumentation-dbapi==0.40b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
 Provides-Extra: instruments
 Provides-Extra: test
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry SQLite3 Instrumentation
 =====================================
 
 |pypi|
```

