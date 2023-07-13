# Comparing `tmp/opentelemetry_semantic_conventions-0.39b0.tar.gz` & `tmp/opentelemetry_semantic_conventions-0.40b0.tar.gz`

## Comparing `opentelemetry_semantic_conventions-0.39b0.tar` & `opentelemetry_semantic_conventions-0.40b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/version.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/metrics/__init__.py
--rw-r--r--   0        0        0    21915 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/resource/__init__.py
--rw-r--r--   0        0        0    38732 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/trace/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/tests/test_semconv.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/LICENSE
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/README.rst
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/version.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/metrics/__init__.py
+-rw-r--r--   0        0        0    21915 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/resource/__init__.py
+-rw-r--r--   0        0        0    38732 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/trace/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/tests/test_semconv.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/LICENSE
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/README.rst
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/version.py` & `opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/version.py`

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

### Comparing `opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/metrics/__init__.py` & `opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/resource/__init__.py` & `opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/src/opentelemetry/semconv/trace/__init__.py` & `opentelemetry_semantic_conventions-0.40b0/src/opentelemetry/semconv/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/tests/test_semconv.py` & `opentelemetry_semantic_conventions-0.40b0/tests/test_semconv.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/.gitignore` & `opentelemetry_semantic_conventions-0.40b0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/LICENSE` & `opentelemetry_semantic_conventions-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/README.rst` & `opentelemetry_semantic_conventions-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/pyproject.toml` & `opentelemetry_semantic_conventions-0.40b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.39b0/PKG-INFO` & `opentelemetry_semantic_conventions-0.40b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-semantic-conventions
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Semantic Conventions
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-semantic-conventions
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

