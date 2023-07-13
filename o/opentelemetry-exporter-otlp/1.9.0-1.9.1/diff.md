# Comparing `tmp/opentelemetry-exporter-otlp-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-otlp-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-otlp-1.9.0.tar", last modified: Wed Jan 26 18:29:18 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-otlp-1.9.1.tar", last modified: Mon Jan 31 10:09:51 2022, max compression
```

## Comparing `opentelemetry-exporter-otlp-1.9.0.tar` & `opentelemetry-exporter-otlp-1.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/src/opentelemetry/exporter/otlp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/src/opentelemetry/exporter/otlp/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/src/opentelemetry/exporter/otlp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:18.000000 opentelemetry-exporter-otlp-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-1.9.0/tests/test_otlp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/src/opentelemetry/exporter/otlp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/src/opentelemetry/exporter/otlp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/src/opentelemetry/exporter/otlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:51.000000 opentelemetry-exporter-otlp-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-1.9.1/tests/test_otlp.py
```

### Comparing `opentelemetry-exporter-otlp-1.9.0/LICENSE` & `opentelemetry-exporter-otlp-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-1.9.0/PKG-INFO` & `opentelemetry-exporter-otlp-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Collector Exporters
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-otlp-1.9.0/README.rst` & `opentelemetry-exporter-otlp-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-1.9.0/opentelemetry_exporter_otlp.egg-info/PKG-INFO` & `opentelemetry-exporter-otlp-1.9.1/opentelemetry_exporter_otlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Collector Exporters
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-otlp-1.9.0/setup.cfg` & `opentelemetry-exporter-otlp-1.9.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 	Programming Language :: Python :: 3.10
 	Typing :: Typed
 
 [options]
 python_requires = >=3.6
 packages = find_namespace:
 install_requires = 
-	opentelemetry-exporter-otlp-proto-grpc == 1.9.0
-	opentelemetry-exporter-otlp-proto-http == 1.9.0
+	opentelemetry-exporter-otlp-proto-grpc == 1.9.1
+	opentelemetry-exporter-otlp-proto-http == 1.9.1
 
 [options.entry_points]
 opentelemetry_traces_exporter = 
 	otlp = opentelemetry.exporter.otlp.proto.grpc.trace_exporter:OTLPSpanExporter
 opentelemetry_logs_exporter = 
 	otlp = opentelemetry.exporter.otlp.proto.grpc._log_exporter:OTLPLogExporter
```

### Comparing `opentelemetry-exporter-otlp-1.9.0/setup.py` & `opentelemetry-exporter-otlp-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-1.9.0/src/opentelemetry/exporter/otlp/version.py` & `opentelemetry-exporter-otlp-1.9.1/src/opentelemetry/exporter/otlp/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `opentelemetry-exporter-otlp-1.9.0/tests/test_otlp.py` & `opentelemetry-exporter-otlp-1.9.1/tests/test_otlp.py`

 * *Files identical despite different names*

