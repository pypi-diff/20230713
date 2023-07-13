# Comparing `tmp/verta-0.9.2.tar.gz` & `tmp/verta-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/verta-0.9.2.tar", last modified: Thu May  2 18:46:44 2019, max compression
+gzip compressed data, was "dist/verta-0.9.3.tar", last modified: Thu May  2 19:35:22 2019, max compression
```

## Comparing `verta-0.9.2.tar` & `verta-0.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 18:46:44.000000 verta-0.9.2/
--rw-r--r--   0 miliu      (501) staff       (20)      378 2019-05-02 18:46:44.000000 verta-0.9.2/PKG-INFO
--rw-r--r--   0 miliu      (501) staff       (20)        0 2019-05-02 14:44:26.000000 verta-0.9.2/README.md
--rw-r--r--   0 miliu      (501) staff       (20)       38 2019-05-02 18:46:44.000000 verta-0.9.2/setup.cfg
--rw-r--r--   0 miliu      (501) staff       (20)      819 2019-05-02 18:46:00.000000 verta-0.9.2/setup.py
-drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 18:46:44.000000 verta-0.9.2/verta/
--rw-r--r--   0 miliu      (501) staff       (20)       27 2019-05-02 14:44:26.000000 verta-0.9.2/verta/__init__.py
--rw-r--r--   0 miliu      (501) staff       (20)     8479 2019-05-02 17:53:45.000000 verta-0.9.2/verta/_artifact_utils.py
--rw-r--r--   0 miliu      (501) staff       (20)     4234 2019-05-02 14:44:26.000000 verta-0.9.2/verta/_demo_utils.py
-drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 18:46:44.000000 verta-0.9.2/verta/_protos/
-drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 18:46:44.000000 verta-0.9.2/verta/_protos/public/
-drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 18:46:44.000000 verta-0.9.2/verta/_protos/public/modeldb/
--rw-r--r--   0 miliu      (501) staff       (20)    20157 2019-04-29 22:04:24.000000 verta-0.9.2/verta/_protos/public/modeldb/CommonService_pb2.py
--rw-r--r--   0 miliu      (501) staff       (20)       83 2019-04-29 22:04:24.000000 verta-0.9.2/verta/_protos/public/modeldb/CommonService_pb2_grpc.py
--rw-r--r--   0 miliu      (501) staff       (20)   149029 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/ExperimentRunService_pb2.py
--rw-r--r--   0 miliu      (501) staff       (20)    32570 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/ExperimentRunService_pb2_grpc.py
--rw-r--r--   0 miliu      (501) staff       (20)    50886 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/ExperimentService_pb2.py
--rw-r--r--   0 miliu      (501) staff       (20)    14357 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/ExperimentService_pb2_grpc.py
--rw-r--r--   0 miliu      (501) staff       (20)    24171 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/Job_pb2.py
--rw-r--r--   0 miliu      (501) staff       (20)     4232 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/Job_pb2_grpc.py
--rw-r--r--   0 miliu      (501) staff       (20)    54264 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/ProjectService_pb2.py
--rw-r--r--   0 miliu      (501) staff       (20)    14867 2019-04-29 23:19:56.000000 verta-0.9.2/verta/_protos/public/modeldb/ProjectService_pb2_grpc.py
--rw-r--r--   0 miliu      (501) staff       (20)        0 2019-04-24 00:50:42.000000 verta-0.9.2/verta/_protos/public/modeldb/__init__.py
--rw-r--r--   0 miliu      (501) staff       (20)     6537 2019-05-02 18:44:28.000000 verta-0.9.2/verta/_utils.py
--rw-r--r--   0 miliu      (501) staff       (20)    68905 2019-05-02 18:44:28.000000 verta-0.9.2/verta/client.py
--rw-r--r--   0 miliu      (501) staff       (20)     1190 2019-05-02 14:44:26.000000 verta-0.9.2/verta/utils.py
-drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 18:46:44.000000 verta-0.9.2/verta.egg-info/
--rw-r--r--   0 miliu      (501) staff       (20)      378 2019-05-02 18:46:43.000000 verta-0.9.2/verta.egg-info/PKG-INFO
--rw-r--r--   0 miliu      (501) staff       (20)      843 2019-05-02 18:46:44.000000 verta-0.9.2/verta.egg-info/SOURCES.txt
--rw-r--r--   0 miliu      (501) staff       (20)        1 2019-05-02 18:46:43.000000 verta-0.9.2/verta.egg-info/dependency_links.txt
--rw-r--r--   0 miliu      (501) staff       (20)      124 2019-05-02 18:46:43.000000 verta-0.9.2/verta.egg-info/requires.txt
--rw-r--r--   0 miliu      (501) staff       (20)        6 2019-05-02 18:46:43.000000 verta-0.9.2/verta.egg-info/top_level.txt
+drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 19:35:22.000000 verta-0.9.3/
+-rw-r--r--   0 miliu      (501) staff       (20)      378 2019-05-02 19:35:22.000000 verta-0.9.3/PKG-INFO
+-rw-r--r--   0 miliu      (501) staff       (20)        0 2019-05-02 14:44:26.000000 verta-0.9.3/README.md
+-rw-r--r--   0 miliu      (501) staff       (20)       38 2019-05-02 19:35:22.000000 verta-0.9.3/setup.cfg
+-rw-r--r--   0 miliu      (501) staff       (20)      820 2019-05-02 19:32:50.000000 verta-0.9.3/setup.py
+drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 19:35:22.000000 verta-0.9.3/verta/
+-rw-r--r--   0 miliu      (501) staff       (20)       27 2019-05-02 14:44:26.000000 verta-0.9.3/verta/__init__.py
+-rw-r--r--   0 miliu      (501) staff       (20)     8479 2019-05-02 18:50:12.000000 verta-0.9.3/verta/_artifact_utils.py
+-rw-r--r--   0 miliu      (501) staff       (20)     4234 2019-05-02 14:44:26.000000 verta-0.9.3/verta/_demo_utils.py
+drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 19:35:22.000000 verta-0.9.3/verta/_protos/
+drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 19:35:22.000000 verta-0.9.3/verta/_protos/public/
+drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 19:35:22.000000 verta-0.9.3/verta/_protos/public/modeldb/
+-rw-r--r--   0 miliu      (501) staff       (20)    20157 2019-04-29 22:04:24.000000 verta-0.9.3/verta/_protos/public/modeldb/CommonService_pb2.py
+-rw-r--r--   0 miliu      (501) staff       (20)       83 2019-04-29 22:04:24.000000 verta-0.9.3/verta/_protos/public/modeldb/CommonService_pb2_grpc.py
+-rw-r--r--   0 miliu      (501) staff       (20)   149029 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/ExperimentRunService_pb2.py
+-rw-r--r--   0 miliu      (501) staff       (20)    32570 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/ExperimentRunService_pb2_grpc.py
+-rw-r--r--   0 miliu      (501) staff       (20)    50886 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/ExperimentService_pb2.py
+-rw-r--r--   0 miliu      (501) staff       (20)    14357 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/ExperimentService_pb2_grpc.py
+-rw-r--r--   0 miliu      (501) staff       (20)    24171 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/Job_pb2.py
+-rw-r--r--   0 miliu      (501) staff       (20)     4232 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/Job_pb2_grpc.py
+-rw-r--r--   0 miliu      (501) staff       (20)    54264 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/ProjectService_pb2.py
+-rw-r--r--   0 miliu      (501) staff       (20)    14867 2019-04-29 23:19:56.000000 verta-0.9.3/verta/_protos/public/modeldb/ProjectService_pb2_grpc.py
+-rw-r--r--   0 miliu      (501) staff       (20)        0 2019-04-24 00:50:42.000000 verta-0.9.3/verta/_protos/public/modeldb/__init__.py
+-rw-r--r--   0 miliu      (501) staff       (20)     6537 2019-05-02 18:50:37.000000 verta-0.9.3/verta/_utils.py
+-rw-r--r--   0 miliu      (501) staff       (20)    68905 2019-05-02 18:50:12.000000 verta-0.9.3/verta/client.py
+-rw-r--r--   0 miliu      (501) staff       (20)     1190 2019-05-02 14:44:26.000000 verta-0.9.3/verta/utils.py
+drwxr-xr-x   0 miliu      (501) staff       (20)        0 2019-05-02 19:35:22.000000 verta-0.9.3/verta.egg-info/
+-rw-r--r--   0 miliu      (501) staff       (20)      378 2019-05-02 19:35:21.000000 verta-0.9.3/verta.egg-info/PKG-INFO
+-rw-r--r--   0 miliu      (501) staff       (20)      843 2019-05-02 19:35:21.000000 verta-0.9.3/verta.egg-info/SOURCES.txt
+-rw-r--r--   0 miliu      (501) staff       (20)        1 2019-05-02 19:35:21.000000 verta-0.9.3/verta.egg-info/dependency_links.txt
+-rw-r--r--   0 miliu      (501) staff       (20)      125 2019-05-02 19:35:21.000000 verta-0.9.3/verta.egg-info/requires.txt
+-rw-r--r--   0 miliu      (501) staff       (20)        6 2019-05-02 19:35:21.000000 verta-0.9.3/verta.egg-info/top_level.txt
```

### Comparing `verta-0.9.2/setup.py` & `verta-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
     name="verta",
