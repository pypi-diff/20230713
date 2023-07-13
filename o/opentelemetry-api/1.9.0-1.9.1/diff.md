# Comparing `tmp/opentelemetry-api-1.9.0.tar.gz` & `tmp/opentelemetry-api-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-api-1.9.0.tar", last modified: Wed Jan 26 18:29:15 2022, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-api-1.9.1.tar", last modified: Mon Jan 31 10:09:48 2022, max compression
```

## Comparing `opentelemetry-api-1.9.0.tar` & `opentelemetry-api-1.9.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/_metrics/
--rw-r--r--   0 runner    (1001) docker     (121)    16091 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7134 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/_metrics/instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/_metrics/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/attributes/
--rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/baggage/
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/baggage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/baggage/propagation/
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/baggage/propagation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/context/
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/context/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/context/contextvars_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/environment_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/propagate/
--rw-r--r--   0 runner    (1001) docker     (121)     5333 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/propagate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/propagators/
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/propagators/composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     6441 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/propagators/textmap.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/
--rw-r--r--   0 runner    (1001) docker     (121)    21249 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/propagation/
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/propagation/tracecontext.py
--rw-r--r--   0 runner    (1001) docker     (121)    17938 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/span.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/trace/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/util/_once.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/util/_providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/util/_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/util/re.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/util/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/src/opentelemetry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/attributes/
--rw-r--r--   0 runner    (1001) docker     (121)     5905 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/attributes/test_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/baggage/
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/baggage/test_baggage.py
--rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/baggage/test_baggage_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/context/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/context/base_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/context/propagation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/context/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/context/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/context/test_contextvars_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/distributedcontext/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/distributedcontext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)    19099 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/metrics/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/metrics/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/metrics/test_meter.py
--rw-r--r--   0 runner    (1001) docker     (121)    11502 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/metrics/test_meter_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/mypysmoke.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/propagators/
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/propagators/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/propagators/test_global_httptextformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3233 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/propagators/test_propagators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/trace/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/trace/propagation/
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/propagation/test_textmap.py
--rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/propagation/test_tracecontexthttptextformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_defaultspan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_immutablespancontext.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_span_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4284 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/trace/test_tracestate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 18:29:15.000000 opentelemetry-api-1.9.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/util/test_once.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-01-26 18:29:09.000000 opentelemetry-api-1.9.0/tests/util/test_re.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)    16091 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7134 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/_metrics/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/_metrics/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/attributes/
+-rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/baggage/
+-rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/baggage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/baggage/propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/baggage/propagation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/context/
+-rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/context/contextvars_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/environment_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/propagate/
+-rw-r--r--   0 runner    (1001) docker     (121)     5333 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/propagate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/propagators/
+-rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/propagators/composite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6441 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/propagators/textmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)    21249 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/propagation/tracecontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17938 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/span.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/trace/status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/util/_once.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/util/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/util/_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/util/re.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/util/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/src/opentelemetry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/attributes/
+-rw-r--r--   0 runner    (1001) docker     (121)     5905 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/attributes/test_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/baggage/
+-rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/baggage/test_baggage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/baggage/test_baggage_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/context/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/context/base_context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/context/propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/context/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/context/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/context/test_contextvars_context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/distributedcontext/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/distributedcontext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)    19099 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/metrics/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/metrics/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3649 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/metrics/test_meter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11502 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/metrics/test_meter_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/mypysmoke.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/propagators/
+-rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/propagators/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/propagators/test_global_httptextformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3233 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/propagators/test_propagators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/trace/propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/propagation/test_textmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/propagation/test_tracecontexthttptextformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_defaultspan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_immutablespancontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_span_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4284 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/trace/test_tracestate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 10:09:48.000000 opentelemetry-api-1.9.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/util/test_once.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-01-31 10:09:42.000000 opentelemetry-api-1.9.1/tests/util/test_re.py
```

### Comparing `opentelemetry-api-1.9.0/LICENSE` & `opentelemetry-api-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/PKG-INFO` & `opentelemetry-api-1.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Python API
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-api
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-api-1.9.0/setup.cfg` & `opentelemetry-api-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/setup.py` & `opentelemetry-api-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/_metrics/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/_metrics/instrument.py` & `opentelemetry-api-1.9.1/src/opentelemetry/_metrics/instrument.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/_metrics/measurement.py` & `opentelemetry-api-1.9.1/src/opentelemetry/_metrics/measurement.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/attributes/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/baggage/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/baggage/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/baggage/propagation/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/baggage/propagation/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/context/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/context/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/context/context.py` & `opentelemetry-api-1.9.1/src/opentelemetry/context/context.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/context/contextvars_context.py` & `opentelemetry-api-1.9.1/src/opentelemetry/context/contextvars_context.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/environment_variables.py` & `opentelemetry-api-1.9.1/src/opentelemetry/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/propagate/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/propagate/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/propagators/composite.py` & `opentelemetry-api-1.9.1/src/opentelemetry/propagators/composite.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/propagators/textmap.py` & `opentelemetry-api-1.9.1/src/opentelemetry/propagators/textmap.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/trace/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/trace/propagation/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/trace/propagation/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/trace/propagation/tracecontext.py` & `opentelemetry-api-1.9.1/src/opentelemetry/trace/propagation/tracecontext.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/trace/span.py` & `opentelemetry-api-1.9.1/src/opentelemetry/trace/span.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/trace/status.py` & `opentelemetry-api-1.9.1/src/opentelemetry/trace/status.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/util/_once.py` & `opentelemetry-api-1.9.1/src/opentelemetry/util/_once.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/util/_providers.py` & `opentelemetry-api-1.9.1/src/opentelemetry/util/_providers.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/util/_time.py` & `opentelemetry-api-1.9.1/src/opentelemetry/util/_time.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/util/re.py` & `opentelemetry-api-1.9.1/src/opentelemetry/util/re.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/util/types.py` & `opentelemetry-api-1.9.1/src/opentelemetry/util/types.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry/version.py` & `opentelemetry-api-1.9.1/tests/distributedcontext/__init__.py`

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

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/PKG-INFO` & `opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: OpenTelemetry Python API
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-api
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/SOURCES.txt` & `opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/src/opentelemetry_api.egg-info/entry_points.txt` & `opentelemetry-api-1.9.1/src/opentelemetry_api.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/__init__.py` & `opentelemetry-api-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/attributes/test_attributes.py` & `opentelemetry-api-1.9.1/tests/attributes/test_attributes.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/baggage/test_baggage.py` & `opentelemetry-api-1.9.1/tests/baggage/test_baggage.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/baggage/test_baggage_propagation.py` & `opentelemetry-api-1.9.1/tests/baggage/test_baggage_propagation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/context/base_context.py` & `opentelemetry-api-1.9.1/tests/context/base_context.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/context/test_context.py` & `opentelemetry-api-1.9.1/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/context/test_contextvars_context.py` & `opentelemetry-api-1.9.1/tests/context/test_contextvars_context.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/distributedcontext/__init__.py` & `opentelemetry-api-1.9.1/tests/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/metrics/test_instruments.py` & `opentelemetry-api-1.9.1/tests/metrics/test_instruments.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/metrics/test_measurement.py` & `opentelemetry-api-1.9.1/tests/metrics/test_measurement.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/metrics/test_meter.py` & `opentelemetry-api-1.9.1/tests/metrics/test_meter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/metrics/test_meter_provider.py` & `opentelemetry-api-1.9.1/tests/metrics/test_meter_provider.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/mypysmoke.py` & `opentelemetry-api-1.9.1/tests/mypysmoke.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/propagators/test_composite.py` & `opentelemetry-api-1.9.1/tests/propagators/test_composite.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/propagators/test_global_httptextformat.py` & `opentelemetry-api-1.9.1/tests/propagators/test_global_httptextformat.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/propagators/test_propagators.py` & `opentelemetry-api-1.9.1/tests/propagators/test_propagators.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/test_implementation.py` & `opentelemetry-api-1.9.1/tests/test_implementation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/__init__.py` & `opentelemetry-api-1.9.1/src/opentelemetry/version.py`

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

