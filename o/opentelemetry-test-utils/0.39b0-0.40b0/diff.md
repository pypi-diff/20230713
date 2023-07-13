# Comparing `tmp/opentelemetry_test_utils-0.39b0.tar.gz` & `tmp/opentelemetry_test_utils-0.40b0.tar.gz`

## Comparing `opentelemetry_test_utils-0.39b0.tar` & `opentelemetry_test_utils-0.40b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/asgitestutil.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/concurrency_test.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/globals_test.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/httptest.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/metrictestutil.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/mock_textmap.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/spantestutil.py
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/test_base.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/version.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/src/opentelemetry/test/wsgitestutil.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/.gitignore
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/README.rst
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/asgitestutil.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/concurrency_test.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/globals_test.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/httptest.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/metrictestutil.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/mock_textmap.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/spantestutil.py
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/test_base.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/version.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/src/opentelemetry/test/wsgitestutil.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/.gitignore
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/README.rst
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/asgitestutil.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/asgitestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/concurrency_test.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/concurrency_test.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/globals_test.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/globals_test.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/httptest.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/httptest.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class HttpTestBase(unittest.TestCase):
     DEFAULT_RESPONSE = b"Hello!"
 
     class Handler(BaseHTTPRequestHandler):
         protocol_version = "HTTP/1.1"  # Support keep-alive.
-        # timeout = 3 # No timeout -- if shutdown hangs, make sure to close your connection
+        timeout = 3  # Seconds
 
         STATUS_RE = re.compile(r"/status/(\d+)")
 
         def do_GET(self):  # pylint:disable=invalid-name
             status_match = self.STATUS_RE.fullmatch(self.path)
             status = 200
             if status_match:
```

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/metrictestutil.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/metrictestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/mock_textmap.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/mock_textmap.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/spantestutil.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/spantestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/test_base.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/test_base.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/src/opentelemetry/test/wsgitestutil.py` & `opentelemetry_test_utils-0.40b0/src/opentelemetry/test/wsgitestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/.gitignore` & `opentelemetry_test_utils-0.40b0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.39b0/pyproject.toml` & `opentelemetry_test_utils-0.40b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
   "asgiref ~= 3.0",
-  "opentelemetry-api == 1.18.0",
-  "opentelemetry-sdk == 1.18.0",
+  "opentelemetry-api == 1.19.0",
+  "opentelemetry-sdk == 1.19.0",
 ]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python/tests/opentelemetry-test-utils"
```

### Comparing `opentelemetry_test_utils-0.39b0/PKG-INFO` & `opentelemetry_test_utils-0.40b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-test-utils
-Version: 0.39b0
+Version: 0.40b0
 Summary: Test utilities for OpenTelemetry unit tests
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tests/opentelemetry-test-utils
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: asgiref~=3.0
-Requires-Dist: opentelemetry-api==1.18.0
-Requires-Dist: opentelemetry-sdk==1.18.0
+Requires-Dist: opentelemetry-api==1.19.0
+Requires-Dist: opentelemetry-sdk==1.19.0
 Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Test Utilities
 ============================
 
 This package provides internal testing utilities for the OpenTelemetry Python project and provides no stability or quality guarantees.
```

