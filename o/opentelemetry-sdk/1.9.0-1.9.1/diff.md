# Comparing `tmp/opentelemetry-sdk-1.9.0.tar.gz` & `tmp/opentelemetry-sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-sdk-1.9.0.tar", last modified: Wed Jan 26 18:29:15 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-sdk-1.9.1.tar", last modified: Mon Jan 31 10:09:48 2022, max compression
```

## Comparing `opentelemetry-sdk-1.9.0.tar` & `opentelemetry-sdk-1.9.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_configuration/
--rw-r--r--   0 runner    (1001) docker     (121)     7632 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/
--rw-r--r--   0 runner    (1001) docker     (121)    16232 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/export/
--rw-r--r--   0 runner    (1001) docker     (121)    10574 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/export/in_memory_log_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/severity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/
--rw-r--r--   0 runner    (1001) docker     (121)     7306 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/export/
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/measurement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/measurement_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/metric_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/metric_reader_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/sdk_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    13688 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/environment_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/error_handler/
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/error_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    12489 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/
--rw-r--r--   0 runner    (1001) docker     (121)    40733 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/export/
--rw-r--r--   0 runner    (1001) docker     (121)    14697 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/export/in_memory_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14649 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/context/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/context/test_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/error_handler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/error_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/error_handler/test_error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/logs/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14583 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/logs/test_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/logs/test_global_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/logs/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/logs/test_log_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     6301 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/logs/test_multi_log_prcessor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/metrics/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/metrics/integration_test/
--rw-r--r--   0 runner    (1001) docker     (121)     8763 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/metrics/integration_test/test_cpu_time.py
--rw-r--r--   0 runner    (1001) docker     (121)    11136 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/metrics/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/metrics/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/metrics/test_measurement_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8683 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/metrics/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3776 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/metrics/test_periodic_exporting_metric_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/performance/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/performance/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/performance/benchmarks/trace/
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/performance/benchmarks/trace/test_benchmark_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/performance/resource-usage/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/performance/resource-usage/trace/
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/performance/resource-usage/trace/profile_resource_usage_batch_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/performance/resource-usage/trace/profile_resource_usage_simple_export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19043 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/resources/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     6894 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4503 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/trace/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/trace/export/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18957 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/export/test_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/export/test_in_memory_span_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-sdk-1.9.0/tests/trace/propagation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/test_implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)    21232 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)    11184 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/test_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)    65073 2022-01-26 18:29:09.000000 opentelemetry-sdk-1.9.0/tests/trace/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)     7632 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/
+-rw-r--r--   0 runner    (1001) docker     (121)    16232 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/export/
+-rw-r--r--   0 runner    (1001) docker     (121)    10574 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/export/in_memory_log_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/severity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)     7284 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/export/
+-rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/measurement_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/metric_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/metric_reader_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/sdk_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13688 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/environment_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/error_handler/
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/error_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)    12489 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)    40733 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/export/
+-rw-r--r--   0 runner    (1001) docker     (121)    14697 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/export/in_memory_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14649 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/context/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/context/test_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/error_handler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/error_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/error_handler/test_error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/logs/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14583 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/logs/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/logs/test_global_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/logs/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/logs/test_log_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6301 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/logs/test_multi_log_prcessor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/metrics/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/metrics/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (121)     8763 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/metrics/integration_test/test_cpu_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11136 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/metrics/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/metrics/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/metrics/test_measurement_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/metrics/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/metrics/test_periodic_exporting_metric_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/performance/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/performance/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/performance/benchmarks/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/performance/benchmarks/trace/test_benchmark_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/performance/resource-usage/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/performance/resource-usage/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/performance/resource-usage/trace/profile_resource_usage_batch_export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/performance/resource-usage/trace/profile_resource_usage_simple_export.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19043 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/resources/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6894 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4503 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/trace/export/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18957 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/export/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/export/test_in_memory_span_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-sdk-1.9.1/tests/trace/propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/test_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21232 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11184 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/test_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65073 2022-01-31 10:09:42.000000 opentelemetry-sdk-1.9.1/tests/trace/test_trace.py
```

### Comparing `opentelemetry-sdk-1.9.0/LICENSE` & `opentelemetry-sdk-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/PKG-INFO` & `opentelemetry-sdk-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Python SDK
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-sdk
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-sdk-1.9.0/setup.cfg` & `opentelemetry-sdk-1.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 python_requires = >=3.6
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 include_package_data = True
 install_requires = 
