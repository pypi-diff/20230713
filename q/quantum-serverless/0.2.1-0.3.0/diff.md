# Comparing `tmp/quantum_serverless-0.2.1.tar.gz` & `tmp/quantum_serverless-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.2.1.tar", last modified: Mon Jun 26 15:38:45 2023, max compression
+gzip compressed data, was "quantum_serverless-0.3.0.tar", last modified: Thu Jul 13 12:05:07 2023, max compression
```

## Comparing `quantum_serverless-0.2.1.tar` & `quantum_serverless-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/visualizaiton/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/visualizaiton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/visualizaiton/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.524255 quantum_serverless-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-13 12:05:07.524255 quantum_serverless-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.516255 quantum_serverless-0.3.0/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/quantum_serverless/visualizaiton/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/visualizaiton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/quantum_serverless/visualizaiton/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.516255 quantum_serverless-0.3.0/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-13 12:05:07.000000 quantum_serverless-0.3.0/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 12:05:07.000000 quantum_serverless-0.3.0/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:05:07.000000 quantum_serverless-0.3.0/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 12:05:07.000000 quantum_serverless-0.3.0/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 12:05:07.000000 quantum_serverless-0.3.0/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 12:05:07.524255 quantum_serverless-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.520255 quantum_serverless-0.3.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:05:07.524255 quantum_serverless-0.3.0/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 12:04:55.000000 quantum_serverless-0.3.0/tests/utils.py
```

### Comparing `quantum_serverless-0.2.1/PKG-INFO` & `quantum_serverless-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.2.1
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.2.1/README.md` & `quantum_serverless-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/__init__.py` & `quantum_serverless-0.3.0/quantum_serverless/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,29 +13,35 @@
 """
 .. currentmodule:: quantum_serverless
 
 .. autosummary::
     :toctree: ../stubs/
 
     QuantumServerless
+    QuantumServerlessException
+    get_auto_discovered_provider
 """
 
 from importlib_metadata import version as metadata_version, PackageNotFoundError
 
 from .core import (
-    Provider,
+    BaseProvider,
     distribute_task,
     get,
     put,
     get_refs_by_status,
     KuberayProvider,
-    GatewayProvider,
+    Provider,
     save_result,
 )
-from .quantum_serverless import QuantumServerless
+from .quantum_serverless import (
+    QuantumServerless,
+    get_auto_discovered_provider,
+    QuantumServerlessException,
+)
 from .core.program import Program
 from .serializers import get_arguments
 
 try:
     __version__ = metadata_version("quantum_serverless")
 except PackageNotFoundError:  # pragma: no cover
     # package is not installed
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/__init__.py` & `quantum_serverless-0.3.0/quantum_serverless/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,19 +23,29 @@
 Core abstractions
 -----------------
 
 .. autosummary::
     :toctree: ../stubs/
 
     Provider
-    GatewayProvider
+    BaseProvider
     KuberayProvider
     ComputeResource
-
+    Job
+    GatewayJobClient
+    BaseJobClient
+    RayJobClient
     save_result
+    Program
+    ProgramStorage
+    ProgramRepository
+    download_and_unpack_artifact
+    Target
+    CircuitMeta
+    fetch_execution_meta
     distribute_task
     get
     put
     get_refs_by_status
 
 
 Events classes
