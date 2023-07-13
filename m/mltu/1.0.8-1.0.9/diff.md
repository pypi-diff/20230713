# Comparing `tmp/mltu-1.0.8.tar.gz` & `tmp/mltu-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltu-1.0.8.tar", last modified: Mon Apr 24 10:23:36 2023, max compression
+gzip compressed data, was "mltu-1.0.9.tar", last modified: Wed May 24 08:38:06 2023, max compression
```

## Comparing `mltu-1.0.8.tar` & `mltu-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2022-12-01 14:15:30.000000 mltu-1.0.8/LICENSE
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       24 2023-03-21 13:22:41.000000 mltu-1.0.8/MANIFEST.in
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-24 10:23:36.463201 mltu-1.0.8/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2054 2023-03-21 13:22:41.000000 mltu-1.0.8/README.md
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.459201 mltu-1.0.8/mltu/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       59 2023-04-24 10:23:12.000000 mltu-1.0.8/mltu/__init__.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.459201 mltu-1.0.8/mltu/annotations/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-22 13:58:16.000000 mltu-1.0.8/mltu/annotations/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3276 2023-03-22 13:58:36.000000 mltu-1.0.8/mltu/annotations/image.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    13996 2023-04-24 10:23:12.000000 mltu-1.0.8/mltu/augmentors.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      867 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/configs.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10449 2023-04-13 14:05:02.000000 mltu-1.0.8/mltu/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2006 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/inferenceModel.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6112 2023-03-22 13:58:36.000000 mltu-1.0.8/mltu/preprocessors.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/mltu/tensorflow/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2718 2023-03-22 13:58:41.000000 mltu-1.0.8/mltu/tensorflow/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      224 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     7266 2023-04-24 10:23:12.000000 mltu-1.0.8/mltu/tensorflow/layers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      896 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/losses.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    12415 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3402 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/tensorflow/model_utils.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/mltu/torch/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    14543 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3810 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3691 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/handlers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1154 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/losses.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     5184 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8139 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/torch/model.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6224 2023-03-22 13:58:16.000000 mltu-1.0.8/mltu/transformers.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.463201 mltu-1.0.8/mltu/utils/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/utils/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3938 2023-03-21 13:22:41.000000 mltu-1.0.8/mltu/utils/text_utils.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-04-24 10:23:36.459201 mltu-1.0.8/mltu.egg-info/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      767 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/SOURCES.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/dependency_links.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      118 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/requires.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        5 2023-04-24 10:23:36.000000 mltu-1.0.8/mltu.egg-info/top_level.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      128 2023-03-21 13:22:41.000000 mltu-1.0.8/requirements.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-04-24 10:23:36.463201 mltu-1.0.8/setup.cfg
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1654 2023-03-22 13:58:16.000000 mltu-1.0.8/setup.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.248852 mltu-1.0.9/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2022-12-01 14:15:30.000000 mltu-1.0.9/LICENSE
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       24 2023-03-21 13:22:41.000000 mltu-1.0.9/MANIFEST.in
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-05-24 08:38:06.248852 mltu-1.0.9/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2054 2023-03-21 13:22:41.000000 mltu-1.0.9/README.md
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.244852 mltu-1.0.9/mltu/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      144 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/__init__.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.244852 mltu-1.0.9/mltu/annotations/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-22 13:58:16.000000 mltu-1.0.9/mltu/annotations/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8026 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/annotations/images.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    13997 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/augmentors.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      868 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/configs.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10447 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2006 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/inferenceModel.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     7461 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/preprocessors.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.248852 mltu-1.0.9/mltu/tensorflow/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2814 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/tensorflow/callbacks.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      224 2023-03-21 13:22:41.000000 mltu-1.0.9/mltu/tensorflow/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     7266 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/tensorflow/layers.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      897 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/tensorflow/losses.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    12415 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/tensorflow/metrics.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3443 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/tensorflow/model_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.248852 mltu-1.0.9/mltu/torch/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.9/mltu/torch/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    14600 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/torch/callbacks.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3810 2023-03-21 13:22:41.000000 mltu-1.0.9/mltu/torch/dataProvider.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3691 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/torch/handlers.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1154 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/torch/losses.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     5188 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/torch/metrics.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8139 2023-03-21 13:22:41.000000 mltu-1.0.9/mltu/torch/model.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6227 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/transformers.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.248852 mltu-1.0.9/mltu/utils/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.0.9/mltu/utils/__init__.py
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3936 2023-05-24 08:34:12.000000 mltu-1.0.9/mltu/utils/text_utils.py
+drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-05-24 08:38:06.244852 mltu-1.0.9/mltu.egg-info/
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2504 2023-05-24 08:38:06.000000 mltu-1.0.9/mltu.egg-info/PKG-INFO
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      768 2023-05-24 08:38:06.000000 mltu-1.0.9/mltu.egg-info/SOURCES.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2023-05-24 08:38:06.000000 mltu-1.0.9/mltu.egg-info/dependency_links.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      148 2023-05-24 08:38:06.000000 mltu-1.0.9/mltu.egg-info/requires.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        5 2023-05-24 08:38:06.000000 mltu-1.0.9/mltu.egg-info/top_level.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      159 2023-05-24 08:34:12.000000 mltu-1.0.9/requirements.txt
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2023-05-24 08:38:06.248852 mltu-1.0.9/setup.cfg
+-rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1647 2023-05-24 08:34:12.000000 mltu-1.0.9/setup.py
```

### Comparing `mltu-1.0.8/LICENSE` & `mltu-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mltu-1.0.8/PKG-INFO` & `mltu-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mltu
-Version: 1.0.8
-Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
+Version: 1.0.9
+Summary: Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch
 Home-page: https://pylessons.com/
 Author: PyLessons
 Author-email: pythonlessons0@gmail.com
 Project-URL: Source, https://github.com/pythonlessons/mltu/
 Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mltu-1.0.8/README.md` & `mltu-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mltu-1.0.8/mltu/augmentors.py` & `mltu-1.0.9/mltu/augmentors.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 - RandomRotate
 - RandomErodeDilate
 - RandomSharpen
 - RandomGaussianBlur
 - RandomSaltAndPepper
 """
 
+
 def randomness_decorator(func):
     """ Decorator for randomness """
     def wrapper(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
         """ Decorator for randomness and type checking
 
         Args:
             image (Image): Image to be adjusted