-    version="0.9.2",
+    version="0.9.3",
     maintainer="Michael Liu",
     maintainer_email="miliu@verta.ai",
     description="Python client for interfacing with ModelDB and the Verta platform",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.verta.ai/",
     packages=[
         "verta",
         "verta._protos.public.modeldb",
     ],
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
     install_requires=[
-        "cloudpickle"
+        "cloudpickle",
         "googleapis-common-protos>=1.5",
         "grpcio>=1.16",
         "pathlib2>=2.1",
         "pillow>=5.2, <7.0",
         "protobuf>=3.6",
         "requests>=2.21",
         "six>=1.12",
```

### Comparing `verta-0.9.2/verta/_artifact_utils.py` & `verta-0.9.3/verta/_artifact_utils.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_demo_utils.py` & `verta-0.9.3/verta/_demo_utils.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/CommonService_pb2.py` & `verta-0.9.3/verta/_protos/public/modeldb/CommonService_pb2.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/ExperimentRunService_pb2.py` & `verta-0.9.3/verta/_protos/public/modeldb/ExperimentRunService_pb2.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/ExperimentRunService_pb2_grpc.py` & `verta-0.9.3/verta/_protos/public/modeldb/ExperimentRunService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/ExperimentService_pb2.py` & `verta-0.9.3/verta/_protos/public/modeldb/ExperimentService_pb2.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/ExperimentService_pb2_grpc.py` & `verta-0.9.3/verta/_protos/public/modeldb/ExperimentService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/Job_pb2.py` & `verta-0.9.3/verta/_protos/public/modeldb/Job_pb2.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/Job_pb2_grpc.py` & `verta-0.9.3/verta/_protos/public/modeldb/Job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/ProjectService_pb2.py` & `verta-0.9.3/verta/_protos/public/modeldb/ProjectService_pb2.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_protos/public/modeldb/ProjectService_pb2_grpc.py` & `verta-0.9.3/verta/_protos/public/modeldb/ProjectService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/_utils.py` & `verta-0.9.3/verta/_utils.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/client.py` & `verta-0.9.3/verta/client.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta/utils.py` & `verta-0.9.3/verta/utils.py`

 * *Files identical despite different names*

### Comparing `verta-0.9.2/verta.egg-info/SOURCES.txt` & `verta-0.9.3/verta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