-	opentelemetry-api == 1.9.0
-	opentelemetry-semantic-conventions == 0.28b0
+	opentelemetry-api == 1.9.1
+	opentelemetry-semantic-conventions == 0.28b1
 	setuptools >= 16.0
 	dataclasses == 0.8; python_version < '3.7'
 	typing-extensions >= 3.7.4
 
 [options.packages.find]
 where = src
```

### Comparing `opentelemetry-sdk-1.9.0/setup.py` & `opentelemetry-sdk-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/__init__.pyi` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_configuration/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/export/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/export/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/export/in_memory_log_exporter.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/export/in_memory_log_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_logs/severity.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_logs/severity.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     MeasurementConsumer,
     SynchronousMeasurementConsumer,
 )
 from opentelemetry.sdk._metrics.metric_reader import MetricReader
 from opentelemetry.sdk._metrics.sdk_configuration import SdkConfiguration
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.util.instrumentation import InstrumentationInfo
+from opentelemetry.util._once import Once
 
 _logger = getLogger(__name__)
 
 
 class Meter(APIMeter):
     def __init__(
         self,
@@ -167,55 +168,53 @@
         if shutdown_on_exit:
             self._atexit_handler = register(self.shutdown)
 
         self._meters = {}
         self._metric_readers = metric_readers
 
         for metric_reader in self._sdk_config.metric_readers:
-            metric_reader._register_measurement_consumer(self)
+            metric_reader._set_collect_callback(
+                self._measurement_consumer.collect
+            )
 
+        self._shutdown_once = Once()
         self._shutdown = False
 
     def force_flush(self) -> bool:
 
         # FIXME implement a timeout
 
-        metric_reader_result = True
-
         for metric_reader in self._sdk_config.metric_readers:
-            metric_reader_result = (
-                metric_reader_result and metric_reader.force_flush()
-            )
-
-        if not metric_reader_result:
-            _logger.warning("Unable to force flush all metric readers")
-
-        return metric_reader_result
+            metric_reader.collect()
+        return True
 
     def shutdown(self):
         # FIXME implement a timeout
 
-        if self._shutdown:
+        def _shutdown():
+            self._shutdown = True
+
+        did_shutdown = self._shutdown_once.do_once(_shutdown)
+
+        if not did_shutdown:
             _logger.warning("shutdown can only be called once")
             return False
 
         overall_result = True
 
         for metric_reader in self._sdk_config.metric_readers:
             metric_reader_result = metric_reader.shutdown()
 
             if not metric_reader_result:
                 _logger.warning(
-                    "MetricReader {metric_reader} failed to shutdown"
+                    "MetricReader %s failed to shutdown", metric_reader
                 )
 
             overall_result = overall_result and metric_reader_result
 
-        self._shutdown = True
-
         if self._atexit_handler is not None:
             unregister(self._atexit_handler)
             self._atexit_handler = None
 
         return overall_result
 
     def get_meter(
```

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/aggregation.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/aggregation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/export/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/export/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/instrument.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/instrument.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/measurement.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/measurement.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/measurement_consumer.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/measurement_consumer.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/metric_reader.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/metric_reader.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/metric_reader_storage.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/metric_reader_storage.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/_metrics/point.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/_metrics/point.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/environment_variables.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/error_handler/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/error_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/resources/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/export/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/export/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/export/in_memory_span_exporter.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/export/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/id_generator.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/id_generator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/trace/sampling.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/trace/sampling.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/__init__.pyi` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/util/instrumentation.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/util/instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry/sdk/version.py` & `opentelemetry-sdk-1.9.1/tests/__init__.py`

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

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/PKG-INFO` & `opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Python SDK
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-sdk
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/SOURCES.txt` & `opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/src/opentelemetry_sdk.egg-info/entry_points.txt` & `opentelemetry-sdk-1.9.1/src/opentelemetry_sdk.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/__init__.py` & `opentelemetry-sdk-1.9.1/tests/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/conftest.py` & `opentelemetry-sdk-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/context/test_asyncio.py` & `opentelemetry-sdk-1.9.1/tests/context/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/error_handler/test_error_handler.py` & `opentelemetry-sdk-1.9.1/tests/error_handler/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/logs/__init__.py` & `opentelemetry-sdk-1.9.1/tests/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/logs/test_export.py` & `opentelemetry-sdk-1.9.1/tests/logs/test_export.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/logs/test_global_provider.py` & `opentelemetry-sdk-1.9.1/tests/logs/test_global_provider.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/logs/test_handler.py` & `opentelemetry-sdk-1.9.1/tests/logs/test_handler.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/logs/test_log_record.py` & `opentelemetry-sdk-1.9.1/tests/logs/test_log_record.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/logs/test_multi_log_prcessor.py` & `opentelemetry-sdk-1.9.1/tests/logs/test_multi_log_prcessor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/metrics/integration_test/test_cpu_time.py` & `opentelemetry-sdk-1.9.1/tests/metrics/integration_test/test_cpu_time.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/metrics/test_aggregation.py` & `opentelemetry-sdk-1.9.1/tests/metrics/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/metrics/test_instrument.py` & `opentelemetry-sdk-1.9.1/tests/metrics/test_instrument.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/metrics/test_measurement_consumer.py` & `opentelemetry-sdk-1.9.1/tests/metrics/test_measurement_consumer.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/metrics/test_metrics.py` & `opentelemetry-sdk-1.9.1/tests/metrics/test_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,43 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from logging import WARNING
 from unittest import TestCase
