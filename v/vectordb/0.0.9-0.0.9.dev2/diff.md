# Comparing `tmp/vectordb-0.0.9.tar.gz` & `tmp/vectordb-0.0.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vectordb-0.0.9.tar", last modified: Tue Jul 11 15:58:29 2023, max compression
+gzip compressed data, was "vectordb-0.0.9.dev2.tar", last modified: Tue Jul 11 15:57:59 2023, max compression
```

## Comparing `vectordb-0.0.9.tar` & `vectordb-0.0.9.dev2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-07-11 15:58:29.000000 vectordb-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-11 15:58:18.000000 vectordb-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:58:29.000000 vectordb-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-11 15:58:18.000000 vectordb-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:58:18.000000 vectordb-0.0.9/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-11 15:58:18.000000 vectordb-0.0.9/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 15:58:29.000000 vectordb-0.0.9/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-11 15:57:53.000000 vectordb-0.0.9.dev2/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:57:59.320327 vectordb-0.0.9.dev2/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 15:57:59.000000 vectordb-0.0.9.dev2/vectordb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vectordb-0.0.9/README.md` & `vectordb-0.0.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/setup.py` & `vectordb-0.0.9.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.9.dev2/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.9.dev2/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.9.dev2/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.9.dev2/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/__main__.py` & `vectordb-0.0.9.dev2/vectordb/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/client/client.py` & `vectordb-0.0.9.dev2/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/db/base.py` & `vectordb-0.0.9.dev2/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.9.dev2/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.9.dev2/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.9.dev2/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/db/service.py` & `vectordb-0.0.9.dev2/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/utils/create_doc_type.py` & `vectordb-0.0.9.dev2/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/utils/pass_parameters.py` & `vectordb-0.0.9.dev2/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.9.dev2/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.9.dev2/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb/utils/unify_input_output.py` & `vectordb-0.0.9.dev2/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.9/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.9.dev2/vectordb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/test_hnswlib_vectordb_serve.py
 tests/integration/test_inmemory_vectordb_serve.py
```

