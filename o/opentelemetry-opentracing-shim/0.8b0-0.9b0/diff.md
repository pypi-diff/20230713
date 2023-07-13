# Comparing `tmp/opentelemetry-opentracing-shim-0.8b0.tar.gz` & `tmp/opentelemetry-opentracing-shim-0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-opentracing-shim-0.8b0.tar", last modified: Wed May 27 22:18:37 2020, max compression
+gzip compressed data, was "/home/runner/work/opentelemetry-python/opentelemetry-python/dist/opentelemetry-opentracing-shim-0.9b0.tar", last modified: Thu Jun 11 04:39:23 2020, max compression
```

## Comparing `opentelemetry-opentracing-shim-0.8b0.tar` & `opentelemetry-opentracing-shim-0.9b0.tar`

### file list

```diff
@@ -1,25 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/
--rw-r--r--   0 runner    (1001) docker     (116)      262 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      169 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1628 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1125 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      904 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/
--rw-r--r--   0 runner    (1001) docker     (116)    28409 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1739 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/util.py
--rw-r--r--   0 runner    (1001) docker     (116)      607 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1628 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      555 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       94 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:37.000000 opentelemetry-opentracing-shim-0.8b0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20246 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/tests/test_shim.py
--rw-r--r--   0 runner    (1001) docker     (116)     2388 2020-05-27 22:18:20.000000 opentelemetry-opentracing-shim-0.8b0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/
+-rw-r--r--   0 runner    (1001) docker     (116)      262 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      169 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1628 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      523 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1147 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      904 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/
+-rw-r--r--   0 runner    (1001) docker     (116)    28448 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1739 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/util.py
+-rw-r--r--   0 runner    (1001) docker     (116)      607 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1628 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2502 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20894 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/test_shim.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2388 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/
+-rw-r--r--   0 runner    (1001) docker     (116)     1578 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      969 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/otel_ot_shim_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_active_span_replacement/
+-rw-r--r--   0 runner    (1001) docker     (116)      679 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_active_span_replacement/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_active_span_replacement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1748 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_active_span_replacement/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1745 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_active_span_replacement/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_client_server/
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_client_server/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_client_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2314 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_client_server/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2157 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_client_server/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_common_request_handler/
+-rw-r--r--   0 runner    (1001) docker     (116)      919 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_common_request_handler/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_common_request_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1151 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_common_request_handler/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4607 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_common_request_handler/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4141 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_common_request_handler/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_late_span_finish/
+-rw-r--r--   0 runner    (1001) docker     (116)      754 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_late_span_finish/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_late_span_finish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1681 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_late_span_finish/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1536 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_late_span_finish/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_listener_per_request/
+-rw-r--r--   0 runner    (1001) docker     (116)      722 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_listener_per_request/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_listener_per_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      155 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_listener_per_request/response_listener.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1284 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_listener_per_request/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1325 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_listener_per_request/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_multiple_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (116)     1698 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_multiple_callbacks/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_multiple_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1811 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_multiple_callbacks/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1796 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_multiple_callbacks/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_nested_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (116)     1501 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_nested_callbacks/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_nested_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1536 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_nested_callbacks/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1916 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_nested_callbacks/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:23.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_subtask_span_propagation/
+-rw-r--r--   0 runner    (1001) docker     (116)     1666 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_subtask_span_propagation/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_subtask_span_propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1042 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_subtask_span_propagation/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1135 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/test_subtask_span_propagation/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1349 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1882 2020-06-11 04:39:17.000000 opentelemetry-opentracing-shim-0.9b0/tests/testbed/utils.py
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/LICENSE` & `opentelemetry-opentracing-shim-0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-opentracing-shim-0.8b0/PKG-INFO` & `opentelemetry-opentracing-shim-0.9b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-opentracing-shim
-Version: 0.8b0
+Version: 0.9b0
 Summary: OpenTracing Shim for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/master/ext/opentelemetry-ext-opentracing-shim
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Description: OpenTracing Shim for OpenTelemetry
         ==================================
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/README.rst` & `opentelemetry-opentracing-shim-0.9b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-opentracing-shim-0.8b0/setup.cfg` & `opentelemetry-opentracing-shim-0.9b0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 python_requires = >=3.4
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
 	Deprecated >= 1.2.6
 	opentracing ~= 2.0
-	opentelemetry-api == 0.8b0
+	opentelemetry-api == 0.9b0
 
 [options.extras_require]
 test = 
-	opentelemetry-test == 0.8b0
+	opentelemetry-test == 0.9b0
+	opentracing ~= 2.2.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/setup.py` & `opentelemetry-opentracing-shim-0.9b0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/__init__.py` & `opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,19 +90,15 @@
 import opentracing
 from deprecated import deprecated
 
 import opentelemetry.trace as trace_api
 from opentelemetry import propagators
 from opentelemetry.ext.opentracing_shim import util
 from opentelemetry.ext.opentracing_shim.version import __version__
