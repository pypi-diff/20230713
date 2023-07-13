# Comparing `tmp/opentelemetry-proto-1.9.0.tar.gz` & `tmp/opentelemetry-proto-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-proto-1.9.0.tar", last modified: Wed Jan 26 18:29:16 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-proto-1.9.1.tar", last modified: Mon Jan 31 10:09:48 2022, max compression
```

## Comparing `opentelemetry-proto-1.9.0.tar` & `opentelemetry-proto-1.9.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/
--rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5305 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15691 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     6630 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/v1/common_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/logs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/logs/v1/
--rw-r--r--   0 runner    (1001) docker     (121)    21545 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/logs/v1/logs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11848 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/logs/v1/logs_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)    13516 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7070 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    66421 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/v1/metrics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    55614 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/v1/metrics_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/v1/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/v1/resource_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    32574 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    26648 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/src/opentelemetry/proto/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-proto-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-01-26 18:29:09.000000 opentelemetry-proto-1.9.0/tests/test_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5305 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15691 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6630 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/v1/common_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/logs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/logs/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)    22974 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/logs/v1/logs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/logs/v1/logs_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)    13516 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7070 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58778 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/v1/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49399 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/v1/metrics_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/v1/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/v1/resource_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    28348 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22640 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/src/opentelemetry/proto/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-proto-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-01-31 10:09:42.000000 opentelemetry-proto-1.9.1/tests/test_proto.py
```

### Comparing `opentelemetry-proto-1.9.0/LICENSE` & `opentelemetry-proto-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/PKG-INFO` & `opentelemetry-proto-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-proto
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Python Proto
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-proto
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-proto-1.9.0/README.rst` & `opentelemetry-proto-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/setup.cfg` & `opentelemetry-proto-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/setup.py` & `opentelemetry-proto-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2_grpc.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/logs/v1/logs_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2_grpc.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/metrics/v1/metrics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2_grpc.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/collector/trace/v1/trace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/v1/common_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/common/v1/common_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/common/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/logs/v1/logs_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/logs/v1/logs_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='opentelemetry/proto/logs/v1/logs.proto',
   package='opentelemetry.proto.logs.v1',
   syntax='proto3',
   serialized_options=b'\n\036io.opentelemetry.proto.logs.v1B\tLogsProtoP\001Z<github.com/open-telemetry/opentelemetry-proto/gen/go/logs/v1',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n&opentelemetry/proto/logs/v1/logs.proto\x12\x1bopentelemetry.proto.logs.v1\x1a*opentelemetry/proto/common/v1/common.proto\x1a.opentelemetry/proto/resource/v1/resource.proto\"\xbe\x01\n\x0cResourceLogs\x12;\n\x08resource\x18\x01 \x01(\x0b\x32).opentelemetry.proto.resource.v1.Resource\x12]\n\x1cinstrumentation_library_logs\x18\x02 \x03(\x0b\x32\x37.opentelemetry.proto.logs.v1.InstrumentationLibraryLogs\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xbe\x01\n\x1aInstrumentationLibraryLogs\x12V\n\x17instrumentation_library\x18\x01 \x01(\x0b\x32\x35.opentelemetry.proto.common.v1.InstrumentationLibrary\x12\x34\n\x04logs\x18\x02 \x03(\x0b\x32&.opentelemetry.proto.logs.v1.LogRecord\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xd6\x02\n\tLogRecord\x12\x16\n\x0etime_unix_nano\x18\x01 \x01(\x06\x12\x44\n\x0fseverity_number\x18\x02 \x01(\x0e\x32+.opentelemetry.proto.logs.v1.SeverityNumber\x12\x15\n\rseverity_text\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x35\n\x04\x62ody\x18\x05 \x01(\x0b\x32\'.opentelemetry.proto.common.v1.AnyValue\x12;\n\nattributes\x18\x06 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x07 \x01(\r\x12\r\n\x05\x66lags\x18\x08 \x01(\x07\x12\x10\n\x08trace_id\x18\t \x01(\x0c\x12\x0f\n\x07span_id\x18\n \x01(\x0c*\xc3\x05\n\x0eSeverityNumber\x12\x1f\n\x1bSEVERITY_NUMBER_UNSPECIFIED\x10\x00\x12\x19\n\x15SEVERITY_NUMBER_TRACE\x10\x01\x12\x1a\n\x16SEVERITY_NUMBER_TRACE2\x10\x02\x12\x1a\n\x16SEVERITY_NUMBER_TRACE3\x10\x03\x12\x1a\n\x16SEVERITY_NUMBER_TRACE4\x10\x04\x12\x19\n\x15SEVERITY_NUMBER_DEBUG\x10\x05\x12\x1a\n\x16SEVERITY_NUMBER_DEBUG2\x10\x06\x12\x1a\n\x16SEVERITY_NUMBER_DEBUG3\x10\x07\x12\x1a\n\x16SEVERITY_NUMBER_DEBUG4\x10\x08\x12\x18\n\x14SEVERITY_NUMBER_INFO\x10\t\x12\x19\n\x15SEVERITY_NUMBER_INFO2\x10\n\x12\x19\n\x15SEVERITY_NUMBER_INFO3\x10\x0b\x12\x19\n\x15SEVERITY_NUMBER_INFO4\x10\x0c\x12\x18\n\x14SEVERITY_NUMBER_WARN\x10\r\x12\x19\n\x15SEVERITY_NUMBER_WARN2\x10\x0e\x12\x19\n\x15SEVERITY_NUMBER_WARN3\x10\x0f\x12\x19\n\x15SEVERITY_NUMBER_WARN4\x10\x10\x12\x19\n\x15SEVERITY_NUMBER_ERROR\x10\x11\x12\x1a\n\x16SEVERITY_NUMBER_ERROR2\x10\x12\x12\x1a\n\x16SEVERITY_NUMBER_ERROR3\x10\x13\x12\x1a\n\x16SEVERITY_NUMBER_ERROR4\x10\x14\x12\x19\n\x15SEVERITY_NUMBER_FATAL\x10\x15\x12\x1a\n\x16SEVERITY_NUMBER_FATAL2\x10\x16\x12\x1a\n\x16SEVERITY_NUMBER_FATAL3\x10\x17\x12\x1a\n\x16SEVERITY_NUMBER_FATAL4\x10\x18*X\n\x0eLogRecordFlags\x12\x1f\n\x1bLOG_RECORD_FLAG_UNSPECIFIED\x10\x00\x12%\n LOG_RECORD_FLAG_TRACE_FLAGS_MASK\x10\xff\x01\x42k\n\x1eio.opentelemetry.proto.logs.v1B\tLogsProtoP\x01Z<github.com/open-telemetry/opentelemetry-proto/gen/go/logs/v1b\x06proto3'
+  serialized_pb=b'\n&opentelemetry/proto/logs/v1/logs.proto\x12\x1bopentelemetry.proto.logs.v1\x1a*opentelemetry/proto/common/v1/common.proto\x1a.opentelemetry/proto/resource/v1/resource.proto\"L\n\x08LogsData\x12@\n\rresource_logs\x18\x01 \x03(\x0b\x32).opentelemetry.proto.logs.v1.ResourceLogs\"\xbe\x01\n\x0cResourceLogs\x12;\n\x08resource\x18\x01 \x01(\x0b\x32).opentelemetry.proto.resource.v1.Resource\x12]\n\x1cinstrumentation_library_logs\x18\x02 \x03(\x0b\x32\x37.opentelemetry.proto.logs.v1.InstrumentationLibraryLogs\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xc5\x01\n\x1aInstrumentationLibraryLogs\x12V\n\x17instrumentation_library\x18\x01 \x01(\x0b\x32\x35.opentelemetry.proto.common.v1.InstrumentationLibrary\x12;\n\x0blog_records\x18\x02 \x03(\x0b\x32&.opentelemetry.proto.logs.v1.LogRecord\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xd6\x02\n\tLogRecord\x12\x16\n\x0etime_unix_nano\x18\x01 \x01(\x06\x12\x44\n\x0fseverity_number\x18\x02 \x01(\x0e\x32+.opentelemetry.proto.logs.v1.SeverityNumber\x12\x15\n\rseverity_text\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x35\n\x04\x62ody\x18\x05 \x01(\x0b\x32\'.opentelemetry.proto.common.v1.AnyValue\x12;\n\nattributes\x18\x06 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x07 \x01(\r\x12\r\n\x05\x66lags\x18\x08 \x01(\x07\x12\x10\n\x08trace_id\x18\t \x01(\x0c\x12\x0f\n\x07span_id\x18\n \x01(\x0c*\xc3\x05\n\x0eSeverityNumber\x12\x1f\n\x1bSEVERITY_NUMBER_UNSPECIFIED\x10\x00\x12\x19\n\x15SEVERITY_NUMBER_TRACE\x10\x01\x12\x1a\n\x16SEVERITY_NUMBER_TRACE2\x10\x02\x12\x1a\n\x16SEVERITY_NUMBER_TRACE3\x10\x03\x12\x1a\n\x16SEVERITY_NUMBER_TRACE4\x10\x04\x12\x19\n\x15SEVERITY_NUMBER_DEBUG\x10\x05\x12\x1a\n\x16SEVERITY_NUMBER_DEBUG2\x10\x06\x12\x1a\n\x16SEVERITY_NUMBER_DEBUG3\x10\x07\x12\x1a\n\x16SEVERITY_NUMBER_DEBUG4\x10\x08\x12\x18\n\x14SEVERITY_NUMBER_INFO\x10\t\x12\x19\n\x15SEVERITY_NUMBER_INFO2\x10\n\x12\x19\n\x15SEVERITY_NUMBER_INFO3\x10\x0b\x12\x19\n\x15SEVERITY_NUMBER_INFO4\x10\x0c\x12\x18\n\x14SEVERITY_NUMBER_WARN\x10\r\x12\x19\n\x15SEVERITY_NUMBER_WARN2\x10\x0e\x12\x19\n\x15SEVERITY_NUMBER_WARN3\x10\x0f\x12\x19\n\x15SEVERITY_NUMBER_WARN4\x10\x10\x12\x19\n\x15SEVERITY_NUMBER_ERROR\x10\x11\x12\x1a\n\x16SEVERITY_NUMBER_ERROR2\x10\x12\x12\x1a\n\x16SEVERITY_NUMBER_ERROR3\x10\x13\x12\x1a\n\x16SEVERITY_NUMBER_ERROR4\x10\x14\x12\x19\n\x15SEVERITY_NUMBER_FATAL\x10\x15\x12\x1a\n\x16SEVERITY_NUMBER_FATAL2\x10\x16\x12\x1a\n\x16SEVERITY_NUMBER_FATAL3\x10\x17\x12\x1a\n\x16SEVERITY_NUMBER_FATAL4\x10\x18*X\n\x0eLogRecordFlags\x12\x1f\n\x1bLOG_RECORD_FLAG_UNSPECIFIED\x10\x00\x12%\n LOG_RECORD_FLAG_TRACE_FLAGS_MASK\x10\xff\x01\x42k\n\x1eio.opentelemetry.proto.logs.v1B\tLogsProtoP\x01Z<github.com/open-telemetry/opentelemetry-proto/gen/go/logs/v1b\x06proto3'
   ,
   dependencies=[opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2.DESCRIPTOR,opentelemetry_dot_proto_dot_resource_dot_v1_dot_resource__pb2.DESCRIPTOR,])
 
 _SEVERITYNUMBER = _descriptor.EnumDescriptor(
   name='SeverityNumber',
   full_name='opentelemetry.proto.logs.v1.SeverityNumber',
   filename=None,
@@ -157,16 +157,16 @@
       name='SEVERITY_NUMBER_FATAL4', index=24, number=24,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=895,
-  serialized_end=1602,
+  serialized_start=980,
+  serialized_end=1687,
 )
 _sym_db.RegisterEnumDescriptor(_SEVERITYNUMBER)
 
 SeverityNumber = enum_type_wrapper.EnumTypeWrapper(_SEVERITYNUMBER)
 _LOGRECORDFLAGS = _descriptor.EnumDescriptor(
   name='LogRecordFlags',
   full_name='opentelemetry.proto.logs.v1.LogRecordFlags',
@@ -183,16 +183,16 @@
       name='LOG_RECORD_FLAG_TRACE_FLAGS_MASK', index=1, number=255,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1604,
-  serialized_end=1692,
+  serialized_start=1689,
+  serialized_end=1777,
 )
 _sym_db.RegisterEnumDescriptor(_LOGRECORDFLAGS)
 
 LogRecordFlags = enum_type_wrapper.EnumTypeWrapper(_LOGRECORDFLAGS)
 SEVERITY_NUMBER_UNSPECIFIED = 0
 SEVERITY_NUMBER_TRACE = 1
 SEVERITY_NUMBER_TRACE2 = 2
@@ -219,14 +219,46 @@
 SEVERITY_NUMBER_FATAL3 = 23
 SEVERITY_NUMBER_FATAL4 = 24
 LOG_RECORD_FLAG_UNSPECIFIED = 0
 LOG_RECORD_FLAG_TRACE_FLAGS_MASK = 255
 
 
 
+_LOGSDATA = _descriptor.Descriptor(
+  name='LogsData',
+  full_name='opentelemetry.proto.logs.v1.LogsData',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='resource_logs', full_name='opentelemetry.proto.logs.v1.LogsData.resource_logs', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=163,
+  serialized_end=239,
+)
+
+
 _RESOURCELOGS = _descriptor.Descriptor(
   name='ResourceLogs',
   full_name='opentelemetry.proto.logs.v1.ResourceLogs',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -260,16 +292,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=164,
-  serialized_end=354,
+  serialized_start=242,
+  serialized_end=432,
 )
 
 
 _INSTRUMENTATIONLIBRARYLOGS = _descriptor.Descriptor(
   name='InstrumentationLibraryLogs',
   full_name='opentelemetry.proto.logs.v1.InstrumentationLibraryLogs',
   filename=None,
@@ -281,15 +313,15 @@
       name='instrumentation_library', full_name='opentelemetry.proto.logs.v1.InstrumentationLibraryLogs.instrumentation_library', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='logs', full_name='opentelemetry.proto.logs.v1.InstrumentationLibraryLogs.logs', index=1,
+      name='log_records', full_name='opentelemetry.proto.logs.v1.InstrumentationLibraryLogs.log_records', index=1,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='schema_url', full_name='opentelemetry.proto.logs.v1.InstrumentationLibraryLogs.schema_url', index=2,
@@ -306,16 +338,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=357,
-  serialized_end=547,
+  serialized_start=435,
+  serialized_end=632,
 )
 
 
 _LOGRECORD = _descriptor.Descriptor(
   name='LogRecord',
   full_name='opentelemetry.proto.logs.v1.LogRecord',
   filename=None,
@@ -401,32 +433,41 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=550,
-  serialized_end=892,
+  serialized_start=635,
+  serialized_end=977,
 )
 
