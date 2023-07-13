# Comparing `tmp/opentelemetry_propagator_ot_trace-0.39b0.tar.gz` & `tmp/opentelemetry_propagator_ot_trace-0.40b0.tar.gz`

## Comparing `opentelemetry_propagator_ot_trace-0.39b0.tar` & `opentelemetry_propagator_ot_trace-0.40b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/src/opentelemetry/propagators/ot_trace/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/src/opentelemetry/propagators/ot_trace/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/tests/test_ot_trace_propagator.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/.gitignore
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/README.rst
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/src/opentelemetry/propagators/ot_trace/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/src/opentelemetry/propagators/ot_trace/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/tests/test_ot_trace_propagator.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/.gitignore
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/README.rst
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 opentelemetry_propagator_ot_trace-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_propagator_ot_trace-0.39b0/src/opentelemetry/propagators/ot_trace/__init__.py` & `opentelemetry_propagator_ot_trace-0.40b0/src/opentelemetry/propagators/ot_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_propagator_ot_trace-0.39b0/src/opentelemetry/propagators/ot_trace/version.py` & `opentelemetry_propagator_ot_trace-0.40b0/src/opentelemetry/propagators/ot_trace/version.py`

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

### Comparing `opentelemetry_propagator_ot_trace-0.39b0/tests/test_ot_trace_propagator.py` & `opentelemetry_propagator_ot_trace-0.40b0/tests/test_ot_trace_propagator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_propagator_ot_trace-0.39b0/README.rst` & `opentelemetry_propagator_ot_trace-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_propagator_ot_trace-0.39b0/pyproject.toml` & `opentelemetry_propagator_ot_trace-0.40b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_propagator_ot_trace-0.39b0/PKG-INFO` & `opentelemetry_propagator_ot_trace-0.40b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-propagator-ot-trace
-Version: 0.39b0
+Version: 0.40b0
 Summary: OT Trace Propagator for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/propagator/opentelemetry-propagator-ot-trace
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