```

### Comparing `mltu-1.0.8/mltu/configs.py` & `mltu-1.0.9/mltu/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
     def __init__(self):
         self.model_path = None
 
     def serialize(self):
         # get object attributes
         return self.__dict__
 
-    def save(self, name: str='configs.yaml'):
+    def save(self, name: str="configs.yaml"):
         if self.model_path is None:
             raise Exception("Model path is not specified")
 
         # create directory if not exist
         if not os.path.exists(self.model_path):
             os.makedirs(self.model_path)
 
-        with open(os.path.join(self.model_path, name), 'w') as f:
+        with open(os.path.join(self.model_path, name), "w") as f:
             yaml.dump(self.serialize(), f)
 
     @staticmethod
     def load(configs_path: str):
-        with open(configs_path, 'r') as f:
+        with open(configs_path, "r") as f:
             configs = yaml.load(f, Loader=yaml.FullLoader)
 
         config = BaseModelConfigs()
         for key, value in configs.items():
             setattr(config, key, value)
 
-        return config
+        return config
```

### Comparing `mltu-1.0.8/mltu/dataProvider.py` & `mltu-1.0.9/mltu/dataProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import pandas as pd
 from tqdm import tqdm
 
 from .augmentors import Augmentor
 from .transformers import Transformer
 
 import logging
-logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s: %(message)s')
+logging.basicConfig(format="%(asctime)s %(levelname)s %(name)s: %(message)s")
+
 
 class DataProvider:
     def __init__(
         self, 
         dataset: typing.Union[str, list, pd.DataFrame],
         data_preprocessors: typing.List[typing.Callable] = None,
         batch_size: int = 4,
@@ -234,15 +235,15 @@
 
         # Convert to numpy array if not already
         if not isinstance(data, np.ndarray):
             data = data.numpy()
 
         # Convert to numpy array if not already
         # TODO: This is a hack, need to fix this
-        if not isinstance(annotation, (np.ndarray, int, float, str, np.uint8, np.float)):
+        if not isinstance(annotation, (np.ndarray, int, float, str, np.uint8, float)):
             annotation = annotation.numpy()
 
         return data, annotation
 
     def __getitem__(self, index: int):
         """ Returns a batch of data by batch index"""
         dataset_batch = self.get_batch_annotations(index)
```

### Comparing `mltu-1.0.8/mltu/inferenceModel.py` & `mltu-1.0.9/mltu/inferenceModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         # check if model path is a directory with os path
         if os.path.isdir(self.model_path):
             self.model_path = os.path.join(self.model_path, self.default_model_name)
 
         if not os.path.exists(self.model_path):
             raise Exception(f"Model path ({self.model_path}) does not exist")
 
-        providers = ['CUDAExecutionProvider', 'CPUExecutionProvider'] if ort.get_device() == "GPU" and not force_cpu else ['CPUExecutionProvider']
+        providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if ort.get_device() == "GPU" and not force_cpu else ["CPUExecutionProvider"]
 
         self.model = ort.InferenceSession(self.model_path, providers=providers)
 
         self.metadata = self.model.get_modelmeta().custom_metadata_map
         if self.metadata:
             # add metadata to self object
             for key, value in self.metadata.items():
                 setattr(self, key, value) 
                 
         # Update providers priority to only CPUExecutionProvider
         if self.force_cpu:
-            self.model.set_providers(['CPUExecutionProvider'])
+            self.model.set_providers(["CPUExecutionProvider"])
 
         self.input_shape = self.model.get_inputs()[0].shape[1:]
         self.input_name = self.model._inputs_meta[0].name
         self.output_name = self.model._outputs_meta[0].name
 
     def predict(self, data: np.ndarray):
         raise NotImplementedError
```

### Comparing `mltu-1.0.8/mltu/tensorflow/callbacks.py` & `mltu-1.0.9/mltu/tensorflow/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,38 +35,42 @@
                 meta = onnx_model.metadata_props.add()
                 meta.key = key
                 meta.value = value
 
             # Save the modified ONNX model
             onnx.save(onnx_model, self.onnx_model_path)
 
+
 class TrainLogger(Callback):
     """Logs training metrics to a file.
     
     Args:
         log_path (str): Path to the directory where the log file will be saved.
         log_file (str, optional): Name of the log file. Defaults to 'logs.log'.
         logLevel (int, optional): Logging level. Defaults to logging.INFO.
     """
-    def __init__(self, log_path: str, log_file: str='logs.log', logLevel=logging.INFO) -> None:
+    def __init__(self, log_path: str, log_file: str="logs.log", logLevel=logging.INFO, console_output=False) -> None:
         super().__init__()
         self.log_path = log_path
         self.log_file = log_file
 
         if not os.path.exists(log_path):
             os.mkdir(log_path)
 
         self.logger = logging.getLogger()
         self.logger.setLevel(logLevel)
 
-        self.formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        self.formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
         self.file_handler = logging.FileHandler(os.path.join(self.log_path, self.log_file))
         self.file_handler.setLevel(logLevel)
         self.file_handler.setFormatter(self.formatter)
 
+        if not console_output:
+            self.logger.handlers[:] = []
+
         self.logger.addHandler(self.file_handler)
 
     def on_epoch_end(self, epoch: int, logs: dict=None):
         epoch_message = f"Epoch {epoch}; "
         logs_message = "; ".join([f"{key}: {value}" for key, value in logs.items()])
         self.logger.info(epoch_message + logs_message)
```

### Comparing `mltu-1.0.8/mltu/tensorflow/layers.py` & `mltu-1.0.9/mltu/tensorflow/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         Args:
             filters (int): The number of filters to use.
 
         Returns:
             tf.keras.layers.Layer: The created convolutional layer.
         """
-        conv = layers.Conv2D(filters=filters, kernel_size=1, strides=1, padding='same')
+        conv = layers.Conv2D(filters=filters, kernel_size=1, strides=1, padding="same")
         if self.wrapper:
             conv = self.wrapper(conv)
 
         return conv
 
     def call(self, inputs: tf.Tensor) -> tf.Tensor:
         """ Apply the self-attention mechanism to the input tensor.
@@ -101,34 +101,34 @@
                 "`power_iterations` should be greater than zero, got "
                 "`power_iterations={}`".format(power_iterations)
             )
         self.power_iterations = power_iterations
         self.eps = eps
         if not isinstance(layer, tf.keras.layers.Layer):
             raise ValueError(
-                'Please initialize `TimeDistributed` layer with a '
-                '`Layer` instance. You passed: {input}'.format(input=layer))
+                "Please initialize `TimeDistributed` layer with a "
+                "`Layer` instance. You passed: {input}".format(input=layer))
 
     def build(self, input_shape):
         if not self.layer.built:
             self.layer.build(input_shape)
 
         self.w = self.layer.kernel
         self.w_shape = self.w.shape.as_list()
 
         # self.v = self.add_weight(shape=(1, self.w_shape[0] * self.w_shape[1] * self.w_shape[2]),
         #                          initializer=tf.initializers.TruncatedNormal(stddev=0.02),
         #                          trainable=False,