+_LOGSDATA.fields_by_name['resource_logs'].message_type = _RESOURCELOGS
 _RESOURCELOGS.fields_by_name['resource'].message_type = opentelemetry_dot_proto_dot_resource_dot_v1_dot_resource__pb2._RESOURCE
 _RESOURCELOGS.fields_by_name['instrumentation_library_logs'].message_type = _INSTRUMENTATIONLIBRARYLOGS
 _INSTRUMENTATIONLIBRARYLOGS.fields_by_name['instrumentation_library'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._INSTRUMENTATIONLIBRARY
-_INSTRUMENTATIONLIBRARYLOGS.fields_by_name['logs'].message_type = _LOGRECORD
+_INSTRUMENTATIONLIBRARYLOGS.fields_by_name['log_records'].message_type = _LOGRECORD
 _LOGRECORD.fields_by_name['severity_number'].enum_type = _SEVERITYNUMBER
 _LOGRECORD.fields_by_name['body'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._ANYVALUE
 _LOGRECORD.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
+DESCRIPTOR.message_types_by_name['LogsData'] = _LOGSDATA
 DESCRIPTOR.message_types_by_name['ResourceLogs'] = _RESOURCELOGS
 DESCRIPTOR.message_types_by_name['InstrumentationLibraryLogs'] = _INSTRUMENTATIONLIBRARYLOGS
 DESCRIPTOR.message_types_by_name['LogRecord'] = _LOGRECORD
 DESCRIPTOR.enum_types_by_name['SeverityNumber'] = _SEVERITYNUMBER
 DESCRIPTOR.enum_types_by_name['LogRecordFlags'] = _LOGRECORDFLAGS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+LogsData = _reflection.GeneratedProtocolMessageType('LogsData', (_message.Message,), {
+  'DESCRIPTOR' : _LOGSDATA,
+  '__module__' : 'opentelemetry.proto.logs.v1.logs_pb2'
+  # @@protoc_insertion_point(class_scope:opentelemetry.proto.logs.v1.LogsData)
+  })
+_sym_db.RegisterMessage(LogsData)
+
 ResourceLogs = _reflection.GeneratedProtocolMessageType('ResourceLogs', (_message.Message,), {
   'DESCRIPTOR' : _RESOURCELOGS,
   '__module__' : 'opentelemetry.proto.logs.v1.logs_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.logs.v1.ResourceLogs)
   })
 _sym_db.RegisterMessage(ResourceLogs)
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/logs/v1/logs_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/logs/v1/logs_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -90,14 +90,44 @@
     LOG_RECORD_FLAG_TRACE_FLAGS_MASK = LogRecordFlags.V(255)
 
 LOG_RECORD_FLAG_UNSPECIFIED = LogRecordFlags.V(0)
 LOG_RECORD_FLAG_TRACE_FLAGS_MASK = LogRecordFlags.V(255)
 global___LogRecordFlags = LogRecordFlags
 
 
+class LogsData(google.protobuf.message.Message):
+    """LogsData represents the logs data that can be stored in a persistent storage,
+    OR can be embedded by other protocols that transfer OTLP logs data but do not
+    implement the OTLP protocol.
+
+    The main difference between this message and collector protocol is that
+    in this message there will not be any "control" or "metadata" specific to
+    OTLP protocol.
+
+    When new fields are added into this message, the OTLP request MUST be updated
+    as well.
+    """
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    RESOURCE_LOGS_FIELD_NUMBER: builtins.int
+    @property
+    def resource_logs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceLogs]:
+        """An array of ResourceLogs.
+        For data coming from a single resource this array will typically contain
+        one element. Intermediary nodes that receive data from multiple origins
+        typically batch the data before forwarding further and in that case this
+        array will contain multiple elements.
+        """
+        pass
+    def __init__(self,
+        *,
+        resource_logs : typing.Optional[typing.Iterable[global___ResourceLogs]] = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resource_logs",b"resource_logs"]) -> None: ...
+global___LogsData = LogsData
+
 class ResourceLogs(google.protobuf.message.Message):
     """A collection of InstrumentationLibraryLogs from a Resource."""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     RESOURCE_FIELD_NUMBER: builtins.int
     INSTRUMENTATION_LIBRARY_LOGS_FIELD_NUMBER: builtins.int
     SCHEMA_URL_FIELD_NUMBER: builtins.int
     @property
@@ -126,38 +156,38 @@
     def ClearField(self, field_name: typing_extensions.Literal["instrumentation_library_logs",b"instrumentation_library_logs","resource",b"resource","schema_url",b"schema_url"]) -> None: ...
 global___ResourceLogs = ResourceLogs
 
 class InstrumentationLibraryLogs(google.protobuf.message.Message):
     """A collection of Logs produced by an InstrumentationLibrary."""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     INSTRUMENTATION_LIBRARY_FIELD_NUMBER: builtins.int
-    LOGS_FIELD_NUMBER: builtins.int
+    LOG_RECORDS_FIELD_NUMBER: builtins.int
     SCHEMA_URL_FIELD_NUMBER: builtins.int
     @property
     def instrumentation_library(self) -> opentelemetry.proto.common.v1.common_pb2.InstrumentationLibrary:
         """The instrumentation library information for the logs in this message.
         Semantically when InstrumentationLibrary isn't set, it is equivalent with
         an empty instrumentation library name (unknown).
         """
         pass
     @property
-    def logs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LogRecord]:
+    def log_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LogRecord]:
         """A list of log records."""
         pass
     schema_url: typing.Text = ...
     """This schema_url applies to all logs in the "logs" field."""
 
     def __init__(self,
         *,
         instrumentation_library : typing.Optional[opentelemetry.proto.common.v1.common_pb2.InstrumentationLibrary] = ...,
-        logs : typing.Optional[typing.Iterable[global___LogRecord]] = ...,
+        log_records : typing.Optional[typing.Iterable[global___LogRecord]] = ...,
         schema_url : typing.Text = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["instrumentation_library",b"instrumentation_library"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instrumentation_library",b"instrumentation_library","logs",b"logs","schema_url",b"schema_url"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instrumentation_library",b"instrumentation_library","log_records",b"log_records","schema_url",b"schema_url"]) -> None: ...
 global___InstrumentationLibraryLogs = InstrumentationLibraryLogs
 
 class LogRecord(google.protobuf.message.Message):
     """A log record according to OpenTelemetry Log Data Model:
     https://github.com/open-telemetry/oteps/blob/main/text/logs/0097-log-data-model.md
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2_grpc.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/experimental/metrics_config_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/v1/metrics_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/v1/metrics_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='opentelemetry/proto/metrics/v1/metrics.proto',
   package='opentelemetry.proto.metrics.v1',
   syntax='proto3',
   serialized_options=b'\n!io.opentelemetry.proto.metrics.v1B\014MetricsProtoP\001Z?github.com/open-telemetry/opentelemetry-proto/gen/go/metrics/v1',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n,opentelemetry/proto/metrics/v1/metrics.proto\x12\x1eopentelemetry.proto.metrics.v1\x1a*opentelemetry/proto/common/v1/common.proto\x1a.opentelemetry/proto/resource/v1/resource.proto\"\xca\x01\n\x0fResourceMetrics\x12;\n\x08resource\x18\x01 \x01(\x0b\x32).opentelemetry.proto.resource.v1.Resource\x12\x66\n\x1finstrumentation_library_metrics\x18\x02 \x03(\x0b\x32=.opentelemetry.proto.metrics.v1.InstrumentationLibraryMetrics\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xc4\x01\n\x1dInstrumentationLibraryMetrics\x12V\n\x17instrumentation_library\x18\x01 \x01(\x0b\x32\x35.opentelemetry.proto.common.v1.InstrumentationLibrary\x12\x37\n\x07metrics\x18\x02 \x03(\x0b\x32&.opentelemetry.proto.metrics.v1.Metric\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xf6\x03\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\x12\x41\n\tint_gauge\x18\x04 \x01(\x0b\x32(.opentelemetry.proto.metrics.v1.IntGaugeB\x02\x18\x01H\x00\x12\x36\n\x05gauge\x18\x05 \x01(\x0b\x32%.opentelemetry.proto.metrics.v1.GaugeH\x00\x12=\n\x07int_sum\x18\x06 \x01(\x0b\x32&.opentelemetry.proto.metrics.v1.IntSumB\x02\x18\x01H\x00\x12\x32\n\x03sum\x18\x07 \x01(\x0b\x32#.opentelemetry.proto.metrics.v1.SumH\x00\x12I\n\rint_histogram\x18\x08 \x01(\x0b\x32,.opentelemetry.proto.metrics.v1.IntHistogramB\x02\x18\x01H\x00\x12>\n\thistogram\x18\t \x01(\x0b\x32).opentelemetry.proto.metrics.v1.HistogramH\x00\x12:\n\x07summary\x18\x0b \x01(\x0b\x32\'.opentelemetry.proto.metrics.v1.SummaryH\x00\x42\x06\n\x04\x64\x61ta\"Q\n\x08IntGauge\x12\x41\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32,.opentelemetry.proto.metrics.v1.IntDataPoint:\x02\x18\x01\"M\n\x05Gauge\x12\x44\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32/.opentelemetry.proto.metrics.v1.NumberDataPoint\"\xbe\x01\n\x06IntSum\x12\x41\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32,.opentelemetry.proto.metrics.v1.IntDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality\x12\x14\n\x0cis_monotonic\x18\x03 \x01(\x08:\x02\x18\x01\"\xba\x01\n\x03Sum\x12\x44\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32/.opentelemetry.proto.metrics.v1.NumberDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality\x12\x14\n\x0cis_monotonic\x18\x03 \x01(\x08\"\xb7\x01\n\x0cIntHistogram\x12J\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32\x35.opentelemetry.proto.metrics.v1.IntHistogramDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality:\x02\x18\x01\"\xad\x01\n\tHistogram\x12G\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32\x32.opentelemetry.proto.metrics.v1.HistogramDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality\"P\n\x07Summary\x12\x45\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32\x30.opentelemetry.proto.metrics.v1.SummaryDataPoint\"\xd6\x01\n\x0cIntDataPoint\x12=\n\x06labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValue\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05value\x18\x04 \x01(\x10\x12>\n\texemplars\x18\x05 \x03(\x0b\x32+.opentelemetry.proto.metrics.v1.IntExemplar:\x02\x18\x01\"\xb4\x02\n\x0fNumberDataPoint\x12;\n\nattributes\x18\x07 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x41\n\x06labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValueB\x02\x18\x01\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\x13\n\tas_double\x18\x04 \x01(\x01H\x00\x12\x10\n\x06\x61s_int\x18\x06 \x01(\x10H\x00\x12;\n\texemplars\x18\x05 \x03(\x0b\x32(.opentelemetry.proto.metrics.v1.ExemplarB\x07\n\x05value\"\x9c\x02\n\x15IntHistogramDataPoint\x12=\n\x06labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValue\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05\x63ount\x18\x04 \x01(\x06\x12\x0b\n\x03sum\x18\x05 \x01(\x10\x12\x15\n\rbucket_counts\x18\x06 \x03(\x06\x12\x17\n\x0f\x65xplicit_bounds\x18\x07 \x03(\x01\x12>\n\texemplars\x18\x08 \x03(\x0b\x32+.opentelemetry.proto.metrics.v1.IntExemplar:\x02\x18\x01\"\xd3\x02\n\x12HistogramDataPoint\x12;\n\nattributes\x18\t \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x41\n\x06labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValueB\x02\x18\x01\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05\x63ount\x18\x04 \x01(\x06\x12\x0b\n\x03sum\x18\x05 \x01(\x01\x12\x15\n\rbucket_counts\x18\x06 \x03(\x06\x12\x17\n\x0f\x65xplicit_bounds\x18\x07 \x03(\x01\x12;\n\texemplars\x18\x08 \x03(\x0b\x32(.opentelemetry.proto.metrics.v1.Exemplar\"\xf3\x02\n\x10SummaryDataPoint\x12;\n\nattributes\x18\x07 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x41\n\x06labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValueB\x02\x18\x01\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05\x63ount\x18\x04 \x01(\x06\x12\x0b\n\x03sum\x18\x05 \x01(\x01\x12Y\n\x0fquantile_values\x18\x06 \x03(\x0b\x32@.opentelemetry.proto.metrics.v1.SummaryDataPoint.ValueAtQuantile\x1a\x32\n\x0fValueAtQuantile\x12\x10\n\x08quantile\x18\x01 \x01(\x01\x12\r\n\x05value\x18\x02 \x01(\x01\"\xa3\x01\n\x0bIntExemplar\x12\x46\n\x0f\x66iltered_labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValue\x12\x16\n\x0etime_unix_nano\x18\x02 \x01(\x06\x12\r\n\x05value\x18\x03 \x01(\x10\x12\x0f\n\x07span_id\x18\x04 \x01(\x0c\x12\x10\n\x08trace_id\x18\x05 \x01(\x0c:\x02\x18\x01\"\x87\x02\n\x08\x45xemplar\x12\x44\n\x13\x66iltered_attributes\x18\x07 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12J\n\x0f\x66iltered_labels\x18\x01 \x03(\x0b\x32-.opentelemetry.proto.common.v1.StringKeyValueB\x02\x18\x01\x12\x16\n\x0etime_unix_nano\x18\x02 \x01(\x06\x12\x13\n\tas_double\x18\x03 \x01(\x01H\x00\x12\x10\n\x06\x61s_int\x18\x06 \x01(\x10H\x00\x12\x0f\n\x07span_id\x18\x04 \x01(\x0c\x12\x10\n\x08trace_id\x18\x05 \x01(\x0c\x42\x07\n\x05value*\x8c\x01\n\x16\x41ggregationTemporality\x12\'\n#AGGREGATION_TEMPORALITY_UNSPECIFIED\x10\x00\x12!\n\x1d\x41GGREGATION_TEMPORALITY_DELTA\x10\x01\x12&\n\"AGGREGATION_TEMPORALITY_CUMULATIVE\x10\x02\x42t\n!io.opentelemetry.proto.metrics.v1B\x0cMetricsProtoP\x01Z?github.com/open-telemetry/opentelemetry-proto/gen/go/metrics/v1b\x06proto3'
+  serialized_pb=b'\n,opentelemetry/proto/metrics/v1/metrics.proto\x12\x1eopentelemetry.proto.metrics.v1\x1a*opentelemetry/proto/common/v1/common.proto\x1a.opentelemetry/proto/resource/v1/resource.proto\"X\n\x0bMetricsData\x12I\n\x10resource_metrics\x18\x01 \x03(\x0b\x32/.opentelemetry.proto.metrics.v1.ResourceMetrics\"\xca\x01\n\x0fResourceMetrics\x12;\n\x08resource\x18\x01 \x01(\x0b\x32).opentelemetry.proto.resource.v1.Resource\x12\x66\n\x1finstrumentation_library_metrics\x18\x02 \x03(\x0b\x32=.opentelemetry.proto.metrics.v1.InstrumentationLibraryMetrics\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xc4\x01\n\x1dInstrumentationLibraryMetrics\x12V\n\x17instrumentation_library\x18\x01 \x01(\x0b\x32\x35.opentelemetry.proto.common.v1.InstrumentationLibrary\x12\x37\n\x07metrics\x18\x02 \x03(\x0b\x32&.opentelemetry.proto.metrics.v1.Metric\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\x92\x03\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\x12\x36\n\x05gauge\x18\x05 \x01(\x0b\x32%.opentelemetry.proto.metrics.v1.GaugeH\x00\x12\x32\n\x03sum\x18\x07 \x01(\x0b\x32#.opentelemetry.proto.metrics.v1.SumH\x00\x12>\n\thistogram\x18\t \x01(\x0b\x32).opentelemetry.proto.metrics.v1.HistogramH\x00\x12U\n\x15\x65xponential_histogram\x18\n \x01(\x0b\x32\x34.opentelemetry.proto.metrics.v1.ExponentialHistogramH\x00\x12:\n\x07summary\x18\x0b \x01(\x0b\x32\'.opentelemetry.proto.metrics.v1.SummaryH\x00\x42\x06\n\x04\x64\x61taJ\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\t\"M\n\x05Gauge\x12\x44\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32/.opentelemetry.proto.metrics.v1.NumberDataPoint\"\xba\x01\n\x03Sum\x12\x44\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32/.opentelemetry.proto.metrics.v1.NumberDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality\x12\x14\n\x0cis_monotonic\x18\x03 \x01(\x08\"\xad\x01\n\tHistogram\x12G\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32\x32.opentelemetry.proto.metrics.v1.HistogramDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality\"\xc3\x01\n\x14\x45xponentialHistogram\x12R\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32=.opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint\x12W\n\x17\x61ggregation_temporality\x18\x02 \x01(\x0e\x32\x36.opentelemetry.proto.metrics.v1.AggregationTemporality\"P\n\x07Summary\x12\x45\n\x0b\x64\x61ta_points\x18\x01 \x03(\x0b\x32\x30.opentelemetry.proto.metrics.v1.SummaryDataPoint\"\x86\x02\n\x0fNumberDataPoint\x12;\n\nattributes\x18\x07 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\x13\n\tas_double\x18\x04 \x01(\x01H\x00\x12\x10\n\x06\x61s_int\x18\x06 \x01(\x10H\x00\x12;\n\texemplars\x18\x05 \x03(\x0b\x32(.opentelemetry.proto.metrics.v1.Exemplar\x12\r\n\x05\x66lags\x18\x08 \x01(\rB\x07\n\x05valueJ\x04\x08\x01\x10\x02\"\xa5\x02\n\x12HistogramDataPoint\x12;\n\nattributes\x18\t \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05\x63ount\x18\x04 \x01(\x06\x12\x0b\n\x03sum\x18\x05 \x01(\x01\x12\x15\n\rbucket_counts\x18\x06 \x03(\x06\x12\x17\n\x0f\x65xplicit_bounds\x18\x07 \x03(\x01\x12;\n\texemplars\x18\x08 \x03(\x0b\x32(.opentelemetry.proto.metrics.v1.Exemplar\x12\r\n\x05\x66lags\x18\n \x01(\rJ\x04\x08\x01\x10\x02\"\x81\x04\n\x1d\x45xponentialHistogramDataPoint\x12;\n\nattributes\x18\x01 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05\x63ount\x18\x04 \x01(\x06\x12\x0b\n\x03sum\x18\x05 \x01(\x01\x12\r\n\x05scale\x18\x06 \x01(\x11\x12\x12\n\nzero_count\x18\x07 \x01(\x06\x12W\n\x08positive\x18\x08 \x01(\x0b\x32\x45.opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.Buckets\x12W\n\x08negative\x18\t \x01(\x0b\x32\x45.opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.Buckets\x12\r\n\x05\x66lags\x18\n \x01(\r\x12;\n\texemplars\x18\x0b \x03(\x0b\x32(.opentelemetry.proto.metrics.v1.Exemplar\x1a\x30\n\x07\x42uckets\x12\x0e\n\x06offset\x18\x01 \x01(\x11\x12\x15\n\rbucket_counts\x18\x02 \x03(\x04\"\xc5\x02\n\x10SummaryDataPoint\x12;\n\nattributes\x18\x07 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x1c\n\x14start_time_unix_nano\x18\x02 \x01(\x06\x12\x16\n\x0etime_unix_nano\x18\x03 \x01(\x06\x12\r\n\x05\x63ount\x18\x04 \x01(\x06\x12\x0b\n\x03sum\x18\x05 \x01(\x01\x12Y\n\x0fquantile_values\x18\x06 \x03(\x0b\x32@.opentelemetry.proto.metrics.v1.SummaryDataPoint.ValueAtQuantile\x12\r\n\x05\x66lags\x18\x08 \x01(\r\x1a\x32\n\x0fValueAtQuantile\x12\x10\n\x08quantile\x18\x01 \x01(\x01\x12\r\n\x05value\x18\x02 \x01(\x01J\x04\x08\x01\x10\x02\"\xc1\x01\n\x08\x45xemplar\x12\x44\n\x13\x66iltered_attributes\x18\x07 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12\x16\n\x0etime_unix_nano\x18\x02 \x01(\x06\x12\x13\n\tas_double\x18\x03 \x01(\x01H\x00\x12\x10\n\x06\x61s_int\x18\x06 \x01(\x10H\x00\x12\x0f\n\x07span_id\x18\x04 \x01(\x0c\x12\x10\n\x08trace_id\x18\x05 \x01(\x0c\x42\x07\n\x05valueJ\x04\x08\x01\x10\x02*\x8c\x01\n\x16\x41ggregationTemporality\x12\'\n#AGGREGATION_TEMPORALITY_UNSPECIFIED\x10\x00\x12!\n\x1d\x41GGREGATION_TEMPORALITY_DELTA\x10\x01\x12&\n\"AGGREGATION_TEMPORALITY_CUMULATIVE\x10\x02*;\n\x0e\x44\x61taPointFlags\x12\r\n\tFLAG_NONE\x10\x00\x12\x1a\n\x16\x46LAG_NO_RECORDED_VALUE\x10\x01\x42t\n!io.opentelemetry.proto.metrics.v1B\x0cMetricsProtoP\x01Z?github.com/open-telemetry/opentelemetry-proto/gen/go/metrics/v1b\x06proto3'
   ,
   dependencies=[opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2.DESCRIPTOR,opentelemetry_dot_proto_dot_resource_dot_v1_dot_resource__pb2.DESCRIPTOR,])
 
 _AGGREGATIONTEMPORALITY = _descriptor.EnumDescriptor(
   name='AggregationTemporality',
   full_name='opentelemetry.proto.metrics.v1.AggregationTemporality',
   filename=None,
@@ -47,24 +47,84 @@
       name='AGGREGATION_TEMPORALITY_CUMULATIVE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=4033,
-  serialized_end=4173,
+  serialized_start=3397,
+  serialized_end=3537,
 )
 _sym_db.RegisterEnumDescriptor(_AGGREGATIONTEMPORALITY)
 
 AggregationTemporality = enum_type_wrapper.EnumTypeWrapper(_AGGREGATIONTEMPORALITY)
+_DATAPOINTFLAGS = _descriptor.EnumDescriptor(
+  name='DataPointFlags',
+  full_name='opentelemetry.proto.metrics.v1.DataPointFlags',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='FLAG_NONE', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='FLAG_NO_RECORDED_VALUE', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=3539,
+  serialized_end=3598,
+)
+_sym_db.RegisterEnumDescriptor(_DATAPOINTFLAGS)
+
+DataPointFlags = enum_type_wrapper.EnumTypeWrapper(_DATAPOINTFLAGS)
 AGGREGATION_TEMPORALITY_UNSPECIFIED = 0
 AGGREGATION_TEMPORALITY_DELTA = 1
 AGGREGATION_TEMPORALITY_CUMULATIVE = 2
+FLAG_NONE = 0
+FLAG_NO_RECORDED_VALUE = 1
+
+
 
+_METRICSDATA = _descriptor.Descriptor(
+  name='MetricsData',
+  full_name='opentelemetry.proto.metrics.v1.MetricsData',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='resource_metrics', full_name='opentelemetry.proto.metrics.v1.MetricsData.resource_metrics', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=172,
+  serialized_end=260,
+)
 
 
 _RESOURCEMETRICS = _descriptor.Descriptor(
   name='ResourceMetrics',
   full_name='opentelemetry.proto.metrics.v1.ResourceMetrics',
   filename=None,
   file=DESCRIPTOR,
@@ -100,16 +160,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=173,
-  serialized_end=375,
+  serialized_start=263,
+  serialized_end=465,
 )
 
 
 _INSTRUMENTATIONLIBRARYMETRICS = _descriptor.Descriptor(
   name='InstrumentationLibraryMetrics',
   full_name='opentelemetry.proto.metrics.v1.InstrumentationLibraryMetrics',
   filename=None,
@@ -146,16 +206,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=378,
-  serialized_end=574,
+  serialized_start=468,
+  serialized_end=664,
 )
 
 
 _METRIC = _descriptor.Descriptor(
   name='Metric',
   full_name='opentelemetry.proto.metrics.v1.Metric',
   filename=None,
@@ -181,57 +241,43 @@
       name='unit', full_name='opentelemetry.proto.metrics.v1.Metric.unit', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='int_gauge', full_name='opentelemetry.proto.metrics.v1.Metric.int_gauge', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='gauge', full_name='opentelemetry.proto.metrics.v1.Metric.gauge', index=4,
+      name='gauge', full_name='opentelemetry.proto.metrics.v1.Metric.gauge', index=3,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='int_sum', full_name='opentelemetry.proto.metrics.v1.Metric.int_sum', index=5,
-      number=6, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='sum', full_name='opentelemetry.proto.metrics.v1.Metric.sum', index=6,
+      name='sum', full_name='opentelemetry.proto.metrics.v1.Metric.sum', index=4,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='int_histogram', full_name='opentelemetry.proto.metrics.v1.Metric.int_histogram', index=7,
-      number=8, type=11, cpp_type=10, label=1,
+      name='histogram', full_name='opentelemetry.proto.metrics.v1.Metric.histogram', index=5,
+      number=9, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='histogram', full_name='opentelemetry.proto.metrics.v1.Metric.histogram', index=8,
-      number=9, type=11, cpp_type=10, label=1,
+      name='exponential_histogram', full_name='opentelemetry.proto.metrics.v1.Metric.exponential_histogram', index=6,
+      number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='summary', full_name='opentelemetry.proto.metrics.v1.Metric.summary', index=9,
+      name='summary', full_name='opentelemetry.proto.metrics.v1.Metric.summary', index=7,
       number=11, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -246,48 +292,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='opentelemetry.proto.metrics.v1.Metric.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=577,
-  serialized_end=1079,
-)
-
-
-_INTGAUGE = _descriptor.Descriptor(
-  name='IntGauge',
-  full_name='opentelemetry.proto.metrics.v1.IntGauge',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='data_points', full_name='opentelemetry.proto.metrics.v1.IntGauge.data_points', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'\030\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1081,
-  serialized_end=1162,
+  serialized_start=667,
+  serialized_end=1069,
 )
 
 
 _GAUGE = _descriptor.Descriptor(
   name='Gauge',
   full_name='opentelemetry.proto.metrics.v1.Gauge',
   filename=None,
@@ -310,62 +324,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1164,
-  serialized_end=1241,
-)
-
-
-_INTSUM = _descriptor.Descriptor(
-  name='IntSum',
-  full_name='opentelemetry.proto.metrics.v1.IntSum',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='data_points', full_name='opentelemetry.proto.metrics.v1.IntSum.data_points', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='aggregation_temporality', full_name='opentelemetry.proto.metrics.v1.IntSum.aggregation_temporality', index=1,
-      number=2, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='is_monotonic', full_name='opentelemetry.proto.metrics.v1.IntSum.is_monotonic', index=2,
-      number=3, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'\030\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1244,
-  serialized_end=1434,
+  serialized_start=1071,
+  serialized_end=1148,
 )
 
 
 _SUM = _descriptor.Descriptor(
   name='Sum',
   full_name='opentelemetry.proto.metrics.v1.Sum',
   filename=None,
@@ -402,75 +370,75 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1437,
-  serialized_end=1623,
+  serialized_start=1151,
+  serialized_end=1337,
 )
 
 
-_INTHISTOGRAM = _descriptor.Descriptor(
-  name='IntHistogram',
-  full_name='opentelemetry.proto.metrics.v1.IntHistogram',
+_HISTOGRAM = _descriptor.Descriptor(
+  name='Histogram',
+  full_name='opentelemetry.proto.metrics.v1.Histogram',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='data_points', full_name='opentelemetry.proto.metrics.v1.IntHistogram.data_points', index=0,
+      name='data_points', full_name='opentelemetry.proto.metrics.v1.Histogram.data_points', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='aggregation_temporality', full_name='opentelemetry.proto.metrics.v1.IntHistogram.aggregation_temporality', index=1,
+      name='aggregation_temporality', full_name='opentelemetry.proto.metrics.v1.Histogram.aggregation_temporality', index=1,
       number=2, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
-  serialized_options=b'\030\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1626,
-  serialized_end=1809,
+  serialized_start=1340,
+  serialized_end=1513,
 )
 
 
-_HISTOGRAM = _descriptor.Descriptor(
-  name='Histogram',
-  full_name='opentelemetry.proto.metrics.v1.Histogram',
+_EXPONENTIALHISTOGRAM = _descriptor.Descriptor(
+  name='ExponentialHistogram',
+  full_name='opentelemetry.proto.metrics.v1.ExponentialHistogram',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='data_points', full_name='opentelemetry.proto.metrics.v1.Histogram.data_points', index=0,
+      name='data_points', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogram.data_points', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='aggregation_temporality', full_name='opentelemetry.proto.metrics.v1.Histogram.aggregation_temporality', index=1,
+      name='aggregation_temporality', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogram.aggregation_temporality', index=1,
       number=2, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -480,16 +448,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1812,
-  serialized_end=1985,
+  serialized_start=1516,
+  serialized_end=1711,
 )
 
 
 _SUMMARY = _descriptor.Descriptor(
   name='Summary',
   full_name='opentelemetry.proto.metrics.v1.Summary',
   filename=None,
@@ -512,76 +480,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1987,
-  serialized_end=2067,
-)
-
-
-_INTDATAPOINT = _descriptor.Descriptor(
-  name='IntDataPoint',
-  full_name='opentelemetry.proto.metrics.v1.IntDataPoint',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='labels', full_name='opentelemetry.proto.metrics.v1.IntDataPoint.labels', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.IntDataPoint.start_time_unix_nano', index=1,
-      number=2, type=6, cpp_type=4, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.IntDataPoint.time_unix_nano', index=2,
-      number=3, type=6, cpp_type=4, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='opentelemetry.proto.metrics.v1.IntDataPoint.value', index=3,
-      number=4, type=16, cpp_type=2, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='exemplars', full_name='opentelemetry.proto.metrics.v1.IntDataPoint.exemplars', index=4,
-      number=5, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'\030\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=2070,
-  serialized_end=2284,
+  serialized_start=1713,
+  serialized_end=1793,
 )
 
 
 _NUMBERDATAPOINT = _descriptor.Descriptor(
   name='NumberDataPoint',
   full_name='opentelemetry.proto.metrics.v1.NumberDataPoint',
   filename=None,
@@ -593,55 +501,55 @@
       name='attributes', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.attributes', index=0,
       number=7, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='labels', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.labels', index=1,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.start_time_unix_nano', index=2,
+      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.start_time_unix_nano', index=1,
       number=2, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.time_unix_nano', index=3,
+      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.time_unix_nano', index=2,
       number=3, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='as_double', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.as_double', index=4,
+      name='as_double', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.as_double', index=3,
       number=4, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='as_int', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.as_int', index=5,
+      name='as_int', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.as_int', index=4,
       number=6, type=16, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='exemplars', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.exemplars', index=6,
+      name='exemplars', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.exemplars', index=5,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='flags', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.flags', index=6,
+      number=8, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -651,185 +559,244 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='value', full_name='opentelemetry.proto.metrics.v1.NumberDataPoint.value',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2287,
-  serialized_end=2595,
+  serialized_start=1796,
+  serialized_end=2058,
 )
 
 
-_INTHISTOGRAMDATAPOINT = _descriptor.Descriptor(
-  name='IntHistogramDataPoint',
-  full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint',
+_HISTOGRAMDATAPOINT = _descriptor.Descriptor(
+  name='HistogramDataPoint',
+  full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='labels', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.labels', index=0,
-      number=1, type=11, cpp_type=10, label=3,
+      name='attributes', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.attributes', index=0,
+      number=9, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.start_time_unix_nano', index=1,
+      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.start_time_unix_nano', index=1,
       number=2, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.time_unix_nano', index=2,
+      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.time_unix_nano', index=2,
       number=3, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='count', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.count', index=3,
+      name='count', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.count', index=3,
       number=4, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sum', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.sum', index=4,
-      number=5, type=16, cpp_type=2, label=1,
-      has_default_value=False, default_value=0,
+      name='sum', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.sum', index=4,
+      number=5, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bucket_counts', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.bucket_counts', index=5,
+      name='bucket_counts', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.bucket_counts', index=5,
       number=6, type=6, cpp_type=4, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='explicit_bounds', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.explicit_bounds', index=6,
+      name='explicit_bounds', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.explicit_bounds', index=6,
       number=7, type=1, cpp_type=5, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='exemplars', full_name='opentelemetry.proto.metrics.v1.IntHistogramDataPoint.exemplars', index=7,
+      name='exemplars', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.exemplars', index=7,
       number=8, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='flags', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.flags', index=8,
+      number=10, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
-  serialized_options=b'\030\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2598,
-  serialized_end=2882,
+  serialized_start=2061,
+  serialized_end=2354,
 )
 
 
-_HISTOGRAMDATAPOINT = _descriptor.Descriptor(
-  name='HistogramDataPoint',
-  full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint',
+_EXPONENTIALHISTOGRAMDATAPOINT_BUCKETS = _descriptor.Descriptor(
+  name='Buckets',
+  full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.Buckets',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='attributes', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.attributes', index=0,
-      number=9, type=11, cpp_type=10, label=3,
+      name='offset', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.Buckets.offset', index=0,
+      number=1, type=17, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='bucket_counts', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.Buckets.bucket_counts', index=1,
+      number=2, type=4, cpp_type=4, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2822,
+  serialized_end=2870,
+)
+
+_EXPONENTIALHISTOGRAMDATAPOINT = _descriptor.Descriptor(
+  name='ExponentialHistogramDataPoint',
+  full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='labels', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.labels', index=1,
+      name='attributes', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.attributes', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.start_time_unix_nano', index=2,
+      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.start_time_unix_nano', index=1,
       number=2, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.time_unix_nano', index=3,
+      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.time_unix_nano', index=2,
       number=3, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='count', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.count', index=4,
+      name='count', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.count', index=3,
       number=4, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sum', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.sum', index=5,
+      name='sum', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.sum', index=4,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bucket_counts', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.bucket_counts', index=6,
-      number=6, type=6, cpp_type=4, label=3,
-      has_default_value=False, default_value=[],
+      name='scale', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.scale', index=5,
+      number=6, type=17, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='explicit_bounds', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.explicit_bounds', index=7,
-      number=7, type=1, cpp_type=5, label=3,
-      has_default_value=False, default_value=[],
+      name='zero_count', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.zero_count', index=6,
+      number=7, type=6, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='exemplars', full_name='opentelemetry.proto.metrics.v1.HistogramDataPoint.exemplars', index=8,
-      number=8, type=11, cpp_type=10, label=3,
+      name='positive', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.positive', index=7,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='negative', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.negative', index=8,
+      number=9, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='flags', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.flags', index=9,
+      number=10, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='exemplars', full_name='opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.exemplars', index=10,
+      number=11, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_EXPONENTIALHISTOGRAMDATAPOINT_BUCKETS, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2885,
-  serialized_end=3224,
+  serialized_start=2357,
+  serialized_end=2870,
 )
 
 
 _SUMMARYDATAPOINT_VALUEATQUANTILE = _descriptor.Descriptor(
   name='ValueAtQuantile',
   full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.ValueAtQuantile',
   filename=None,
@@ -859,16 +826,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3548,
-  serialized_end=3598,
+  serialized_start=3142,
+  serialized_end=3192,
 )
 
 _SUMMARYDATAPOINT = _descriptor.Descriptor(
   name='SummaryDataPoint',
   full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint',
   filename=None,
   file=DESCRIPTOR,
@@ -879,129 +846,69 @@
       name='attributes', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.attributes', index=0,
       number=7, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='labels', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.labels', index=1,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.start_time_unix_nano', index=2,
+      name='start_time_unix_nano', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.start_time_unix_nano', index=1,
       number=2, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.time_unix_nano', index=3,
+      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.time_unix_nano', index=2,
       number=3, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='count', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.count', index=4,
+      name='count', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.count', index=3,
       number=4, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sum', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.sum', index=5,
+      name='sum', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.sum', index=4,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='quantile_values', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.quantile_values', index=6,
+      name='quantile_values', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.quantile_values', index=5,
       number=6, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_SUMMARYDATAPOINT_VALUEATQUANTILE, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=3227,
-  serialized_end=3598,
-)
-
-
-_INTEXEMPLAR = _descriptor.Descriptor(
-  name='IntExemplar',
-  full_name='opentelemetry.proto.metrics.v1.IntExemplar',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='filtered_labels', full_name='opentelemetry.proto.metrics.v1.IntExemplar.filtered_labels', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.IntExemplar.time_unix_nano', index=1,
-      number=2, type=6, cpp_type=4, label=1,
+      name='flags', full_name='opentelemetry.proto.metrics.v1.SummaryDataPoint.flags', index=6,
+      number=8, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='opentelemetry.proto.metrics.v1.IntExemplar.value', index=2,
-      number=3, type=16, cpp_type=2, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='span_id', full_name='opentelemetry.proto.metrics.v1.IntExemplar.span_id', index=3,
-      number=4, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='trace_id', full_name='opentelemetry.proto.metrics.v1.IntExemplar.trace_id', index=4,
-      number=5, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_SUMMARYDATAPOINT_VALUEATQUANTILE, ],
   enum_types=[
   ],
-  serialized_options=b'\030\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3601,
-  serialized_end=3764,
+  serialized_start=2873,
+  serialized_end=3198,
 )
 
 
 _EXEMPLAR = _descriptor.Descriptor(
   name='Exemplar',
   full_name='opentelemetry.proto.metrics.v1.Exemplar',
   filename=None,
@@ -1013,50 +920,43 @@
       name='filtered_attributes', full_name='opentelemetry.proto.metrics.v1.Exemplar.filtered_attributes', index=0,
       number=7, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='filtered_labels', full_name='opentelemetry.proto.metrics.v1.Exemplar.filtered_labels', index=1,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.Exemplar.time_unix_nano', index=2,
+      name='time_unix_nano', full_name='opentelemetry.proto.metrics.v1.Exemplar.time_unix_nano', index=1,
       number=2, type=6, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='as_double', full_name='opentelemetry.proto.metrics.v1.Exemplar.as_double', index=3,
+      name='as_double', full_name='opentelemetry.proto.metrics.v1.Exemplar.as_double', index=2,
       number=3, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='as_int', full_name='opentelemetry.proto.metrics.v1.Exemplar.as_int', index=4,
+      name='as_int', full_name='opentelemetry.proto.metrics.v1.Exemplar.as_int', index=3,
       number=6, type=16, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='span_id', full_name='opentelemetry.proto.metrics.v1.Exemplar.span_id', index=5,
+      name='span_id', full_name='opentelemetry.proto.metrics.v1.Exemplar.span_id', index=4,
       number=4, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='trace_id', full_name='opentelemetry.proto.metrics.v1.Exemplar.trace_id', index=6,
+      name='trace_id', full_name='opentelemetry.proto.metrics.v1.Exemplar.trace_id', index=5,
       number=5, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1071,110 +971,101 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='value', full_name='opentelemetry.proto.metrics.v1.Exemplar.value',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3767,
-  serialized_end=4030,
+  serialized_start=3201,
+  serialized_end=3394,
 )
 
+_METRICSDATA.fields_by_name['resource_metrics'].message_type = _RESOURCEMETRICS
 _RESOURCEMETRICS.fields_by_name['resource'].message_type = opentelemetry_dot_proto_dot_resource_dot_v1_dot_resource__pb2._RESOURCE
 _RESOURCEMETRICS.fields_by_name['instrumentation_library_metrics'].message_type = _INSTRUMENTATIONLIBRARYMETRICS
 _INSTRUMENTATIONLIBRARYMETRICS.fields_by_name['instrumentation_library'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._INSTRUMENTATIONLIBRARY
 _INSTRUMENTATIONLIBRARYMETRICS.fields_by_name['metrics'].message_type = _METRIC
-_METRIC.fields_by_name['int_gauge'].message_type = _INTGAUGE
 _METRIC.fields_by_name['gauge'].message_type = _GAUGE
-_METRIC.fields_by_name['int_sum'].message_type = _INTSUM
 _METRIC.fields_by_name['sum'].message_type = _SUM
-_METRIC.fields_by_name['int_histogram'].message_type = _INTHISTOGRAM
 _METRIC.fields_by_name['histogram'].message_type = _HISTOGRAM
+_METRIC.fields_by_name['exponential_histogram'].message_type = _EXPONENTIALHISTOGRAM
 _METRIC.fields_by_name['summary'].message_type = _SUMMARY
 _METRIC.oneofs_by_name['data'].fields.append(
-  _METRIC.fields_by_name['int_gauge'])
-_METRIC.fields_by_name['int_gauge'].containing_oneof = _METRIC.oneofs_by_name['data']
-_METRIC.oneofs_by_name['data'].fields.append(
   _METRIC.fields_by_name['gauge'])
 _METRIC.fields_by_name['gauge'].containing_oneof = _METRIC.oneofs_by_name['data']
 _METRIC.oneofs_by_name['data'].fields.append(
-  _METRIC.fields_by_name['int_sum'])
-_METRIC.fields_by_name['int_sum'].containing_oneof = _METRIC.oneofs_by_name['data']
-_METRIC.oneofs_by_name['data'].fields.append(
   _METRIC.fields_by_name['sum'])
 _METRIC.fields_by_name['sum'].containing_oneof = _METRIC.oneofs_by_name['data']
 _METRIC.oneofs_by_name['data'].fields.append(
-  _METRIC.fields_by_name['int_histogram'])
-_METRIC.fields_by_name['int_histogram'].containing_oneof = _METRIC.oneofs_by_name['data']
-_METRIC.oneofs_by_name['data'].fields.append(
   _METRIC.fields_by_name['histogram'])
 _METRIC.fields_by_name['histogram'].containing_oneof = _METRIC.oneofs_by_name['data']
 _METRIC.oneofs_by_name['data'].fields.append(
+  _METRIC.fields_by_name['exponential_histogram'])
+_METRIC.fields_by_name['exponential_histogram'].containing_oneof = _METRIC.oneofs_by_name['data']
+_METRIC.oneofs_by_name['data'].fields.append(
   _METRIC.fields_by_name['summary'])
 _METRIC.fields_by_name['summary'].containing_oneof = _METRIC.oneofs_by_name['data']
-_INTGAUGE.fields_by_name['data_points'].message_type = _INTDATAPOINT
 _GAUGE.fields_by_name['data_points'].message_type = _NUMBERDATAPOINT
-_INTSUM.fields_by_name['data_points'].message_type = _INTDATAPOINT
-_INTSUM.fields_by_name['aggregation_temporality'].enum_type = _AGGREGATIONTEMPORALITY
 _SUM.fields_by_name['data_points'].message_type = _NUMBERDATAPOINT
 _SUM.fields_by_name['aggregation_temporality'].enum_type = _AGGREGATIONTEMPORALITY
-_INTHISTOGRAM.fields_by_name['data_points'].message_type = _INTHISTOGRAMDATAPOINT
-_INTHISTOGRAM.fields_by_name['aggregation_temporality'].enum_type = _AGGREGATIONTEMPORALITY
 _HISTOGRAM.fields_by_name['data_points'].message_type = _HISTOGRAMDATAPOINT
 _HISTOGRAM.fields_by_name['aggregation_temporality'].enum_type = _AGGREGATIONTEMPORALITY
+_EXPONENTIALHISTOGRAM.fields_by_name['data_points'].message_type = _EXPONENTIALHISTOGRAMDATAPOINT
+_EXPONENTIALHISTOGRAM.fields_by_name['aggregation_temporality'].enum_type = _AGGREGATIONTEMPORALITY
 _SUMMARY.fields_by_name['data_points'].message_type = _SUMMARYDATAPOINT
-_INTDATAPOINT.fields_by_name['labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
-_INTDATAPOINT.fields_by_name['exemplars'].message_type = _INTEXEMPLAR
 _NUMBERDATAPOINT.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
-_NUMBERDATAPOINT.fields_by_name['labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
 _NUMBERDATAPOINT.fields_by_name['exemplars'].message_type = _EXEMPLAR
 _NUMBERDATAPOINT.oneofs_by_name['value'].fields.append(
   _NUMBERDATAPOINT.fields_by_name['as_double'])
 _NUMBERDATAPOINT.fields_by_name['as_double'].containing_oneof = _NUMBERDATAPOINT.oneofs_by_name['value']
 _NUMBERDATAPOINT.oneofs_by_name['value'].fields.append(
   _NUMBERDATAPOINT.fields_by_name['as_int'])
 _NUMBERDATAPOINT.fields_by_name['as_int'].containing_oneof = _NUMBERDATAPOINT.oneofs_by_name['value']
-_INTHISTOGRAMDATAPOINT.fields_by_name['labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
-_INTHISTOGRAMDATAPOINT.fields_by_name['exemplars'].message_type = _INTEXEMPLAR
 _HISTOGRAMDATAPOINT.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
-_HISTOGRAMDATAPOINT.fields_by_name['labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
 _HISTOGRAMDATAPOINT.fields_by_name['exemplars'].message_type = _EXEMPLAR
+_EXPONENTIALHISTOGRAMDATAPOINT_BUCKETS.containing_type = _EXPONENTIALHISTOGRAMDATAPOINT
+_EXPONENTIALHISTOGRAMDATAPOINT.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
+_EXPONENTIALHISTOGRAMDATAPOINT.fields_by_name['positive'].message_type = _EXPONENTIALHISTOGRAMDATAPOINT_BUCKETS
+_EXPONENTIALHISTOGRAMDATAPOINT.fields_by_name['negative'].message_type = _EXPONENTIALHISTOGRAMDATAPOINT_BUCKETS
+_EXPONENTIALHISTOGRAMDATAPOINT.fields_by_name['exemplars'].message_type = _EXEMPLAR
 _SUMMARYDATAPOINT_VALUEATQUANTILE.containing_type = _SUMMARYDATAPOINT
 _SUMMARYDATAPOINT.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
-_SUMMARYDATAPOINT.fields_by_name['labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
 _SUMMARYDATAPOINT.fields_by_name['quantile_values'].message_type = _SUMMARYDATAPOINT_VALUEATQUANTILE
-_INTEXEMPLAR.fields_by_name['filtered_labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
 _EXEMPLAR.fields_by_name['filtered_attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
-_EXEMPLAR.fields_by_name['filtered_labels'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._STRINGKEYVALUE
 _EXEMPLAR.oneofs_by_name['value'].fields.append(
   _EXEMPLAR.fields_by_name['as_double'])
 _EXEMPLAR.fields_by_name['as_double'].containing_oneof = _EXEMPLAR.oneofs_by_name['value']
 _EXEMPLAR.oneofs_by_name['value'].fields.append(
   _EXEMPLAR.fields_by_name['as_int'])
 _EXEMPLAR.fields_by_name['as_int'].containing_oneof = _EXEMPLAR.oneofs_by_name['value']
+DESCRIPTOR.message_types_by_name['MetricsData'] = _METRICSDATA
 DESCRIPTOR.message_types_by_name['ResourceMetrics'] = _RESOURCEMETRICS
 DESCRIPTOR.message_types_by_name['InstrumentationLibraryMetrics'] = _INSTRUMENTATIONLIBRARYMETRICS
 DESCRIPTOR.message_types_by_name['Metric'] = _METRIC
-DESCRIPTOR.message_types_by_name['IntGauge'] = _INTGAUGE
 DESCRIPTOR.message_types_by_name['Gauge'] = _GAUGE
-DESCRIPTOR.message_types_by_name['IntSum'] = _INTSUM
 DESCRIPTOR.message_types_by_name['Sum'] = _SUM
-DESCRIPTOR.message_types_by_name['IntHistogram'] = _INTHISTOGRAM
 DESCRIPTOR.message_types_by_name['Histogram'] = _HISTOGRAM
+DESCRIPTOR.message_types_by_name['ExponentialHistogram'] = _EXPONENTIALHISTOGRAM
 DESCRIPTOR.message_types_by_name['Summary'] = _SUMMARY
-DESCRIPTOR.message_types_by_name['IntDataPoint'] = _INTDATAPOINT
 DESCRIPTOR.message_types_by_name['NumberDataPoint'] = _NUMBERDATAPOINT
-DESCRIPTOR.message_types_by_name['IntHistogramDataPoint'] = _INTHISTOGRAMDATAPOINT
 DESCRIPTOR.message_types_by_name['HistogramDataPoint'] = _HISTOGRAMDATAPOINT
+DESCRIPTOR.message_types_by_name['ExponentialHistogramDataPoint'] = _EXPONENTIALHISTOGRAMDATAPOINT
 DESCRIPTOR.message_types_by_name['SummaryDataPoint'] = _SUMMARYDATAPOINT
-DESCRIPTOR.message_types_by_name['IntExemplar'] = _INTEXEMPLAR
 DESCRIPTOR.message_types_by_name['Exemplar'] = _EXEMPLAR
 DESCRIPTOR.enum_types_by_name['AggregationTemporality'] = _AGGREGATIONTEMPORALITY
+DESCRIPTOR.enum_types_by_name['DataPointFlags'] = _DATAPOINTFLAGS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+MetricsData = _reflection.GeneratedProtocolMessageType('MetricsData', (_message.Message,), {
+  'DESCRIPTOR' : _METRICSDATA,
+  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
+  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.MetricsData)
+  })
+_sym_db.RegisterMessage(MetricsData)
+
 ResourceMetrics = _reflection.GeneratedProtocolMessageType('ResourceMetrics', (_message.Message,), {
   'DESCRIPTOR' : _RESOURCEMETRICS,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.ResourceMetrics)
   })
 _sym_db.RegisterMessage(ResourceMetrics)
 
@@ -1188,91 +1079,78 @@
 Metric = _reflection.GeneratedProtocolMessageType('Metric', (_message.Message,), {
   'DESCRIPTOR' : _METRIC,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.Metric)
   })
 _sym_db.RegisterMessage(Metric)
 
-IntGauge = _reflection.GeneratedProtocolMessageType('IntGauge', (_message.Message,), {
-  'DESCRIPTOR' : _INTGAUGE,
-  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
-  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.IntGauge)
-  })
-_sym_db.RegisterMessage(IntGauge)
-
 Gauge = _reflection.GeneratedProtocolMessageType('Gauge', (_message.Message,), {
   'DESCRIPTOR' : _GAUGE,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.Gauge)
   })
 _sym_db.RegisterMessage(Gauge)
 
-IntSum = _reflection.GeneratedProtocolMessageType('IntSum', (_message.Message,), {
-  'DESCRIPTOR' : _INTSUM,
-  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
-  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.IntSum)
-  })
-_sym_db.RegisterMessage(IntSum)
-
 Sum = _reflection.GeneratedProtocolMessageType('Sum', (_message.Message,), {
   'DESCRIPTOR' : _SUM,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.Sum)
   })
 _sym_db.RegisterMessage(Sum)
 
-IntHistogram = _reflection.GeneratedProtocolMessageType('IntHistogram', (_message.Message,), {
-  'DESCRIPTOR' : _INTHISTOGRAM,
-  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
-  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.IntHistogram)
-  })
-_sym_db.RegisterMessage(IntHistogram)
-
 Histogram = _reflection.GeneratedProtocolMessageType('Histogram', (_message.Message,), {
   'DESCRIPTOR' : _HISTOGRAM,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.Histogram)
   })
 _sym_db.RegisterMessage(Histogram)
 
+ExponentialHistogram = _reflection.GeneratedProtocolMessageType('ExponentialHistogram', (_message.Message,), {
+  'DESCRIPTOR' : _EXPONENTIALHISTOGRAM,
+  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
+  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.ExponentialHistogram)
+  })
+_sym_db.RegisterMessage(ExponentialHistogram)
+
 Summary = _reflection.GeneratedProtocolMessageType('Summary', (_message.Message,), {
   'DESCRIPTOR' : _SUMMARY,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.Summary)
   })
 _sym_db.RegisterMessage(Summary)
 
-IntDataPoint = _reflection.GeneratedProtocolMessageType('IntDataPoint', (_message.Message,), {
-  'DESCRIPTOR' : _INTDATAPOINT,
-  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
-  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.IntDataPoint)
-  })
-_sym_db.RegisterMessage(IntDataPoint)
-
 NumberDataPoint = _reflection.GeneratedProtocolMessageType('NumberDataPoint', (_message.Message,), {
   'DESCRIPTOR' : _NUMBERDATAPOINT,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.NumberDataPoint)
   })
 _sym_db.RegisterMessage(NumberDataPoint)
 
-IntHistogramDataPoint = _reflection.GeneratedProtocolMessageType('IntHistogramDataPoint', (_message.Message,), {
-  'DESCRIPTOR' : _INTHISTOGRAMDATAPOINT,
-  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
-  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.IntHistogramDataPoint)
-  })
-_sym_db.RegisterMessage(IntHistogramDataPoint)
-
 HistogramDataPoint = _reflection.GeneratedProtocolMessageType('HistogramDataPoint', (_message.Message,), {
   'DESCRIPTOR' : _HISTOGRAMDATAPOINT,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.HistogramDataPoint)
   })
 _sym_db.RegisterMessage(HistogramDataPoint)
 
+ExponentialHistogramDataPoint = _reflection.GeneratedProtocolMessageType('ExponentialHistogramDataPoint', (_message.Message,), {
+
+  'Buckets' : _reflection.GeneratedProtocolMessageType('Buckets', (_message.Message,), {
+    'DESCRIPTOR' : _EXPONENTIALHISTOGRAMDATAPOINT_BUCKETS,
+    '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
+    # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint.Buckets)
+    })
+  ,
+  'DESCRIPTOR' : _EXPONENTIALHISTOGRAMDATAPOINT,
+  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
+  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.ExponentialHistogramDataPoint)
+  })
+_sym_db.RegisterMessage(ExponentialHistogramDataPoint)
+_sym_db.RegisterMessage(ExponentialHistogramDataPoint.Buckets)
+
 SummaryDataPoint = _reflection.GeneratedProtocolMessageType('SummaryDataPoint', (_message.Message,), {
 
   'ValueAtQuantile' : _reflection.GeneratedProtocolMessageType('ValueAtQuantile', (_message.Message,), {
     'DESCRIPTOR' : _SUMMARYDATAPOINT_VALUEATQUANTILE,
     '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
     # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.SummaryDataPoint.ValueAtQuantile)
     })
@@ -1280,37 +1158,17 @@
   'DESCRIPTOR' : _SUMMARYDATAPOINT,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.SummaryDataPoint)
   })
 _sym_db.RegisterMessage(SummaryDataPoint)
 _sym_db.RegisterMessage(SummaryDataPoint.ValueAtQuantile)
 
-IntExemplar = _reflection.GeneratedProtocolMessageType('IntExemplar', (_message.Message,), {
-  'DESCRIPTOR' : _INTEXEMPLAR,
-  '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
-  # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.IntExemplar)
-  })
-_sym_db.RegisterMessage(IntExemplar)
-
 Exemplar = _reflection.GeneratedProtocolMessageType('Exemplar', (_message.Message,), {
   'DESCRIPTOR' : _EXEMPLAR,
   '__module__' : 'opentelemetry.proto.metrics.v1.metrics_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.metrics.v1.Exemplar)
   })
 _sym_db.RegisterMessage(Exemplar)
 
 
 DESCRIPTOR._options = None
-_METRIC.fields_by_name['int_gauge']._options = None
-_METRIC.fields_by_name['int_sum']._options = None
-_METRIC.fields_by_name['int_histogram']._options = None
-_INTGAUGE._options = None
-_INTSUM._options = None
-_INTHISTOGRAM._options = None
-_INTDATAPOINT._options = None
-_NUMBERDATAPOINT.fields_by_name['labels']._options = None
-_INTHISTOGRAMDATAPOINT._options = None
-_HISTOGRAMDATAPOINT.fields_by_name['labels']._options = None
-_SUMMARYDATAPOINT.fields_by_name['labels']._options = None
-_INTEXEMPLAR._options = None
-_EXEMPLAR.fields_by_name['filtered_labels']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/metrics/v1/metrics_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/metrics/v1/metrics_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -160,14 +160,75 @@
 systems that do not use start_time to determine when the aggregation
 value was reset (e.g. Prometheus).
 """
 
 global___AggregationTemporality = AggregationTemporality
 
 