-from opentelemetry.trace import DefaultSpan
-from opentelemetry.trace.propagation import (
-    get_span_from_context,
-    set_span_in_context,
-)
+from opentelemetry.trace import DefaultSpan, set_span_in_context
 
 logger = logging.getLogger(__name__)
 
 
 def create_tracer(otel_tracer_provider):
     """Creates a :class:`TracerShim` object from the provided OpenTelemetry
     :class:`opentelemetry.trace.TracerProvider`.
@@ -469,15 +465,15 @@
             Calling :meth:`ScopeShim.close` on the :class:`ScopeShim` returned
             by this property **always ends the corresponding span**, regardless
             of the *finish_on_close* value used when activating the span. This
             is a limitation of the current implementation of the OpenTracing
             shim and is likely to be handled in future versions.
         """
 
-        span = self._tracer.unwrap().get_current_span()
+        span = trace_api.get_current_span()
         if span is None:
             return None
 
         span_context = SpanContextShim(span.get_context())
         wrapped_span = SpanShim(self._tracer, span_context, span)
         return ScopeShim(self, span=wrapped_span)
         # TODO: The returned `ScopeShim` instance here always ends the
@@ -699,10 +695,14 @@
 
         def get_as_list(dict_object, key):
             value = dict_object.get(key)
             return [value] if value is not None else []
 
         propagator = propagators.get_global_httptextformat()
         ctx = propagator.extract(get_as_list, carrier)
-        otel_context = get_span_from_context(ctx).get_context()
+        span = trace_api.get_current_span(ctx)
+        if span is not None:
+            otel_context = span.get_context()
+        else:
+            otel_context = trace_api.INVALID_SPAN_CONTEXT
 
         return SpanContextShim(otel_context)
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/util.py` & `opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/util.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-opentracing-shim-0.8b0/src/opentelemetry/ext/opentracing_shim/version.py` & `opentelemetry-opentracing-shim-0.9b0/src/opentelemetry/ext/opentracing_shim/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.8b0"
+__version__ = "0.9b0"
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/src/opentelemetry_opentracing_shim.egg-info/PKG-INFO` & `opentelemetry-opentracing-shim-0.9b0/src/opentelemetry_opentracing_shim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-opentracing-shim
-Version: 0.8b0
+Version: 0.9b0
 Summary: OpenTracing Shim for OpenTelemetry
 Home-page: https://github.com/open-telemetry/opentelemetry-python/tree/master/ext/opentelemetry-ext-opentracing-shim
 Author: OpenTelemetry Authors
 Author-email: cncf-opentelemetry-contributors@lists.cncf.io
 License: Apache-2.0
 Description: OpenTracing Shim for OpenTelemetry
         ==================================
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/tests/test_shim.py` & `opentelemetry-opentracing-shim-0.9b0/tests/test_shim.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 
 import opentracing
 
 import opentelemetry.ext.opentracing_shim as opentracingshim
 from opentelemetry import propagators, trace
 from opentelemetry.ext.opentracing_shim import util
 from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.test.mock_httptextformat import MockHTTPTextFormat
+from opentelemetry.test.mock_httptextformat import (
+    MockHTTPTextFormat,
+    NOOPHTTPTextFormat,
+)
 
 
 class TestShim(TestCase):
     # pylint: disable=too-many-public-methods
 
     def setUp(self):
         """Create an OpenTelemetry tracer and a shim before every test case."""
@@ -511,14 +514,28 @@
             MockHTTPTextFormat.SPAN_ID_KEY: 7478,
         }
 
         ctx = self.shim.extract(opentracing.Format.HTTP_HEADERS, carrier)
         self.assertEqual(ctx.unwrap().trace_id, 1220)
         self.assertEqual(ctx.unwrap().span_id, 7478)
 
+    def test_extract_empty_context_returns_invalid_context(self):
+        """In the case where the propagator cannot extract a
+        SpanContext, extract should return and invalid span context.
+        """
+        _old_propagator = propagators.get_global_httptextformat()
+        propagators.set_global_httptextformat(NOOPHTTPTextFormat())
+        try:
+            carrier = {}
+
+            ctx = self.shim.extract(opentracing.Format.HTTP_HEADERS, carrier)
+            self.assertEqual(ctx.unwrap(), trace.INVALID_SPAN_CONTEXT)
+        finally:
+            propagators.set_global_httptextformat(_old_propagator)
+
     def test_extract_text_map(self):
         """Test `extract()` method for Format.TEXT_MAP."""
 
         carrier = {
             MockHTTPTextFormat.TRACE_ID_KEY: 1220,
             MockHTTPTextFormat.SPAN_ID_KEY: 7478,
         }
```

### Comparing `opentelemetry-opentracing-shim-0.8b0/tests/test_util.py` & `opentelemetry-opentracing-shim-0.9b0/tests/test_util.py`

 * *Files identical despite different names*