-        #                          name='sn_v',
+        #                          name="sn_v",
         #                          dtype=tf.float32)
 
         self.u = self.add_weight(shape=(1, self.w_shape[-1]),
                                  initializer=tf.initializers.TruncatedNormal(stddev=0.02),
                                  trainable=False,
-                                 name='sn_u',
+                                 name="sn_u",
                                  dtype=tf.float32)
 
         super(SpectralNormalization, self).build()
 
     def l2normalize(self, v, eps=1e-12):
         return v / (tf.reduce_sum(v ** 2) ** 0.5 + eps)
```

### Comparing `mltu-1.0.8/mltu/tensorflow/losses.py` & `mltu-1.0.9/mltu/tensorflow/losses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import tensorflow as tf
 
+
 class CTCloss(tf.keras.losses.Loss):
     """ CTCLoss objec for training the model"""
-    def __init__(self, name: str = 'CTCloss') -> None:
+    def __init__(self, name: str = "CTCloss") -> None:
         super(CTCloss, self).__init__()
         self.name = name
         self.loss_fn = tf.keras.backend.ctc_batch_cost
 
     def __call__(self, y_true: tf.Tensor, y_pred: tf.Tensor, sample_weight=None) -> tf.Tensor:
         """ Compute the training batch CTC loss value"""
         batch_len = tf.cast(tf.shape(y_true)[0], dtype="int64")
```

### Comparing `mltu-1.0.8/mltu/tensorflow/metrics.py` & `mltu-1.0.9/mltu/tensorflow/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """A custom TensorFlow metric to compute the Character Error Rate (CER).
     
     Args:
         padding_token: An integer representing the padding token in the input data.
         name: (Optional) string name of the metric instance.
         **kwargs: Additional keyword arguments.
     """
-    def __init__(self, padding_token, name='CWER', **kwargs):
+    def __init__(self, padding_token, name="CWER", **kwargs):
         # Initialize the base Metric class
         super(CWERMetric, self).__init__(name=name, **kwargs)
         
         # Initialize variables to keep track of the cumulative character/word error rates and counter
         self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
         self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
         self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
@@ -27,15 +27,15 @@
         Args:
             y_true: A tensor of true labels with shape (batch_size, sequence_length).
             y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
             sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
         """
         # Get the input shape and length
         input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
+        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
 
         # Decode the predicted labels using greedy decoding
         decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
 
         # Convert the dense decode tensor to a sparse tensor
         predicted_labels_sparse = tf.keras.backend.ctc_label_dense_to_sparse(decode_predicted[0], input_length)
         
@@ -75,15 +75,15 @@
     """A custom TensorFlow metric to compute the Character Error Rate (CER).
     
     Args:
         vocabulary: A string of the vocabulary used to encode the labels.
         name: (Optional) string name of the metric instance.
         **kwargs: Additional keyword arguments.
     """
-    def __init__(self, vocabulary, name='CER', **kwargs):
+    def __init__(self, vocabulary, name="CER", **kwargs):
         # Initialize the base Metric class
         super(CERMetric, self).__init__(name=name, **kwargs)
         
         # Initialize variables to keep track of the cumulative character/word error rates and counter
         self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
         self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
         
@@ -130,15 +130,15 @@
         Args:
             y_true: A tensor of true labels with shape (batch_size, sequence_length).
             y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
             sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
         """
         # Get the input shape and length
         input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
+        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
 
         # Decode the predicted labels using greedy decoding
         decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
 
         # Calculate the normalized edit distance between the predicted labels and true labels tensors
         distance = self.get_cer(decode_predicted[0], y_true, self.vocabulary)
 
@@ -161,15 +161,15 @@
     """A custom TensorFlow metric to compute the Word Error Rate (WER).
     
     Attributes:
         vocabulary: A string of the vocabulary used to encode the labels.
         name: (Optional) string name of the metric instance.
         **kwargs: Additional keyword arguments.
     """