+class DataPointFlags(_DataPointFlags, metaclass=_DataPointFlagsEnumTypeWrapper):
+    """DataPointFlags is defined as a protobuf 'uint32' type and is to be used as a
+    bit-field representing 32 distinct boolean flags.  Each flag defined in this
+    enum is a bit-mask.  To test the presence of a single flag in the flags of
+    a data point, for example, use an expression like:
+
+      (point.flags & FLAG_NO_RECORDED_VALUE) == FLAG_NO_RECORDED_VALUE
+    """
+    pass
+class _DataPointFlags:
+    V = typing.NewType('V', builtins.int)
+class _DataPointFlagsEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DataPointFlags.V], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
+    FLAG_NONE = DataPointFlags.V(0)
+    FLAG_NO_RECORDED_VALUE = DataPointFlags.V(1)
+    """This DataPoint is valid but has no recorded value.  This value
+    SHOULD be used to reflect explicitly missing data in a series, as
+    for an equivalent to the Prometheus "staleness marker".
+    """
+
+
+FLAG_NONE = DataPointFlags.V(0)
+FLAG_NO_RECORDED_VALUE = DataPointFlags.V(1)
+"""This DataPoint is valid but has no recorded value.  This value
+SHOULD be used to reflect explicitly missing data in a series, as
+for an equivalent to the Prometheus "staleness marker".
+"""
+
+global___DataPointFlags = DataPointFlags
+
+
+class MetricsData(google.protobuf.message.Message):
+    """MetricsData represents the metrics data that can be stored in a persistent
+    storage, OR can be embedded by other protocols that transfer OTLP metrics
+    data but do not implement the OTLP protocol.
+
+    The main difference between this message and collector protocol is that
+    in this message there will not be any "control" or "metadata" specific to
+    OTLP protocol.
+
+    When new fields are added into this message, the OTLP request MUST be updated
+    as well.
+    """
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    RESOURCE_METRICS_FIELD_NUMBER: builtins.int
+    @property
+    def resource_metrics(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceMetrics]:
+        """An array of ResourceMetrics.
+        For data coming from a single resource this array will typically contain
+        one element. Intermediary nodes that receive data from multiple origins
+        typically batch the data before forwarding further and in that case this
+        array will contain multiple elements.
+        """
+        pass
+    def __init__(self,
+        *,
+        resource_metrics : typing.Optional[typing.Iterable[global___ResourceMetrics]] = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resource_metrics",b"resource_metrics"]) -> None: ...
+global___MetricsData = MetricsData
+
 class ResourceMetrics(google.protobuf.message.Message):
     """A collection of InstrumentationLibraryMetrics from a Resource."""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     RESOURCE_FIELD_NUMBER: builtins.int
     INSTRUMENTATION_LIBRARY_METRICS_FIELD_NUMBER: builtins.int
     SCHEMA_URL_FIELD_NUMBER: builtins.int
     @property
@@ -313,111 +374,58 @@
     when the start time is truly unknown, setting StartTimeUnixNano is
     strongly encouraged.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     NAME_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
-    INT_GAUGE_FIELD_NUMBER: builtins.int
     GAUGE_FIELD_NUMBER: builtins.int
-    INT_SUM_FIELD_NUMBER: builtins.int
     SUM_FIELD_NUMBER: builtins.int
-    INT_HISTOGRAM_FIELD_NUMBER: builtins.int
     HISTOGRAM_FIELD_NUMBER: builtins.int
+    EXPONENTIAL_HISTOGRAM_FIELD_NUMBER: builtins.int
     SUMMARY_FIELD_NUMBER: builtins.int
     name: typing.Text = ...
     """name of the metric, including its DNS name prefix. It must be unique."""
 
     description: typing.Text = ...
     """description of the metric, which can be used in documentation."""
 
     unit: typing.Text = ...
     """unit in which the metric value is reported. Follows the format
     described by http://unitsofmeasure.org/ucum.html.
     """
 
     @property
-    def int_gauge(self) -> global___IntGauge:
-        """IntGauge and IntSum are deprecated and will be removed soon.
-        1. Old senders and receivers that are not aware of this change will
-        continue using the `int_gauge` and `int_sum` fields.
-        2. New senders, which are aware of this change MUST send only `gauge`
-        and `sum` fields.
-        3. New receivers, which are aware of this change MUST convert these into
-        `gauge` and `sum` by using the provided as_int field in the oneof values.
-        This field will be removed in ~3 months, on July 1, 2021.
-        """
-        pass
-    @property
     def gauge(self) -> global___Gauge: ...
     @property
-    def int_sum(self) -> global___IntSum:
-        """This field will be removed in ~3 months, on July 1, 2021."""
-        pass
-    @property
     def sum(self) -> global___Sum: ...
     @property
-    def int_histogram(self) -> global___IntHistogram:
-        """IntHistogram is deprecated and will be removed soon.
-        1. Old senders and receivers that are not aware of this change will
-        continue using the `int_histogram` field.
-        2. New senders, which are aware of this change MUST send only `histogram`.
-        3. New receivers, which are aware of this change MUST convert this into
-        `histogram` by simply converting all int64 values into float.
-        This field will be removed in ~3 months, on July 1, 2021.
-        """
-        pass
-    @property
     def histogram(self) -> global___Histogram: ...
     @property
+    def exponential_histogram(self) -> global___ExponentialHistogram: ...
+    @property
     def summary(self) -> global___Summary: ...
     def __init__(self,
         *,
         name : typing.Text = ...,
         description : typing.Text = ...,
         unit : typing.Text = ...,
-        int_gauge : typing.Optional[global___IntGauge] = ...,
         gauge : typing.Optional[global___Gauge] = ...,
-        int_sum : typing.Optional[global___IntSum] = ...,
         sum : typing.Optional[global___Sum] = ...,
-        int_histogram : typing.Optional[global___IntHistogram] = ...,
         histogram : typing.Optional[global___Histogram] = ...,
+        exponential_histogram : typing.Optional[global___ExponentialHistogram] = ...,
         summary : typing.Optional[global___Summary] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data",b"data","gauge",b"gauge","histogram",b"histogram","int_gauge",b"int_gauge","int_histogram",b"int_histogram","int_sum",b"int_sum","sum",b"sum","summary",b"summary"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data",b"data","description",b"description","gauge",b"gauge","histogram",b"histogram","int_gauge",b"int_gauge","int_histogram",b"int_histogram","int_sum",b"int_sum","name",b"name","sum",b"sum","summary",b"summary","unit",b"unit"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["data",b"data"]) -> typing.Optional[typing_extensions.Literal["int_gauge","gauge","int_sum","sum","int_histogram","histogram","summary"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["data",b"data","exponential_histogram",b"exponential_histogram","gauge",b"gauge","histogram",b"histogram","sum",b"sum","summary",b"summary"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["data",b"data","description",b"description","exponential_histogram",b"exponential_histogram","gauge",b"gauge","histogram",b"histogram","name",b"name","sum",b"sum","summary",b"summary","unit",b"unit"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["data",b"data"]) -> typing.Optional[typing_extensions.Literal["gauge","sum","histogram","exponential_histogram","summary"]]: ...
 global___Metric = Metric
 
-class IntGauge(google.protobuf.message.Message):
-    """IntGauge is deprecated.  Use Gauge with an integer value in NumberDataPoint.
-
-    IntGauge represents the type of a int scalar metric that always exports the
-    "current value" for every data point. It should be used for an "unknown"
-    aggregation.
-
-    A Gauge does not support different aggregation temporalities. Given the
-    aggregation is unknown, points cannot be combined using the same
-    aggregation, regardless of aggregation temporalities. Therefore,
-    AggregationTemporality is not included. Consequently, this also means
-    "StartTimeUnixNano" is ignored for all data points.
-    """
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    DATA_POINTS_FIELD_NUMBER: builtins.int
-    @property
-    def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntDataPoint]: ...
-    def __init__(self,
-        *,
-        data_points : typing.Optional[typing.Iterable[global___IntDataPoint]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data_points",b"data_points"]) -> None: ...
-global___IntGauge = IntGauge
-
 class Gauge(google.protobuf.message.Message):
-    """Gauge represents the type of a double scalar metric that always exports the
+    """Gauge represents the type of a scalar metric that always exports the
     "current value" for every data point. It should be used for an "unknown"
     aggregation.
 
     A Gauge does not support different aggregation temporalities. Given the
     aggregation is unknown, points cannot be combined using the same
     aggregation, regardless of aggregation temporalities. Therefore,
     AggregationTemporality is not included. Consequently, this also means
@@ -430,46 +438,17 @@
     def __init__(self,
         *,
         data_points : typing.Optional[typing.Iterable[global___NumberDataPoint]] = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_points",b"data_points"]) -> None: ...
 global___Gauge = Gauge
 
-class IntSum(google.protobuf.message.Message):
-    """IntSum is deprecated.  Use Sum with an integer value in NumberDataPoint.
-
-    IntSum represents the type of a numeric int scalar metric that is calculated as
-    a sum of all reported measurements over a time interval.
-    """
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    DATA_POINTS_FIELD_NUMBER: builtins.int
-    AGGREGATION_TEMPORALITY_FIELD_NUMBER: builtins.int
-    IS_MONOTONIC_FIELD_NUMBER: builtins.int
-    @property
-    def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntDataPoint]: ...
-    aggregation_temporality: global___AggregationTemporality.V = ...
-    """aggregation_temporality describes if the aggregator reports delta changes
-    since last report time, or cumulative changes since a fixed start time.
-    """
-
-    is_monotonic: builtins.bool = ...
-    """If "true" means that the sum is monotonic."""
-
-    def __init__(self,
-        *,
-        data_points : typing.Optional[typing.Iterable[global___IntDataPoint]] = ...,
-        aggregation_temporality : global___AggregationTemporality.V = ...,
-        is_monotonic : builtins.bool = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aggregation_temporality",b"aggregation_temporality","data_points",b"data_points","is_monotonic",b"is_monotonic"]) -> None: ...
-global___IntSum = IntSum
-
 class Sum(google.protobuf.message.Message):
-    """Sum represents the type of a numeric double scalar metric that is calculated
-    as a sum of all reported measurements over a time interval.
+    """Sum represents the type of a scalar metric that is calculated as a sum of all
+    reported measurements over a time interval.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     DATA_POINTS_FIELD_NUMBER: builtins.int
     AGGREGATION_TEMPORALITY_FIELD_NUMBER: builtins.int
     IS_MONOTONIC_FIELD_NUMBER: builtins.int
     @property
     def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NumberDataPoint]: ...
@@ -486,60 +465,57 @@
         data_points : typing.Optional[typing.Iterable[global___NumberDataPoint]] = ...,
         aggregation_temporality : global___AggregationTemporality.V = ...,
         is_monotonic : builtins.bool = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregation_temporality",b"aggregation_temporality","data_points",b"data_points","is_monotonic",b"is_monotonic"]) -> None: ...
 global___Sum = Sum
 
-class IntHistogram(google.protobuf.message.Message):
-    """IntHistogram is deprecated, replaced by Histogram points using double-
-    valued exemplars.
-
-    This represents the type of a metric that is calculated by aggregating as a
-    Histogram of all reported int measurements over a time interval.
+class Histogram(google.protobuf.message.Message):
+    """Histogram represents the type of a metric that is calculated by aggregating
+    as a Histogram of all reported measurements over a time interval.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     DATA_POINTS_FIELD_NUMBER: builtins.int
     AGGREGATION_TEMPORALITY_FIELD_NUMBER: builtins.int
     @property
-    def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntHistogramDataPoint]: ...
+    def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HistogramDataPoint]: ...
     aggregation_temporality: global___AggregationTemporality.V = ...
     """aggregation_temporality describes if the aggregator reports delta changes
     since last report time, or cumulative changes since a fixed start time.
     """
 
     def __init__(self,
         *,
-        data_points : typing.Optional[typing.Iterable[global___IntHistogramDataPoint]] = ...,
+        data_points : typing.Optional[typing.Iterable[global___HistogramDataPoint]] = ...,
         aggregation_temporality : global___AggregationTemporality.V = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregation_temporality",b"aggregation_temporality","data_points",b"data_points"]) -> None: ...
-global___IntHistogram = IntHistogram
+global___Histogram = Histogram
 
-class Histogram(google.protobuf.message.Message):
-    """Histogram represents the type of a metric that is calculated by aggregating
-    as a Histogram of all reported double measurements over a time interval.
+class ExponentialHistogram(google.protobuf.message.Message):
+    """ExponentialHistogram represents the type of a metric that is calculated by aggregating
+    as a ExponentialHistogram of all reported double measurements over a time interval.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     DATA_POINTS_FIELD_NUMBER: builtins.int
     AGGREGATION_TEMPORALITY_FIELD_NUMBER: builtins.int
     @property
-    def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HistogramDataPoint]: ...
+    def data_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ExponentialHistogramDataPoint]: ...
     aggregation_temporality: global___AggregationTemporality.V = ...
     """aggregation_temporality describes if the aggregator reports delta changes
     since last report time, or cumulative changes since a fixed start time.
     """
 
     def __init__(self,
         *,
-        data_points : typing.Optional[typing.Iterable[global___HistogramDataPoint]] = ...,
+        data_points : typing.Optional[typing.Iterable[global___ExponentialHistogramDataPoint]] = ...,
         aggregation_temporality : global___AggregationTemporality.V = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregation_temporality",b"aggregation_temporality","data_points",b"data_points"]) -> None: ...
-global___Histogram = Histogram
+global___ExponentialHistogram = ExponentialHistogram
 
 class Summary(google.protobuf.message.Message):
     """Summary metric data are used to convey quantile summaries,
     a Prometheus (see: https://prometheus.io/docs/concepts/metric_types/#summary)
     and OpenMetrics (see: https://github.com/OpenObservability/OpenMetrics/blob/4dbf6075567ab43296eed941037c12951faafb92/protos/prometheus.proto#L45)
     data type. These data points cannot always be merged in a meaningful way.
     While they can be useful in some applications, histogram data points are
@@ -552,96 +528,35 @@
     def __init__(self,
         *,
         data_points : typing.Optional[typing.Iterable[global___SummaryDataPoint]] = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_points",b"data_points"]) -> None: ...
 global___Summary = Summary
 
-class IntDataPoint(google.protobuf.message.Message):
-    """IntDataPoint is a single data point in a timeseries that describes the
-    time-varying values of a int64 metric.
-    """
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    LABELS_FIELD_NUMBER: builtins.int
-    START_TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
-    TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
-    VALUE_FIELD_NUMBER: builtins.int
-    EXEMPLARS_FIELD_NUMBER: builtins.int
-    @property
-    def labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """The set of labels that uniquely identify this timeseries."""
-        pass
-    start_time_unix_nano: builtins.int = ...
-    """StartTimeUnixNano is optional but strongly encouraged, see the
-    the detiled comments above Metric.
-
-    Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
-    1970.
-    """
-
-    time_unix_nano: builtins.int = ...
-    """TimeUnixNano is required, see the detailed comments above Metric.
-
-    Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
-    1970.
-    """
-
-    value: builtins.int = ...
-    """value itself."""
-
-    @property
-    def exemplars(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntExemplar]:
-        """(Optional) List of exemplars collected from
-        measurements that were used to form the data point
-        """
-        pass
-    def __init__(self,
-        *,
-        labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
-        start_time_unix_nano : builtins.int = ...,
-        time_unix_nano : builtins.int = ...,
-        value : builtins.int = ...,
-        exemplars : typing.Optional[typing.Iterable[global___IntExemplar]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exemplars",b"exemplars","labels",b"labels","start_time_unix_nano",b"start_time_unix_nano","time_unix_nano",b"time_unix_nano","value",b"value"]) -> None: ...
-global___IntDataPoint = IntDataPoint
-
 class NumberDataPoint(google.protobuf.message.Message):
     """NumberDataPoint is a single data point in a timeseries that describes the
-    time-varying value of a double metric.
+    time-varying scalar value of a metric.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     ATTRIBUTES_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
     START_TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     AS_DOUBLE_FIELD_NUMBER: builtins.int
     AS_INT_FIELD_NUMBER: builtins.int
     EXEMPLARS_FIELD_NUMBER: builtins.int
+    FLAGS_FIELD_NUMBER: builtins.int
     @property
     def attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.KeyValue]:
         """The set of key/value pairs that uniquely identify the timeseries from
         where this point belongs. The list may be empty (may contain 0 elements).
         """
         pass
-    @property
-    def labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """Labels is deprecated and will be removed soon.
-        1. Old senders and receivers that are not aware of this change will
-        continue using the `labels` field.
-        2. New senders, which are aware of this change MUST send only `attributes`.
-        3. New receivers, which are aware of this change MUST convert this into
-        `labels` by simply converting all int64 values into float.
-
-        This field will be removed in ~3 months, on July 1, 2021.
-        """
-        pass
     start_time_unix_nano: builtins.int = ...
     """StartTimeUnixNano is optional but strongly encouraged, see the
-    the detiled comments above Metric.
+    the detailed comments above Metric.
 
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
     1970.
     """
 
     time_unix_nano: builtins.int = ...
     """TimeUnixNano is required, see the detailed comments above Metric.
@@ -654,59 +569,65 @@
     as_int: builtins.int = ...
     @property
     def exemplars(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Exemplar]:
         """(Optional) List of exemplars collected from
         measurements that were used to form the data point
         """
         pass
+    flags: builtins.int = ...
+    """Flags that apply to this specific data point.  See DataPointFlags
+    for the available flags and their meaning.
+    """
+
     def __init__(self,
         *,
         attributes : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.KeyValue]] = ...,
-        labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
         start_time_unix_nano : builtins.int = ...,
         time_unix_nano : builtins.int = ...,
         as_double : builtins.float = ...,
         as_int : builtins.int = ...,
         exemplars : typing.Optional[typing.Iterable[global___Exemplar]] = ...,
+        flags : builtins.int = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["as_double",b"as_double","as_int",b"as_int","value",b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["as_double",b"as_double","as_int",b"as_int","attributes",b"attributes","exemplars",b"exemplars","labels",b"labels","start_time_unix_nano",b"start_time_unix_nano","time_unix_nano",b"time_unix_nano","value",b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["as_double",b"as_double","as_int",b"as_int","attributes",b"attributes","exemplars",b"exemplars","flags",b"flags","start_time_unix_nano",b"start_time_unix_nano","time_unix_nano",b"time_unix_nano","value",b"value"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["value",b"value"]) -> typing.Optional[typing_extensions.Literal["as_double","as_int"]]: ...
 global___NumberDataPoint = NumberDataPoint
 
-class IntHistogramDataPoint(google.protobuf.message.Message):
-    """IntHistogramDataPoint is deprecated; use HistogramDataPoint.
-
-    This is a single data point in a timeseries that describes
-    the time-varying values of a Histogram of int values. A Histogram contains
-    summary statistics for a population of values, it may optionally contain
-    the distribution of those values across a set of buckets.
+class HistogramDataPoint(google.protobuf.message.Message):
+    """HistogramDataPoint is a single data point in a timeseries that describes the
+    time-varying values of a Histogram. A Histogram contains summary statistics
+    for a population of values, it may optionally contain the distribution of
+    those values across a set of buckets.
 
     If the histogram contains the distribution of values, then both
     "explicit_bounds" and "bucket counts" fields must be defined.
     If the histogram does not contain the distribution of values, then both
     "explicit_bounds" and "bucket_counts" must be omitted and only "count" and
     "sum" are known.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    LABELS_FIELD_NUMBER: builtins.int
+    ATTRIBUTES_FIELD_NUMBER: builtins.int
     START_TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     COUNT_FIELD_NUMBER: builtins.int
     SUM_FIELD_NUMBER: builtins.int
     BUCKET_COUNTS_FIELD_NUMBER: builtins.int
     EXPLICIT_BOUNDS_FIELD_NUMBER: builtins.int
     EXEMPLARS_FIELD_NUMBER: builtins.int
+    FLAGS_FIELD_NUMBER: builtins.int
     @property
-    def labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """The set of labels that uniquely identify this timeseries."""
+    def attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.KeyValue]:
+        """The set of key/value pairs that uniquely identify the timeseries from
+        where this point belongs. The list may be empty (may contain 0 elements).
+        """
         pass
     start_time_unix_nano: builtins.int = ...
     """StartTimeUnixNano is optional but strongly encouraged, see the
-    the detiled comments above Metric.
+    the detailed comments above Metric.
 
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
     1970.
     """
 
     time_unix_nano: builtins.int = ...
     """TimeUnixNano is required, see the detailed comments above Metric.
@@ -717,18 +638,23 @@
 
     count: builtins.int = ...
     """count is the number of values in the population. Must be non-negative. This
     value must be equal to the sum of the "count" fields in buckets if a
     histogram is provided.
     """
 
-    sum: builtins.int = ...
+    sum: builtins.float = ...
     """sum of the values in the population. If count is zero then this field
-    must be zero. This value must be equal to the sum of the "sum" fields in
-    buckets if a histogram is provided.
+    must be zero.
+
+    Note: Sum should only be filled out when measuring non-negative discrete
+    events, and is assumed to be monotonic over the values of these events.
+    Negative events *can* be recorded, but sum should not be filled out when
+    doing so.  This is specifically to enforce compatibility w/ OpenMetrics,
+    see: https://github.com/OpenObservability/OpenMetrics/blob/main/specification/OpenMetrics.md#histogram
     """
 
     @property
     def bucket_counts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """bucket_counts is an optional field contains the count values of histogram
         for each bucket.
 
@@ -738,170 +664,207 @@
         the number of elements in explicit_bounds array.
         """
         pass
     @property
     def explicit_bounds(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """explicit_bounds specifies buckets with explicitly defined bounds for values.
 
-        This defines size(explicit_bounds) + 1 (= N) buckets. The boundaries for
-        bucket at index i are:
+        The boundaries for bucket at index i are:
 
         (-infinity, explicit_bounds[i]] for i == 0
-        (explicit_bounds[i-1], explicit_bounds[i]] for 0 < i < N-1
-        (explicit_bounds[i], +infinity) for i == N-1
+        (explicit_bounds[i-1], explicit_bounds[i]] for 0 < i < size(explicit_bounds)
+        (explicit_bounds[i-1], +infinity) for i == size(explicit_bounds)
 
         The values in the explicit_bounds array must be strictly increasing.
 
         Histogram buckets are inclusive of their upper boundary, except the last
         bucket where the boundary is at infinity. This format is intentionally
         compatible with the OpenMetrics histogram definition.
         """
         pass
     @property
-    def exemplars(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntExemplar]:
+    def exemplars(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Exemplar]:
         """(Optional) List of exemplars collected from
         measurements that were used to form the data point
         """
         pass
+    flags: builtins.int = ...
+    """Flags that apply to this specific data point.  See DataPointFlags
+    for the available flags and their meaning.
+    """
+
     def __init__(self,
         *,
-        labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
+        attributes : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.KeyValue]] = ...,
         start_time_unix_nano : builtins.int = ...,
         time_unix_nano : builtins.int = ...,
         count : builtins.int = ...,
-        sum : builtins.int = ...,
+        sum : builtins.float = ...,
         bucket_counts : typing.Optional[typing.Iterable[builtins.int]] = ...,
         explicit_bounds : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        exemplars : typing.Optional[typing.Iterable[global___IntExemplar]] = ...,
+        exemplars : typing.Optional[typing.Iterable[global___Exemplar]] = ...,
+        flags : builtins.int = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bucket_counts",b"bucket_counts","count",b"count","exemplars",b"exemplars","explicit_bounds",b"explicit_bounds","labels",b"labels","start_time_unix_nano",b"start_time_unix_nano","sum",b"sum","time_unix_nano",b"time_unix_nano"]) -> None: ...
-global___IntHistogramDataPoint = IntHistogramDataPoint
+    def ClearField(self, field_name: typing_extensions.Literal["attributes",b"attributes","bucket_counts",b"bucket_counts","count",b"count","exemplars",b"exemplars","explicit_bounds",b"explicit_bounds","flags",b"flags","start_time_unix_nano",b"start_time_unix_nano","sum",b"sum","time_unix_nano",b"time_unix_nano"]) -> None: ...
+global___HistogramDataPoint = HistogramDataPoint
 
-class HistogramDataPoint(google.protobuf.message.Message):
-    """HistogramDataPoint is a single data point in a timeseries that describes the
-    time-varying values of a Histogram of double values. A Histogram contains
+class ExponentialHistogramDataPoint(google.protobuf.message.Message):
+    """ExponentialHistogramDataPoint is a single data point in a timeseries that describes the
+    time-varying values of a ExponentialHistogram of double values. A ExponentialHistogram contains
     summary statistics for a population of values, it may optionally contain the
     distribution of those values across a set of buckets.
-
-    If the histogram contains the distribution of values, then both
-    "explicit_bounds" and "bucket counts" fields must be defined.
-    If the histogram does not contain the distribution of values, then both
-    "explicit_bounds" and "bucket_counts" must be omitted and only "count" and
-    "sum" are known.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    class Buckets(google.protobuf.message.Message):
+        """Buckets are a set of bucket counts, encoded in a contiguous array
+        of counts.
+        """
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        OFFSET_FIELD_NUMBER: builtins.int
+        BUCKET_COUNTS_FIELD_NUMBER: builtins.int
+        offset: builtins.int = ...
+        """Offset is the bucket index of the first entry in the bucket_counts array.
+
+        Note: This uses a varint encoding as a simple form of compression.
+        """
+
+        @property
+        def bucket_counts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+            """Count is an array of counts, where count[i] carries the count
+            of the bucket at index (offset+i).  count[i] is the count of
+            values greater than or equal to base^(offset+i) and less than
+            base^(offset+i+1).
+
+            Note: By contrast, the explicit HistogramDataPoint uses
+            fixed64.  This field is expected to have many buckets,
+            especially zeros, so uint64 has been selected to ensure
+            varint encoding.
+            """
+            pass
+        def __init__(self,
+            *,
+            offset : builtins.int = ...,
+            bucket_counts : typing.Optional[typing.Iterable[builtins.int]] = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["bucket_counts",b"bucket_counts","offset",b"offset"]) -> None: ...
+
     ATTRIBUTES_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
     START_TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     COUNT_FIELD_NUMBER: builtins.int
     SUM_FIELD_NUMBER: builtins.int
-    BUCKET_COUNTS_FIELD_NUMBER: builtins.int
-    EXPLICIT_BOUNDS_FIELD_NUMBER: builtins.int
+    SCALE_FIELD_NUMBER: builtins.int
+    ZERO_COUNT_FIELD_NUMBER: builtins.int
+    POSITIVE_FIELD_NUMBER: builtins.int
+    NEGATIVE_FIELD_NUMBER: builtins.int
+    FLAGS_FIELD_NUMBER: builtins.int
     EXEMPLARS_FIELD_NUMBER: builtins.int
     @property
     def attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.KeyValue]:
         """The set of key/value pairs that uniquely identify the timeseries from
         where this point belongs. The list may be empty (may contain 0 elements).
         """
         pass
-    @property
-    def labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """Labels is deprecated and will be removed soon.
-        1. Old senders and receivers that are not aware of this change will
-        continue using the `labels` field.
-        2. New senders, which are aware of this change MUST send only `attributes`.
-        3. New receivers, which are aware of this change MUST convert this into
-        `labels` by simply converting all int64 values into float.
-
-        This field will be removed in ~3 months, on July 1, 2021.
-        """
-        pass
     start_time_unix_nano: builtins.int = ...
     """StartTimeUnixNano is optional but strongly encouraged, see the
-    the detiled comments above Metric.
+    the detailed comments above Metric.
 
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
     1970.
     """
 
     time_unix_nano: builtins.int = ...
     """TimeUnixNano is required, see the detailed comments above Metric.
 
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
     1970.
     """
 
     count: builtins.int = ...
-    """count is the number of values in the population. Must be non-negative. This
-    value must be equal to the sum of the "count" fields in buckets if a
-    histogram is provided.
+    """count is the number of values in the population. Must be
+    non-negative. This value must be equal to the sum of the "bucket_counts"
+    values in the positive and negative Buckets plus the "zero_count" field.
     """
 
     sum: builtins.float = ...
     """sum of the values in the population. If count is zero then this field
-    must be zero. This value must be equal to the sum of the "sum" fields in
-    buckets if a histogram is provided.
+    must be zero.
 
     Note: Sum should only be filled out when measuring non-negative discrete
     events, and is assumed to be monotonic over the values of these events.
     Negative events *can* be recorded, but sum should not be filled out when
     doing so.  This is specifically to enforce compatibility w/ OpenMetrics,
     see: https://github.com/OpenObservability/OpenMetrics/blob/main/specification/OpenMetrics.md#histogram
     """
 
-    @property
-    def bucket_counts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """bucket_counts is an optional field contains the count values of histogram
-        for each bucket.
+    scale: builtins.int = ...
+    """scale describes the resolution of the histogram.  Boundaries are
+    located at powers of the base, where:
 
-        The sum of the bucket_counts must equal the value in the count field.
+      base = (2^(2^-scale))
 
-        The number of elements in bucket_counts array must be by one greater than
-        the number of elements in explicit_bounds array.
-        """
-        pass
-    @property
-    def explicit_bounds(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
-        """explicit_bounds specifies buckets with explicitly defined bounds for values.
+    The histogram bucket identified by `index`, a signed integer,
+    contains values that are greater than or equal to (base^index) and
+    less than (base^(index+1)).
 
-        This defines size(explicit_bounds) + 1 (= N) buckets. The boundaries for
-        bucket at index i are:
+    The positive and negative ranges of the histogram are expressed
+    separately.  Negative values are mapped by their absolute value
+    into the negative range using the same scale as the positive range.
 
-        (-infinity, explicit_bounds[i]] for i == 0
-        (explicit_bounds[i-1], explicit_bounds[i]] for 0 < i < N-1
-        (explicit_bounds[i], +infinity) for i == N-1
+    scale is not restricted by the protocol, as the permissible
+    values depend on the range of the data.
+    """
 
-        The values in the explicit_bounds array must be strictly increasing.
+    zero_count: builtins.int = ...
+    """zero_count is the count of values that are either exactly zero or
+    within the region considered zero by the instrumentation at the
+    tolerated degree of precision.  This bucket stores values that
+    cannot be expressed using the standard exponential formula as
+    well as values that have been rounded to zero.
 
-        Histogram buckets are inclusive of their upper boundary, except the last
-        bucket where the boundary is at infinity. This format is intentionally
-        compatible with the OpenMetrics histogram definition.
-        """
+    Implementations MAY consider the zero bucket to have probability
+    mass equal to (zero_count / count).
+    """
+
+    @property
+    def positive(self) -> global___ExponentialHistogramDataPoint.Buckets:
+        """positive carries the positive range of exponential bucket counts."""
         pass
     @property
+    def negative(self) -> global___ExponentialHistogramDataPoint.Buckets:
+        """negative carries the negative range of exponential bucket counts."""
+        pass
+    flags: builtins.int = ...
+    """Flags that apply to this specific data point.  See DataPointFlags
+    for the available flags and their meaning.
+    """
+
+    @property
     def exemplars(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Exemplar]:
         """(Optional) List of exemplars collected from
         measurements that were used to form the data point
         """
         pass
     def __init__(self,
         *,
         attributes : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.KeyValue]] = ...,
-        labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
         start_time_unix_nano : builtins.int = ...,
         time_unix_nano : builtins.int = ...,
         count : builtins.int = ...,
         sum : builtins.float = ...,
-        bucket_counts : typing.Optional[typing.Iterable[builtins.int]] = ...,
-        explicit_bounds : typing.Optional[typing.Iterable[builtins.float]] = ...,
+        scale : builtins.int = ...,
+        zero_count : builtins.int = ...,
+        positive : typing.Optional[global___ExponentialHistogramDataPoint.Buckets] = ...,
+        negative : typing.Optional[global___ExponentialHistogramDataPoint.Buckets] = ...,
+        flags : builtins.int = ...,
         exemplars : typing.Optional[typing.Iterable[global___Exemplar]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["attributes",b"attributes","bucket_counts",b"bucket_counts","count",b"count","exemplars",b"exemplars","explicit_bounds",b"explicit_bounds","labels",b"labels","start_time_unix_nano",b"start_time_unix_nano","sum",b"sum","time_unix_nano",b"time_unix_nano"]) -> None: ...
-global___HistogramDataPoint = HistogramDataPoint
+    def HasField(self, field_name: typing_extensions.Literal["negative",b"negative","positive",b"positive"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["attributes",b"attributes","count",b"count","exemplars",b"exemplars","flags",b"flags","negative",b"negative","positive",b"positive","scale",b"scale","start_time_unix_nano",b"start_time_unix_nano","sum",b"sum","time_unix_nano",b"time_unix_nano","zero_count",b"zero_count"]) -> None: ...
+global___ExponentialHistogramDataPoint = ExponentialHistogramDataPoint
 
 class SummaryDataPoint(google.protobuf.message.Message):
     """SummaryDataPoint is a single data point in a timeseries that describes the
     time-varying values of a Summary metric.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     class ValueAtQuantile(google.protobuf.message.Message):
@@ -932,41 +895,29 @@
             *,
             quantile : builtins.float = ...,
             value : builtins.float = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["quantile",b"quantile","value",b"value"]) -> None: ...
 
     ATTRIBUTES_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
     START_TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     COUNT_FIELD_NUMBER: builtins.int
     SUM_FIELD_NUMBER: builtins.int
     QUANTILE_VALUES_FIELD_NUMBER: builtins.int
+    FLAGS_FIELD_NUMBER: builtins.int
     @property
     def attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.KeyValue]:
         """The set of key/value pairs that uniquely identify the timeseries from
         where this point belongs. The list may be empty (may contain 0 elements).
         """
         pass
