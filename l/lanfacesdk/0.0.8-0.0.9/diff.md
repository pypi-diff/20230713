# Comparing `tmp/lanfacesdk-0.0.8.tar.gz` & `tmp/lanfacesdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lanfacesdk-0.0.8.tar", last modified: Mon Jun 20 11:41:16 2022, max compression
+gzip compressed data, was "dist/lanfacesdk-0.0.9.tar", last modified: Mon Jun 20 11:43:34 2022, max compression
```

## Comparing `lanfacesdk-0.0.8.tar` & `lanfacesdk-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:41:16.990486 lanfacesdk-0.0.8/
--rw-r--r--   0 changwei   (501) staff       (20)      195 2022-06-20 11:41:16.990200 lanfacesdk-0.0.8/PKG-INFO
--rw-r--r--   0 changwei   (501) staff       (20)      629 2021-10-29 06:49:44.000000 lanfacesdk-0.0.8/README.md
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:41:16.985291 lanfacesdk-0.0.8/lanfacesdk/
--rw-r--r--   0 changwei   (501) staff       (20)      768 2021-12-08 08:43:37.000000 lanfacesdk-0.0.8/lanfacesdk/facemodel.py
--rw-r--r--   0 changwei   (501) staff       (20)     2720 2021-10-29 06:31:18.000000 lanfacesdk-0.0.8/lanfacesdk/model_1.py
--rw-r--r--   0 changwei   (501) staff       (20)     2195 2022-06-20 11:40:57.000000 lanfacesdk-0.0.8/lanfacesdk/model_2.py
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:41:16.988600 lanfacesdk-0.0.8/lanfacesdk/proto_1/
--rw-r--r--   0 changwei   (501) staff       (20)     3971 2021-10-29 05:39:25.000000 lanfacesdk-0.0.8/lanfacesdk/proto_1/face_grpc_pb2.py
--rw-r--r--   0 changwei   (501) staff       (20)     1506 2021-10-29 06:03:42.000000 lanfacesdk-0.0.8/lanfacesdk/proto_1/face_grpc_pb2_grpc.py
--rw-r--r--   0 changwei   (501) staff       (20)    10794 2021-10-29 05:39:25.000000 lanfacesdk-0.0.8/lanfacesdk/proto_1/facerecog_pb2.py
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:41:16.989743 lanfacesdk-0.0.8/lanfacesdk/proto_2/
--rw-r--r--   0 changwei   (501) staff       (20)        0 2021-10-29 05:39:40.000000 lanfacesdk-0.0.8/lanfacesdk/proto_2/__init__.py
--rw-r--r--   0 changwei   (501) staff       (20)    13342 2021-10-29 05:39:40.000000 lanfacesdk-0.0.8/lanfacesdk/proto_2/facerec_pb2.py
--rw-r--r--   0 changwei   (501) staff       (20)     3772 2021-10-29 05:39:40.000000 lanfacesdk-0.0.8/lanfacesdk/proto_2/facerec_pb2_grpc.py
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:41:16.986997 lanfacesdk-0.0.8/lanfacesdk.egg-info/
--rw-r--r--   0 changwei   (501) staff       (20)      195 2022-06-20 11:41:16.000000 lanfacesdk-0.0.8/lanfacesdk.egg-info/PKG-INFO
--rw-r--r--   0 changwei   (501) staff       (20)      468 2022-06-20 11:41:16.000000 lanfacesdk-0.0.8/lanfacesdk.egg-info/SOURCES.txt
--rw-r--r--   0 changwei   (501) staff       (20)        1 2022-06-20 11:41:16.000000 lanfacesdk-0.0.8/lanfacesdk.egg-info/dependency_links.txt
--rw-r--r--   0 changwei   (501) staff       (20)       49 2022-06-20 11:41:16.000000 lanfacesdk-0.0.8/lanfacesdk.egg-info/top_level.txt
--rw-r--r--   0 changwei   (501) staff       (20)        1 2022-06-20 11:41:16.000000 lanfacesdk-0.0.8/lanfacesdk.egg-info/zip-safe
--rw-r--r--   0 changwei   (501) staff       (20)       38 2022-06-20 11:41:16.990600 lanfacesdk-0.0.8/setup.cfg
--rw-r--r--   0 changwei   (501) staff       (20)      871 2022-06-20 11:41:06.000000 lanfacesdk-0.0.8/setup.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:43:34.251124 lanfacesdk-0.0.9/
+-rw-r--r--   0 changwei   (501) staff       (20)      195 2022-06-20 11:43:34.250727 lanfacesdk-0.0.9/PKG-INFO
+-rw-r--r--   0 changwei   (501) staff       (20)      629 2021-10-29 06:49:44.000000 lanfacesdk-0.0.9/README.md
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:43:34.244726 lanfacesdk-0.0.9/lanfacesdk/
+-rw-r--r--   0 changwei   (501) staff       (20)      768 2021-12-08 08:43:37.000000 lanfacesdk-0.0.9/lanfacesdk/facemodel.py
+-rw-r--r--   0 changwei   (501) staff       (20)     2720 2021-10-29 06:31:18.000000 lanfacesdk-0.0.9/lanfacesdk/model_1.py
+-rw-r--r--   0 changwei   (501) staff       (20)     2224 2022-06-20 11:43:25.000000 lanfacesdk-0.0.9/lanfacesdk/model_2.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:43:34.248690 lanfacesdk-0.0.9/lanfacesdk/proto_1/
+-rw-r--r--   0 changwei   (501) staff       (20)     3971 2021-10-29 05:39:25.000000 lanfacesdk-0.0.9/lanfacesdk/proto_1/face_grpc_pb2.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1506 2021-10-29 06:03:42.000000 lanfacesdk-0.0.9/lanfacesdk/proto_1/face_grpc_pb2_grpc.py
+-rw-r--r--   0 changwei   (501) staff       (20)    10794 2021-10-29 05:39:25.000000 lanfacesdk-0.0.9/lanfacesdk/proto_1/facerecog_pb2.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:43:34.250092 lanfacesdk-0.0.9/lanfacesdk/proto_2/
+-rw-r--r--   0 changwei   (501) staff       (20)        0 2021-10-29 05:39:40.000000 lanfacesdk-0.0.9/lanfacesdk/proto_2/__init__.py
+-rw-r--r--   0 changwei   (501) staff       (20)    13342 2021-10-29 05:39:40.000000 lanfacesdk-0.0.9/lanfacesdk/proto_2/facerec_pb2.py
+-rw-r--r--   0 changwei   (501) staff       (20)     3772 2021-10-29 05:39:40.000000 lanfacesdk-0.0.9/lanfacesdk/proto_2/facerec_pb2_grpc.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2022-06-20 11:43:34.247198 lanfacesdk-0.0.9/lanfacesdk.egg-info/
+-rw-r--r--   0 changwei   (501) staff       (20)      195 2022-06-20 11:43:34.000000 lanfacesdk-0.0.9/lanfacesdk.egg-info/PKG-INFO
+-rw-r--r--   0 changwei   (501) staff       (20)      468 2022-06-20 11:43:34.000000 lanfacesdk-0.0.9/lanfacesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 changwei   (501) staff       (20)        1 2022-06-20 11:43:34.000000 lanfacesdk-0.0.9/lanfacesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 changwei   (501) staff       (20)       49 2022-06-20 11:43:34.000000 lanfacesdk-0.0.9/lanfacesdk.egg-info/top_level.txt
+-rw-r--r--   0 changwei   (501) staff       (20)        1 2022-06-20 11:43:34.000000 lanfacesdk-0.0.9/lanfacesdk.egg-info/zip-safe
+-rw-r--r--   0 changwei   (501) staff       (20)       38 2022-06-20 11:43:34.251273 lanfacesdk-0.0.9/setup.cfg
+-rw-r--r--   0 changwei   (501) staff       (20)      871 2022-06-20 11:43:29.000000 lanfacesdk-0.0.9/setup.py
```

### Comparing `lanfacesdk-0.0.8/README.md` & `lanfacesdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/facemodel.py` & `lanfacesdk-0.0.9/lanfacesdk/facemodel.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/model_1.py` & `lanfacesdk-0.0.9/lanfacesdk/model_1.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/model_2.py` & `lanfacesdk-0.0.9/lanfacesdk/model_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 
 class FaceModel(BaseFaceMoel):
     def __init__(self, filename, channel, *, is_full=False, min_area=-1, input_type="file"):
         super().__init__(filename, channel, is_full=is_full, min_area=min_area)
 
         self._features = [] 
         self._load_features()