@@ -54,18 +64,27 @@
 .. autosummary::
     :toctree: ../stubs/
 
     StateHandler
     RedisStateHandler
 """
 
-from .provider import Provider, ComputeResource, KuberayProvider, GatewayProvider
+from .provider import BaseProvider, ComputeResource, KuberayProvider, Provider
+from .job import BaseJobClient, RayJobClient, GatewayJobClient, Job, save_result
+from .program import (
+    Program,
+    ProgramStorage,
+    ProgramRepository,
+    download_and_unpack_artifact,
+)
 from .decorators import (
     remote,
     get,
     put,
     get_refs_by_status,
+    fetch_execution_meta,
     distribute_task,
+    Target,
+    CircuitMeta,
 )
 from .events import RedisEventHandler, EventHandler, ExecutionMessage
 from .state import RedisStateHandler, StateHandler
-from .job import save_result
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/constants.py` & `quantum_serverless-0.3.0/quantum_serverless/core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,7 +44,10 @@
 GATEWAY_PROVIDER_VERSION_DEFAULT = "v1"
 
 # auth
 ENV_JOB_GATEWAY_TOKEN = "ENV_JOB_GATEWAY_TOKEN"
 ENV_JOB_GATEWAY_HOST = "ENV_JOB_GATEWAY_HOST"
 ENV_JOB_ID_GATEWAY = "ENV_JOB_ID_GATEWAY"
 ENV_JOB_ARGUMENTS = "ENV_JOB_ARGUMENTS"
+
+# artifact
+MAX_ARTIFACT_FILE_SIZE_MB = 20
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/decorators.py` & `quantum_serverless-0.3.0/quantum_serverless/core/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,25 +46,67 @@
     OT_TRACEPARENT_ID_KEY,
 )
 from quantum_serverless.core.state import StateHandler
 from quantum_serverless.core.tracing import get_tracer, _trace_env_vars
 from quantum_serverless.utils import JsonSerializable
 
 remote = ray.remote
-get = ray.get
-put = ray.put
-get_refs_by_status = ray.wait
+
+
+def put(value: Any, **kwargs):
+    """Puts object into shared distributed storage
+
+    Args:
+        value: object to put to object store
+        **kwargs: other arguments
+
+    Returns:
+
+    """
+    return ray.put(value=value, **kwargs)
+
+
+def get_refs_by_status(object_refs: List["ray.ObjectRef"], **kwargs):
+    """Get references by status.
+
+    Args:
+        object_refs: object references
+        **kwargs: other arguments
+
+    Returns:
+        A list of refs that are ready and a list of the remaining references.
+    """
+    return ray.wait(object_refs=object_refs, **kwargs)
+
+
+def get(
+    object_refs: Union[ray.ObjectRef, Sequence[ray.ObjectRef]],
+    *,
+    timeout: Optional[float] = None,
+) -> Any:
+    """Get results from distributed tasks.
+
+    Args:
+        object_refs: Object ref of the object to get or a list of object refs
+            to get.
+        timeout (Optional[float]): The maximum amount of time in seconds to
+            wait before returning.
+
+    Returns:
+        A object or a list of objects.
+    """
+    return ray.get(object_refs=object_refs, timeout=timeout)
 
 
 @dataclass
 class Target(JsonSerializable):
     """Quantum serverless target.
 
     Example:
-        >>> @run_qiskit_remote(target=Target(cpu=1))
+        >>> @distribute_task(target=Target(cpu=1))
         >>> def awesome_function():
         >>>     return 42
     """
 
     cpu: int = 1
     gpu: int = 0
     qpu: int = 0
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/events.py` & `quantum_serverless-0.3.0/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/job.py` & `quantum_serverless-0.3.0/quantum_serverless/core/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Job
 """
 import json
 import logging
 import os
 import tarfile
 import time
+from pathlib import Path
 from typing import Dict, Any, Optional, List
 from uuid import uuid4
 
 import ray.runtime_env
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
@@ -43,16 +44,18 @@
     OT_PROGRAM_NAME,
     REQUESTS_TIMEOUT,
     ENV_JOB_GATEWAY_TOKEN,
     ENV_JOB_GATEWAY_HOST,
     ENV_JOB_ID_GATEWAY,
     ENV_GATEWAY_PROVIDER_VERSION,
     GATEWAY_PROVIDER_VERSION_DEFAULT,
+    MAX_ARTIFACT_FILE_SIZE_MB,
 )
 from quantum_serverless.core.program import Program