-    @property
-    def labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """Labels is deprecated and will be removed soon.
-        1. Old senders and receivers that are not aware of this change will
-        continue using the `labels` field.
-        2. New senders, which are aware of this change MUST send only `attributes`.
-        3. New receivers, which are aware of this change MUST convert this into
-        `labels` by simply converting all int64 values into float.
-
-        This field will be removed in ~3 months, on July 1, 2021.
-        """
-        pass
     start_time_unix_nano: builtins.int = ...
     """StartTimeUnixNano is optional but strongly encouraged, see the
-    the detiled comments above Metric.
+    the detailed comments above Metric.
 
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
     1970.
     """
 
     time_unix_nano: builtins.int = ...
     """TimeUnixNano is required, see the detailed comments above Metric.
@@ -991,113 +942,52 @@
 
     @property
     def quantile_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SummaryDataPoint.ValueAtQuantile]:
         """(Optional) list of values at different quantiles of the distribution calculated
         from the current snapshot. The quantiles must be strictly increasing.
         """
         pass
+    flags: builtins.int = ...
+    """Flags that apply to this specific data point.  See DataPointFlags
+    for the available flags and their meaning.
+    """
+
     def __init__(self,
         *,
         attributes : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.KeyValue]] = ...,
-        labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
         start_time_unix_nano : builtins.int = ...,
         time_unix_nano : builtins.int = ...,
         count : builtins.int = ...,
         sum : builtins.float = ...,
         quantile_values : typing.Optional[typing.Iterable[global___SummaryDataPoint.ValueAtQuantile]] = ...,
+        flags : builtins.int = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["attributes",b"attributes","count",b"count","labels",b"labels","quantile_values",b"quantile_values","start_time_unix_nano",b"start_time_unix_nano","sum",b"sum","time_unix_nano",b"time_unix_nano"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["attributes",b"attributes","count",b"count","flags",b"flags","quantile_values",b"quantile_values","start_time_unix_nano",b"start_time_unix_nano","sum",b"sum","time_unix_nano",b"time_unix_nano"]) -> None: ...
 global___SummaryDataPoint = SummaryDataPoint
 
-class IntExemplar(google.protobuf.message.Message):
-    """A representation of an exemplar, which is a sample input int measurement.
-    Exemplars also hold information about the environment when the measurement
-    was recorded, for example the span and trace ID of the active span when the
-    exemplar was recorded.
-    """
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    FILTERED_LABELS_FIELD_NUMBER: builtins.int
-    TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
-    VALUE_FIELD_NUMBER: builtins.int
-    SPAN_ID_FIELD_NUMBER: builtins.int
-    TRACE_ID_FIELD_NUMBER: builtins.int
-    @property
-    def filtered_labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """The set of labels that were filtered out by the aggregator, but recorded
-        alongside the original measurement. Only labels that were filtered out
-        by the aggregator should be included
-        """
-        pass
-    time_unix_nano: builtins.int = ...
-    """time_unix_nano is the exact time when this exemplar was recorded
-
-    Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
-    1970.
-    """
-
-    value: builtins.int = ...
-    """Numerical int value of the measurement that was recorded."""
-
-    span_id: builtins.bytes = ...
-    """(Optional) Span ID of the exemplar trace.
-    span_id may be missing if the measurement is not recorded inside a trace
-    or if the trace is not sampled.
-    """
-
-    trace_id: builtins.bytes = ...
-    """(Optional) Trace ID of the exemplar trace.
-    trace_id may be missing if the measurement is not recorded inside a trace
-    or if the trace is not sampled.
-    """
-
-    def __init__(self,
-        *,
-        filtered_labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
-        time_unix_nano : builtins.int = ...,
-        value : builtins.int = ...,
-        span_id : builtins.bytes = ...,
-        trace_id : builtins.bytes = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["filtered_labels",b"filtered_labels","span_id",b"span_id","time_unix_nano",b"time_unix_nano","trace_id",b"trace_id","value",b"value"]) -> None: ...
-global___IntExemplar = IntExemplar
-
 class Exemplar(google.protobuf.message.Message):
     """A representation of an exemplar, which is a sample input measurement.
     Exemplars also hold information about the environment when the measurement
     was recorded, for example the span and trace ID of the active span when the
     exemplar was recorded.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     FILTERED_ATTRIBUTES_FIELD_NUMBER: builtins.int