-    def __init__(self, vocabulary: str, name='WER', **kwargs):
+    def __init__(self, vocabulary: str, name="WER", **kwargs):
         # Initialize the base Metric class
         super(WERMetric, self).__init__(name=name, **kwargs)
         
         # Initialize variables to keep track of the cumulative character/word error rates and counter
         self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
         self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
         
@@ -197,18 +197,18 @@
         # Convert the valid input tensor to a ragged tensor with padding
         input_ragged = tf.RaggedTensor.from_tensor(valid_input, padding=padding)
 
         # Use the vocabulary tensor to get the strings corresponding to the indices in the ragged tensor
         input_binary_chars = tf.gather(vocab, input_ragged)
 
         # Join the binary character tensor along the sequence axis to get the input strings
-        input_strings = tf.strings.reduce_join(input_binary_chars, axis=1, separator='')
+        input_strings = tf.strings.reduce_join(input_binary_chars, axis=1, separator="")
 
         # Convert the input strings tensor to a sparse tensor
-        input_sparse_string = tf.strings.split(input_strings, sep=' ').to_sparse()
+        input_sparse_string = tf.strings.split(input_strings, sep=" ").to_sparse()
 
         return input_sparse_string
 
     @staticmethod
     def get_wer(pred_decoded, y_true, vocab, padding=-1):
         """ Calculate the normalized WER distance between the predicted labels and true labels tensors
 
@@ -228,15 +228,15 @@
         return distance
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         """
         """
         # Get the input shape and length
         input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype='int32') * tf.cast(input_shape[1], 'int32')
+        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
 
         # Decode the predicted labels using greedy decoding
         decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
 
         # Calculate the normalized edit distance between the predicted labels and true labels tensors
         distance = self.get_wer(decode_predicted[0], y_true, self.vocabulary)
```

### Comparing `mltu-1.0.8/mltu/tensorflow/model_utils.py` & `mltu-1.0.9/mltu/tensorflow/model_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,41 +36,42 @@
         # Update the metrics
         self.compiled_metrics.update_state(targets, results)
 
         # Return a dict mapping metric names to current value.
         # Note that it will include the loss (tracked in self.metrics).
         return {m.name: m.result() for m in self.metrics}
 
-def activation_layer(layer, activation: str='relu', alpha: float=0.1) -> tf.Tensor:
+
+def activation_layer(layer, activation: str="relu", alpha: float=0.1) -> tf.Tensor:
     """ Activation layer wrapper for LeakyReLU and ReLU activation functions
     Args:
         layer: tf.Tensor
         activation: str, activation function name (default: 'relu')
         alpha: float (LeakyReLU activation function parameter)
     Returns:
         tf.Tensor
     """
-    if activation == 'relu':
+    if activation == "relu":
         layer = layers.ReLU()(layer)
-    elif activation == 'leaky_relu':
+    elif activation == "leaky_relu":
         layer = layers.LeakyReLU(alpha=alpha)(layer)
 
     return layer
 
+
 def residual_block(
-    x: tf.Tensor,
-    filter_num: int,
-    strides: typing.Union[int, list]=2, 
-    kernel_size: typing.Union[int, list]=3, 
-    skip_conv: bool=True, 
-    padding: str='same', 
-    kernel_initializer: str='he_uniform', 
-    activation: str='relu', 
-    dropout: float=0.2
-    ):
+        x: tf.Tensor,
+        filter_num: int,
+        strides: typing.Union[int, list] = 2,
+        kernel_size: typing.Union[int, list] = 3,
+        skip_conv: bool = True,
+        padding: str = "same",
+        kernel_initializer: str = "he_uniform",
+        activation: str = "relu",
+        dropout: float = 0.2):
     # Create skip connection tensor
     x_skip = x
 
     # Perform 1-st convolution
     x = layers.Conv2D(filter_num, kernel_size, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x)
     x = layers.BatchNormalization()(x)
     x = activation_layer(x, activation=activation)
```

### Comparing `mltu-1.0.8/mltu/torch/callbacks.py` & `mltu-1.0.9/mltu/torch/callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,28 +246,29 @@
 
     def on_train_end(self, logs=None):
         self.writer.close()
 
 
 class Model2onnx(Callback):
     """Converts the model from PyTorch to ONNX format after training."""
+
     def __init__(
-        self, 
-        saved_model_path: str,
-        input_shape: tuple,
-        export_params: bool=True,
-        opset_version: int=14,
-        do_constant_folding: bool=True,
-        input_names: list=['input'],
-        output_names: list=['output'],
-        dynamic_axes: dict={'input' : {0 : 'batch_size'}, 
-                            'output' : {0 : 'batch_size'}},
-        verbose: bool=False,
-        metadata: dict=None,
-        ) -> None:
+            self,
+            saved_model_path: str,
+            input_shape: tuple,
+            export_params: bool = True,
+            opset_version: int = 14,
+            do_constant_folding: bool = True,
+            input_names: list = ["input"],
+            output_names: list = ["output"],
+            dynamic_axes: dict = {"input": {0: "batch_size"},
+                                  "output": {0: "batch_size"}},
+            verbose: bool = False,
+            metadata: dict = None,
+    ) -> None:
         """ Converts the model from PyTorch to ONNX format after training.
 
         Args:
             saved_model_path (str): path to the saved model
             input_shape (tuple): input shape of the model
             export_params (bool, optional): if True, all model parameters will be exported. Defaults to True.
             opset_version (int, optional): the ONNX version to export the model to. Defaults to 14.
