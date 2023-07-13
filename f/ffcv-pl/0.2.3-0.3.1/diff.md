# Comparing `tmp/ffcv_pl-0.2.3.tar.gz` & `tmp/ffcv_pl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffcv_pl-0.2.3.tar", last modified: Thu Jun  1 13:21:24 2023, max compression
+gzip compressed data, was "ffcv_pl-0.3.1.tar", last modified: Thu Jul 13 11:35:36 2023, max compression
```

## Comparing `ffcv_pl-0.2.3.tar` & `ffcv_pl-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.249804 ffcv_pl-0.2.3/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/PKG-INFO
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/ffcv_pl/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.2.3/ffcv_pl/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    11222 2023-06-01 13:21:01.000000 ffcv_pl-0.2.3/ffcv_pl/data_loading.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/augmentations.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      935 2023-05-17 14:39:06.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/decoders.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      446 2023-05-10 14:49:01.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/utils.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     2304 2023-05-17 12:45:28.000000 ffcv_pl-0.2.3/ffcv_pl/generate_dataset.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/ffcv_pl.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      360 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 12:19:44.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-06-01 13:21:24.249804 ffcv_pl-0.2.3/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      433 2023-06-01 13:21:19.000000 ffcv_pl-0.2.3/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/PKG-INFO
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.741825 ffcv_pl-0.3.1/ffcv_pl/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.3.1/ffcv_pl/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     4497 2023-07-13 09:22:10.000000 ffcv_pl-0.3.1/ffcv_pl/data_loading.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/augmentations.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     2597 2023-07-13 09:21:21.000000 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/utils.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     2520 2023-07-13 09:56:55.000000 ffcv_pl-0.3.1/ffcv_pl/generate_dataset.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/ffcv_pl.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      329 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-13 10:18:03.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      483 2023-07-13 11:35:07.000000 ffcv_pl-0.3.1/setup.py
```

### Comparing `ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/augmentations.py` & `ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.2.3/ffcv_pl/generate_dataset.py` & `ffcv_pl-0.3.1/ffcv_pl/generate_dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,66 @@
 from ffcv import DatasetWriter
-from ffcv.fields import Field
 from torch.utils.data import Dataset
-from ffcv_pl.ffcv_utils.utils import field_to_str
+import os
 
+from ffcv_pl.ffcv_utils.utils import field_to_str, obj_to_field
 
-def create_beton_wrapper(torch_dataset: Dataset, output_path: str, fields: tuple[Field, ...]) -> None:
+
+def create_beton_wrapper(torch_dataset: Dataset, output_path: str) -> None:
     """
-    :param torch_dataset:
-    Predefined Pytorch Dataset object.
-    Can have any number/type of parameters in the __init__ method.
+    :param torch_dataset: Pytorch Dataset object (https://pytorch.org/tutorials/beginner/basics/data_tutorial.html).
+
+    The dataset can have any number/type of parameters in the __init__ method.
+
     Constraints on the __get_item__ method:
-    According to the official ffcv docs, the dataset must return a tuple object of any length.
-    See for example: https://docs.ffcv.io/writing_datasets.html
-    The type of the elements inside the tuple is restricted to the ffcv.fields admitted
-    types: https://docs.ffcv.io/api/fields.html
-    (PIL Images - RGBImageField, strings or variable length bytes for BytesField, integers for IntField,
-    floats for FloatField, numpy arrays for NDArrayField, dicts for JSONField and torch tensors for TorchTensorField)
-
-    :param output_path: complete string for the beton output path, without extension. Example: "./train" will create a
-    "./train.beton" file at the end of process.
-
-    :param fields: iterable of ffcv.fields objects specifying types that the __get_item__ method of
-    the torch_dataset returns.
-    For example, a torch dataset that returns a tuple: (PILImage, intlabel) in the __get_item__ method should specify an
-    iterable like: (RGBImageField(), IntField) \n
-    Note that some fields require one or more parameters, like shape and dtype for NDArrays and Torch Tensors.
-    Check https://docs.ffcv.io/api/fields.html for a complete documentation.
+        According to the official ffcv docs, the dataset must return a tuple object of any length.
+        See for example: https://docs.ffcv.io/writing_datasets.html
+
+        The type of the elements inside the tuple is restricted to the ffcv.fields admitted types:
+        https://docs.ffcv.io/api/fields.html
+
+        (PIL Images - RGBImageField, integers for IntField, floats for FloatField, numpy arrays for NDArrayField,
+        dicts for JSONField, torch tensors for TorchTensorField and
+        1D uint8 numpy array of variable length for BytesField)
+
+    :param output_path: desired path for .beton output file, "/" separated. E.g. "./my_dataset.beton"
+
     """
 
     # 1. format output path
     assert len(output_path) > 0, 'param: output_path cannot be an empty string'
 
     if not output_path.endswith('.beton'):
         output_path = f'{output_path}.beton'
 
-    # 2. create dict of fields
-    assert len(fields) > 0, '*fields parameter must be an iterable with at least one element'
+    # find dir
+    dir_name = '/'.join(output_path.split('/')[:-1])
+    if not os.path.exists(dir_name):
+        print(f'[INFO] Creating output folder: {dir_name}')
+        os.makedirs(dir_name)
+
+    # 2. check that dataset __get_item__ returns a tuple and get fields.
+    tuple_obj = torch_dataset[0]
+
+    if not isinstance(tuple_obj, tuple):
+        raise AttributeError("According to the official ffcv docs, the dataset must return a tuple object. "
+                             "See for example: https://docs.ffcv.io/writing_datasets.html")
+
+    fields = []
+    for obj in tuple_obj:
+        fields.append(obj_to_field(obj))
 
+    # 2. create dict of fields
     final_mapping = {}
     for i, f in enumerate(fields):
         final_mapping[f'{field_to_str(type(f))}_{i}'] = f
 
     # official guidelines: https://docs.ffcv.io/writing_datasets.html
     print(f'[INFO] creating ffcv dataset into file: {output_path}')
+    print(f'[INFO] number of items: {len(torch_dataset)}')
+    print(f'[INFO] ffcv fields of items: {fields}')
+
     writer = DatasetWriter(output_path, final_mapping)
     writer.from_indexed_dataset(torch_dataset)
+
+    print(f'[INFO] Done.')
+    print(f'#' * 30)
```

