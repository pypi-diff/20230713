# Comparing `tmp/opentelemetry-exporter-otlp-proto-grpc-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-otlp-proto-grpc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-otlp-proto-grpc-1.9.0.tar", last modified: Wed Jan 26 18:29:17 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-otlp-proto-grpc-1.9.1.tar", last modified: Mon Jan 31 10:09:50 2022, max compression
```

## Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0.tar` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/_log_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)     6183 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/_log_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/_metric_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/_metric_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10932 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/trace_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)    11782 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/trace_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/fixtures/test.cert
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/logs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19656 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/logs/test_otlp_logs_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21067 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/metrics/test_otlp_metrics_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/performance/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:17.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/performance/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/performance/benchmarks/test_benchmark_trace_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/test_otlp_exporter_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    36988 2022-01-26 18:29:09.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/test_otlp_trace_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/_log_exporter/
+-rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/_log_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/_metric_exporter/
+-rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/_metric_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10932 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/trace_exporter/
+-rw-r--r--   0 runner    (1001) docker     (121)    11485 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/trace_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/fixtures/test.cert
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/logs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19684 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/logs/test_otlp_logs_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21067 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/metrics/test_otlp_metrics_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/performance/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:50.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/performance/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/performance/benchmarks/test_benchmark_trace_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/test_otlp_exporter_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36687 2022-01-31 10:09:42.000000 opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/test_otlp_trace_exporter.py
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/LICENSE` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/PKG-INFO` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp-proto-grpc
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Collector Protobuf over gRPC Exporter
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-grpc
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/README.rst` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/setup.cfg` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	=src
 packages = find_namespace:
 install_requires = 
 	grpcio >= 1.0.0, < 2.0.0
 	googleapis-common-protos ~= 1.52
 	opentelemetry-api ~= 1.3
 	opentelemetry-sdk ~= 1.3
-	opentelemetry-proto == 1.9.0
+	opentelemetry-proto == 1.9.1
 	backoff ~= 1.10.0
 
 [options.extras_require]
 test = 
 	pytest-grpc
 
 [options.packages.find]
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/setup.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/__init__.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/_log_exporter/__init__.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/_log_exporter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 log_data.log_record.attributes
             )
 
             self._collector_kwargs[
                 "severity_number"
             ] = log_data.log_record.severity_number.value
 