```

### Comparing `mltu-1.0.8/mltu/torch/dataProvider.py` & `mltu-1.0.9/mltu/torch/dataProvider.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.8/mltu/torch/handlers.py` & `mltu-1.0.9/mltu/torch/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,36 +8,36 @@
     def __init__(self, metrics: typing.List[Metric]):
         self.metrics = metrics
 
         # Validate metrics
         if not all(isinstance(m, Metric) for m in self.metrics):
             raise TypeError("all items in the metrics argument must be of type Metric (Check mltu.metrics.metrics.py for more information)")
         
-        self.train_results_dict = {'loss': None}
+        self.train_results_dict = {"loss": None}
         self.train_results_dict.update({metric.name: None for metric in self.metrics})
         
-        self.val_results_dict = {'val_loss': None}
+        self.val_results_dict = {"val_loss": None}
         self.val_results_dict.update({"val_" + metric.name: None for metric in self.metrics})
 
     def update(self, target, output):
         for metric in self.metrics:
             metric.update(output, target)
 
     def reset(self):
         for metric in self.metrics:
             metric.reset()
 
     def results(self, loss, train: bool=True):
         if train:
-            self.train_results_dict['loss'] = loss
+            self.train_results_dict["loss"] = loss
             for metric in self.metrics:
                 self.train_results_dict[metric.name] = metric.result()
             return self.train_results_dict
         
-        self.val_results_dict['val_loss'] = loss
+        self.val_results_dict["val_loss"] = loss
         for metric in self.metrics:
             self.val_results_dict["val_" + metric.name] = metric.result()  
         return self.val_results_dict
     
     def description(self, epoch: int=None, train: bool=True):
         epoch_desc = f"Epoch {epoch} - " if epoch is not None else "          "
         dict = self.train_results_dict if train else self.val_results_dict
```

### Comparing `mltu-1.0.8/mltu/torch/losses.py` & `mltu-1.0.9/mltu/torch/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, blank: int):
         """ CTC loss for PyTorch
 
         Args:
             blank: Index of the blank label
         """
         super(CTCLoss, self).__init__()
-        self.ctc_loss = nn.CTCLoss(blank=blank, reduction='mean', zero_infinity=False)
+        self.ctc_loss = nn.CTCLoss(blank=blank, reduction="mean", zero_infinity=False)
         self.blank = blank
 
     def forward(self, output, target):
         """
         Args:
             output: Tensor of shape (batch_size, num_classes, sequence_length)
             target: Tensor of shape (batch_size, sequence_length)
```

### Comparing `mltu-1.0.8/mltu/torch/metrics.py` & `mltu-1.0.9/mltu/torch/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class Accuracy(Metric):
     """ Accuracy metric class
     
     Args:
         name (str, optional): name of metric. Defaults to 'accuracy'.
     """
-    def __init__(self, name='accuracy') -> None:
+    def __init__(self, name="accuracy") -> None:
         super(Accuracy, self).__init__(name=name)
         self.correct = 0
         self.total = 0
 
     def update(self, output: torch.Tensor, target: torch.Tensor):
         """ Update metric state with new data
 
