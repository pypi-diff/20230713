# Comparing `tmp/opentelemetry-exporter-jaeger-proto-grpc-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-jaeger-proto-grpc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-jaeger-proto-grpc-1.9.0.tar", last modified: Wed Jan 26 18:29:16 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-jaeger-proto-grpc-1.9.1.tar", last modified: Mon Jan 31 10:09:49 2022, max compression
```

## Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0.tar` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4972 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/gogoproto/
--rw-r--r--   0 runner    (1001) docker     (121)    48873 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/gogoproto/gogo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10685 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    28871 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/model_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/
--rw-r--r--   0 runner    (1001) docker     (121)     5613 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    81503 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/send/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/send/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/translate/
--rw-r--r--   0 runner    (1001) docker     (121)    12535 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/tests/certs/cred.cert
--rw-r--r--   0 runner    (1001) docker     (121)    18743 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.0/tests/test_jaeger_exporter_protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)     6481 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4972 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/gogoproto/
+-rw-r--r--   0 runner    (1001) docker     (121)    48873 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/gogoproto/gogo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10685 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28871 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/model_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/
+-rw-r--r--   0 runner    (1001) docker     (121)     5613 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81503 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/send/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/send/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/translate/
+-rw-r--r--   0 runner    (1001) docker     (121)    12535 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/tests/certs/cred.cert
+-rw-r--r--   0 runner    (1001) docker     (121)    18743 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-proto-grpc-1.9.1/tests/test_jaeger_exporter_protobuf.py
```

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/LICENSE` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/PKG-INFO` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-jaeger-proto-grpc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Jaeger Protobuf Exporter for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-jaeger-proto-grpc
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/README.rst` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/setup.cfg` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/setup.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/__init__.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2_grpc.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/collector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/gogoproto/gogo_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/annotations_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/http_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/model_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/model_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/annotations_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/openapiv2_pb2.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/gen/protoc_gen_swagger/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/translate/__init__.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/util.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/util.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry/exporter/jaeger/proto/grpc/version.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry/exporter/jaeger/proto/grpc/version.py`

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

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/PKG-INFO` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-jaeger-proto-grpc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Jaeger Protobuf Exporter for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-jaeger-proto-grpc
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/SOURCES.txt` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/src/opentelemetry_exporter_jaeger_proto_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-proto-grpc-1.9.0/tests/test_jaeger_exporter_protobuf.py` & `opentelemetry-exporter-jaeger-proto-grpc-1.9.1/tests/test_jaeger_exporter_protobuf.py`

 * *Files identical despite different names*