-    FILTERED_LABELS_FIELD_NUMBER: builtins.int
     TIME_UNIX_NANO_FIELD_NUMBER: builtins.int
     AS_DOUBLE_FIELD_NUMBER: builtins.int
     AS_INT_FIELD_NUMBER: builtins.int
     SPAN_ID_FIELD_NUMBER: builtins.int
     TRACE_ID_FIELD_NUMBER: builtins.int
     @property
     def filtered_attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.KeyValue]:
         """The set of key/value pairs that were filtered out by the aggregator, but
         recorded alongside the original measurement. Only key/value pairs that were
         filtered out by the aggregator should be included
         """
         pass
-    @property
-    def filtered_labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]:
-        """Labels is deprecated and will be removed soon.
-        1. Old senders and receivers that are not aware of this change will
-        continue using the `filtered_labels` field.
-        2. New senders, which are aware of this change MUST send only
-        `filtered_attributes`.
-        3. New receivers, which are aware of this change MUST convert this into
-        `filtered_labels` by simply converting all int64 values into float.
-
-        This field will be removed in ~3 months, on July 1, 2021.
-        """
-        pass
     time_unix_nano: builtins.int = ...
     """time_unix_nano is the exact time when this exemplar was recorded
 
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January
     1970.
     """
 
@@ -1114,18 +1004,17 @@
     trace_id may be missing if the measurement is not recorded inside a trace
     or if the trace is not sampled.
     """
 
     def __init__(self,
         *,
         filtered_attributes : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.KeyValue]] = ...,
-        filtered_labels : typing.Optional[typing.Iterable[opentelemetry.proto.common.v1.common_pb2.StringKeyValue]] = ...,
         time_unix_nano : builtins.int = ...,
         as_double : builtins.float = ...,
         as_int : builtins.int = ...,
         span_id : builtins.bytes = ...,
         trace_id : builtins.bytes = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["as_double",b"as_double","as_int",b"as_int","value",b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["as_double",b"as_double","as_int",b"as_int","filtered_attributes",b"filtered_attributes","filtered_labels",b"filtered_labels","span_id",b"span_id","time_unix_nano",b"time_unix_nano","trace_id",b"trace_id","value",b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["as_double",b"as_double","as_int",b"as_int","filtered_attributes",b"filtered_attributes","span_id",b"span_id","time_unix_nano",b"time_unix_nano","trace_id",b"trace_id","value",b"value"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["value",b"value"]) -> typing.Optional[typing_extensions.Literal["as_double","as_int"]]: ...
 global___Exemplar = Exemplar
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/v1/resource_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/resource/v1/resource_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/resource/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_config_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_config_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_config_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_pb2.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='opentelemetry/proto/trace/v1/trace.proto',
   package='opentelemetry.proto.trace.v1',
   syntax='proto3',
   serialized_options=b'\n\037io.opentelemetry.proto.trace.v1B\nTraceProtoP\001Z=github.com/open-telemetry/opentelemetry-proto/gen/go/trace/v1',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n(opentelemetry/proto/trace/v1/trace.proto\x12\x1copentelemetry.proto.trace.v1\x1a*opentelemetry/proto/common/v1/common.proto\x1a.opentelemetry/proto/resource/v1/resource.proto\"\xc2\x01\n\rResourceSpans\x12;\n\x08resource\x18\x01 \x01(\x0b\x32).opentelemetry.proto.resource.v1.Resource\x12`\n\x1dinstrumentation_library_spans\x18\x02 \x03(\x0b\x32\x39.opentelemetry.proto.trace.v1.InstrumentationLibrarySpans\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xbc\x01\n\x1bInstrumentationLibrarySpans\x12V\n\x17instrumentation_library\x18\x01 \x01(\x0b\x32\x35.opentelemetry.proto.common.v1.InstrumentationLibrary\x12\x31\n\x05spans\x18\x02 \x03(\x0b\x32\".opentelemetry.proto.trace.v1.Span\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xe6\x07\n\x04Span\x12\x10\n\x08trace_id\x18\x01 \x01(\x0c\x12\x0f\n\x07span_id\x18\x02 \x01(\x0c\x12\x13\n\x0btrace_state\x18\x03 \x01(\t\x12\x16\n\x0eparent_span_id\x18\x04 \x01(\x0c\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x39\n\x04kind\x18\x06 \x01(\x0e\x32+.opentelemetry.proto.trace.v1.Span.SpanKind\x12\x1c\n\x14start_time_unix_nano\x18\x07 \x01(\x06\x12\x1a\n\x12\x65nd_time_unix_nano\x18\x08 \x01(\x06\x12;\n\nattributes\x18\t \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\n \x01(\r\x12\x38\n\x06\x65vents\x18\x0b \x03(\x0b\x32(.opentelemetry.proto.trace.v1.Span.Event\x12\x1c\n\x14\x64ropped_events_count\x18\x0c \x01(\r\x12\x36\n\x05links\x18\r \x03(\x0b\x32\'.opentelemetry.proto.trace.v1.Span.Link\x12\x1b\n\x13\x64ropped_links_count\x18\x0e \x01(\r\x12\x34\n\x06status\x18\x0f \x01(\x0b\x32$.opentelemetry.proto.trace.v1.Status\x1a\x8c\x01\n\x05\x45vent\x12\x16\n\x0etime_unix_nano\x18\x01 \x01(\x06\x12\x0c\n\x04name\x18\x02 \x01(\t\x12;\n\nattributes\x18\x03 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x04 \x01(\r\x1a\x9d\x01\n\x04Link\x12\x10\n\x08trace_id\x18\x01 \x01(\x0c\x12\x0f\n\x07span_id\x18\x02 \x01(\x0c\x12\x13\n\x0btrace_state\x18\x03 \x01(\t\x12;\n\nattributes\x18\x04 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x05 \x01(\r\"\x99\x01\n\x08SpanKind\x12\x19\n\x15SPAN_KIND_UNSPECIFIED\x10\x00\x12\x16\n\x12SPAN_KIND_INTERNAL\x10\x01\x12\x14\n\x10SPAN_KIND_SERVER\x10\x02\x12\x14\n\x10SPAN_KIND_CLIENT\x10\x03\x12\x16\n\x12SPAN_KIND_PRODUCER\x10\x04\x12\x16\n\x12SPAN_KIND_CONSUMER\x10\x05\"\xdd\x07\n\x06Status\x12V\n\x0f\x64\x65precated_code\x18\x01 \x01(\x0e\x32\x39.opentelemetry.proto.trace.v1.Status.DeprecatedStatusCodeB\x02\x18\x01\x12\x0f\n\x07message\x18\x02 \x01(\t\x12=\n\x04\x63ode\x18\x03 \x01(\x0e\x32/.opentelemetry.proto.trace.v1.Status.StatusCode\"\xda\x05\n\x14\x44\x65precatedStatusCode\x12\x1d\n\x19\x44\x45PRECATED_STATUS_CODE_OK\x10\x00\x12$\n DEPRECATED_STATUS_CODE_CANCELLED\x10\x01\x12(\n$DEPRECATED_STATUS_CODE_UNKNOWN_ERROR\x10\x02\x12+\n\'DEPRECATED_STATUS_CODE_INVALID_ARGUMENT\x10\x03\x12,\n(DEPRECATED_STATUS_CODE_DEADLINE_EXCEEDED\x10\x04\x12$\n DEPRECATED_STATUS_CODE_NOT_FOUND\x10\x05\x12)\n%DEPRECATED_STATUS_CODE_ALREADY_EXISTS\x10\x06\x12,\n(DEPRECATED_STATUS_CODE_PERMISSION_DENIED\x10\x07\x12-\n)DEPRECATED_STATUS_CODE_RESOURCE_EXHAUSTED\x10\x08\x12.\n*DEPRECATED_STATUS_CODE_FAILED_PRECONDITION\x10\t\x12\"\n\x1e\x44\x45PRECATED_STATUS_CODE_ABORTED\x10\n\x12\'\n#DEPRECATED_STATUS_CODE_OUT_OF_RANGE\x10\x0b\x12(\n$DEPRECATED_STATUS_CODE_UNIMPLEMENTED\x10\x0c\x12)\n%DEPRECATED_STATUS_CODE_INTERNAL_ERROR\x10\r\x12&\n\"DEPRECATED_STATUS_CODE_UNAVAILABLE\x10\x0e\x12$\n DEPRECATED_STATUS_CODE_DATA_LOSS\x10\x0f\x12*\n&DEPRECATED_STATUS_CODE_UNAUTHENTICATED\x10\x10\"N\n\nStatusCode\x12\x15\n\x11STATUS_CODE_UNSET\x10\x00\x12\x12\n\x0eSTATUS_CODE_OK\x10\x01\x12\x15\n\x11STATUS_CODE_ERROR\x10\x02\x42n\n\x1fio.opentelemetry.proto.trace.v1B\nTraceProtoP\x01Z=github.com/open-telemetry/opentelemetry-proto/gen/go/trace/v1b\x06proto3'
+  serialized_pb=b'\n(opentelemetry/proto/trace/v1/trace.proto\x12\x1copentelemetry.proto.trace.v1\x1a*opentelemetry/proto/common/v1/common.proto\x1a.opentelemetry/proto/resource/v1/resource.proto\"Q\n\nTracesData\x12\x43\n\x0eresource_spans\x18\x01 \x03(\x0b\x32+.opentelemetry.proto.trace.v1.ResourceSpans\"\xc2\x01\n\rResourceSpans\x12;\n\x08resource\x18\x01 \x01(\x0b\x32).opentelemetry.proto.resource.v1.Resource\x12`\n\x1dinstrumentation_library_spans\x18\x02 \x03(\x0b\x32\x39.opentelemetry.proto.trace.v1.InstrumentationLibrarySpans\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xbc\x01\n\x1bInstrumentationLibrarySpans\x12V\n\x17instrumentation_library\x18\x01 \x01(\x0b\x32\x35.opentelemetry.proto.common.v1.InstrumentationLibrary\x12\x31\n\x05spans\x18\x02 \x03(\x0b\x32\".opentelemetry.proto.trace.v1.Span\x12\x12\n\nschema_url\x18\x03 \x01(\t\"\xe6\x07\n\x04Span\x12\x10\n\x08trace_id\x18\x01 \x01(\x0c\x12\x0f\n\x07span_id\x18\x02 \x01(\x0c\x12\x13\n\x0btrace_state\x18\x03 \x01(\t\x12\x16\n\x0eparent_span_id\x18\x04 \x01(\x0c\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x39\n\x04kind\x18\x06 \x01(\x0e\x32+.opentelemetry.proto.trace.v1.Span.SpanKind\x12\x1c\n\x14start_time_unix_nano\x18\x07 \x01(\x06\x12\x1a\n\x12\x65nd_time_unix_nano\x18\x08 \x01(\x06\x12;\n\nattributes\x18\t \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\n \x01(\r\x12\x38\n\x06\x65vents\x18\x0b \x03(\x0b\x32(.opentelemetry.proto.trace.v1.Span.Event\x12\x1c\n\x14\x64ropped_events_count\x18\x0c \x01(\r\x12\x36\n\x05links\x18\r \x03(\x0b\x32\'.opentelemetry.proto.trace.v1.Span.Link\x12\x1b\n\x13\x64ropped_links_count\x18\x0e \x01(\r\x12\x34\n\x06status\x18\x0f \x01(\x0b\x32$.opentelemetry.proto.trace.v1.Status\x1a\x8c\x01\n\x05\x45vent\x12\x16\n\x0etime_unix_nano\x18\x01 \x01(\x06\x12\x0c\n\x04name\x18\x02 \x01(\t\x12;\n\nattributes\x18\x03 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x04 \x01(\r\x1a\x9d\x01\n\x04Link\x12\x10\n\x08trace_id\x18\x01 \x01(\x0c\x12\x0f\n\x07span_id\x18\x02 \x01(\x0c\x12\x13\n\x0btrace_state\x18\x03 \x01(\t\x12;\n\nattributes\x18\x04 \x03(\x0b\x32\'.opentelemetry.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x05 \x01(\r\"\x99\x01\n\x08SpanKind\x12\x19\n\x15SPAN_KIND_UNSPECIFIED\x10\x00\x12\x16\n\x12SPAN_KIND_INTERNAL\x10\x01\x12\x14\n\x10SPAN_KIND_SERVER\x10\x02\x12\x14\n\x10SPAN_KIND_CLIENT\x10\x03\x12\x16\n\x12SPAN_KIND_PRODUCER\x10\x04\x12\x16\n\x12SPAN_KIND_CONSUMER\x10\x05\"\xae\x01\n\x06Status\x12\x0f\n\x07message\x18\x02 \x01(\t\x12=\n\x04\x63ode\x18\x03 \x01(\x0e\x32/.opentelemetry.proto.trace.v1.Status.StatusCode\"N\n\nStatusCode\x12\x15\n\x11STATUS_CODE_UNSET\x10\x00\x12\x12\n\x0eSTATUS_CODE_OK\x10\x01\x12\x15\n\x11STATUS_CODE_ERROR\x10\x02J\x04\x08\x01\x10\x02\x42n\n\x1fio.opentelemetry.proto.trace.v1B\nTraceProtoP\x01Z=github.com/open-telemetry/opentelemetry-proto/gen/go/trace/v1b\x06proto3'
   ,
   dependencies=[opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2.DESCRIPTOR,opentelemetry_dot_proto_dot_resource_dot_v1_dot_resource__pb2.DESCRIPTOR,])
 
 
 
 _SPAN_SPANKIND = _descriptor.EnumDescriptor(
   name='SpanKind',
@@ -63,119 +63,19 @@
       name='SPAN_KIND_CONSUMER', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1400,
-  serialized_end=1553,
+  serialized_start=1483,
+  serialized_end=1636,
 )
 _sym_db.RegisterEnumDescriptor(_SPAN_SPANKIND)
 
-_STATUS_DEPRECATEDSTATUSCODE = _descriptor.EnumDescriptor(
-  name='DeprecatedStatusCode',
-  full_name='opentelemetry.proto.trace.v1.Status.DeprecatedStatusCode',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_OK', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_CANCELLED', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_UNKNOWN_ERROR', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_INVALID_ARGUMENT', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_DEADLINE_EXCEEDED', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_NOT_FOUND', index=5, number=5,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_ALREADY_EXISTS', index=6, number=6,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_PERMISSION_DENIED', index=7, number=7,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_RESOURCE_EXHAUSTED', index=8, number=8,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_FAILED_PRECONDITION', index=9, number=9,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_ABORTED', index=10, number=10,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_OUT_OF_RANGE', index=11, number=11,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_UNIMPLEMENTED', index=12, number=12,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_INTERNAL_ERROR', index=13, number=13,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_UNAVAILABLE', index=14, number=14,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_DATA_LOSS', index=15, number=15,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DEPRECATED_STATUS_CODE_UNAUTHENTICATED', index=16, number=16,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=1735,
-  serialized_end=2465,
-)
-_sym_db.RegisterEnumDescriptor(_STATUS_DEPRECATEDSTATUSCODE)
-
 _STATUS_STATUSCODE = _descriptor.EnumDescriptor(
   name='StatusCode',
   full_name='opentelemetry.proto.trace.v1.Status.StatusCode',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
@@ -193,20 +93,52 @@
       name='STATUS_CODE_ERROR', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2467,
-  serialized_end=2545,
+  serialized_start=1729,
+  serialized_end=1807,
 )
 _sym_db.RegisterEnumDescriptor(_STATUS_STATUSCODE)
 
 
+_TRACESDATA = _descriptor.Descriptor(
+  name='TracesData',
+  full_name='opentelemetry.proto.trace.v1.TracesData',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='resource_spans', full_name='opentelemetry.proto.trace.v1.TracesData.resource_spans', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=166,
+  serialized_end=247,
+)
+
+
 _RESOURCESPANS = _descriptor.Descriptor(
   name='ResourceSpans',
   full_name='opentelemetry.proto.trace.v1.ResourceSpans',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -240,16 +172,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=167,
-  serialized_end=361,
+  serialized_start=250,
+  serialized_end=444,
 )
 
 
 _INSTRUMENTATIONLIBRARYSPANS = _descriptor.Descriptor(
   name='InstrumentationLibrarySpans',
   full_name='opentelemetry.proto.trace.v1.InstrumentationLibrarySpans',
   filename=None,
@@ -286,16 +218,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=364,
-  serialized_end=552,
+  serialized_start=447,
+  serialized_end=635,
 )
 
 
 _SPAN_EVENT = _descriptor.Descriptor(
   name='Event',
   full_name='opentelemetry.proto.trace.v1.Span.Event',
   filename=None,
@@ -339,16 +271,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1097,
-  serialized_end=1237,
+  serialized_start=1180,
+  serialized_end=1320,
 )
 
 _SPAN_LINK = _descriptor.Descriptor(
   name='Link',
   full_name='opentelemetry.proto.trace.v1.Span.Link',
   filename=None,
   file=DESCRIPTOR,
@@ -398,16 +330,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1240,
-  serialized_end=1397,
+  serialized_start=1323,
+  serialized_end=1480,
 )
 
 _SPAN = _descriptor.Descriptor(
   name='Span',
   full_name='opentelemetry.proto.trace.v1.Span',
   filename=None,
   file=DESCRIPTOR,
@@ -528,90 +460,89 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=555,
-  serialized_end=1553,
+  serialized_start=638,
+  serialized_end=1636,
 )
 
 
 _STATUS = _descriptor.Descriptor(
   name='Status',
   full_name='opentelemetry.proto.trace.v1.Status',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='deprecated_code', full_name='opentelemetry.proto.trace.v1.Status.deprecated_code', index=0,
-      number=1, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\030\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='message', full_name='opentelemetry.proto.trace.v1.Status.message', index=1,
+      name='message', full_name='opentelemetry.proto.trace.v1.Status.message', index=0,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='code', full_name='opentelemetry.proto.trace.v1.Status.code', index=2,
+      name='code', full_name='opentelemetry.proto.trace.v1.Status.code', index=1,
       number=3, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
-    _STATUS_DEPRECATEDSTATUSCODE,
     _STATUS_STATUSCODE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1556,
-  serialized_end=2545,
+  serialized_start=1639,
+  serialized_end=1813,
 )
 
+_TRACESDATA.fields_by_name['resource_spans'].message_type = _RESOURCESPANS
 _RESOURCESPANS.fields_by_name['resource'].message_type = opentelemetry_dot_proto_dot_resource_dot_v1_dot_resource__pb2._RESOURCE
 _RESOURCESPANS.fields_by_name['instrumentation_library_spans'].message_type = _INSTRUMENTATIONLIBRARYSPANS
 _INSTRUMENTATIONLIBRARYSPANS.fields_by_name['instrumentation_library'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._INSTRUMENTATIONLIBRARY
 _INSTRUMENTATIONLIBRARYSPANS.fields_by_name['spans'].message_type = _SPAN
 _SPAN_EVENT.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
 _SPAN_EVENT.containing_type = _SPAN
 _SPAN_LINK.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
 _SPAN_LINK.containing_type = _SPAN
 _SPAN.fields_by_name['kind'].enum_type = _SPAN_SPANKIND
 _SPAN.fields_by_name['attributes'].message_type = opentelemetry_dot_proto_dot_common_dot_v1_dot_common__pb2._KEYVALUE
 _SPAN.fields_by_name['events'].message_type = _SPAN_EVENT
 _SPAN.fields_by_name['links'].message_type = _SPAN_LINK
 _SPAN.fields_by_name['status'].message_type = _STATUS
 _SPAN_SPANKIND.containing_type = _SPAN
-_STATUS.fields_by_name['deprecated_code'].enum_type = _STATUS_DEPRECATEDSTATUSCODE
 _STATUS.fields_by_name['code'].enum_type = _STATUS_STATUSCODE
-_STATUS_DEPRECATEDSTATUSCODE.containing_type = _STATUS
 _STATUS_STATUSCODE.containing_type = _STATUS
+DESCRIPTOR.message_types_by_name['TracesData'] = _TRACESDATA
 DESCRIPTOR.message_types_by_name['ResourceSpans'] = _RESOURCESPANS
 DESCRIPTOR.message_types_by_name['InstrumentationLibrarySpans'] = _INSTRUMENTATIONLIBRARYSPANS
 DESCRIPTOR.message_types_by_name['Span'] = _SPAN
 DESCRIPTOR.message_types_by_name['Status'] = _STATUS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+TracesData = _reflection.GeneratedProtocolMessageType('TracesData', (_message.Message,), {
+  'DESCRIPTOR' : _TRACESDATA,
+  '__module__' : 'opentelemetry.proto.trace.v1.trace_pb2'
+  # @@protoc_insertion_point(class_scope:opentelemetry.proto.trace.v1.TracesData)
+  })
+_sym_db.RegisterMessage(TracesData)
+
 ResourceSpans = _reflection.GeneratedProtocolMessageType('ResourceSpans', (_message.Message,), {
   'DESCRIPTOR' : _RESOURCESPANS,
   '__module__' : 'opentelemetry.proto.trace.v1.trace_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.trace.v1.ResourceSpans)
   })
 _sym_db.RegisterMessage(ResourceSpans)
 
@@ -650,9 +581,8 @@
   '__module__' : 'opentelemetry.proto.trace.v1.trace_pb2'
   # @@protoc_insertion_point(class_scope:opentelemetry.proto.trace.v1.Status)
   })
 _sym_db.RegisterMessage(Status)
 
 
 DESCRIPTOR._options = None
-_STATUS.fields_by_name['deprecated_code']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/trace/v1/trace_pb2.pyi` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/trace/v1/trace_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,44 @@
 import opentelemetry.proto.common.v1.common_pb2
 import opentelemetry.proto.resource.v1.resource_pb2
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
+class TracesData(google.protobuf.message.Message):
+    """TracesData represents the traces data that can be stored in a persistent storage,
+    OR can be embedded by other protocols that transfer OTLP traces data but do
+    not implement the OTLP protocol.
+
+    The main difference between this message and collector protocol is that
+    in this message there will not be any "control" or "metadata" specific to
+    OTLP protocol.
+
+    When new fields are added into this message, the OTLP request MUST be updated
+    as well.
+    """
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    RESOURCE_SPANS_FIELD_NUMBER: builtins.int
+    @property
+    def resource_spans(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceSpans]:
+        """An array of ResourceSpans.
+        For data coming from a single resource this array will typically contain
+        one element. Intermediary nodes that receive data from multiple origins
+        typically batch the data before forwarding further and in that case this
+        array will contain multiple elements.
+        """
+        pass
+    def __init__(self,
+        *,
+        resource_spans : typing.Optional[typing.Iterable[global___ResourceSpans]] = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resource_spans",b"resource_spans"]) -> None: ...
+global___TracesData = TracesData
+
 class ResourceSpans(google.protobuf.message.Message):
     """A collection of InstrumentationLibrarySpans from a Resource."""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     RESOURCE_FIELD_NUMBER: builtins.int
     INSTRUMENTATION_LIBRARY_SPANS_FIELD_NUMBER: builtins.int
     SCHEMA_URL_FIELD_NUMBER: builtins.int
     @property
@@ -291,17 +321,15 @@
 
     For example, the name can be a qualified method name or a file name
     and a line number where the operation is called. A best practice is to use
     the same display name at the same call point in an application.
     This makes it easier to correlate spans in different traces.
 
     This field is semantically required to be set to non-empty string.
-    When null or empty string received - receiver may use string "name"
-    as a replacement. There might be smarted algorithms implemented by
-    receiver to fix the empty span name.
+    Empty value is equivalent to an unknown span name.
 
     This field is required.
     """
 
     kind: global___Span.SpanKind.V = ...
     """Distinguishes between spans generated in a particular context. For example,
     two spans with the same name may be distinguished using `CLIENT` (caller)
@@ -324,22 +352,24 @@
     Value is UNIX Epoch time in nanoseconds since 00:00:00 UTC on 1 January 1970.
 
     This field is semantically required and it is expected that end_time >= start_time.
     """
 
     @property
     def attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[opentelemetry.proto.common.v1.common_pb2.KeyValue]:
-        """attributes is a collection of key/value pairs. The value can be a string,
-        an integer, a double or the Boolean values `true` or `false`. Note, global attributes
+        """attributes is a collection of key/value pairs. Note, global attributes
         like server name can be set using the resource API. Examples of attributes:
 
             "/http/user_agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/71.0.3578.98 Safari/537.36"
             "/http/server_latency": 300
             "abc.com/myattribute": true
             "abc.com/score": 10.239
+
+        The OpenTelemetry API specification further restricts the allowed value types:
+        https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/common/common.md#attributes
         """
         pass
     dropped_attributes_count: builtins.int = ...
     """dropped_attributes_count is the number of attributes that were discarded. Attributes
     can be discarded because their keys are too long or because there are too many
     attributes. If this value is 0, then no attributes were dropped.
     """
@@ -391,96 +421,16 @@
     def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["attributes",b"attributes","dropped_attributes_count",b"dropped_attributes_count","dropped_events_count",b"dropped_events_count","dropped_links_count",b"dropped_links_count","end_time_unix_nano",b"end_time_unix_nano","events",b"events","kind",b"kind","links",b"links","name",b"name","parent_span_id",b"parent_span_id","span_id",b"span_id","start_time_unix_nano",b"start_time_unix_nano","status",b"status","trace_id",b"trace_id","trace_state",b"trace_state"]) -> None: ...
 global___Span = Span
 
 class Status(google.protobuf.message.Message):
     """The Status type defines a logical error model that is suitable for different
     programming environments, including REST APIs and RPC APIs.
