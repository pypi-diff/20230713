# Comparing `tmp/dequeai-0.8230.tar.gz` & `tmp/dequeai-0.8232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.8230.tar", last modified: Thu Jul 13 00:04:14 2023, max compression
+gzip compressed data, was "dequeai-0.8232.tar", last modified: Thu Jul 13 19:30:37 2023, max compression
```

## Comparing `dequeai-0.8230.tar` & `dequeai-0.8232.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:04:14.262365 dequeai-0.8230/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 00:04:14.262365 dequeai-0.8230/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:04:14.262365 dequeai-0.8230/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8230/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16632 2023-07-13 00:04:01.000000 dequeai-0.8230/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8230/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8230/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8230/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8230/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8230/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8230/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8230/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8230/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8230/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:04:14.262365 dequeai-0.8230/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 00:04:13.000000 dequeai-0.8230/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-13 00:04:14.000000 dequeai-0.8230/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:04:13.000000 dequeai-0.8230/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-13 00:04:14.000000 dequeai-0.8230/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-13 00:04:14.000000 dequeai-0.8230/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 00:04:14.262365 dequeai-0.8230/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-13 00:04:01.000000 dequeai-0.8230/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:30:37.743265 dequeai-0.8232/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 19:30:37.743265 dequeai-0.8232/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:30:37.743265 dequeai-0.8232/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8232/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17283 2023-07-13 19:30:08.000000 dequeai-0.8232/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8232/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8232/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8232/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8232/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8232/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8232/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8232/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8232/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8232/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:30:37.743265 dequeai-0.8232/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 19:30:37.743265 dequeai-0.8232/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-13 19:30:25.000000 dequeai-0.8232/setup.py
```

### Comparing `dequeai-0.8230/dequeai/datatypes.py` & `dequeai-0.8232/dequeai/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
                     self._box_data.append(box_data)
             elif data.ndim == 4:
                 for i, d in enumerate(data):
 
                     image_i = d[i]
                     self._process_image(image_i, mode)
                     if box_data is not None:
+                        if not isinstance(box_data, list):
+                            raise ValueError("box_data must be a list of BoundingBox2d objects")
                         for b in box_data[i]:
                             if not isinstance(b, BoundingBox2D):
                                 raise ValueError("All elements in box_data list must be BoundingBox2d objects")
                         self._box_data.append(box_data[i])
             else:
                 raise ValueError("numpy array must be 3 or 4 dimensional")
 
@@ -117,28 +119,36 @@
 
     def _tensor_to_numpy_image(self, torch_module, pic, mode):
 
         if not (isinstance(pic, torch_module.Tensor) or isinstance(pic, np.ndarray)):
             raise TypeError(f"pic should be Tensor or ndarray. Got {type(pic)}.")
 
         elif isinstance(pic, torch_module.Tensor):
-            if pic.ndimension() not in {2, 3}:
+            if pic.ndimension() not in {2, 3, 4}:
+                print(f"torch tensor pic should be 2/3/4 dimensional. Got {pic.ndim} dimensions.")
                 raise ValueError(f"pic should be 2/3 dimensional. Got {pic.ndimension()} dimensions.")
 
             elif pic.ndimension() == 2:
                 # if 2D image, add channel dimension (CHW)
                 pic = pic.unsqueeze(0)
 
             # check number of channels
-            if pic.shape[-3] > 4:
-                raise ValueError(f"pic should not have > 4 channels. Got {pic.shape[-3]} channels.")
+                # pic is a batch of images, process each one individually
+                images = []
+                for img in pic:
+                    # Convert tensor to numpy array, transpose dimensions, and convert to Image
+                    npimg = img.numpy()
+                    npimg = np.transpose(npimg, (1, 2, 0))
+                    image = Image.fromarray(np.uint8(npimg))
+                    images.append(image)
 
         elif isinstance(pic, np.ndarray):
-            if pic.ndim not in {2, 3}:
-                raise ValueError(f"pic should be 2/3 dimensional. Got {pic.ndim} dimensions.")
+            if pic.ndim not in {2, 3, 4}:
+                print(f"numpy pic should be 2/3/4 dimensional. Got {pic.ndim} dimensions.")
+                raise ValueError(f"pic should be 2/3/4 dimensional. Got {pic.ndim} dimensions.")
 
             elif pic.ndim == 2:
                 # if 2D image, add channel dimension (HWC)
                 pic = np.expand_dims(pic, 2)
 
             # check number of channels
             if pic.shape[-1] > 4:
```

### Comparing `dequeai-0.8230/dequeai/dequeai.py` & `dequeai-0.8232/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8230/dequeai/dequeai_model.py` & `dequeai-0.8232/dequeai/dequeai_model.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8230/dequeai/dequeai_run.py` & `dequeai-0.8232/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8230/dequeai/parsing_service.py` & `dequeai-0.8232/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8230/dequeai/rest_connect.py` & `dequeai-0.8232/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8230/dequeai/util.py` & `dequeai-0.8232/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8230/setup.py` & `dequeai-0.8232/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.000008230',
+    version='0.000008232',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='dequeai client for deep learning',
     install_requires=[
```