+        self.input_type=input_type
 
     def _compute(self, num):
         return math.ceil(num/160)*160
 
     def _load_features(self):
         
         with self._channel() as ch:
             stub = facerec_pb2_grpc.FaceRecStub(ch)
 
-            if input_type=='file':
+            if self.input_type=='file':
                 img = cv2.imread(self.filename)
-            elif input_type == 'img':
+            elif self.input_type == 'img':
                 img = self.filename
             else:
                 raise Exception("错误的类型")
-                
+
             height,width,_ = img.shape
 
             img_encode = cv2.imencode('.jpg', img)[1]
             img_data = img_encode.tobytes()
             resp = stub.GetFeatures(facerec_pb2.ImageReq(image=img_data, width=640, height=640))
             #ch.close()
```

### Comparing `lanfacesdk-0.0.8/lanfacesdk/proto_1/face_grpc_pb2.py` & `lanfacesdk-0.0.9/lanfacesdk/proto_1/face_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/proto_1/face_grpc_pb2_grpc.py` & `lanfacesdk-0.0.9/lanfacesdk/proto_1/face_grpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/proto_1/facerecog_pb2.py` & `lanfacesdk-0.0.9/lanfacesdk/proto_1/facerecog_pb2.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/proto_2/facerec_pb2.py` & `lanfacesdk-0.0.9/lanfacesdk/proto_2/facerec_pb2.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/lanfacesdk/proto_2/facerec_pb2_grpc.py` & `lanfacesdk-0.0.9/lanfacesdk/proto_2/facerec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lanfacesdk-0.0.8/setup.py` & `lanfacesdk-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #-*- encoding: UTF-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name = "lanfacesdk",                # 包名
     author = "changwei",
     author_email = "nkchwfree@163.com",
-    version = "0.0.8",              # 版本信息
+    version = "0.0.9",              # 版本信息
     packages = ['lanfacesdk', 'lanfacesdk/proto_1', 'lanfacesdk/proto_2'],          # 要打包的项目文件夹
     include_package_data=True,    # 自动打包文件夹内所有数据
     zip_safe=True,                # 设定项目包为安全，不用每次都检测其安全性
     install_requires = [          # 安装依赖的其他包（测试数据）
     ],
 
     # 设置程序的入口为path
```