-    IMPORTANT: Backward compatibility notes:
-
-    To ensure any pair of senders and receivers continues to correctly signal and
-    interpret erroneous situations, the senders and receivers MUST follow these rules:
-
-    1. Old senders and receivers that are not aware of `code` field will continue using
-    the `deprecated_code` field to signal and interpret erroneous situation.
-
-    2. New senders, which are aware of the `code` field MUST set both the
-    `deprecated_code` and `code` fields according to the following rules:
-
-      if code==STATUS_CODE_UNSET then `deprecated_code` MUST be
-      set to DEPRECATED_STATUS_CODE_OK.
-
-      if code==STATUS_CODE_OK then `deprecated_code` MUST be
-      set to DEPRECATED_STATUS_CODE_OK.
-
-      if code==STATUS_CODE_ERROR then `deprecated_code` MUST be
-      set to DEPRECATED_STATUS_CODE_UNKNOWN_ERROR.
-
-    These rules allow old receivers to correctly interpret data received from new senders.
-
-    3. New receivers MUST look at both the `code` and `deprecated_code` fields in order
-    to interpret the overall status:
-
-      If code==STATUS_CODE_UNSET then the value of `deprecated_code` is the
-      carrier of the overall status according to these rules:
-
-        if deprecated_code==DEPRECATED_STATUS_CODE_OK then the receiver MUST interpret
-        the overall status to be STATUS_CODE_UNSET.
-
-        if deprecated_code!=DEPRECATED_STATUS_CODE_OK then the receiver MUST interpret
-        the overall status to be STATUS_CODE_ERROR.
-
-      If code!=STATUS_CODE_UNSET then the value of `deprecated_code` MUST be
-      ignored, the `code` field is the sole carrier of the status.
-
-    These rules allow new receivers to correctly interpret data received from old senders.
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class DeprecatedStatusCode(_DeprecatedStatusCode, metaclass=_DeprecatedStatusCodeEnumTypeWrapper):
-        pass
-    class _DeprecatedStatusCode:
-        V = typing.NewType('V', builtins.int)
-    class _DeprecatedStatusCodeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DeprecatedStatusCode.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        DEPRECATED_STATUS_CODE_OK = Status.DeprecatedStatusCode.V(0)
-        DEPRECATED_STATUS_CODE_CANCELLED = Status.DeprecatedStatusCode.V(1)
-        DEPRECATED_STATUS_CODE_UNKNOWN_ERROR = Status.DeprecatedStatusCode.V(2)
-        DEPRECATED_STATUS_CODE_INVALID_ARGUMENT = Status.DeprecatedStatusCode.V(3)
-        DEPRECATED_STATUS_CODE_DEADLINE_EXCEEDED = Status.DeprecatedStatusCode.V(4)
-        DEPRECATED_STATUS_CODE_NOT_FOUND = Status.DeprecatedStatusCode.V(5)
-        DEPRECATED_STATUS_CODE_ALREADY_EXISTS = Status.DeprecatedStatusCode.V(6)
-        DEPRECATED_STATUS_CODE_PERMISSION_DENIED = Status.DeprecatedStatusCode.V(7)
-        DEPRECATED_STATUS_CODE_RESOURCE_EXHAUSTED = Status.DeprecatedStatusCode.V(8)
-        DEPRECATED_STATUS_CODE_FAILED_PRECONDITION = Status.DeprecatedStatusCode.V(9)
-        DEPRECATED_STATUS_CODE_ABORTED = Status.DeprecatedStatusCode.V(10)
-        DEPRECATED_STATUS_CODE_OUT_OF_RANGE = Status.DeprecatedStatusCode.V(11)
-        DEPRECATED_STATUS_CODE_UNIMPLEMENTED = Status.DeprecatedStatusCode.V(12)
-        DEPRECATED_STATUS_CODE_INTERNAL_ERROR = Status.DeprecatedStatusCode.V(13)
-        DEPRECATED_STATUS_CODE_UNAVAILABLE = Status.DeprecatedStatusCode.V(14)
-        DEPRECATED_STATUS_CODE_DATA_LOSS = Status.DeprecatedStatusCode.V(15)
-        DEPRECATED_STATUS_CODE_UNAUTHENTICATED = Status.DeprecatedStatusCode.V(16)
-
-    DEPRECATED_STATUS_CODE_OK = Status.DeprecatedStatusCode.V(0)
-    DEPRECATED_STATUS_CODE_CANCELLED = Status.DeprecatedStatusCode.V(1)
-    DEPRECATED_STATUS_CODE_UNKNOWN_ERROR = Status.DeprecatedStatusCode.V(2)
-    DEPRECATED_STATUS_CODE_INVALID_ARGUMENT = Status.DeprecatedStatusCode.V(3)
-    DEPRECATED_STATUS_CODE_DEADLINE_EXCEEDED = Status.DeprecatedStatusCode.V(4)
-    DEPRECATED_STATUS_CODE_NOT_FOUND = Status.DeprecatedStatusCode.V(5)
-    DEPRECATED_STATUS_CODE_ALREADY_EXISTS = Status.DeprecatedStatusCode.V(6)
-    DEPRECATED_STATUS_CODE_PERMISSION_DENIED = Status.DeprecatedStatusCode.V(7)
-    DEPRECATED_STATUS_CODE_RESOURCE_EXHAUSTED = Status.DeprecatedStatusCode.V(8)
-    DEPRECATED_STATUS_CODE_FAILED_PRECONDITION = Status.DeprecatedStatusCode.V(9)
-    DEPRECATED_STATUS_CODE_ABORTED = Status.DeprecatedStatusCode.V(10)
-    DEPRECATED_STATUS_CODE_OUT_OF_RANGE = Status.DeprecatedStatusCode.V(11)
-    DEPRECATED_STATUS_CODE_UNIMPLEMENTED = Status.DeprecatedStatusCode.V(12)
-    DEPRECATED_STATUS_CODE_INTERNAL_ERROR = Status.DeprecatedStatusCode.V(13)
-    DEPRECATED_STATUS_CODE_UNAVAILABLE = Status.DeprecatedStatusCode.V(14)
-    DEPRECATED_STATUS_CODE_DATA_LOSS = Status.DeprecatedStatusCode.V(15)
-    DEPRECATED_STATUS_CODE_UNAUTHENTICATED = Status.DeprecatedStatusCode.V(16)
-
     class StatusCode(_StatusCode, metaclass=_StatusCodeEnumTypeWrapper):
         """For the semantics of status codes see
         https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/trace/api.md#set-status
         """
         pass
     class _StatusCode:
         V = typing.NewType('V', builtins.int)
