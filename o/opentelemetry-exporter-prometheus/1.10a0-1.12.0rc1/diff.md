# Comparing `tmp/opentelemetry-exporter-prometheus-1.10a0.tar.gz` & `tmp/opentelemetry-exporter-prometheus-1.12.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-prometheus-1.10a0.tar", last modified: Wed Apr  7 16:18:17 2021, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-prometheus-1.12.0rc1.tar", last modified: Tue May 17 20:52:38 2022, max compression
```

## Comparing `opentelemetry-exporter-prometheus-1.10a0.tar` & `opentelemetry-exporter-prometheus-1.12.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      651 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      903 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry/exporter/prometheus/
--rw-r--r--   0 runner    (1001) docker     (121)     6673 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry/exporter/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry/exporter/prometheus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-07 16:18:17.000000 opentelemetry-exporter-prometheus-1.10a0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6648 2021-04-07 16:18:13.000000 opentelemetry-exporter-prometheus-1.10a0/tests/test_prometheus_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:38.000000 opentelemetry-exporter-prometheus-1.12.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-05-17 20:52:38.000000 opentelemetry-exporter-prometheus-1.12.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-05-17 20:52:38.000000 opentelemetry-exporter-prometheus-1.12.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:38.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry/exporter/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (121)    10936 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry/exporter/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry/exporter/prometheus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:38.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-17 20:52:37.000000 opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 20:52:38.000000 opentelemetry-exporter-prometheus-1.12.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10591 2022-05-17 20:52:16.000000 opentelemetry-exporter-prometheus-1.12.0rc1/tests/test_prometheus_exporter.py
```

### Comparing `opentelemetry-exporter-prometheus-1.10a0/LICENSE` & `opentelemetry-exporter-prometheus-1.12.0rc1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright The OpenTelemetry Authors
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `opentelemetry-exporter-prometheus-1.10a0/README.rst` & `opentelemetry-exporter-prometheus-1.12.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-prometheus-1.10a0/setup.cfg` & `opentelemetry-exporter-prometheus-1.12.0rc1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,42 @@
 long_description_content_type = text/x-rst
 author = OpenTelemetry Authors
 author_email = cncf-opentelemetry-contributors@lists.cncf.io
 url = https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-prometheus
 platforms = any
 license = Apache-2.0
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 python_requires = >=3.6
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
 	prometheus_client >= 0.5.0, < 1.0.0
-	opentelemetry-api == 1.10a0
-	opentelemetry-sdk == 1.10a0
+	opentelemetry-api >= 1.10.0
+	opentelemetry-sdk >= 1.10.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
 
 [options.entry_points]
-opentelemetry_exporter = 
-	prometheus = opentelemetry.exporter.prometheus:PrometheusMetricsExporter
+opentelemetry_metric_reader = 
+	prometheus = opentelemetry.exporter.prometheus:PrometheusMetricReader
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `opentelemetry-exporter-prometheus-1.10a0/setup.py` & `opentelemetry-exporter-prometheus-1.12.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 import setuptools
 
-BASE_DIR = os.path.dirname(__file__)
-VERSION_FILENAME = os.path.join(
-    BASE_DIR, "src", "opentelemetry", "exporter", "prometheus", "version.py"
+_BASE_DIR = os.path.dirname(__file__)
+_VERSION_FILENAME = os.path.join(
+    _BASE_DIR, "src", "opentelemetry", "exporter", "prometheus", "version.py"
 )
-PACKAGE_INFO = {}
-with open(VERSION_FILENAME) as f:
-    exec(f.read(), PACKAGE_INFO)
+_PACKAGE_INFO = {}
+with open(_VERSION_FILENAME, encoding="utf-8") as f:
+    exec(f.read(), _PACKAGE_INFO)
 
-setuptools.setup(version=PACKAGE_INFO["__version__"])
+setuptools.setup(version=_PACKAGE_INFO["__version__"])
```

### Comparing `opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry/exporter/prometheus/version.py` & `opentelemetry-exporter-prometheus-1.12.0rc1/tests/__init__.py`

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
-__version__ = "1.10a0"
```

### Comparing `opentelemetry-exporter-prometheus-1.10a0/src/opentelemetry_exporter_prometheus.egg-info/SOURCES.txt` & `opentelemetry-exporter-prometheus-1.12.0rc1/src/opentelemetry_exporter_prometheus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

