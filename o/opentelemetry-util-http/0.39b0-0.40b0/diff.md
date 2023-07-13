# Comparing `tmp/opentelemetry_util_http-0.39b0.tar.gz` & `tmp/opentelemetry_util_http-0.40b0.tar.gz`

## Comparing `opentelemetry_util_http-0.39b0.tar` & `opentelemetry_util_http-0.40b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/src/opentelemetry/util/http/__init__.py
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/src/opentelemetry/util/http/httplib.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/src/opentelemetry/util/http/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/tests/test_capture_custom_headers.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/tests/test_http_base.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/tests/test_http_excluded_urls.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/README.rst
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/src/opentelemetry/util/http/__init__.py
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/src/opentelemetry/util/http/httplib.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/src/opentelemetry/util/http/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/tests/test_capture_custom_headers.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/tests/test_http_base.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/tests/test_http_excluded_urls.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/README.rst
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 opentelemetry_util_http-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_util_http-0.39b0/src/opentelemetry/util/http/__init__.py` & `opentelemetry_util_http-0.40b0/src/opentelemetry/util/http/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/src/opentelemetry/util/http/httplib.py` & `opentelemetry_util_http-0.40b0/src/opentelemetry/util/http/httplib.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/src/opentelemetry/util/http/version.py` & `opentelemetry_util_http-0.40b0/src/opentelemetry/util/http/version.py`

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

### Comparing `opentelemetry_util_http-0.39b0/tests/test_capture_custom_headers.py` & `opentelemetry_util_http-0.40b0/tests/test_capture_custom_headers.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/tests/test_http_base.py` & `opentelemetry_util_http-0.40b0/tests/test_http_base.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/tests/test_http_excluded_urls.py` & `opentelemetry_util_http-0.40b0/tests/test_http_excluded_urls.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/README.rst` & `opentelemetry_util_http-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/pyproject.toml` & `opentelemetry_util_http-0.40b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_util_http-0.39b0/PKG-INFO` & `opentelemetry_util_http-0.40b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-util-http
-Version: 0.39b0
+Version: 0.40b0
 Summary: Web util for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/util/opentelemetry-util-http
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

