# Comparing `tmp/opentelemetry-propagator-b3-1.9.0.tar.gz` & `tmp/opentelemetry-propagator-b3-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-propagator-b3-1.9.0.tar", last modified: Wed Jan 26 18:29:19 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-propagator-b3-1.9.1.tar", last modified: Mon Jan 31 10:09:52 2022, max compression
```

## Comparing `opentelemetry-propagator-b3-1.9.0.tar` & `opentelemetry-propagator-b3-1.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/b3/
--rw-r--r--   0 runner    (1001) docker     (121)     6700 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/b3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/b3/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/b3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/tests/performance/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/tests/performance/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/tests/performance/benchmarks/trace/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:19.000000 opentelemetry-propagator-b3-1.9.0/tests/performance/benchmarks/trace/propagation/
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/tests/performance/benchmarks/trace/propagation/test_benchmark_b3_format.py
--rw-r--r--   0 runner    (1001) docker     (121)    16625 2022-01-26 18:29:09.000000 opentelemetry-propagator-b3-1.9.0/tests/test_b3_format.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/b3/
+-rw-r--r--   0 runner    (1001) docker     (121)     6700 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/b3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/b3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/b3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/tests/performance/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/tests/performance/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/tests/performance/benchmarks/trace/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:52.000000 opentelemetry-propagator-b3-1.9.1/tests/performance/benchmarks/trace/propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/tests/performance/benchmarks/trace/propagation/test_benchmark_b3_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16625 2022-01-31 10:09:42.000000 opentelemetry-propagator-b3-1.9.1/tests/test_b3_format.py
```

### Comparing `opentelemetry-propagator-b3-1.9.0/LICENSE` & `opentelemetry-propagator-b3-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-b3-1.9.0/PKG-INFO` & `opentelemetry-propagator-b3-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-propagator-b3
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry B3 Propagator
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/propagator/opentelemetry-propagator-b3
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-propagator-b3-1.9.0/setup.cfg` & `opentelemetry-propagator-b3-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-b3-1.9.0/setup.py` & `opentelemetry-propagator-b3-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/b3/__init__.py` & `opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/b3/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-b3-1.9.0/src/opentelemetry/propagators/b3/version.py` & `opentelemetry-propagator-b3-1.9.1/tests/__init__.py`

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

### Comparing `opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/PKG-INFO` & `opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-propagator-b3
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry B3 Propagator
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/propagator/opentelemetry-propagator-b3
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-propagator-b3-1.9.0/src/opentelemetry_propagator_b3.egg-info/SOURCES.txt` & `opentelemetry-propagator-b3-1.9.1/src/opentelemetry_propagator_b3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-b3-1.9.0/tests/__init__.py` & `opentelemetry-propagator-b3-1.9.1/src/opentelemetry/propagators/b3/version.py`

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

### Comparing `opentelemetry-propagator-b3-1.9.0/tests/performance/benchmarks/trace/propagation/test_benchmark_b3_format.py` & `opentelemetry-propagator-b3-1.9.1/tests/performance/benchmarks/trace/propagation/test_benchmark_b3_format.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-b3-1.9.0/tests/test_b3_format.py` & `opentelemetry-propagator-b3-1.9.1/tests/test_b3_format.py`

 * *Files identical despite different names*