@@ -69,15 +69,15 @@
         name: (Optional) string name of the metric instance.
 
     # TODO: implement everything in Torch to avoid converting to numpy
     """
     def __init__(
         self, 
         vocabulary: typing.Union[str, list],
-        name: str='CER'
+        name: str = "CER"
     ) -> None:
         super(CERMetric, self).__init__(name=name)
         self.vocabulary = vocabulary
         self.reset()
 
     def reset(self):
         """ Reset metric state to initial values"""
@@ -122,15 +122,15 @@
         name: (Optional) string name of the metric instance.
 
     # TODO: implement everything in Torch to avoid converting to numpy
     """
     def __init__(
         self, 
         vocabulary: typing.Union[str, list],
-        name: str='WER'
+        name: str = "WER"
     ) -> None:
         super(WERMetric, self).__init__(name=name)
         self.vocabulary = vocabulary
         self.reset()
 
     def reset(self):
         """ Reset metric state to initial values"""
```

### Comparing `mltu-1.0.8/mltu/torch/model.py` & `mltu-1.0.9/mltu/torch/model.py`

 * *Files identical despite different names*

### Comparing `mltu-1.0.8/mltu/transformers.py` & `mltu-1.0.9/mltu/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import cv2
 import typing
 import numpy as np
 
 from . import Image
 
 import logging
-logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s: %(message)s')
+logging.basicConfig(format="%(asctime)s %(levelname)s %(name)s: %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 class Transformer:
     def __init__(self, log_level: int = logging.INFO) -> None:
         self._log_level = log_level
@@ -121,15 +121,16 @@
         max_word_length: int, 
         padding_value: int
         ) -> None:
         self.max_word_length = max_word_length
         self.padding_value = padding_value
 
     def __call__(self, data: np.ndarray, label: np.ndarray):
-        return data, np.pad(label, (0, self.max_word_length - len(label)), 'constant', constant_values=self.padding_value)
+        return data, np.pad(label, (0, self.max_word_length - len(label)), "constant", constant_values=self.padding_value)
+
 
 class SpectrogramPadding(Transformer):
     """Pad spectrogram to max_spectrogram_length
     
     Attributes:
         max_spectrogram_length (int): Maximum length of spectrogram
         padding_value (int): Value to pad
@@ -139,26 +140,27 @@
         max_spectrogram_length: int, 
         padding_value: int
         ) -> None:
         self.max_spectrogram_length = max_spectrogram_length
         self.padding_value = padding_value
 
     def __call__(self, spectrogram: np.ndarray, label: np.ndarray):
-        padded_spectrogram = np.pad(spectrogram, ((self.max_spectrogram_length - spectrogram.shape[0], 0),(0,0)), mode='constant', constant_values=self.padding_value)
+        padded_spectrogram = np.pad(spectrogram, ((self.max_spectrogram_length - spectrogram.shape[0], 0),(0,0)), mode="constant", constant_values=self.padding_value)
 
         return padded_spectrogram, label
 
+
 class ImageShowCV2(Transformer):
     """Show image for visual inspection
     """
     def __init__(
         self, 
-        verbose: bool=True, 
+        verbose: bool = True,
         log_level: int = logging.INFO,
-        name: str = 'Image'
+        name: str = "Image"
         ) -> None:
         """
         Args:
             verbose (bool): Whether to log label
             log_level (int): Logging level (default: logging.INFO)
             name (str): Name of window to show image
         """
@@ -175,14 +177,14 @@
         
         Returns:
             data (np.ndarray): Image data
             label (np.ndarray): Label data (unchanged)
         """
         if self.verbose:
             if isinstance(label, (str, int, float)):
-                self.logger.info(f'Label: {label}')
+                self.logger.info(f"Label: {label}")
 
         cv2.imshow(self.name, image.numpy())
         cv2.waitKey(0)
         cv2.destroyAllWindows()
 
         return image, label
```

### Comparing `mltu-1.0.8/mltu/utils/text_utils.py` & `mltu-1.0.9/mltu/utils/text_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import typing
 import numpy as np
 from itertools import groupby
-    
+
+
 def ctc_decoder(predictions: np.ndarray, chars: typing.Union[str, list]) -> typing.List[str]:
