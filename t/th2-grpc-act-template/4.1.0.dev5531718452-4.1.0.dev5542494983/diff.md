# Comparing `tmp/th2_grpc_act_template-4.1.0.dev5531718452.tar.gz` & `tmp/th2_grpc_act_template-4.1.0.dev5542494983.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_template-4.1.0.dev5531718452.tar", last modified: Wed Jul 12 12:43:33 2023, max compression
+gzip compressed data, was "dist/th2_grpc_act_template-4.1.0.dev5542494983.tar", last modified: Thu Jul 13 11:26:02 2023, max compression
```

## Comparing `th2_grpc_act_template-4.1.0.dev5531718452.tar` & `th2_grpc_act_template-4.1.0.dev5542494983.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-07-12 12:42:42.000000 th2_grpc_act_template-4.1.0.dev5531718452/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-12 12:42:43.000000 th2_grpc_act_template-4.1.0.dev5531718452/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-07-12 12:42:42.000000 th2_grpc_act_template-4.1.0.dev5531718452/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-12 12:43:14.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-12 12:42:42.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-12 12:43:33.000000 th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-07-13 11:24:56.000000 th2_grpc_act_template-4.1.0.dev5542494983/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-13 11:24:57.000000 th2_grpc_act_template-4.1.0.dev5542494983/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-07-13 11:24:56.000000 th2_grpc_act_template-4.1.0.dev5542494983/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-13 11:25:38.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-13 11:24:56.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-13 11:26:01.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-07-13 11:26:01.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-07-13 11:26:01.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-13 11:26:02.000000 th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/PKG-INFO` & `th2_grpc_act_template-4.1.0.dev5542494983/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_template
-Version: 4.1.0.dev5531718452
+Version: 4.1.0.dev5542494983
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
```

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/README.md` & `th2_grpc_act_template-4.1.0.dev5542494983/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/setup.py` & `th2_grpc_act_template-4.1.0.dev5542494983/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_service.py` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template.proto` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template_pb2.py` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template_pb2.pyi` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template/act_template_pb2_grpc.py` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template/act_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/PKG-INFO` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-template
-Version: 4.1.0.dev5531718452
+Version: 4.1.0.dev5542494983
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
```

### Comparing `th2_grpc_act_template-4.1.0.dev5531718452/th2_grpc_act_template.egg-info/SOURCES.txt` & `th2_grpc_act_template-4.1.0.dev5542494983/th2_grpc_act_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

