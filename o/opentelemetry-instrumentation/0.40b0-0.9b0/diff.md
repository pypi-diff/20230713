# Comparing `tmp/opentelemetry_instrumentation-0.40b0.tar.gz` & `tmp/opentelemetry-instrumentation-0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-instrumentation-0.9b0.tar", last modified: Thu Jun 11 04:39:20 2020, max compression
```

## Comparing `opentelemetry_instrumentation-0.40b0.tar` & `opentelemetry-instrumentation-0.9b0.tar`

### file list

```diff
@@ -1,28 +1,24 @@
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/bootstrap.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/bootstrap_gen.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/dependencies.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/distro.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/environment_variables.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/instrumentor.py
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/propagators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/py.typed
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/sqlcommenter_utils.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/version.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/auto_instrumentation/__init__.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/auto_instrumentation/_load.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/auto_instrumentation/sitecustomize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/__init__.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/test_bootstrap.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/test_dependencies.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/test_distro.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/test_instrumentor.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/test_propagators.py
--rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/test_utils.py
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/auto_instrumentation/test_load.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/tests/auto_instrumentation/test_run.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/LICENSE
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/README.rst
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/pyproject.toml
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 opentelemetry_instrumentation-0.40b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/
+-rw-r--r--   0 runner    (1001) docker     (116)      132 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1493 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      371 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1347 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      898 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (116)     1455 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1552 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/auto_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6443 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3255 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/instrumentor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2611 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      607 2020-06-11 04:39:17.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1493 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      781 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2020-06-11 04:39:20.000000 opentelemetry-instrumentation-0.9b0/src/opentelemetry_instrumentation.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `opentelemetry_instrumentation-0.40b0/src/opentelemetry/instrumentation/version.py` & `opentelemetry-instrumentation-0.9b0/src/opentelemetry/instrumentation/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.40b0"
+__version__ = "0.9b0"
```