-    ''' CTC greedy decoder for predictions
+    """ CTC greedy decoder for predictions
     
     Args:
         predictions (np.ndarray): predictions from model
         chars (typing.Union[str, list]): list of characters
 
     Returns:
         typing.List[str]: list of words
-    '''
+    """
     # use argmax to find the index of the highest probability
     argmax_preds = np.argmax(predictions, axis=-1)
     
     # use groupby to find continuous same indexes
     grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
 
     # convert indexes to chars
@@ -107,18 +108,19 @@
     total_words = len(target)
 
     if total_words == 0:
         return 0.0
 
     return errors / total_words
 
-if __name__ == '__main__':
-    c1 = 'ROKAS'
-    c2 = 'ROKAZ '
 
-    w1 = 'ROKAS GOOD BOY'
-    w2 = 'ROKAZ IS A GOOD BOY'
+if __name__ == "__main__":
+    c1 = "ROKAS"
+    c2 = "ROKAZ "
+
+    w1 = "ROKAS GOOD BOY"
+    w2 = "ROKAZ IS A GOOD BOY"
 
     cer = get_cer(c1, c2)
     wer = get_wer(w1, w2)
 
     print(wer)
```

### Comparing `mltu-1.0.8/mltu.egg-info/PKG-INFO` & `mltu-1.0.9/mltu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mltu
-Version: 1.0.8
-Summary: Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch
+Version: 1.0.9
+Summary: Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch
 Home-page: https://pylessons.com/
 Author: PyLessons
 Author-email: pythonlessons0@gmail.com
 Project-URL: Source, https://github.com/pythonlessons/mltu/
 Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mltu-1.0.8/mltu.egg-info/SOURCES.txt` & `mltu-1.0.9/mltu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 mltu/transformers.py
 mltu.egg-info/PKG-INFO
 mltu.egg-info/SOURCES.txt
 mltu.egg-info/dependency_links.txt
 mltu.egg-info/requires.txt
 mltu.egg-info/top_level.txt
 mltu/annotations/__init__.py
-mltu/annotations/image.py
+mltu/annotations/images.py
 mltu/tensorflow/callbacks.py
 mltu/tensorflow/dataProvider.py
 mltu/tensorflow/layers.py
 mltu/tensorflow/losses.py
 mltu/tensorflow/metrics.py
 mltu/tensorflow/model_utils.py
 mltu/torch/__init__.py
```

### Comparing `mltu-1.0.8/setup.py` & `mltu-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 from setuptools import setup
 
 DIR = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(DIR, 'README.md')) as fh:
+with open(os.path.join(DIR, "README.md")) as fh:
     long_description = fh.read()
 
-with open(os.path.join(DIR, 'requirements.txt')) as fh:
+with open(os.path.join(DIR, "requirements.txt")) as fh:
     requirements = fh.read().splitlines()
 
+
 def get_version(initpath: str) -> str:
     """ Get from the init of the source code the version string
 
     Params:
         initpath (str): path to the init file of the python package relative to the setup file
 
     Returns:
@@ -24,28 +25,29 @@
     with open(path, "r") as handle:
         for line in handle.read().splitlines():
             if line.startswith("__version__"):
                 return line.split("=")[1].strip().strip("\"'")
         else:
             raise RuntimeError("Unable to find version string.")
 
+
 setup(
-    name = 'mltu',
-    version = get_version("mltu/__init__.py"),
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    url='https://pylessons.com/',
-    author='PyLessons',
-    author_email='pythonlessons0@gmail.com',
+    name="mltu",
+    version=get_version("mltu/__init__.py"),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://pylessons.com/",
+    author="PyLessons",
+    author_email="pythonlessons0@gmail.com",
     install_requires=requirements,
     extras_require={
-        'gpu': ['onnxruntime-gpu'],
+        "gpu": ["onnxruntime-gpu"],
     },
-    python_requires='>=3',
-    packages = ['mltu', 'mltu.utils', 'mltu.torch', 'mltu.tensorflow', 'mltu.annotations'],
+    python_requires=">=3",
+    packages=["mltu", "mltu.utils", "mltu.torch", "mltu.tensorflow", "mltu.annotations"],
     include_package_data=True,
     project_urls={
-        'Source': 'https://github.com/pythonlessons/mltu/',
-        'Tracker': 'https://github.com/pythonlessons/mltu/issues',
+        "Source": "https://github.com/pythonlessons/mltu/",
+        "Tracker": "https://github.com/pythonlessons/mltu/issues",
     },
-    description="Machine Learning Training Utilities (MLTU) for TenosrFlow and PyTorch",
-)
+    description="Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch",
+)
```

