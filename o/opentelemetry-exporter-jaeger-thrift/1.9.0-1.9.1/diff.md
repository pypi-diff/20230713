# Comparing `tmp/opentelemetry-exporter-jaeger-thrift-1.9.0.tar.gz` & `tmp/opentelemetry-exporter-jaeger-thrift-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-jaeger-thrift-1.9.0.tar", last modified: Wed Jan 26 18:29:16 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-exporter-jaeger-thrift-1.9.1.tar", last modified: Mon Jan 31 10:09:49 2022, max compression
```

## Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0.tar` & `opentelemetry-exporter-jaeger-thrift-1.9.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/
--rw-r--r--   0 runner    (1001) docker     (121)     8329 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent-remote
--rw-r--r--   0 runner    (1001) docker     (121)     7630 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector-remote
--rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    29841 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector-remote
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    24275 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/send.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/translate/
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:16.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/tests/certs/cred.cert
--rw-r--r--   0 runner    (1001) docker     (121)    24906 2022-01-26 18:29:09.000000 opentelemetry-exporter-jaeger-thrift-1.9.0/tests/test_jaeger_exporter_thrift.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/
+-rw-r--r--   0 runner    (1001) docker     (121)     8329 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent-remote
+-rw-r--r--   0 runner    (1001) docker     (121)     7630 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector-remote
+-rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29841 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector-remote
+-rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24275 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/send.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/translate/
+-rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:49.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/tests/certs/cred.cert
+-rw-r--r--   0 runner    (1001) docker     (121)    24906 2022-01-31 10:09:42.000000 opentelemetry-exporter-jaeger-thrift-1.9.1/tests/test_jaeger_exporter_thrift.py
```

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/LICENSE` & `opentelemetry-exporter-jaeger-thrift-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/PKG-INFO` & `opentelemetry-exporter-jaeger-thrift-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-jaeger-thrift
-Version: 1.9.0
+Version: 1.9.1
 Summary: Jaeger Thrift Exporter for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-jaeger-thrift
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/README.rst` & `opentelemetry-exporter-jaeger-thrift-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/setup.cfg` & `opentelemetry-exporter-jaeger-thrift-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/setup.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/__init__.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent-remote` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent-remote`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/agent/Agent.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector-remote` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector-remote`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/Collector.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/ttypes.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/jaeger/ttypes.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector-remote` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector-remote`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ZipkinCollector.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/constants.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/constants.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ttypes.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/gen/zipkincore/ttypes.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/send.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/send.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/translate/__init__.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry/exporter/jaeger/thrift/version.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry/exporter/jaeger/thrift/version.py`

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

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/PKG-INFO` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-jaeger-thrift
-Version: 1.9.0
+Version: 1.9.1
 Summary: Jaeger Thrift Exporter for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-jaeger-thrift
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/src/opentelemetry_exporter_jaeger_thrift.egg-info/SOURCES.txt` & `opentelemetry-exporter-jaeger-thrift-1.9.1/src/opentelemetry_exporter_jaeger_thrift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-jaeger-thrift-1.9.0/tests/test_jaeger_exporter_thrift.py` & `opentelemetry-exporter-jaeger-thrift-1.9.1/tests/test_jaeger_exporter_thrift.py`

 * *Files identical despite different names*

