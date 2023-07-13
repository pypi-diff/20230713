# Comparing `tmp/opentelemetry-exporter-zipkin-proto-http-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-zipkin-proto-http-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-zipkin-proto-http-1.9.0.tar", last modified: Wed Jan 26 18:29:18 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-zipkin-proto-http-1.9.1.tar", last modified: Mon Jan 31 10:09:51 2022, max compression
```

## Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0.tar` & `opentelemetry-exporter-zipkin-proto-http-1.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/
--rw-r--r--   0 runner    (1001) docker     (121)     6372 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/
--rw-r--r--   0 runner    (1001) docker     (121)     4745 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18283 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     8922 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/encoder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19998 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/encoder/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     9921 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/encoder/test_v2_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8517 2022-01-26 18:29:09.000000 opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/test_zipkin_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/
+-rw-r--r--   0 runner    (1001) docker     (121)     6372 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/
+-rw-r--r--   0 runner    (1001) docker     (121)     4745 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18283 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8922 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/encoder/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19998 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/encoder/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9921 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/encoder/test_v2_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8517 2022-01-31 10:09:42.000000 opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/test_zipkin_exporter.py
```

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/LICENSE` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/PKG-INFO` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-zipkin-proto-http
-Version: 1.9.0
+Version: 1.9.1
 Summary: Zipkin Span Protobuf Exporter for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-zipkin-proto-http
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/README.rst` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/setup.cfg` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	=src
 packages = find_namespace:
 install_requires = 
 	protobuf >= 3.12
 	requests ~= 2.7
 	opentelemetry-api ~= 1.3
 	opentelemetry-sdk ~= 1.3
-	opentelemetry-exporter-zipkin-json == 1.9.0
+	opentelemetry-exporter-zipkin-json == 1.9.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test =
```

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/setup.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/__init__.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/__init__.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.pyi` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/v2/gen/zipkin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry/exporter/zipkin/proto/http/version.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "1.9.0"
```

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/PKG-INFO` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-zipkin-proto-http
-Version: 1.9.0
+Version: 1.9.1
 Summary: Zipkin Span Protobuf Exporter for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-zipkin-proto-http
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/src/opentelemetry_exporter_zipkin_proto_http.egg-info/SOURCES.txt` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry_exporter_zipkin_proto_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/__init__.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/src/opentelemetry/exporter/zipkin/proto/http/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = "1.9.1"
```

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/encoder/common_tests.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/encoder/common_tests.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/encoder/test_v2_protobuf.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/encoder/test_v2_protobuf.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-zipkin-proto-http-1.9.0/tests/test_zipkin_exporter.py` & `opentelemetry-exporter-zipkin-proto-http-1.9.1/tests/test_zipkin_exporter.py`

 * *Files identical despite different names*