-from unittest.mock import Mock, patch
+from unittest.mock import MagicMock, Mock, patch
 
 from opentelemetry.sdk._metrics import Meter, MeterProvider
 from opentelemetry.sdk._metrics.instrument import (
     Counter,
     Histogram,
     ObservableCounter,
     ObservableGauge,
     ObservableUpDownCounter,
     UpDownCounter,
 )
+from opentelemetry.sdk._metrics.metric_reader import MetricReader
+from opentelemetry.sdk._metrics.point import AggregationTemporality
 from opentelemetry.sdk.resources import Resource
+from opentelemetry.test.concurrency_test import ConcurrencyTestBase, MockFunc
 
 
-class TestMeterProvider(TestCase):
+class DummyMetricReader(MetricReader):
+    def __init__(self):
+        super().__init__(AggregationTemporality.CUMULATIVE)
+
+    def _receive_metrics(self, metrics):
+        pass
+
+    def shutdown(self):
+        return True
+
+
+class TestMeterProvider(ConcurrencyTestBase):
     def test_resource(self):
         """
         `MeterProvider` provides a way to allow a `Resource` to be specified.
         """
 
         meter_provider_0 = MeterProvider()
         meter_provider_1 = MeterProvider()
@@ -88,22 +102,32 @@
             schema_url="schema_url",
         )
         self.assertIs(meter1, meter2)
         self.assertIsNot(meter1, meter3)
 
     def test_shutdown(self):
 
-        mock_metric_reader_0 = Mock(**{"shutdown.return_value": False})
+        mock_metric_reader_0 = MagicMock(
+            **{
+                "shutdown.return_value": False,
+                "__str__.return_value": "mock_metric_reader_0",
+            }
+        )
         mock_metric_reader_1 = Mock(**{"shutdown.return_value": True})
 
         meter_provider = MeterProvider(
             metric_readers=[mock_metric_reader_0, mock_metric_reader_1]
         )
 