### Comparing `opentelemetry-api-1.9.0/tests/trace/propagation/test_textmap.py` & `opentelemetry-api-1.9.1/tests/trace/propagation/test_textmap.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/propagation/test_tracecontexthttptextformat.py` & `opentelemetry-api-1.9.1/tests/trace/propagation/test_tracecontexthttptextformat.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_defaultspan.py` & `opentelemetry-api-1.9.1/tests/trace/test_defaultspan.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_globals.py` & `opentelemetry-api-1.9.1/tests/trace/test_globals.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_immutablespancontext.py` & `opentelemetry-api-1.9.1/tests/trace/test_immutablespancontext.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_proxy.py` & `opentelemetry-api-1.9.1/tests/trace/test_proxy.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_span_context.py` & `opentelemetry-api-1.9.1/tests/trace/test_span_context.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_status.py` & `opentelemetry-api-1.9.1/tests/trace/test_status.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_tracer.py` & `opentelemetry-api-1.9.1/tests/trace/test_tracer.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/trace/test_tracestate.py` & `opentelemetry-api-1.9.1/tests/trace/test_tracestate.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/util/test_once.py` & `opentelemetry-api-1.9.1/tests/util/test_once.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-api-1.9.0/tests/util/test_re.py` & `opentelemetry-api-1.9.1/tests/util/test_re.py`

 * *Files identical despite different names*

