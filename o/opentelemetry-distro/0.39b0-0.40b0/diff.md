# Comparing `tmp/opentelemetry_distro-0.39b0.tar.gz` & `tmp/opentelemetry_distro-0.40b0.tar.gz`

## Comparing `opentelemetry_distro-0.39b0.tar` & `opentelemetry_distro-0.40b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/src/opentelemetry/distro/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/src/opentelemetry/distro/py.typed
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/src/opentelemetry/distro/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/tests/test_distro.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/.gitignore
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/README.rst
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 opentelemetry_distro-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/src/opentelemetry/distro/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/src/opentelemetry/distro/py.typed
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/src/opentelemetry/distro/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/tests/test_distro.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/.gitignore
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/README.rst
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 opentelemetry_distro-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_distro-0.39b0/src/opentelemetry/distro/__init__.py` & `opentelemetry_distro-0.40b0/src/opentelemetry/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_distro-0.39b0/src/opentelemetry/distro/version.py` & `opentelemetry_distro-0.40b0/src/opentelemetry/distro/version.py`

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

### Comparing `opentelemetry_distro-0.39b0/tests/test_distro.py` & `opentelemetry_distro-0.40b0/tests/test_distro.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_distro-0.39b0/pyproject.toml` & `opentelemetry_distro-0.40b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -20,21 +20,21 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Typing :: Typed",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
   "opentelemetry-sdk ~= 1.13",
 ]
 
 [project.optional-dependencies]
 otlp = [
-  "opentelemetry-exporter-otlp == 1.18.0",
+  "opentelemetry-exporter-otlp == 1.19.0",
 ]
 test = []
 
 [project.entry-points.opentelemetry_configurator]
 configurator = "opentelemetry.distro:OpenTelemetryConfigurator"
 
 [project.entry-points.opentelemetry_distro]
```

### Comparing `opentelemetry_distro-0.39b0/PKG-INFO` & `opentelemetry_distro-0.40b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: opentelemetry-distro
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Python Distro
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/opentelemetry-distro
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
 Requires-Dist: opentelemetry-sdk~=1.13
 Provides-Extra: otlp
-Requires-Dist: opentelemetry-exporter-otlp==1.18.0; extra == 'otlp'
+Requires-Dist: opentelemetry-exporter-otlp==1.19.0; extra == 'otlp'
 Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Distro
 ====================
 
 |pypi|
```

