# Comparing `tmp/opentelemetry_exporter_richconsole-0.39b0.tar.gz` & `tmp/opentelemetry_exporter_richconsole-0.40b0.tar.gz`

## Comparing `opentelemetry_exporter_richconsole-0.39b0.tar` & `opentelemetry_exporter_richconsole-0.40b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/src/opentelemetry/exporter/richconsole/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/src/opentelemetry/exporter/richconsole/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/tests/test_rich_exporter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/.gitignore
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/README.rst
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/src/opentelemetry/exporter/richconsole/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/src/opentelemetry/exporter/richconsole/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/tests/test_rich_exporter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/.gitignore
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/README.rst
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 opentelemetry_exporter_richconsole-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_exporter_richconsole-0.39b0/src/opentelemetry/exporter/richconsole/__init__.py` & `opentelemetry_exporter_richconsole-0.40b0/src/opentelemetry/exporter/richconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_richconsole-0.39b0/src/opentelemetry/exporter/richconsole/version.py` & `opentelemetry_exporter_richconsole-0.40b0/src/opentelemetry/exporter/richconsole/version.py`

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

### Comparing `opentelemetry_exporter_richconsole-0.39b0/tests/test_rich_exporter.py` & `opentelemetry_exporter_richconsole-0.40b0/tests/test_rich_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_richconsole-0.39b0/README.rst` & `opentelemetry_exporter_richconsole-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_richconsole-0.39b0/pyproject.toml` & `opentelemetry_exporter_richconsole-0.40b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
   "opentelemetry-sdk ~= 1.12",
-  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
   "rich>=10.0.0",
 ]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
```

### Comparing `opentelemetry_exporter_richconsole-0.39b0/PKG-INFO` & `opentelemetry_exporter_richconsole-0.40b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-richconsole
-Version: 0.39b0
+Version: 0.40b0
 Summary: Rich Console Exporter for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/exporter/opentelemetry-exporter-richconsole
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
 Requires-Dist: opentelemetry-sdk~=1.12
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Requires-Dist: rich>=10.0.0
 Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Rich Console Exporter
 ===================================
```