-        self.assertFalse(meter_provider.shutdown())
+        with self.assertLogs(level=WARNING) as log:
+            self.assertFalse(meter_provider.shutdown())
+            self.assertEqual(
+                log.records[0].getMessage(),
+                "MetricReader mock_metric_reader_0 failed to shutdown",
+            )
         mock_metric_reader_0.shutdown.assert_called_once()
         mock_metric_reader_1.shutdown.assert_called_once()
 
         mock_metric_reader_0 = Mock(**{"shutdown.return_value": True})
         mock_metric_reader_1 = Mock(**{"shutdown.return_value": True})
 
         meter_provider = MeterProvider(
@@ -125,14 +149,39 @@
         with self.assertRaises(AssertionError):
             with self.assertLogs(level=WARNING):
                 meter_provider.shutdown()
 
         with self.assertLogs(level=WARNING):
             meter_provider.shutdown()
 
+    @patch("opentelemetry.sdk._metrics._logger")
+    def test_shutdown_race(self, mock_logger):
+        mock_logger.warning = MockFunc()
+        meter_provider = MeterProvider()
+        num_threads = 70
+        self.run_with_many_threads(
+            meter_provider.shutdown, num_threads=num_threads
+        )
+        self.assertEqual(mock_logger.warning.call_count, num_threads - 1)
+
+    @patch("opentelemetry.sdk._metrics.SynchronousMeasurementConsumer")
+    def test_measurement_collect_callback(
+        self, mock_sync_measurement_consumer
+    ):
+        metric_readers = [DummyMetricReader()] * 5
+        sync_consumer_instance = mock_sync_measurement_consumer()
+        sync_consumer_instance.collect = MockFunc()
+        MeterProvider(metric_readers=metric_readers)
+
+        for reader in metric_readers:
+            reader.collect()
+        self.assertEqual(
+            sync_consumer_instance.collect.call_count, len(metric_readers)
+        )
+
     @patch("opentelemetry.sdk._metrics.SynchronousMeasurementConsumer")
     def test_creates_sync_measurement_consumer(
         self, mock_sync_measurement_consumer
     ):
         MeterProvider()
         mock_sync_measurement_consumer.assert_called()
```

### Comparing `opentelemetry-sdk-1.9.0/tests/metrics/test_periodic_exporting_metric_reader.py` & `opentelemetry-sdk-1.9.1/tests/metrics/test_periodic_exporting_metric_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     def test_ticker_collects_metrics(self):
         exporter = FakeMetricsExporter()
 
         pmr = self._create_periodic_reader(
             metrics_list, exporter, interval=100
         )
-        time.sleep(0.2)
+        time.sleep(0.11)
         self.assertEqual(exporter.metrics, metrics_list)
         pmr.shutdown()
 
     def test_shutdown(self):
         exporter = FakeMetricsExporter()
 
         pmr = self._create_periodic_reader([], exporter)
```

### Comparing `opentelemetry-sdk-1.9.0/tests/performance/benchmarks/trace/test_benchmark_trace.py` & `opentelemetry-sdk-1.9.1/tests/performance/benchmarks/trace/test_benchmark_trace.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/performance/resource-usage/trace/profile_resource_usage_batch_export.py` & `opentelemetry-sdk-1.9.1/tests/performance/resource-usage/trace/profile_resource_usage_batch_export.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/performance/resource-usage/trace/profile_resource_usage_simple_export.py` & `opentelemetry-sdk-1.9.1/tests/performance/resource-usage/trace/profile_resource_usage_simple_export.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/resources/test_resources.py` & `opentelemetry-sdk-1.9.1/tests/resources/test_resources.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/test_configurator.py` & `opentelemetry-sdk-1.9.1/tests/test_configurator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/test_util.py` & `opentelemetry-sdk-1.9.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/__init__.py` & `opentelemetry-sdk-1.9.1/tests/trace/export/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/export/__init__.py` & `opentelemetry-sdk-1.9.1/src/opentelemetry/sdk/version.py`

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

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/export/test_export.py` & `opentelemetry-sdk-1.9.1/tests/trace/export/test_export.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/export/test_in_memory_span_exporter.py` & `opentelemetry-sdk-1.9.1/tests/trace/export/test_in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/test_globals.py` & `opentelemetry-sdk-1.9.1/tests/trace/test_globals.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/test_implementation.py` & `opentelemetry-sdk-1.9.1/tests/trace/test_implementation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/test_sampling.py` & `opentelemetry-sdk-1.9.1/tests/trace/test_sampling.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/test_span_processor.py` & `opentelemetry-sdk-1.9.1/tests/trace/test_span_processor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-sdk-1.9.0/tests/trace/test_trace.py` & `opentelemetry-sdk-1.9.1/tests/trace/test_trace.py`

 * *Files identical despite different names*

