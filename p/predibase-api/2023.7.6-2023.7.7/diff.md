# Comparing `tmp/predibase-api-2023.7.6.tar.gz` & `tmp/predibase-api-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2023.7.6.tar", last modified: Fri Jul  7 22:43:53 2023, max compression
+gzip compressed data, was "predibase-api-2023.7.7.tar", last modified: Thu Jul 13 05:17:35 2023, max compression
```

## Comparing `predibase-api-2023.7.6.tar` & `predibase-api-2023.7.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.026620 predibase-api-2023.7.6/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 22:43:52.000000 predibase-api-2023.7.6/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 22:43:52.000000 predibase-api-2023.7.6/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:43:52.000000 predibase-api-2023.7.6/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:43:20.000000 predibase-api-2023.7.6/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 22:43:52.000000 predibase-api-2023.7.6/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 22:43:52.000000 predibase-api-2023.7.6/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:43:53.030620 predibase-api-2023.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-07 22:42:40.000000 predibase-api-2023.7.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 22:43:40.000000 predibase-api-2023.7.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.416872 predibase-api-2023.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 05:17:35.416872 predibase-api-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.404872 predibase-api-2023.7.7/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.408872 predibase-api-2023.7.7/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.408872 predibase-api-2023.7.7/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.408872 predibase-api-2023.7.7/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.412872 predibase-api-2023.7.7/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.412872 predibase-api-2023.7.7/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.412872 predibase-api-2023.7.7/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.412872 predibase-api-2023.7.7/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.416872 predibase-api-2023.7.7/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.416872 predibase-api-2023.7.7/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.416872 predibase-api-2023.7.7/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:17:35.408872 predibase-api-2023.7.7/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 05:17:35.000000 predibase-api-2023.7.7/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-13 05:17:35.000000 predibase-api-2023.7.7/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:17:35.000000 predibase-api-2023.7.7/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:17:01.000000 predibase-api-2023.7.7/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 05:17:35.000000 predibase-api-2023.7.7/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 05:17:35.000000 predibase-api-2023.7.7/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:17:35.416872 predibase-api-2023.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 05:16:25.000000 predibase-api-2023.7.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 05:17:24.000000 predibase-api-2023.7.7/version.txt
```

### Comparing `predibase-api-2023.7.6/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2023.7.7/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2023.7.7/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2023.7.7/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2023.7.7/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2023.7.7/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2023.7.7/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2023.7.7/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.6/setup.py` & `predibase-api-2023.7.7/setup.py`

 * *Files identical despite different names*

