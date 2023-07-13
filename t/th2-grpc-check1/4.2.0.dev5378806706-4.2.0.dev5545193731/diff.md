# Comparing `tmp/th2_grpc_check1-4.2.0.dev5378806706.tar.gz` & `tmp/th2_grpc_check1-4.2.0.dev5545193731.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_check1-4.2.0.dev5378806706.tar", last modified: Mon Jun 26 13:38:17 2023, max compression
+gzip compressed data, was "dist/th2_grpc_check1-4.2.0.dev5545193731.tar", last modified: Thu Jul 13 15:51:37 2023, max compression
```

## Comparing `th2_grpc_check1-4.2.0.dev5378806706.tar` & `th2_grpc_check1-4.2.0.dev5545193731.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6110 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    17519 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7709 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-26 13:37:50.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_service.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-07-13 15:50:21.000000 th2_grpc_check1-4.2.0.dev5545193731/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-13 15:50:22.000000 th2_grpc_check1-4.2.0.dev5545193731/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4567 2023-07-13 15:50:21.000000 th2_grpc_check1-4.2.0.dev5545193731/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-07-13 15:50:21.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6110 2023-07-13 15:51:36.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17519 2023-07-13 15:51:36.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7709 2023-07-13 15:51:36.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-07-13 15:51:09.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-13 15:51:37.000000 th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/top_level.txt
```

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/PKG-INFO` & `th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_grpc_check1
-Version: 4.2.0.dev5378806706
+Name: th2-grpc-check1
+Version: 4.2.0.dev5545193731
 Summary: th2_grpc_check1
 Home-page: https://github.com/th2-net/th2-grpc-check1
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC check1 library (4.2.0)
```

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/README.md` & `th2_grpc_check1-4.2.0.dev5545193731/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/setup.py` & `th2_grpc_check1-4.2.0.dev5545193731/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.strict_mode = False
 
     def finalize_options(self):
         pass
 
     def run(self):
         proto_path = os.path.abspath('src/main/proto')
-        gen_path = os.path.abspath('src/gen/main/python')
+        gen_path = os.path.abspath('build/generated/source/proto/main/services/python')
 
         if not os.path.exists(gen_path):
             os.makedirs(gen_path)
 
         proto_files = []
         for root, _, files in os.walk(proto_path):
             for filename in files:
@@ -68,16 +68,15 @@
 
 
 class CustomDist(sdist):
 
     def run(self):
         copy_tree(f'src/main/proto/{package_name}', package_name)
 
-        copy_tree(f'src/gen/main/python/{package_name}', package_name)
-        copy_tree(f'src/gen/main/services/python/{package_name}', package_name)
+        copy_tree(f'build/generated/source/proto/main/services/python/{package_name}', package_name)
         Path(f'{package_name}/__init__.py').touch()
         Path(f'{package_name}/py.typed').touch()
 
         def make_packages(root_dir):
             for path in Path(root_dir).iterdir():
                 if path.is_dir():
                     path.joinpath('__init__.py').touch()
```

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1.proto` & `th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.py` & `th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.pyi` & `th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2_grpc.py` & `th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_service.py` & `th2_grpc_check1-4.2.0.dev5545193731/th2_grpc_check1/check1_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/PKG-INFO` & `th2_grpc_check1-4.2.0.dev5545193731/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-grpc-check1
-Version: 4.2.0.dev5378806706
+Name: th2_grpc_check1
+Version: 4.2.0.dev5545193731
 Summary: th2_grpc_check1
 Home-page: https://github.com/th2-net/th2-grpc-check1
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC check1 library (4.2.0)
```