-            instrumentation_library_logs.logs.append(
+            instrumentation_library_logs.log_records.append(
                 PB2LogRecord(**self._collector_kwargs)
             )
 
         return ExportLogsServiceRequest(
             resource_logs=get_resource_data(
                 sdk_resource_instrumentation_library_logs,
                 ResourceLogs,
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/_metric_exporter/__init__.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/_metric_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/exporter.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/trace_exporter/__init__.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/trace_exporter/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     OTEL_EXPORTER_OTLP_TRACES_ENDPOINT,
     OTEL_EXPORTER_OTLP_TRACES_HEADERS,
     OTEL_EXPORTER_OTLP_TRACES_INSECURE,
     OTEL_EXPORTER_OTLP_TRACES_TIMEOUT,
 )
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
-from opentelemetry.trace import StatusCode
 
 logger = logging.getLogger(__name__)
 
 
 # pylint: disable=no-member
 class OTLPSpanExporter(
     SpanExporter,
@@ -204,19 +203,15 @@
                         logger.exception(error)
 
                 self._collector_kwargs["links"].append(collector_span_link)
 
     def _translate_status(self, sdk_span: ReadableSpan) -> None:
         # pylint: disable=no-member
         if sdk_span.status is not None:
-            deprecated_code = Status.DEPRECATED_STATUS_CODE_OK
-            if sdk_span.status.status_code == StatusCode.ERROR:
-                deprecated_code = Status.DEPRECATED_STATUS_CODE_UNKNOWN_ERROR
             self._collector_kwargs["status"] = Status(
-                deprecated_code=deprecated_code,
                 code=sdk_span.status.status_code.value,
                 message=sdk_span.status.description,
             )
 
     def _translate_data(
         self, data: Sequence[ReadableSpan]
     ) -> ExportTraceServiceRequest:
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry/exporter/otlp/proto/grpc/version.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry/exporter/otlp/proto/grpc/version.py`

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

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/PKG-INFO` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-otlp-proto-grpc
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Collector Protobuf over gRPC Exporter
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-otlp-proto-grpc
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/SOURCES.txt` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/src/opentelemetry_exporter_otlp_proto_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/logs/test_otlp_logs_exporter.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/logs/test_otlp_logs_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
                         ]
                     ),
                     instrumentation_library_logs=[
                         InstrumentationLibraryLogs(
                             instrumentation_library=InstrumentationLibrary(
                                 name="first_name", version="first_version"
                             ),
-                            logs=[
+                            log_records=[
                                 PB2LogRecord(
                                     # pylint: disable=no-member
                                     name="name",
                                     time_unix_nano=self.log_data_1.log_record.timestamp,
                                     severity_number=self.log_data_1.log_record.severity_number.value,
                                     severity_text="WARNING",
                                     span_id=int.to_bytes(
@@ -368,15 +368,15 @@
                         ]
                     ),
                     instrumentation_library_logs=[
                         InstrumentationLibraryLogs(
                             instrumentation_library=InstrumentationLibrary(
                                 name="first_name", version="first_version"
                             ),
-                            logs=[
+                            log_records=[
                                 PB2LogRecord(
                                     # pylint: disable=no-member
                                     name="name",
                                     time_unix_nano=self.log_data_1.log_record.timestamp,
                                     severity_number=self.log_data_1.log_record.severity_number.value,
                                     severity_text="WARNING",
                                     span_id=int.to_bytes(
@@ -406,15 +406,15 @@
                                 )
                             ],
                         ),
                         InstrumentationLibraryLogs(
                             instrumentation_library=InstrumentationLibrary(
                                 name="second_name", version="second_version"
                             ),
-                            logs=[
+                            log_records=[
                                 PB2LogRecord(
                                     # pylint: disable=no-member
                                     name="info name",
                                     time_unix_nano=self.log_data_2.log_record.timestamp,
                                     severity_number=self.log_data_2.log_record.severity_number.value,
                                     severity_text="INFO",
                                     span_id=int.to_bytes(
@@ -452,15 +452,15 @@
                         ]
                     ),
                     instrumentation_library_logs=[
                         InstrumentationLibraryLogs(
                             instrumentation_library=InstrumentationLibrary(
                                 name="third_name", version="third_version"
                             ),
-                            logs=[
+                            log_records=[
                                 PB2LogRecord(
                                     # pylint: disable=no-member
                                     name="error name",
                                     time_unix_nano=self.log_data_3.log_record.timestamp,
                                     severity_number=self.log_data_3.log_record.severity_number.value,
                                     severity_text="ERROR",
                                     span_id=int.to_bytes(
```

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/metrics/test_otlp_metrics_exporter.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/metrics/test_otlp_metrics_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/performance/benchmarks/test_benchmark_trace_exporter.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/performance/benchmarks/test_benchmark_trace_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/test_otlp_exporter_mixin.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/test_otlp_exporter_mixin.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-otlp-proto-grpc-1.9.0/tests/test_otlp_trace_exporter.py` & `opentelemetry-exporter-otlp-proto-grpc-1.9.1/tests/test_otlp_trace_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -758,31 +758,26 @@
             self.exporter._translate_data([self.span, self.span2, self.span3]),
         )
 
     def _check_translated_status(
         self,
         translated: ExportTraceServiceRequest,
         code_expected: Status,
-        deprecated_code_expected: Status,
     ):
         status = (
             translated.resource_spans[0]
             .instrumentation_library_spans[0]
             .spans[0]
             .status
         )
 
         self.assertEqual(
             status.code,
             code_expected,
         )
-        self.assertEqual(
-            status.deprecated_code,
-            deprecated_code_expected,
-        )
 
     def test_span_status_translate(self):
         # pylint: disable=protected-access,no-member
         unset = SDKStatus(status_code=SDKStatusCode.UNSET)
         ok = SDKStatus(status_code=SDKStatusCode.OK)
         error = SDKStatus(status_code=SDKStatusCode.ERROR)
         unset_translated = self.exporter._translate_data(
@@ -793,25 +788,22 @@
         )
         error_translated = self.exporter._translate_data(
             [_create_span_with_status(error)]
         )
         self._check_translated_status(
             unset_translated,
             Status.STATUS_CODE_UNSET,
-            Status.DEPRECATED_STATUS_CODE_OK,
         )
         self._check_translated_status(
             ok_translated,
             Status.STATUS_CODE_OK,
-            Status.DEPRECATED_STATUS_CODE_OK,
         )
         self._check_translated_status(
             error_translated,
             Status.STATUS_CODE_ERROR,
-            Status.DEPRECATED_STATUS_CODE_UNKNOWN_ERROR,
         )
 
     # pylint:disable=no-member
     def test_translate_key_values(self):
         bool_value = _translate_key_values("bool_type", False)
         self.assertTrue(isinstance(bool_value, KeyValue))
         self.assertEqual(bool_value.key, "bool_type")
```