@@ -506,33 +456,22 @@
     completed successfully.
     """
 
     STATUS_CODE_ERROR = Status.StatusCode.V(2)
     """The Span contains an error."""
 
 
-    DEPRECATED_CODE_FIELD_NUMBER: builtins.int
     MESSAGE_FIELD_NUMBER: builtins.int
     CODE_FIELD_NUMBER: builtins.int
-    deprecated_code: global___Status.DeprecatedStatusCode.V = ...
-    """The deprecated status code. This is an optional field.
-
-    This field is deprecated and is replaced by the `code` field below. See backward
-    compatibility notes below. According to our stability guarantees this field
-    will be removed in 12 months, on Oct 22, 2021. All usage of old senders and
-    receivers that do not understand the `code` field MUST be phased out by then.
-    """
-
     message: typing.Text = ...
     """A developer-facing human readable error message."""
 
     code: global___Status.StatusCode.V = ...
     """The status code."""
 
     def __init__(self,
         *,
-        deprecated_code : global___Status.DeprecatedStatusCode.V = ...,
         message : typing.Text = ...,
         code : global___Status.StatusCode.V = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code",b"code","deprecated_code",b"deprecated_code","message",b"message"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["code",b"code","message",b"message"]) -> None: ...
 global___Status = Status
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry/proto/version.py` & `opentelemetry-proto-1.9.1/src/opentelemetry/proto/version.py`

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

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/PKG-INFO` & `opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-proto
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Python Proto
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-proto
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-proto-1.9.0/src/opentelemetry_proto.egg-info/SOURCES.txt` & `opentelemetry-proto-1.9.1/src/opentelemetry_proto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-proto-1.9.0/tests/test_proto.py` & `opentelemetry-proto-1.9.1/tests/test_proto.py`

 * *Files identical despite different names*