+from quantum_serverless.exception import QuantumServerlessException
 from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
 from quantum_serverless.utils.json import is_jsonable, safe_json_request
 
 RuntimeEnv = ray.runtime_env.RuntimeEnv
 
 
 class BaseJobClient:
@@ -169,19 +172,35 @@
 
     def run(  # pylint: disable=too-many-locals
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
         url = f"{self.host}/api/{self.version}/programs/run/"
         artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
 
+        # check if entrypoint exists
+        if not os.path.exists(os.path.join(program.working_dir, program.entrypoint)):
+            raise QuantumServerlessException(
+                f"Entrypoint file [{program.entrypoint}] does not exist "
+                f"in [{program.working_dir}] working directory."
+            )
+
         with tarfile.open(artifact_file_path, "w") as tar:
             for filename in os.listdir(program.working_dir):
                 fpath = os.path.join(program.working_dir, filename)
                 tar.add(fpath, arcname=filename)
 
+        # check file size
+        size_in_mb = Path(artifact_file_path).stat().st_size / 1024**2
+        if size_in_mb > MAX_ARTIFACT_FILE_SIZE_MB:
+            raise QuantumServerlessException(
+                f"Artifact size is {int(size_in_mb)} Mb, "
+                f"which is greater than {MAX_ARTIFACT_FILE_SIZE_MB} allowed. "
+                f"Try to reduce size of `working_dir`."
+            )
+
         with open(artifact_file_path, "rb") as file:
             response_data = safe_json_request(
                 request=lambda: requests.post(
                     url=url,
                     data={
                         "title": program.title,
                         "entrypoint": program.entrypoint,
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/program.py` & `quantum_serverless-0.3.0/quantum_serverless/core/program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/provider.py` & `quantum_serverless-0.3.0/quantum_serverless/core/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             return self.name == other.name and self.host == other.host
         return False
 
     def __repr__(self):
         return f"<ComputeResource: {self.name}>"
 
 
-class Provider(JsonSerializable):
+class BaseProvider(JsonSerializable):
     """Provider."""
 
     def __init__(
         self,
         name: str,
         host: Optional[str] = None,
         token: Optional[str] = None,
@@ -182,15 +182,15 @@
                 available_compute_resources = [compute_resource]
             else:
                 available_compute_resources = []
         self.available_compute_resources = available_compute_resources
 
     @classmethod
     def from_dict(cls, dictionary: dict):
-        return Provider(**dictionary)
+        return BaseProvider(**dictionary)
 
     def job_client(self):
         """Return job client for configured compute resource of provider.
 
         Returns:
             job client
         """
@@ -201,15 +201,15 @@
         if self.compute_resource is None:
             raise QuantumServerlessException(
                 f"ComputeResource was not selected for provider {self.name}"
             )
         return self.compute_resource.context(**kwargs)
 
     def __eq__(self, other):
-        if isinstance(other, Provider):
+        if isinstance(other, BaseProvider):
             return self.name == other.name
 
         return False
 
     def __repr__(self):
         return f"<Provider: {self.name}>"
 
@@ -281,15 +281,15 @@
                 f"Selected provider: {self}"
             )
             return None
 
         return job_client.run(program, arguments)
 
 
-class KuberayProvider(Provider):
+class KuberayProvider(BaseProvider):
     """(Deprecated) Implements CRUD for Kuberay API server."""
 
     def __init__(
         self,
         name: str,
         host: Optional[str] = None,
         namespace: Optional[str] = "default",
@@ -321,15 +321,15 @@
             compute_resource: selected compute_resource from provider
             available_compute_resources: available clusters in provider
         """
         super().__init__(name)
         warnings.warn(
             "`KuberayProvider` is deprecated "
             "and will be removed in v0.3. "
-            "Please, consider using `GatewayProvider`.",
+            "Please, consider using `Provider`.",
             DeprecationWarning,
             stacklevel=2,
         )
 
         self.name = name
         self.host = host
         self.token = token
@@ -475,28 +475,28 @@
             timeout=TIMEOUT,
         )
 
     def get_jobs(self, **kwargs) -> List[Job]:
         raise NotImplementedError
 
 
-class GatewayProvider(Provider):
-    """GatewayProvider."""
+class Provider(BaseProvider):
+    """Provider."""
 
     def __init__(
         self,
         name: Optional[str] = None,
         host: Optional[str] = None,
         version: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token: Optional[str] = None,
         verbose: bool = False,
     ):
-        """GatewayProvider.
+        """Provider.
 
         Args:
             name: name of provider
             host: host of gateway
             version: version of gateway
             username: username
             password: password
@@ -519,14 +519,16 @@
                 "and `password` or `token`."
             )
 
         super().__init__(name)
         self.verbose = verbose
         self.host = host
         self.version = version
+        if token is not None:
+            self._verify_token(token)
         self._token = token
         if token is None:
             self._fetch_token(username, password)
 
         self._job_client = GatewayJobClient(self.host, self._token, self.version)
 
     def get_compute_resources(self) -> List[ComputeResource]:
@@ -549,11 +551,26 @@
 
     def _fetch_token(self, username: str, password: str):
         response_data = safe_json_request(
             request=lambda: requests.post(
                 url=f"{self.host}/dj-rest-auth/keycloak/login/",
                 data={"username": username, "password": password},
                 timeout=REQUESTS_TIMEOUT,
-            )
+            ),
+            verbose=self.verbose,
         )
 
         self._token = response_data.get("access")
+
+    def _verify_token(self, token: str):
+        """Verify token."""
+        try:
+            safe_json_request(
+                request=lambda: requests.get(
+                    url=f"{self.host}/api/v1/programs/",
+                    headers={"Authorization": f"Bearer {token}"},
+                    timeout=REQUESTS_TIMEOUT,
+                ),
+                verbose=self.verbose,
+            )
+        except QuantumServerlessException as reason:
+            raise QuantumServerlessException("Cannot verify token.") from reason
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/state.py` & `quantum_serverless-0.3.0/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/core/tracing.py` & `quantum_serverless-0.3.0/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/exception.py` & `quantum_serverless-0.3.0/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/library/__init__.py` & `quantum_serverless-0.3.0/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.3.0/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.3.0/quantum_serverless/quantum_serverless.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,41 +30,43 @@
 from typing import Optional, Union, List, Dict, Any
 
 import requests
 from ray._private.worker import BaseContext
 
 from quantum_serverless.core.job import Job
 from quantum_serverless.core.program import Program
-from quantum_serverless.core.provider import Provider, ComputeResource
+from quantum_serverless.core.provider import BaseProvider, ComputeResource
 from quantum_serverless.exception import QuantumServerlessException
 from quantum_serverless.visualizaiton import Widget
 
 Context = Union[BaseContext]
 
 
 class QuantumServerless:
     """QuantumServerless class."""
 
-    def __init__(self, providers: Optional[Union[Provider, List[Provider]]] = None):
+    def __init__(
+        self, providers: Optional[Union[BaseProvider, List[BaseProvider]]] = None
+    ):
         """Quantum serverless management class.
 
         Args:
             config: configuration
 
         Raises:
             QuantumServerlessException
         """
         if providers is None:
             providers = [
-                Provider("local", compute_resource=ComputeResource(name="local"))
+                BaseProvider("local", compute_resource=ComputeResource(name="local"))
             ]
-        elif isinstance(providers, Provider):
+        elif isinstance(providers, BaseProvider):
             providers = [providers]
-        self._providers: List[Provider] = providers
-        self._selected_provider: Provider = self._providers[-1]
+        self._providers: List[BaseProvider] = providers
+        self._selected_provider: BaseProvider = self._providers[-1]
 
         self._allocated_context: Optional[Context] = None
 
     @property
     def job_client(self):
         """Job client for given provider."""
         return self._selected_provider.job_client()
@@ -112,35 +114,35 @@
         Returns:
             list of jobs
         """
         return self._selected_provider.get_jobs(**kwargs)
 
     def context(
         self,
-        provider: Optional[Union[str, Provider]] = None,
+        provider: Optional[Union[str, BaseProvider]] = None,
         **kwargs,
     ):
         """Sets context for allocation
 
         Args:
             provider: Provider instance or name of provider
             **kwargs: arguments that will be passed to context initialization.
                 See https://docs.ray.io/en/latest/ray-core/package-ref.html#ray-init
 
         Returns:
             Context
         """
         if provider is not None:
-            if isinstance(provider, Provider) and provider.compute_resource is None:
+            if isinstance(provider, BaseProvider) and provider.compute_resource is None:
                 raise QuantumServerlessException(
                     "Given provider does not have compute_resources"
                 )
 
             if isinstance(provider, str):
-                available_providers: Dict[str, Provider] = {
+                available_providers: Dict[str, BaseProvider] = {
                     p.name: p for p in self._providers
                 }
                 if provider in available_providers:
                     provider = available_providers[provider]
                 else:
                     raise QuantumServerlessException(
                         f"Provider {provider} is not in a list of available providers "
@@ -149,42 +151,44 @@
         else:
             provider = self._selected_provider
 
         return provider.context(**kwargs)
 
     def provider(
         self,
-        provider: Union[str, Provider],
+        provider: Union[str, BaseProvider],
         **kwargs,
     ) -> Context:
         """Sets provider for context allocation.
 
         Args:
             provider: Provider instance or name of provider
             **kwargs: arguments that will be passed to context initialization.
                 See https://docs.ray.io/en/latest/ray-core/package-ref.html#ray-init
 
         Returns:
             Context
         """
         return self.context(provider=provider, **kwargs)
 
-    def add_provider(self, provider: Provider) -> "QuantumServerless":
+    def add_provider(self, provider: BaseProvider) -> "QuantumServerless":
         """Adds provider to the list of available providers.
 
         Args:
             provider: provider instance
 
         Returns:
             QuantumServerless instance
         """
         self._providers.append(provider)
         return self
 
-    def set_provider(self, provider: Union[str, int, Provider]) -> "QuantumServerless":
+    def set_provider(
+        self, provider: Union[str, int, BaseProvider]
+    ) -> "QuantumServerless":
         """Set provider for default context allocation.
 
         Args:
             provider: provider instance
 
         Returns:
             QuantumServerless instance
@@ -204,20 +208,20 @@
             if provider not in provider_names:
                 raise QuantumServerlessException(
                     f"{provider} name is not in a list "
                     f"of available provider names: {provider_names}."
                 )
             self._selected_provider = providers[provider_names.index(provider)]
 
-        elif isinstance(provider, Provider):
+        elif isinstance(provider, BaseProvider):
             self._selected_provider = provider
 
         return self
 
-    def providers(self) -> List[Provider]:
+    def providers(self) -> List[BaseProvider]:
         """Returns list of available providers.
 
         Returns:
             list of providers
         """
         return self._providers
 
@@ -228,15 +232,15 @@
     def __repr__(self):
         providers = ", ".join(provider.name for provider in self.providers())
         return f"<QuantumServerless | providers [{providers}]>"
 
 
 def get_auto_discovered_provider(
     manager_address: str, token: Optional[str] = None
-) -> Optional[Provider]:
+) -> Optional[BaseProvider]:
     """Makes http request to manager to get available clusters."""
     compute_resources = []
 
     headers = {"Authorization": f"Bearer {token}"} if token else None
     url = f"{manager_address}/quantum-serverless-manager/cluster/"
 
     try:
@@ -263,14 +267,14 @@
 
     except Exception:  # pylint: disable=broad-except
         logging.info(
             "Autodiscovery: was not able to autodiscover additional resources."
         )
 
     if len(compute_resources) > 0:
-        return Provider(
+        return BaseProvider(
             name="auto_discovered",
             compute_resource=compute_resources[0],
             available_compute_resources=compute_resources,
         )
 
     return None
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.3.0/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.3.0/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.3.0/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.3.0/quantum_serverless/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,12 +19,16 @@
 
 Quantum serverless utilities
 ==============================
 
 .. autosummary::
     :toctree: ../stubs/
 
+    BaseStorage
+    S3Storage
+    ErrorCodes
     JsonSerializable
 """
 
 from .json import JsonSerializable
-from .storage import S3Storage
+from .errors import ErrorCodes
+from .storage import S3Storage, BaseStorage
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/utils/errors.py` & `quantum_serverless-0.3.0/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/utils/json.py` & `quantum_serverless-0.3.0/quantum_serverless/utils/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,54 +70,55 @@
     try:
         json.dumps(data, cls=cls)
         return True
     except (TypeError, OverflowError):
         return False
 
 
-def safe_json_request(request: Callable) -> Dict[str, Any]:
+def safe_json_request(request: Callable, verbose: bool = False) -> Dict[str, Any]:
     """Returns parsed json data from request.
 
     Args:
         request: callable for request.
+        verbose: post reason in error message
 
     Example:
         >>> safe_json_request(request=lambda: requests.get("https://ibm.com"))
 
     Returns:
         parsed json response
     """
     error_message: Optional[str] = None
     try:
         response = request()
     except requests.exceptions.RequestException as request_exception:
         error_message = format_err_msg(
             ErrorCodes.AUTH1001,
-            str(request_exception.args),
+            str(request_exception.args) if verbose else None,
         )
         response = None
 
     if error_message:
         raise QuantumServerlessException(error_message)
 
     if response is not None and not response.ok:
         raise QuantumServerlessException(
             format_err_msg(
                 response.status_code,
-                str(response.text),
+                str(response.text) if verbose else None,
             )
         )
 
     decoding_error_message: Optional[str] = None
     try:
         json_data = json.loads(response.text)
     except json.JSONDecodeError as json_error:
         decoding_error_message = format_err_msg(
             ErrorCodes.JSON1001,
-            str(json_error.args),
+            str(json_error.args) if verbose else None,
         )
         json_data = {}
 
     if decoding_error_message:
         raise QuantumServerlessException(decoding_error_message)
 
     return json_data
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/utils/storage.py` & `quantum_serverless-0.3.0/quantum_serverless/utils/storage.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless/visualizaiton/__init__.py` & `quantum_serverless-0.3.0/quantum_serverless/visualizaiton/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 =====================================================
-Core module (:mod:`quantum_serverless.visualization`)
+Visualization (:mod:`quantum_serverless.visualization`)
 =====================================================
 
 .. currentmodule:: quantum_serverless.visualization
 
 Quantum serverless visualisation module classes and functions
 =============================================================
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless/visualizaiton/widget.py` & `quantum_serverless-0.3.0/quantum_serverless/visualizaiton/widget.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.3.0/quantum_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.2.1
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.2.1/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.3.0/quantum_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/setup.py` & `quantum_serverless-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/tests/core/test_decorator.py` & `quantum_serverless-0.3.0/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/tests/core/test_program.py` & `quantum_serverless-0.3.0/tests/core/test_program.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests jobs."""
 import os
 
 from ray.dashboard.modules.job.common import JobStatus
 from testcontainers.compose import DockerCompose
 
-from quantum_serverless import QuantumServerless, Provider
+from quantum_serverless import QuantumServerless, BaseProvider
 from quantum_serverless.core import ComputeResource
 from quantum_serverless.core.job import Job
 from quantum_serverless.core.program import Program
 from tests.utils import wait_for_job_client, wait_for_job_completion
 
 resources_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "../resources"
@@ -20,15 +20,15 @@
 
     with DockerCompose(
         resources_path, compose_file_name="test-compose.yml", pull=True
     ) as compose:
         host = compose.get_service_host("testrayhead", 8265)
         port = compose.get_service_port("testrayhead", 8265)
 
-        provider = Provider(
+        provider = BaseProvider(
             name="docker",
             compute_resource=ComputeResource(
                 name="docker", host=host, port_job_server=port
             ),
         )
         serverless = QuantumServerless(provider).set_provider("docker")
```

### Comparing `quantum_serverless-0.2.1/tests/core/test_program_repository.py` & `quantum_serverless-0.3.0/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/tests/core/test_state.py` & `quantum_serverless-0.3.0/tests/core/test_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """Test state handlers."""
 import os
 
 from ray.dashboard.modules.job.common import JobStatus
 from testcontainers.compose import DockerCompose
 
-from quantum_serverless import QuantumServerless, Program, Provider
+from quantum_serverless import QuantumServerless, Program, BaseProvider
 from quantum_serverless.core import ComputeResource
 from quantum_serverless.core.state import RedisStateHandler
 from tests.utils import wait_for_job_client, wait_for_job_completion
 
 resources_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "../resources"
 )
@@ -42,15 +42,15 @@
 
         state_handler = RedisStateHandler(redis_host, redis_port)
 
         state_handler.set("some_key", {"key": "value"})
 
         assert state_handler.get("some_key") == {"key": "value"}
 
-        provider = Provider(
+        provider = BaseProvider(
             name="test_docker",
             compute_resource=ComputeResource(
                 name="test_docker", host=host, port_job_server=port
             ),
         )
         serverless = QuantumServerless(provider).set_provider("test_docker")
```

### Comparing `quantum_serverless-0.2.1/tests/library/test_transpiler.py` & `quantum_serverless-0.3.0/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.3.0/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/tests/serializers/test_serializers.py` & `quantum_serverless-0.3.0/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.1/tests/test_quantum_serverless.py` & `quantum_serverless-0.3.0/tests/test_quantum_serverless.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """Tests for QuantumServerless."""
 import json
 from unittest import TestCase
 
 import ray
 import requests_mock
 
-from quantum_serverless import QuantumServerless, Provider
+from quantum_serverless import QuantumServerless, BaseProvider
 from quantum_serverless.core import ComputeResource
 from quantum_serverless.quantum_serverless import get_auto_discovered_provider
 
 
 class TestQuantumServerless(TestCase):
     """Tests for QuantumServerless."""
 
@@ -41,15 +41,15 @@
         self.assertEqual(len(serverless.providers()), 1)
 
     def test_add_provider(self):
         """Test addition of provider."""
         serverless = QuantumServerless()
         self.assertEqual(len(serverless.providers()), 1)
 
-        serverless.add_provider(Provider("my_provider"))
+        serverless.add_provider(BaseProvider("my_provider"))
         self.assertEqual(len(serverless.providers()), 2)
 
     def test_all_context_allocations(self):
         """Test context allocation from provider and compute_resource calls."""
         serverless = QuantumServerless()
 
         with serverless.context():
@@ -84,18 +84,18 @@
                     ),
                 )
             serverless = QuantumServerless()
             providers = serverless.providers()
 
             self.assertEqual(len(providers), 1)
             for provider in providers:
-                self.assertIsInstance(provider, Provider)
+                self.assertIsInstance(provider, BaseProvider)
 
             provider = get_auto_discovered_provider(manager_address, token="token")
 
-            self.assertIsInstance(provider, Provider)
+            self.assertIsInstance(provider, BaseProvider)
 
-            if isinstance(provider, Provider):
+            if isinstance(provider, BaseProvider):
                 self.assertIsInstance(provider.compute_resource, ComputeResource)
                 self.assertEqual(len(provider.available_compute_resources), 4)
                 for cluster in provider.available_compute_resources:
                     self.assertIsInstance(cluster, ComputeResource)
```

### Comparing `quantum_serverless-0.2.1/tests/utils.py` & `quantum_serverless-0.3.0/tests/utils.py`

 * *Files identical despite different names*

