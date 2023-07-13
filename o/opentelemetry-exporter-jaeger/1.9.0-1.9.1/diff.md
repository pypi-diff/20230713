# Comparing `tmp/opentelemetry-exporter-jaeger-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-jaeger-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-jaeger-1.9.0.tar", last modified: Wed Jan 26 18:29:17 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-jaeger-1.9.1.tar", last modified: Mon Jan 31 10:09:49 2022, max compression
```

## Comparing `opentelemetry-exporter-jaeger-1.9.0.tar` & `opentelemetry-exporter-jaeger-1.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/src/opentelemetry/exporter/jaeger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/src/opentelemetry/exporter/jaeger/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/src/opentelemetry/exporter/jaeger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-jaeger-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-1.9.0/tests/test_jaeger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/src/opentelemetry/exporter/jaeger/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/src/opentelemetry/exporter/jaeger/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/src/opentelemetry/exporter/jaeger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-1.9.1/tests/test_jaeger.py
```

### Comparing `opentelemetry-exporter-jaeger-1.9.0/LICENSE` & `opentelemetry-exporter-jaeger-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-1.9.0/PKG-INFO` & `opentelemetry-exporter-jaeger-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-jaeger
-Version: 1.9.0
+Version: 1.9.1
 Summary: Jaeger Exporters for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-jaeger
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-jaeger-1.9.0/README.rst` & `opentelemetry-exporter-jaeger-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-1.9.0/opentelemetry_exporter_jaeger.egg-info/PKG-INFO` & `opentelemetry-exporter-jaeger-1.9.1/opentelemetry_exporter_jaeger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-jaeger
-Version: 1.9.0
+Version: 1.9.1
 Summary: Jaeger Exporters for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-jaeger
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-jaeger-1.9.0/setup.cfg` & `opentelemetry-exporter-jaeger-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 	Programming Language :: Python :: 3.10
 	Typing :: Typed
 
 [options]
 python_requires = >=3.6
 packages = find_namespace:
 install_requires = 
-	opentelemetry-exporter-jaeger-proto-grpc == 1.9.0
-	opentelemetry-exporter-jaeger-thrift == 1.9.0
+	opentelemetry-exporter-jaeger-proto-grpc == 1.9.1
+	opentelemetry-exporter-jaeger-thrift == 1.9.1
 
 [options.extras_require]
 test = 
 
 [options.entry_points]
 opentelemetry_traces_exporter = 
 	jaeger = opentelemetry.exporter.jaeger.proto.grpc:JaegerExporter
```

### Comparing `opentelemetry-exporter-jaeger-1.9.0/setup.py` & `opentelemetry-exporter-jaeger-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-1.9.0/src/opentelemetry/exporter/jaeger/version.py` & `opentelemetry-exporter-jaeger-1.9.1/src/opentelemetry/exporter/jaeger/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `opentelemetry-exporter-jaeger-1.9.0/tests/test_jaeger.py` & `opentelemetry-exporter-jaeger-1.9.1/tests/test_jaeger.py`

 * *Files identical despite different names*

