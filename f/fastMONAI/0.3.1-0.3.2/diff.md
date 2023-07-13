# Comparing `tmp/fastMONAI-0.3.1.tar.gz` & `tmp/fastMONAI-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastMONAI-0.3.1.tar", last modified: Mon Jul 10 11:23:35 2023, max compression
+gzip compressed data, was "fastMONAI-0.3.2.tar", last modified: Thu Jul 13 09:17:04 2023, max compression
```

## Comparing `fastMONAI-0.3.1.tar` & `fastMONAI-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      138 2022-09-05 07:20:58.000000 fastMONAI-0.3.1/CONTRIBUTING.md
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.1/LICENSE
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.1/MANIFEST.in
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.1/README.md
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/fastMONAI/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/__init__.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    29361 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/_modidx.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4795 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/dataset_info.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     8357 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/external_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.1/fastMONAI/research_utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1431 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.1/fastMONAI/vision_all.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9887 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_augmentation.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     6553 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_core.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9193 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3352 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_inference.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3674 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_loss.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3035 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_metrics.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2997 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_plot.py
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/fastMONAI.egg-info/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/SOURCES.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/dependency_links.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/entry_points.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.1/fastMONAI.egg-info/not-zip-safe
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/requires.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/top_level.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-07-10 11:19:23.000000 fastMONAI-0.3.1/settings.ini
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/setup.cfg
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.1/setup.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1101 2023-07-12 10:04:27.000000 fastMONAI-0.3.2/CONTRIBUTING.md
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.2/LICENSE
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.2/MANIFEST.in
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.2/README.md
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/fastMONAI/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-13 09:11:37.000000 fastMONAI-0.3.2/fastMONAI/__init__.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    27510 2023-07-13 09:11:37.000000 fastMONAI-0.3.2/fastMONAI/_modidx.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4948 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/dataset_info.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10970 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/external_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.2/fastMONAI/research_utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1406 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.2/fastMONAI/vision_all.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9070 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_augmentation.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     7428 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_core.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10530 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3699 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_inference.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3591 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_loss.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3549 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_metrics.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3095 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_plot.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/fastMONAI.egg-info/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/entry_points.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.2/fastMONAI.egg-info/not-zip-safe
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/requires.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/top_level.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-07-12 08:55:41.000000 fastMONAI-0.3.2/settings.ini
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/setup.cfg
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.2/setup.py
```

### Comparing `fastMONAI-0.3.1/LICENSE` & `fastMONAI-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.1/PKG-INFO` & `fastMONAI-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.1
+Version: 0.3.2
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.1/README.md` & `fastMONAI-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.1/fastMONAI/_modidx.py` & `fastMONAI-0.3.2/fastMONAI/_modidx.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,24 +25,26 @@
                                                                                         'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data._create_spine_df': ( 'external_data.html#_create_spine_df',
                                                                                        'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data._df_sort_and_add_columns': ( 'external_data.html#_df_sort_and_add_columns',
                                                                                                'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data._process_ixi_xls': ( 'external_data.html#_process_ixi_xls',
                                                                                        'fastMONAI/external_data.py'),
-                                         'fastMONAI.external_data._process_nodule_img': ( 'external_data.html#_process_nodule_img',
-                                                                                          'fastMONAI/external_data.py'),
-                                         'fastMONAI.external_data.download_NoduleMNIST3D': ( 'external_data.html#download_nodulemnist3d',
-                                                                                             'fastMONAI/external_data.py'),
+                                         'fastMONAI.external_data._process_medmnist_img': ( 'external_data.html#_process_medmnist_img',
+                                                                                            'fastMONAI/external_data.py'),
+                                         'fastMONAI.external_data.download_example_endometrial_cancer_data': ( 'external_data.html#download_example_endometrial_cancer_data',
+                                                                                                               'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data.download_example_spine_data': ( 'external_data.html#download_example_spine_data',
                                                                                                   'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data.download_ixi_data': ( 'external_data.html#download_ixi_data',
                                                                                         'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data.download_ixi_tiny': ( 'external_data.html#download_ixi_tiny',
                                                                                         'fastMONAI/external_data.py'),
+                                         'fastMONAI.external_data.download_medmnist3d_dataset': ( 'external_data.html#download_medmnist3d_dataset',
+                                                                                                  'fastMONAI/external_data.py'),
                                          'fastMONAI.external_data.download_spine_test_data': ( 'external_data.html#download_spine_test_data',
                                                                                                'fastMONAI/external_data.py')},
             'fastMONAI.research_utils': { 'fastMONAI.research_utils.pred_postprocess': ( 'research_utils.html#pred_postprocess',
                                                                                          'fastMONAI/research_utils.py')},
             'fastMONAI.utils': { 'fastMONAI.utils.load_variables': ('utils.html#load_variables', 'fastMONAI/utils.py'),
                                  'fastMONAI.utils.print_colab_gpu_info': ('utils.html#print_colab_gpu_info', 'fastMONAI/utils.py'),
                                  'fastMONAI.utils.store_variables': ('utils.html#store_variables', 'fastMONAI/utils.py')},
@@ -127,30 +129,14 @@
                                                                                                       'fastMONAI/vision_augmentation.py'),
                                                'fastMONAI.vision_augmentation.ZNormalization': ( 'vision_augment.html#znormalization',
                                                                                                  'fastMONAI/vision_augmentation.py'),
                                                'fastMONAI.vision_augmentation.ZNormalization.__init__': ( 'vision_augment.html#znormalization.__init__',
                                                                                                           'fastMONAI/vision_augmentation.py'),
                                                'fastMONAI.vision_augmentation.ZNormalization.encodes': ( 'vision_augment.html#znormalization.encodes',
                                                                                                          'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_biasfield': ( 'vision_augment.html#_do_rand_biasfield',
-                                                                                                     'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_blur': ( 'vision_augment.html#_do_rand_blur',
-                                                                                                'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_gamma': ( 'vision_augment.html#_do_rand_gamma',
-                                                                                                 'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_ghosting': ( 'vision_augment.html#_do_rand_ghosting',
-                                                                                                    'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_motion': ( 'vision_augment.html#_do_rand_motion',
-                                                                                                  'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_noise': ( 'vision_augment.html#_do_rand_noise',
-                                                                                                 'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_rand_spike': ( 'vision_augment.html#_do_rand_spike',
-                                                                                                 'fastMONAI/vision_augmentation.py'),
-                                               'fastMONAI.vision_augmentation._do_z_normalization': ( 'vision_augment.html#_do_z_normalization',
-                                                                                                      'fastMONAI/vision_augmentation.py'),
                                                'fastMONAI.vision_augmentation.do_pad_or_crop': ( 'vision_augment.html#do_pad_or_crop',
                                                                                                  'fastMONAI/vision_augmentation.py')},
             'fastMONAI.vision_core': { 'fastMONAI.vision_core.MedBase': ('vision_core.html#medbase', 'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MedBase.__repr__': ( 'vision_core.html#medbase.__repr__',
                                                                                    'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MedBase.create': ( 'vision_core.html#medbase.create',
                                                                                  'fastMONAI/vision_core.py'),
```

### Comparing `fastMONAI-0.3.1/fastMONAI/dataset_info.py` & `fastMONAI-0.3.2/fastMONAI/dataset_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,105 +10,113 @@
 from concurrent.futures import ThreadPoolExecutor
 import pandas as pd
 import numpy as np
 import torch
 import glob
 
 # %% ../nbs/08_dataset_info.ipynb 4
-class MedDataset():
-    '''A class to extract and present information about the dataset.'''
+class MedDataset:
+    """A class to extract and present information about the dataset."""
 
-    def __init__(self, path=None, # Path to the image folder
-                 postfix:str='', # Specify the file type if there are different files in the folder
-                 img_list:list=None, # Alternatively pass in a list with image paths
-                 reorder:bool=False, # Whether to reorder the data to be closest to canonical (RAS+) orientation
-                 dtype:(MedImage, MedMask)=MedImage, # Load data as datatype
-                 max_workers:int=1 #  The number of worker threads
-                ):
-        '''Constructs all the necessary attributes for the MedDataset object.'''
+    def __init__(self, path=None, postfix: str = '', img_list: list = None,
+                 reorder: bool = False, dtype: (MedImage, MedMask) = MedImage,
+                 max_workers: int = 1):
+        """Constructs MedDataset object.
 
+        Args:
+            path (str, optional): Path to the image folder.
+            postfix (str, optional): Specify the file type if there are different files in the folder.
+            img_list (List[str], optional): Alternatively, pass in a list with image paths.
+            reorder (bool, optional): Whether to reorder the data to be closest to canonical (RAS+) orientation.
+            dtype (Union[MedImage, MedMask], optional): Load data as datatype. Default is MedImage.
+            max_workers (int, optional): The number of worker threads. Default is 1.
+        """
+                     
         self.path = path
         self.postfix = postfix
         self.img_list = img_list
         self.reorder = reorder
         self.dtype = dtype
         self.max_workers = max_workers
         self.df = self._create_data_frame()
 
     def _create_data_frame(self):
-        '''Private method that returns a dataframe with information about the dataset
-
-        Returns:
-            DataFrame: A DataFrame with information about the dataset.
-        '''
+        """Private method that returns a dataframe with information about the dataset."""
 
         if self.path:
             self.img_list = glob.glob(f'{self.path}/*{self.postfix}*')
             if not self.img_list: print('Could not find images. Check the image path')
-        
+
         with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
             data_info_dict = list(executor.map(self._get_data_info, self.img_list))
-        
+
         df = pd.DataFrame(data_info_dict)
-        if df.orientation.nunique() > 1: print('The volumes in this dataset have different orientations. Recommended to pass in the argument reorder=True when creating a MedDataset object for this dataset')
+        
+        if df.orientation.nunique() > 1:
+            print('The volumes in this dataset have different orientations. '
+                  'Recommended to pass in the argument reorder=True when creating a MedDataset object for this dataset')
+
         return df
 
     def summary(self):
-        '''Summary DataFrame of the dataset with example path for similar data.'''
-
+        """Summary DataFrame of the dataset with example path for similar data."""
+        
         columns = ['dim_0', 'dim_1', 'dim_2', 'voxel_0', 'voxel_1', 'voxel_2', 'orientation']
-        return self.df.groupby(columns,as_index=False).agg(example_path=('path', 'min'), total=('path', 'size')).sort_values('total', ascending=False)
+        
+        return self.df.groupby(columns, as_index=False).agg(
+            example_path=('path', 'min'), total=('path', 'size')
+        ).sort_values('total', ascending=False)
 
     def suggestion(self):
-        '''Voxel value that appears most often in dim_0, dim_1 and dim_2, and wheter the data should be reoriented.'''
+        """Voxel value that appears most often in dim_0, dim_1 and dim_2, and whether the data should be reoriented."""
+        
         resample = [self.df.voxel_0.mode()[0], self.df.voxel_1.mode()[0], self.df.voxel_2.mode()[0]]
-
         return resample, self.reorder
 
-    def _get_data_info(self, fn:str):
-        '''Private method to collect information about an image file.
+    def _get_data_info(self, fn: str):
+        """Private method to collect information about an image file."""
+        _, o, _ = med_img_reader(fn, dtype=self.dtype, reorder=self.reorder, only_tensor=False)
 
-        Args:
-            fn: Image file path.
-
-        Returns:
-            dict: A dictionary with information about the image file
-        '''
-
-        _,o,_ = med_img_reader(fn, dtype=self.dtype, reorder=self.reorder, only_tensor=False)
-
-        info_dict = {'path': fn,  'dim_0': o.shape[1],  'dim_1': o.shape[2],  'dim_2' :o.shape[3],
+        info_dict = {'path': fn, 'dim_0': o.shape[1], 'dim_1': o.shape[2], 'dim_2': o.shape[3],
                      'voxel_0': round(o.spacing[0], 4), 'voxel_1': round(o.spacing[1], 4), 'voxel_2': round(o.spacing[2], 4),
                      'orientation': f'{"".join(o.orientation)}+'}
 
         if self.dtype is MedMask:
             mask_labels_dict = o.count_labels()
             mask_labels_dict = {f'voxel_count_{int(key)}': val for key, val in mask_labels_dict.items()}
             info_dict.update(mask_labels_dict)
 
         return info_dict
 
-    def get_largest_img_size(self,
-                             resample:list=None # A list with voxel spacing [dim_0, dim_1, dim_2]
-                            ) -> list:
-        '''Get the largest image size in the dataset.'''
-        dims = None 
+    def get_largest_img_size(self, resample: list = None) -> list:
+        """Get the largest image size in the dataset."""
         
-        if resample is not None: 
-            
+        dims = None
+
+        if resample is not None:
             org_voxels = self.df[["voxel_0", "voxel_1", 'voxel_2']].values
             org_dims = self.df[["dim_0", "dim_1", 'dim_2']].values
-            
+
             ratio = org_voxels/resample
             new_dims = (org_dims * ratio).T
             dims = [new_dims[0].max().round(), new_dims[1].max().round(), new_dims[2].max().round()]
-        
-        else: dims = [df.dim_0.max(), df.dim_1.max(), df.dim_2.max()]
-        
+
+        else:
+            dims = [df.dim_0.max(), df.dim_1.max(), df.dim_2.max()]
+
         return dims
 
 # %% ../nbs/08_dataset_info.ipynb 5
-def get_class_weights(train_labels:(np.array, list), class_weight='balanced'): 
-    '''calculate class weights.'''
+def get_class_weights(labels: (np.array, list), class_weight: str = 'balanced') -> torch.Tensor: 
+    """Calculates and returns the class weights.
+
+    Args:
+        labels: An array or list of class labels for each instance in the dataset.
+        class_weight: Defaults to 'balanced'.
+
+    Returns:
+        A tensor of class weights.
+    """
+    
+    class_weights =  compute_class_weight(class_weight=class_weight, classes=np.unique(labels), y=labels)
     
-    class_weights =  compute_class_weight(class_weight=class_weight, classes=np.unique(train_labels), y=train_labels)
     return torch.Tensor(class_weights)
```

### Comparing `fastMONAI-0.3.1/fastMONAI/external_data.py` & `fastMONAI-0.3.2/fastMONAI/external_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,299 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/09_external_data.ipynb.
 
 # %% auto 0
 __all__ = ['MURLs', 'download_ixi_data', 'download_ixi_tiny', 'download_spine_test_data', 'download_example_spine_data',
-           'download_NoduleMNIST3D']
+           'download_medmnist3d_dataset', 'download_example_endometrial_cancer_data']
 
-# %% ../nbs/09_external_data.ipynb 2
+# %% ../nbs/09_external_data.ipynb 1
 from pathlib import Path
 from glob import glob
 from numpy import load 
 import pandas as pd
 from monai.apps import download_url, download_and_extract
 from torchio.datasets.ixi import IXITiny
 from torchio import ScalarImage
 import multiprocessing as mp
 from functools import partial
 
-# %% ../nbs/09_external_data.ipynb 4
+# %% ../nbs/09_external_data.ipynb 3
 class MURLs():
-    '''A class with external medical dataset URLs.'''
+    """A class with external medical dataset URLs."""
 
     IXI_DATA = 'http://biomedic.doc.ic.ac.uk/brain-development/downloads/IXI/IXI-T1.tar'
     IXI_DEMOGRAPHIC_INFORMATION = 'http://biomedic.doc.ic.ac.uk/brain-development/downloads/IXI/IXI.xls'
     CHENGWEN_CHU_SPINE_DATA = 'https://drive.google.com/uc?id=1rbm9-KKAexpNm2mC9FsSbfnS8VJaF3Kn&confirm=t'
     EXAMPLE_SPINE_DATA = 'https://drive.google.com/uc?id=1Ms3Q6MYQrQUA_PKZbJ2t2NeYFQ5jloMh'
-    NODULE_MNIST_DATA = 'https://zenodo.org/record/6496656/files/nodulemnist3d.npz?download=1'
+    MEDMNIST_DICT = {'OrganMNIST3D': 'https://zenodo.org/record/6496656/files/organmnist3d.npz?download=1',	
+                     'NoduleMNIST3D': 'https://zenodo.org/record/6496656/files/nodulemnist3d.npz?download=1',
+                     'AdrenalMNIST3D': 'https://zenodo.org/record/6496656/files/adrenalmnist3d.npz?download=1',	
+                     'FractureMNIST3D': 'https://zenodo.org/record/6496656/files/fracturemnist3d.npz?download=1',
+                     'VesselMNIST3D': 'https://zenodo.org/record/6496656/files/vesselmnist3d.npz?download=1', 
+                     'SynapseMNIST3D': 'https://zenodo.org/record/6496656/files/synapsemnist3d.npz?download=1'}
+    EXAMPLE_EC_DATA = 'https://drive.google.com/uc?id=1cjOBhkdRsoX3unxHiL377R5j8ottN4An'
 
-# %% ../nbs/09_external_data.ipynb 5
-def _process_ixi_xls(xls_path:(str, Path), img_path: Path):
-    '''Private method to process the demographic information for the IXI dataset.
+# %% ../nbs/09_external_data.ipynb 4
+def _process_ixi_xls(xls_path: (str, Path), img_path: Path) -> pd.DataFrame:
+    """Private method to process the demographic information for the IXI dataset.
 
     Args:
         xls_path: File path to the xls file with the demographic information.
-        img_path: Folder path to the images
+        img_path: Folder path to the images.
 
     Returns:
-        DataFrame: A processed dataframe with image path and demographic information.
-    '''
+        A processed dataframe with image path and demographic information.
+
+    Raises:
+        ValueError: If xls_path or img_path do not exist.
+    """
 
     print('Preprocessing ' + str(xls_path))
 
     df = pd.read_excel(xls_path)
 
     duplicate_subject_ids = df[df.duplicated(['IXI_ID'], keep=False)].IXI_ID.unique()
 
     for subject_id in duplicate_subject_ids:
         age = df.loc[df.IXI_ID == subject_id].AGE.nunique()
-        if age != 1: df = df.loc[df.IXI_ID != subject_id] #Remove duplicates with two different age values
+        if age != 1: df = df.loc[df.IXI_ID != subject_id]  # Remove duplicates with two different age values
 
     df = df.drop_duplicates(subset='IXI_ID', keep='first').reset_index(drop=True)
 
     df['subject_id'] = ['IXI' + str(subject_id).zfill(3) for subject_id in df.IXI_ID.values]
     df = df.rename(columns={'SEX_ID (1=m, 2=f)': 'gender'})
     df['age_at_scan'] = df.AGE.round(2)
-    df = df.replace({'gender': {1:'M', 2:'F'}})
+    df = df.replace({'gender': {1: 'M', 2: 'F'}})
 
     img_list = list(img_path.glob('*.nii.gz'))
     for path in img_list:
         subject_id = path.parts[-1].split('-')[0]
         df.loc[df.subject_id == subject_id, 't1_path'] = str(path)
 
     df = df.dropna()
     df = df[['t1_path', 'subject_id', 'gender', 'age_at_scan']]
+    
     return df
 
-# %% ../nbs/09_external_data.ipynb 7
-def download_ixi_data(path:(str, Path)='../data' # Path to the directory where the data will be stored
-                     ):
-    '''Download T1 scans and demographic information from the IXI dataset, then process the demographic 
-        information for each subject and save the information as a CSV file.
-    Returns path to the stored CSV file.
-    '''
-    path = Path(path)/'IXI'
-    img_path = path/'T1_images' 
+# %% ../nbs/09_external_data.ipynb 6
+def download_ixi_data(path: (str, Path) = '../data') -> Path:
+    """Download T1 scans and demographic information from the IXI dataset.
+    
+    Args:
+        path: Path to the directory where the data will be stored. Defaults to '../data'.
+
+    Returns:
+        The path to the stored CSV file.
+    """
+
+    path = Path(path) / 'IXI'
+    img_path = path / 'T1_images'
 
     # Check whether image data already present in img_path:
-    is_extracted=False
+    is_extracted = False
     try:
-        if len(list(img_path.iterdir())) >= 581: # 581 imgs in the IXI dataset
-            is_extracted=True
+        if len(list(img_path.iterdir())) >= 581:  # 581 imgs in the IXI dataset
+            is_extracted = True
             print(f"Images already downloaded and extracted to {img_path}")
     except:
-        is_extracted=False
-
-    # Download and extract images
-    if not is_extracted: 
-        download_and_extract(url=MURLs.IXI_DATA, filepath=path/'IXI-T1.tar', output_dir=img_path)
-        (path/'IXI-T1.tar').unlink()
+        is_extracted = False
 
+    if not is_extracted:
+        download_and_extract(url=MURLs.IXI_DATA, filepath=path / 'IXI-T1.tar', output_dir=img_path)
+        (path / 'IXI-T1.tar').unlink()
 
-    # Download demographic info
-    download_url(url=MURLs.IXI_DEMOGRAPHIC_INFORMATION, filepath=path/'IXI.xls')
+    download_url(url=MURLs.IXI_DEMOGRAPHIC_INFORMATION, filepath=path / 'IXI.xls')
 
-    processed_df = _process_ixi_xls(xls_path=path/'IXI.xls', img_path=img_path)
-    processed_df.to_csv(path/'dataset.csv',index=False)
+    processed_df = _process_ixi_xls(xls_path=path / 'IXI.xls', img_path=img_path)
+    processed_df.to_csv(path / 'dataset.csv', index=False)
 
     return path
 
-# %% ../nbs/09_external_data.ipynb 9
-def download_ixi_tiny(path:(str, Path)='../data'):
-    ''' Download tiny version of IXI provided by TorchIO, containing 566 T1 brain MR scans and their corresponding brain segmentations.'''
+# %% ../nbs/09_external_data.ipynb 8
+def download_ixi_tiny(path: (str, Path) = '../data') -> Path:
+    """Download the tiny version of the IXI dataset provided by TorchIO.
+
+    Args:
+        path: The directory where the data will be 
+            stored. If not provided, defaults to '../data'.
+
+    Returns:
+        The path to the directory where the data is stored.
+    """
     
-    path = Path(path)/'IXITiny'
+    path = Path(path) / 'IXITiny'
     
-    #Download MR scans and segmentation masks
     IXITiny(root=str(path), download=True)
-    # Download demographic info
     download_url(url=MURLs.IXI_DEMOGRAPHIC_INFORMATION, filepath=path/'IXI.xls')
     
     processed_df = _process_ixi_xls(xls_path=path/'IXI.xls', img_path=path/'image')
     processed_df['labels'] = processed_df['t1_path'].str.replace('image','label')
     
     processed_df.to_csv(path/'dataset.csv', index=False)
     
     return path
 
 # %% ../nbs/09_external_data.ipynb 10
-def _create_spine_df(test_dir:Path):
-    # Get a list of the image files in the 'img' directory
-    img_list = glob(str(test_dir/'img/*.nii.gz'))
+def _create_spine_df(dir: Path) -> pd.DataFrame:
+    """Create a pandas DataFrame containing information about spinal images.
 
-    # Create a list of the corresponding mask files in the 'seg' directory
-    mask_list = [str(fn).replace('img', 'seg') for fn in img_list]
+    Args:
+        dir: Directory path where data (image and segmentation 
+            mask files) are stored.
 
-    # Create a list of the subject IDs for each image file
+    Returns:
+         A DataFrame containing the paths to the image files and their 
+            corresponding mask files, the subject IDs, and a flag indicating that 
+            these are test data.
+    """
+    
+    img_list = glob(str(dir / 'img/*.nii.gz'))
+    mask_list = [str(fn).replace('img', 'seg') for fn in img_list]
     subject_id_list = [fn.split('_')[-1].split('.')[0] for fn in mask_list]
     
-    # Create a dictionary containing the test data
-    test_data = {'t2_img_path':img_list, 't2_mask_path':mask_list, 'subject_id':subject_id_list, 'is_test':True}
+    test_data = {
+        't2_img_path': img_list,
+        't2_mask_path': mask_list,
+        'subject_id': subject_id_list,
+        'is_test': True,
+    }
 
-    # Create a DataFrame from the example data dictionary
     return pd.DataFrame(test_data)
 
-# %% ../nbs/09_external_data.ipynb 12
-def download_spine_test_data(path:(str, Path)='../data'):
+# %% ../nbs/09_external_data.ipynb 11
+def download_spine_test_data(path: (str, Path) = '../data') -> pd.DataFrame:
+    """Downloads T2w scans from the study 'Fully Automatic Localization and 
+    Segmentation of 3D Vertebral Bodies from CT/MR Images via a Learning-Based 
+    Method' by Chu et. al. 
+
+    Args:
+        path: Directory where the downloaded data 
+            will be stored and extracted. Defaults to '../data'.
+
+    Returns:
+        Processed dataframe containing image paths, label paths, and subject IDs.
+    """
     
-    ''' Download T2w scans from 'Fully Automatic Localization and Segmentation of 3D Vertebral Bodies from CT/MR Images via a Learning-Based Method' study by Chu et. al. 
-    Returns a processed dataframe with image path, label path and subject IDs. 
-    '''
     study = 'chengwen_chu_2015'
     
-    download_and_extract(url=MURLs.CHENGWEN_CHU_SPINE_DATA, filepath=f'{study}.zip', output_dir=path)
+    download_and_extract(
+        url=MURLs.CHENGWEN_CHU_SPINE_DATA, 
+        filepath=f'{study}.zip', 
+        output_dir=path
+    )
     Path(f'{study}.zip').unlink()
     
-    return _create_spine_df(Path(path)/study)
+    return _create_spine_df(Path(path) / study)
+
+# %% ../nbs/09_external_data.ipynb 12
+def download_example_spine_data(path: (str, Path) = '../data') -> Path:
+    """Downloads example T2w scan and corresponding predicted mask.
+    
+    Args:
+        path: Directory where the downloaded data 
+            will be stored and extracted. Defaults to '../data'.
 
-# %% ../nbs/09_external_data.ipynb 13
-def download_example_spine_data(path:(str, Path)='../data'): 
+    Returns:
+        Path to the directory where the example data has been extracted.
+    """
     
-    '''Download example T2w scan and predicted mask.'''
     study = 'example_data'
     
-    download_and_extract(url=MURLs.EXAMPLE_SPINE_DATA, filepath='example_data.zip', output_dir=path);
+    download_and_extract(
+        url=MURLs.EXAMPLE_SPINE_DATA, 
+        filepath='example_data.zip', 
+        output_dir=path
+    )
     Path('example_data.zip').unlink()
     
-    return Path(path/study)
+    return Path(path) / study
 
-# %% ../nbs/09_external_data.ipynb 15
-def _process_nodule_img(path, idx_arr):
-    '''Save tensor as NIfTI.'''
+# %% ../nbs/09_external_data.ipynb 14
+def _process_medmnist_img(path, idx_arr):
+    """Save tensor as NIfTI."""
+    
     idx, arr = idx_arr
     img = ScalarImage(tensor=arr[None, :])
     fn = path/f'{idx}_nodule.nii.gz'
     img.save(fn)
     return str(fn)
 
-# %% ../nbs/09_external_data.ipynb 16
+# %% ../nbs/09_external_data.ipynb 15
 def _df_sort_and_add_columns(df, label_list, is_val):
-    '''Sort the dataframe based on img_idx and add labels and if it is validation data column'''
+    """Sort the dataframe based on img_idx and add labels and if it is validation data column."""
+    
     df = df.sort_values(by='img_idx').reset_index(drop=True)
     df['labels'], df['is_val'] = label_list, is_val     
-    df = df.replace({"labels": {0:'b', 1:'m'}})
+    #df = df.replace({"labels": {0:'b', 1:'m'}})
     df = df.drop('img_idx', axis=1)
     
     return df 
 
-# %% ../nbs/09_external_data.ipynb 17
+# %% ../nbs/09_external_data.ipynb 16
 def _create_nodule_df(pool, output_dir, imgs, labels, is_val=False): 
-    '''Create dataframe for NoduleMNIST3D data.'''
-    img_path_list = pool.map(partial(_process_nodule_img, output_dir), enumerate(imgs))
+    """Create dataframe for MedMNIST data."""
+    
+    img_path_list = pool.map(partial(_process_medmnist_img, output_dir), enumerate(imgs))
     img_idx = [float(Path(fn).parts[-1].split('_')[0]) for fn in img_path_list]
     
     df = pd.DataFrame(list(zip(img_path_list, img_idx)), columns=['img_path','img_idx'])        
     return  _df_sort_and_add_columns(df, labels, is_val)
 
-# %% ../nbs/09_external_data.ipynb 18
-def download_NoduleMNIST3D(path:(str, Path)='../data', max_workers=1): 
-    
-    '''Download ....'''
-    study = 'NoduleMNIST3D'
-    path = Path(path)/study
-    
-    download_url(url=MURLs.NODULE_MNIST_DATA, filepath=path/f'{study}.npz');
-    data = load(path/f'{study}.npz')
-    key_fn = ['train_images', 'val_images', 'test_images']    
-    for fn in key_fn: (path/fn).mkdir(exist_ok=True)
-    
-    
-    train_imgs, val_imgs, test_imgs = data[key_fn[0]], data[key_fn[1]], data[key_fn[2]]
+# %% ../nbs/09_external_data.ipynb 17
+def download_medmnist3d_dataset(study: str, path: (str, Path) = '../data',
+                                max_workers: int = 1):
+    """Downloads and processes a particular MedMNIST3D dataset.
 
+    Args:
+        study: MedMNIST dataset ('OrganMNIST3D', 'NoduleMNIST3D', 
+               'AdrenalMNIST3D', 'FractureMNIST3D', 'VesselMNIST3D', 'SynapseMNIST3D')
+        path: Directory to store and extract downloaded data. Defaults to '../data'.
+        max_workers: Maximum number of worker processes for data processing. 
+                     Defaults to 1.
+
+    Returns:
+        Two pandas DataFrames. The first DataFrame combines training and validation 
+        data, and the second DataFrame contains the testing data.
+    """
+    path = Path(path) / study
+    dataset_file_path = path / f'{study}.npz'
+
+    try:
+        download_url(url=MURLs.MEDMNIST_DICT[study], filepath=dataset_file_path)
+    except:
+        raise ValueError(f"Dataset '{study}' does not exist.")
+
+    data = load(dataset_file_path)
+    keys = ['train_images', 'val_images', 'test_images']
+
+    for key in keys:
+        (path / key).mkdir(exist_ok=True)
+
+    train_imgs = data[keys[0]]
+    val_imgs = data[keys[1]]
+    test_imgs = data[keys[2]]
 
     with mp.Pool(processes=max_workers) as pool:
-        
-        train_df = _create_nodule_df(pool, path/key_fn[0], train_imgs, data['train_labels'])
-        val_df = _create_nodule_df(pool, path/key_fn[1], val_imgs, data['val_labels'], is_val=True)
-        test_df = _create_nodule_df(pool, path/key_fn[2], test_imgs, data['test_labels'])
-        
+        train_df = _create_nodule_df(pool, path / keys[0], train_imgs, 
+                                     data['train_labels'])
+        val_df = _create_nodule_df(pool, path / keys[1], val_imgs, 
+                                   data['val_labels'], is_val=True)
+        test_df = _create_nodule_df(pool, path / keys[2], test_imgs, 
+                                    data['test_labels'])
+
     train_val_df = pd.concat([train_df, val_df], ignore_index=True)
-    
+
+    dataset_file_path.unlink()
+
     return train_val_df, test_df
+
+# %% ../nbs/09_external_data.ipynb 19
+def download_example_endometrial_cancer_data(path: (str, Path) = '../data') -> Path:
+    study = 'ec'
+    
+    download_and_extract(
+        url=MURLs.EXAMPLE_EC_DATA, 
+        filepath='ec.zip', 
+        output_dir=path
+    )
+    Path('ec.zip').unlink()
+    
+    return Path(path) / study
```

### Comparing `fastMONAI-0.3.1/fastMONAI/research_utils.py` & `fastMONAI-0.3.2/fastMONAI/research_utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.1/fastMONAI/utils.py` & `fastMONAI-0.3.2/fastMONAI/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,40 +5,38 @@
 
 # %% ../nbs/07_utils.ipynb 1
 import pickle
 import torch
 from pathlib import Path
 
 # %% ../nbs/07_utils.ipynb 3
-def store_variables(pkl_fn:(str, Path),
-                    size:list,
-                    reorder:bool,
-                    resample:(int,list),
-                   ) -> None:
-    '''Save variable values in a pickle file.'''
+def store_variables(pkl_fn: (str, Path), size: list, reorder: bool, resample: (int, list)):
+    """Save variable values in a pickle file."""
     
     var_vals = [size, reorder, resample]
     
     with open(pkl_fn, 'wb') as f:
         pickle.dump(var_vals, f)
 
 # %% ../nbs/07_utils.ipynb 4
-def load_variables(pkl_fn # Filename of the pickle file
-                  ):
-    '''Load stored variable values from a pickle file.
+def load_variables(pkl_fn: (str, Path)):
+    """Loads stored variable values from a pickle file.
 
-    Returns: A list of variable values.
-    '''
+    Args:
+        pkl_fn: File path of the pickle file to be loaded.
 
+    Returns:
+        The deserialized value of the pickled data.
+    """
     with open(pkl_fn, 'rb') as f:
         return pickle.load(f)
 
 # %% ../nbs/07_utils.ipynb 5
 def print_colab_gpu_info(): 
-    '''Check if we have a GPU attached to the runtime.'''
+    """Check if we have a GPU attached to the runtime."""
     
     colab_gpu_msg =(f"{'#'*80}\n"
                     "Remember to attach a GPU to your Colab Runtime:"
                     "\n1. From the **Runtime** menu select **Change Runtime Type**"
                     "\n2. Choose **GPU** from the drop-down menu"
                     "\n3. Click **'SAVE'**\n"
                     f"{'#'*80}")
```

### Comparing `fastMONAI-0.3.1/fastMONAI/vision_augmentation.py` & `fastMONAI-0.3.2/fastMONAI/vision_augmentation.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,253 +8,274 @@
 # %% ../nbs/03_vision_augment.ipynb 2
 from fastai.data.all import *
 from .vision_core import *
 import torchio as tio
 
 # %% ../nbs/03_vision_augment.ipynb 5
 class CustomDictTransform(ItemTransform):
-    '''Wrapper to perform an identical transformation on both image and target (if it is a mask) during training.'''
+    """A class that serves as a wrapper to perform an identical transformation on both 
+    the image and the target (if it's a mask).
+    """
     
-    split_idx = 0
-    def __init__(self, aug): self.aug = aug
+    split_idx = 0  # Only perform transformations on training data. Use TTA() for transformations on validation data.
+
+    def __init__(self, aug):
+        """Constructs CustomDictTransform object.
+
+        Args:
+            aug (Callable): Function to apply augmentation on the image.
+        """
+        self.aug = aug
 
     def encodes(self, x):
-        '''Apply transformation to an image, and the same random transformation to the target if it is a mask.
+        """
+        Applies the stored transformation to an image, and the same random transformation 
+        to the target if it is a mask. If the target is not a mask, it returns the target as is.
 
         Args:
-            x: Contains image and target.
+            x (Tuple[MedImage, Union[MedMask, TensorCategory]]): A tuple containing the 
+            image and the target.
 
         Returns:
-            MedImage: Transformed image data.
-            (MedMask, TensorCategory, ...todo): If the target is a mask, then return a transformed mask data. Otherwise, return target value.
-        '''
-
+            Tuple[MedImage, Union[MedMask, TensorCategory]]: The transformed image and target. 
+            If the target is a mask, it's transformed identically to the image. If the target 
+            is not a mask, the original target is returned.
+        """
         img, y_true = x
 
         if isinstance(y_true, (MedMask)):
-            aug = self.aug(tio.Subject(img=tio.ScalarImage(tensor=img, affine=MedImage.affine_matrix), mask=tio.LabelMap(tensor=y_true, affine=MedImage.affine_matrix)))
+            aug = self.aug(tio.Subject(img=tio.ScalarImage(tensor=img, affine=MedImage.affine_matrix), 
+                                        mask=tio.LabelMap(tensor=y_true, affine=MedImage.affine_matrix)))
             return MedImage.create(aug['img'].data), MedMask.create(aug['mask'].data)
-        else:
-            aug = self.aug(tio.Subject(img=tio.ScalarImage(tensor=img)))
-            return MedImage.create(aug['img'].data), y_true
 
-# %% ../nbs/03_vision_augment.ipynb 8
-def do_pad_or_crop(o, target_shape, padding_mode, mask_name, dtype=torch.Tensor):
+        aug = self.aug(tio.Subject(img=tio.ScalarImage(tensor=img)))
+        return MedImage.create(aug['img'].data), y_true
+
 
+# %% ../nbs/03_vision_augment.ipynb 7
+def do_pad_or_crop(o, target_shape, padding_mode, mask_name, dtype=torch.Tensor):
+    #TODO:refactorize
     pad_or_crop = tio.CropOrPad(target_shape=target_shape, padding_mode=padding_mode, mask_name=mask_name)
     return dtype(pad_or_crop(o))
 
-# %% ../nbs/03_vision_augment.ipynb 9
+# %% ../nbs/03_vision_augment.ipynb 8
 class PadOrCrop(DisplayedTransform):
-    '''Resize image using TorchIO `CropOrPad`.'''
+    """Resize image using TorchIO `CropOrPad`."""
+    
+    order = 0
 
-    order=0
     def __init__(self, size, padding_mode=0, mask_name=None):
-        if not is_listy(size): size=[size,size,size]
-        self.size, self.padding_mode, self.mask_name = size, padding_mode, mask_name
+        if not is_listy(size): 
+            size = [size, size, size]
+        self.pad_or_crop = tio.CropOrPad(target_shape=size,
+                                    padding_mode=padding_mode, 
+                                    mask_name=mask_name)
 
-    def encodes(self, o:(MedImage, MedMask)):
-        return do_pad_or_crop(o,target_shape=self.size, padding_mode=self.padding_mode, mask_name=self.mask_name, dtype=type(o))
+    def encodes(self, o: (MedImage, MedMask)):
+        return type(o)(self.pad_or_crop(o))
 
-# %% ../nbs/03_vision_augment.ipynb 11
-def _do_z_normalization(o, masking_method, channel_wise):
-
-    z_normalization = tio.ZNormalization(masking_method=masking_method)
-    normalized_tensor = torch.zeros(o.shape)
+# %% ../nbs/03_vision_augment.ipynb 9
+class ZNormalization(DisplayedTransform):
+    """Apply TorchIO `ZNormalization`."""
 
-    if channel_wise:
-        for idx, c in enumerate(o): 
-            normalized_tensor[idx] = z_normalization(c[None])[0]
-            
-    else: normalized_tensor = z_normalization(o)
+    order = 0
 
-    return normalized_tensor
+    def __init__(self, masking_method=None, channel_wise=True):
+        self.z_normalization = tio.ZNormalization(masking_method=masking_method)
+        self.channel_wise = channel_wise
 
-# %% ../nbs/03_vision_augment.ipynb 12
-class ZNormalization(DisplayedTransform):
-    '''Apply TorchIO `ZNormalization`.'''
+    def encodes(self, o: MedImage):
+        if self.channel_wise:
+            o = torch.stack([self.z_normalization(c[None])[0] for c in o])
+        else: o = self.z_normalization(o) 
 
-    order=0
-    def __init__(self, masking_method=None, channel_wise=True):
-        self.masking_method, self.channel_wise = masking_method, channel_wise
+        return MedImage.create(o)
 
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_z_normalization(o, self.masking_method, self.channel_wise))
-    def encodes(self, o:(MedMask)):return o
+    def encodes(self, o: MedMask):
+        return o
 
-# %% ../nbs/03_vision_augment.ipynb 14
+# %% ../nbs/03_vision_augment.ipynb 10
 class BraTSMaskConverter(DisplayedTransform):
     '''Convert BraTS masks.'''
 
     order=1
 
     def encodes(self, o:(MedImage)): return o
 
     def encodes(self, o:(MedMask)):
         o = torch.where(o==4, 3., o)
         return MedMask.create(o)
 
-# %% ../nbs/03_vision_augment.ipynb 16
+# %% ../nbs/03_vision_augment.ipynb 11
 class BinaryConverter(DisplayedTransform):
     '''Convert to binary mask.'''
 
     order=1
 
-    def encodes(self, o:(MedImage)): return o
+    def encodes(self, o: MedImage): 
+        return o
 
-    def encodes(self, o:(MedMask)):
+    def encodes(self, o: MedMask):
         o = torch.where(o>0, 1., 0)
         return MedMask.create(o)
 
-# %% ../nbs/03_vision_augment.ipynb 18
-def _do_rand_ghosting(o, intensity, p):
-    
-    add_ghosts = tio.RandomGhosting(intensity=intensity, p=p)
-    return add_ghosts(o)
-
-# %% ../nbs/03_vision_augment.ipynb 19
+# %% ../nbs/03_vision_augment.ipynb 12
 class RandomGhosting(DisplayedTransform):
-    '''Apply TorchIO `RandomGhosting`.'''
-
-    split_idx,order=0,1
+    """Apply TorchIO `RandomGhosting`."""
+    
+    split_idx, order = 0, 1
 
-    def __init__(self, intensity =(0.5, 1), p=0.5):
-        self.intensity, self.p  = intensity, p
+    def __init__(self, intensity=(0.5, 1), p=0.5):
+        self.add_ghosts = tio.RandomGhosting(intensity=intensity, p=p)
 
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_ghosting(o, self.intensity, self.p))
-    def encodes(self, o:(MedMask)):return o
+    def encodes(self, o: MedImage):
+        return MedImage.create(self.add_ghosts(o))
 
-# %% ../nbs/03_vision_augment.ipynb 21
-def _do_rand_spike(o, num_spikes, intensity, p):
+    def encodes(self, o: MedMask):
+        return o
 
-    add_spikes = tio.RandomSpike(num_spikes=num_spikes, intensity=intensity, p=p)
-    return add_spikes(o) #return torch tensor
-
-# %% ../nbs/03_vision_augment.ipynb 22
+# %% ../nbs/03_vision_augment.ipynb 13
 class RandomSpike(DisplayedTransform):
     '''Apply TorchIO `RandomSpike`.'''
     
     split_idx,order=0,1
 
     def __init__(self, num_spikes=1, intensity=(1, 3), p=0.5):
-        self.num_spikes, self.intensity, self.p  = num_spikes, intensity, p
-
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_spike(o, self.num_spikes, self.intensity, self.p))
-    def encodes(self, o:(MedMask)):return o
+        self.add_spikes = tio.RandomSpike(num_spikes=num_spikes, intensity=intensity, p=p)
 
-# %% ../nbs/03_vision_augment.ipynb 24
-def _do_rand_noise(o, mean, std, p):
+    def encodes(self, o:MedImage): 
+        return MedImage.create(self.add_spikes(o))
+        
+    def encodes(self, o:MedMask):
+        return o
 
-    add_noise = tio.RandomNoise(mean=mean, std=std, p=p)
-    return add_noise(o) #return torch tensor
-
-# %% ../nbs/03_vision_augment.ipynb 25
+# %% ../nbs/03_vision_augment.ipynb 14
 class RandomNoise(DisplayedTransform):
     '''Apply TorchIO `RandomNoise`.'''
 
     split_idx,order=0,1
 
     def __init__(self, mean=0, std=(0, 0.25), p=0.5):
-        self.mean, self.std, self.p  = mean, std, p
-
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_noise(o, mean=self.mean, std=self.std, p=self.p))
-    def encodes(self, o:(MedMask)):return o
-
-# %% ../nbs/03_vision_augment.ipynb 27
-def _do_rand_biasfield(o, coefficients, order, p):
+        self.add_noise = tio.RandomNoise(mean=mean, std=std, p=p)
 
-    add_biasfield = tio.RandomBiasField(coefficients=coefficients, order=order, p=p)
-    return add_biasfield(o) #return torch tensor
+    def encodes(self, o: MedImage): 
+        return MedImage.create(self.add_noise(o))
+    
+    def encodes(self, o: MedMask):
+        return o
 
-# %% ../nbs/03_vision_augment.ipynb 28
+# %% ../nbs/03_vision_augment.ipynb 15
 class RandomBiasField(DisplayedTransform):
     '''Apply TorchIO `RandomBiasField`.'''
 
     split_idx,order=0,1
 
     def __init__(self, coefficients=0.5, order=3, p=0.5):
-        self.coefficients, self.order, self.p  = coefficients, order, p
-
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_biasfield(o, coefficients=self.coefficients, order=self.order, p=self.p))
-    def encodes(self, o:(MedMask)):return o
-
-# %% ../nbs/03_vision_augment.ipynb 30
-def _do_rand_blur(o, std, p):
+        self.add_biasfield = tio.RandomBiasField(coefficients=coefficients, order=order, p=p)
 
-    add_blur = tio.RandomBlur(std=std, p=p)
-    return add_blur(o) 
+    def encodes(self, o: MedImage): 
+        return MedImage.create(self.add_biasfield(o))
+        
+    def encodes(self, o: MedMask):
+        return o
 
-# %% ../nbs/03_vision_augment.ipynb 31
+# %% ../nbs/03_vision_augment.ipynb 16
 class RandomBlur(DisplayedTransform):
     '''Apply TorchIO `RandomBiasField`.'''
 
     split_idx,order=0,1
 
     def __init__(self, std=(0, 2), p=0.5):
-        self.std, self.p  = std, p
-
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_blur(o, std=self.std, p=self.p))
-    def encodes(self, o:(MedMask)):return o
-
-# %% ../nbs/03_vision_augment.ipynb 33
-def _do_rand_gamma(o, log_gamma, p):
-
-    add_gamma = tio.RandomGamma(log_gamma=log_gamma, p=p)
-    return add_gamma(o) 
+        self.add_blur = tio.RandomBlur(std=std, p=p)
+        
+    def encodes(self, o: MedImage): 
+        return MedImage.create(self.add_blur(o))
+    
+    def encodes(self, o: MedMask):
+        return o
 
-# %% ../nbs/03_vision_augment.ipynb 34
+# %% ../nbs/03_vision_augment.ipynb 17
 class RandomGamma(DisplayedTransform):
     '''Apply TorchIO `RandomGamma`.'''
 
 
     split_idx,order=0,1
 
     def __init__(self, log_gamma=(-0.3, 0.3), p=0.5):
-        self.log_gamma, self.p  = log_gamma, p
-
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_gamma(o, log_gamma=self.log_gamma, p=self.p))
-    def encodes(self, o:(MedMask)):return o
-
-# %% ../nbs/03_vision_augment.ipynb 36
-def _do_rand_motion(o, degrees, translation, num_transforms, image_interpolation, p):
+        self.add_gamma = tio.RandomGamma(log_gamma=log_gamma, p=p)
 
-    add_motion = tio.RandomMotion(degrees=degrees, translation=translation, num_transforms=num_transforms, image_interpolation=image_interpolation, p=p)
-    return add_motion(o) #return torch tensor
+    def encodes(self, o: MedImage): 
+        return MedImage.create(self.add_gamma(o))
+    
+    def encodes(self, o: MedMask):
+        return o
 
-# %% ../nbs/03_vision_augment.ipynb 37
+# %% ../nbs/03_vision_augment.ipynb 18
 class RandomMotion(DisplayedTransform):
-    '''Apply TorchIO `RandomMotion`.'''
+    """Apply TorchIO `RandomMotion`."""
 
-    split_idx,order=0,1
+    split_idx, order = 0, 1
 
-    def __init__(self, degrees=10, translation=10, num_transforms=2, image_interpolation='linear', p=0.5):
-        self.degrees,self.translation, self.num_transforms, self.image_interpolation, self.p = degrees,translation, num_transforms, image_interpolation, p
+    def __init__(
+            self, 
+            degrees=10, 
+            translation=10, 
+            num_transforms=2, 
+            image_interpolation='linear', 
+            p=0.5
+        ):
+        self.add_motion = tio.RandomMotion(
+            degrees=degrees, 
+            translation=translation, 
+            num_transforms=num_transforms, 
+            image_interpolation=image_interpolation, 
+            p=p
+        )
 
-    def encodes(self, o:(MedImage)): return MedImage.create(_do_rand_motion(o, degrees=self.degrees,translation=self.translation, num_transforms=self.num_transforms, image_interpolation=self.image_interpolation, p=self.p))
-    def encodes(self, o:(MedMask)):return o
+    def encodes(self, o: MedImage):
+        return MedImage.create(self.add_motion(o))
 
-# %% ../nbs/03_vision_augment.ipynb 40
+    def encodes(self, o: MedMask):
+        return o
+
+# %% ../nbs/03_vision_augment.ipynb 20
 class RandomElasticDeformation(CustomDictTransform):
-    '''Apply TorchIO `RandomElasticDeformation`.'''
+    """Apply TorchIO `RandomElasticDeformation`."""
 
-    def __init__(self,num_control_points=7, max_displacement=7.5, image_interpolation='linear', p=0.5): 
-        super().__init__(tio.RandomElasticDeformation(num_control_points=num_control_points, max_displacement=max_displacement, image_interpolation=image_interpolation, p=p))
+    def __init__(self, num_control_points=7, max_displacement=7.5,
+                 image_interpolation='linear', p=0.5):
+                     
+        super().__init__(tio.RandomElasticDeformation(
+            num_control_points=num_control_points,
+            max_displacement=max_displacement,
+            image_interpolation=image_interpolation,
+            p=p))
 
-# %% ../nbs/03_vision_augment.ipynb 42
+# %% ../nbs/03_vision_augment.ipynb 21
 class RandomAffine(CustomDictTransform):
-    '''Apply TorchIO `RandomAffine`.'''
+    """Apply TorchIO `RandomAffine`."""
 
-    def __init__(self, scales=0, degrees=10, translation=0, isotropic=False, image_interpolation='linear', default_pad_value=0., p=0.5): 
-        super().__init__(tio.RandomAffine(scales=scales, degrees=degrees, translation=translation, isotropic=isotropic, image_interpolation=image_interpolation, default_pad_value=default_pad_value, p=p))
+    def __init__(self, scales=0, degrees=10, translation=0, isotropic=False,
+                 image_interpolation='linear', default_pad_value=0., p=0.5):
+                     
+        super().__init__(tio.RandomAffine(
+            scales=scales,
+            degrees=degrees,
+            translation=translation,
+            isotropic=isotropic,
+            image_interpolation=image_interpolation,
+            default_pad_value=default_pad_value,
+            p=p))
 
-# %% ../nbs/03_vision_augment.ipynb 44
+# %% ../nbs/03_vision_augment.ipynb 22
 class RandomFlip(CustomDictTransform):
-    '''Apply TorchIO `RandomFlip`.'''
+    """Apply TorchIO `RandomFlip`."""
 
     def __init__(self, axes='LR', p=0.5):
         super().__init__(tio.RandomFlip(axes=axes, flip_probability=p))
 
-# %% ../nbs/03_vision_augment.ipynb 46
+# %% ../nbs/03_vision_augment.ipynb 23
 class OneOf(CustomDictTransform):
-    '''Apply only one of the given transforms using TorchIO `OneOf`.'''
+    """Apply only one of the given transforms using TorchIO `OneOf`."""
 
     def __init__(self, transform_dict, p=1):
         super().__init__(tio.OneOf(transform_dict, p=p))
```

### Comparing `fastMONAI-0.3.1/fastMONAI/vision_core.py` & `fastMONAI-0.3.2/fastMONAI/vision_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # %% ../nbs/01_vision_core.ipynb 2
 from .vision_plot import *
 from fastai.data.all import *
 from torchio import ScalarImage, LabelMap, ToCanonical, Resample
 
 # %% ../nbs/01_vision_core.ipynb 5
 def _preprocess(obj, reorder, resample):
-    """Preprocesses the given object.
+    """
+    Preprocesses the given object.
 
     Args:
         obj: The object to preprocess.
         reorder: Whether to reorder the object.
         resample: Whether to resample the object.
 
     Returns:
@@ -79,20 +80,16 @@
        return dtype(tensor) 
 
     input_img.set_data(tensor)
     return org_img, input_img, org_size
 
 
 # %% ../nbs/01_vision_core.ipynb 8
-def med_img_reader(
-        file_path: (str, Path),
-        dtype=torch.Tensor,
-        reorder: bool = False,
-        resample: list = None,
-        only_tensor: bool = True
+def med_img_reader(file_path: (str, Path), dtype=torch.Tensor, reorder: bool = False,
+                   resample: list = None, only_tensor: bool = True
 ):
     """Loads and preprocesses a medical image.
 
     Args:
         file_path: Path to the image. Can be a string or a Path object.
         dtype: Datatype for the return value. Defaults to torch.Tensor.
         reorder: Whether to reorder the data to be closest to canonical 
@@ -116,76 +113,95 @@
     if only_tensor:
         return dtype(input_img.data.type(torch.float))
 
     return org_img, input_img, org_size
 
 # %% ../nbs/01_vision_core.ipynb 10
 class MetaResolver(type(torch.Tensor), metaclass=BypassNewMeta):
-    '''A class to bypass metaclass conflict:
+    """
+    A class to bypass metaclass conflict:
     https://pytorch-geometric.readthedocs.io/en/latest/_modules/torch_geometric/data/batch.html
-    '''
+    """
     pass
 
 # %% ../nbs/01_vision_core.ipynb 11
-class MedBase(torch.Tensor, metaclass=MetaResolver): 
-    '''A class that represents an image object. Metaclass casts x to this class if it is of type cls._bypass_type.'''
-
-    _bypass_type=torch.Tensor
+class MedBase(torch.Tensor, metaclass=MetaResolver):
+    """A class that represents an image object.
+    Metaclass casts `x` to this class if it is of type `cls._bypass_type`."""
+    
+    _bypass_type = torch.Tensor
     _show_args = {'cmap':'gray'}
     resample, reorder = None, False
     affine_matrix = None
 
-
     @classmethod
-    def create(cls, fn: (Path, str, torch.Tensor), **kwargs):
+    def create(cls, fn: (Path, str, torch.Tensor), **kwargs) -> torch.Tensor:
         """
-        Open a medical image and cast to MedBase object. If it is a torch.Tensor, cast to MedBase object.
+        Opens a medical image and casts it to MedBase object.
+        If `fn` is a torch.Tensor, it's cast to MedBase object.
 
         Args:
-            fn: Image path or a 4D torch.Tensor.
-            kwargs: Additional parameters.
+            fn : (Path, str, torch.Tensor)
+                Image path or a 4D torch.Tensor.
+            kwargs : dict
+                Additional parameters for the medical image reader.
 
         Returns:
-            A 4D tensor as MedBase object.
+            torch.Tensor : A 4D tensor as a MedBase object.
         """
         if isinstance(fn, torch.Tensor):
             return cls(fn)
 
         return med_img_reader(fn, dtype=cls, resample=cls.resample, reorder=cls.reorder)
 
     @classmethod
     def item_preprocessing(cls, resample: (list, int, tuple), reorder: bool):
         """
-        Change the values for the class variables `resample` and `reorder`.
+        Changes the values for the class variables `resample` and `reorder`.
 
         Args:
-            resample: A list with voxel spacing.
-            reorder: Whether to reorder the data to be closest to canonical (RAS+) orientation.
+            resample : (list, int, tuple)
+                A list with voxel spacing.
+            reorder : bool
+                Whether to reorder the data to be closest to canonical (RAS+) orientation.
         """
         cls.resample = resample
         cls.reorder = reorder
 
-    def show(self, ctx=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
+    def show(self, ctx=None, channel: int = 0, indices: int = None, anatomical_plane: int = 0, **kwargs):
         """
-        Show Medimage using `merge(self._show_args, kwargs)`.
+        Displays the Medimage using `merge(self._show_args, kwargs)`.
+
+        Args:
+            ctx : Any, optional
+                Context to use for the display. Defaults to None.
+            channel : int, optional
+                The channel of the image to be displayed. Defaults to 0.
+            indices : list or None, optional
+                Indices of the images to be displayed. Defaults to None.
+            anatomical_plane : int, optional
+                Anatomical plane of the image to be displayed. Defaults to 0.
+            kwargs : dict, optional
+                Additional parameters for the show function.
 
         Returns:
             Shown image.
         """
         return show_med_img(
             self, ctx=ctx, channel=channel, indices=indices, 
             anatomical_plane=anatomical_plane, voxel_size=self.resample,  
             **merge(self._show_args, kwargs)
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
+        """Returns the string representation of the MedBase instance."""
         return f'{self.__class__.__name__} mode={self.mode} size={"x".join([str(d) for d in self.size])}'
 
 # %% ../nbs/01_vision_core.ipynb 12
 class MedImage(MedBase):
-    '''Subclass of MedBase that represents an image object.'''
+    """Subclass of MedBase that represents an image object."""
     pass
 
 # %% ../nbs/01_vision_core.ipynb 13
 class MedMask(MedBase):
-    '''Subclass of MedBase that represents an mask object.'''
+    """Subclass of MedBase that represents an mask object."""
     _show_args = {'alpha':0.5, 'cmap':'tab20'}
```

### Comparing `fastMONAI-0.3.1/fastMONAI/vision_data.py` & `fastMONAI-0.3.2/fastMONAI/vision_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,172 +6,262 @@
 
 # %% ../nbs/02_vision_data.ipynb 2
 from fastai.data.all import *
 from fastai.vision.data import *
 from .vision_core import *
 
 # %% ../nbs/02_vision_data.ipynb 5
-def pred_to_multiclass_mask(pred:torch.Tensor # [C,W,H,D] activation tensor
-                           ) -> torch.Tensor:
-    '''Apply Softmax function on the predicted tensor to rescale the values in the range [0, 1] and sum to 1.
-    Then apply argmax to get the indices of the maximum value of all elements in the predicted Tensor.
-    Returns: Predicted mask.
-    '''
+def pred_to_multiclass_mask(pred: torch.Tensor) -> torch.Tensor:
+    """Apply Softmax on the predicted tensor to rescale the values in the range [0, 1]
+    and sum to 1. Then apply argmax to get the indices of the maximum value of all 
+    elements in the predicted Tensor.
+
+    Args:
+        pred: [C,W,H,D] activation tensor.
+
+    Returns: 
+        Predicted mask.
+    """
+    
     pred = pred.softmax(dim=0)
+
     return pred.argmax(dim=0, keepdims=True)
 
 # %% ../nbs/02_vision_data.ipynb 6
-def batch_pred_to_multiclass_mask(pred:torch.Tensor # [B, C, W, H, D] batch of activations
-                                 ) -> (torch.Tensor, int):
-    '''Convert a batch of predicted activation tensors to masks.
-    Returns batch of predicted masks and number of classes.
-    '''
-
+def batch_pred_to_multiclass_mask(pred: torch.Tensor) -> (torch.Tensor, int):
+    """Convert a batch of predicted activation tensors to masks.
+    
+    Args:
+        pred: [B, C, W, H, D] batch of activations.
+
+    Returns:
+        Tuple of batch of predicted masks and number of classes.
+    """
+    
     n_classes = pred.shape[1]
     pred = [pred_to_multiclass_mask(p) for p in pred]
 
     return torch.stack(pred), n_classes
 
 # %% ../nbs/02_vision_data.ipynb 7
-def pred_to_binary_mask(pred # [B, C, W, H, D] or [C, W, H, D] activation tensor
-                       ) -> torch.Tensor:
-    '''Apply Sigmoid function that squishes activations into a range between 0 and 1.
-    Then we classify all values greater than or equal to 0.5 to 1, and the values below 0.5 to 0.
-
-    Returns predicted binary mask(s).
-    '''
-
+def pred_to_binary_mask(pred: torch.Tensor) -> torch.Tensor:
+    """Apply Sigmoid function that squishes activations into a range between 0 and 1.
+    Then we classify all values greater than or equal to 0.5 to 1, 
+    and the values below 0.5 to 0.
+
+    Args:
+        pred: [B, C, W, H, D] or [C, W, H, D] activation tensor
+
+    Returns:
+        Predicted binary mask(s).
+    """
+    
     pred = torch.sigmoid(pred)
-    return torch.where(pred>=0.5, 1, 0)
+
+    return torch.where(pred >= 0.5, 1, 0)
 
 # %% ../nbs/02_vision_data.ipynb 9
 class MedDataBlock(DataBlock):
-    '''Container to quickly build dataloaders.'''
+    """Container to quickly build dataloaders."""
+    #TODO add get_x
+    def __init__(self, blocks: list = None, dl_type: TfmdDL = None, getters: list = None,
+                 n_inp: int = None, item_tfms: list = None, batch_tfms: list = None,
+                 reorder: bool = False, resample: (int, list) = None, **kwargs):
 
-    def __init__(self, blocks:list=None,dl_type:TfmdDL=None, getters:list=None, n_inp:int=None, item_tfms:list=None,
-                 batch_tfms:list=None, reorder:bool=False, resample:(int, list)=None, **kwargs):
+        super().__init__(blocks, dl_type, getters, n_inp, item_tfms,
+                         batch_tfms, **kwargs)
 
-        super().__init__(blocks, dl_type, getters, n_inp, item_tfms, batch_tfms, **kwargs)
-        MedBase.item_preprocessing(resample,reorder)
+        MedBase.item_preprocessing(resample, reorder)
 
-# %% ../nbs/02_vision_data.ipynb 12
+# %% ../nbs/02_vision_data.ipynb 11
 def MedMaskBlock():
+    """Create a TransformBlock for medical masks."""
     return TransformBlock(type_tfms=MedMask.create)
 
-# %% ../nbs/02_vision_data.ipynb 14
+# %% ../nbs/02_vision_data.ipynb 13
 class MedImageDataLoaders(DataLoaders):
-    '''Higher-level `MedDataBlock` API.'''
-
+    """Higher-level `MedDataBlock` API."""
+    
     @classmethod
     @delegates(DataLoaders.from_dblock)
-    def from_df(cls, df, valid_pct=0.2, seed=None, fn_col=0, folder=None, suff='', label_col=1, label_delim=None,
-                y_block=None, valid_col=None, item_tfms=None, batch_tfms=None, reorder=False, resample=None, **kwargs):
-        '''Create from DataFrame.'''
-
+    def from_df(cls, df, valid_pct=0.2, seed=None, fn_col=0, folder=None, suff='',
+                label_col=1, label_delim=None, y_block=None, valid_col=None,
+                item_tfms=None, batch_tfms=None, reorder=False, resample=None, **kwargs):
+        """Create from DataFrame."""
+                    
         if y_block is None:
             is_multi = (is_listy(label_col) and len(label_col) > 1) or label_delim is not None
             y_block = MultiCategoryBlock if is_multi else CategoryBlock
-        splitter = RandomSplitter(valid_pct, seed=seed) if valid_col is None else ColSplitter(valid_col)
 
+        splitter = (RandomSplitter(valid_pct, seed=seed) 
+                    if valid_col is None else ColSplitter(valid_col))
 
-        dblock = MedDataBlock(blocks=(ImageBlock(cls=MedImage), y_block), get_x=ColReader(fn_col, suff=suff),
-                              get_y=ColReader(label_col, label_delim=label_delim),
-                              splitter=splitter,
-                              item_tfms=item_tfms,
-                              reorder=reorder,
-                              resample=resample)
+        dblock = MedDataBlock(
+            blocks=(ImageBlock(cls=MedImage), y_block),
+            get_x=ColReader(fn_col, suff=suff),
+            get_y=ColReader(label_col, label_delim=label_delim),
+            splitter=splitter,
+            item_tfms=item_tfms,
+            reorder=reorder,
+            resample=resample
+        )
 
         return cls.from_dblock(dblock, df, **kwargs)
 
-# %% ../nbs/02_vision_data.ipynb 19
+# %% ../nbs/02_vision_data.ipynb 16
 @typedispatch
-def show_batch(x:MedImage, y, samples, ctxs=None, max_n=6, nrows=None, ncols=None, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    '''Showing a batch of samples for classification and regression tasks.'''
-
-    if ctxs is None: ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
+def show_batch(x: MedImage, y, samples, ctxs=None, max_n=6, nrows=None, 
+               ncols=None, figsize=None, channel: int = 0, indices=None, 
+               anatomical_plane: int = 0, **kwargs):
+    """Showing a batch of samples for classification and regression tasks."""
+    
+    if ctxs is None: 
+        ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
+    
     n = 1 if y is None else 2
+    
     for i in range(n):
-        ctxs = [b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) for b,c,_ in zip(samples.itemgot(i),ctxs,range(max_n))]
+        ctxs = [
+            b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) 
+            for b, c, _ in zip(samples.itemgot(i), ctxs, range(max_n))
+        ]
 
     plt.tight_layout()
+    
     return ctxs
 
-# %% ../nbs/02_vision_data.ipynb 20
+# %% ../nbs/02_vision_data.ipynb 17
 @typedispatch
-def show_batch(x:MedImage, y:MedMask, samples, ctxs=None, max_n=6, nrows=None, ncols=None, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    '''Showing a batch of decoded segmentation samples.'''
+def show_batch(x: MedImage, y: MedMask, samples, ctxs=None, max_n=6, nrows: int = None,
+               ncols: int = None, figsize=None, channel: int = 0, indices: int = None,
+               anatomical_plane: int = 0, **kwargs):
+    """Showing a batch of decoded segmentation samples."""
 
     nrows, ncols = min(len(samples), max_n), x.shape[1] + 1
     imgs = []
 
-    fig,axs = subplots(nrows, ncols, figsize=figsize, **kwargs)
+    fig, axs = subplots(nrows, ncols, figsize=figsize, **kwargs)
     axs = axs.flatten()
 
-    for img, mask in list(zip(x,y)):
+    for img, mask in zip(x, y):
         im_channels = [MedImage(c_img[None]) for c_img in img]
         im_channels.append(MedMask(mask))
         imgs.extend(im_channels)
 
-    ctxs = [im.show(ax=ax, indices=indices, anatomical_plane=anatomical_plane) for im, ax in zip(imgs, axs)]
+    ctxs = [im.show(ax=ax, indices=indices, anatomical_plane=anatomical_plane)
+            for im, ax in zip(imgs, axs)]
+
     plt.tight_layout()
 
     return ctxs
 
-# %% ../nbs/02_vision_data.ipynb 22
+# %% ../nbs/02_vision_data.ipynb 19
 @typedispatch
-def show_results(x:MedImage, y:torch.Tensor, samples, outs, ctxs=None, max_n=6, nrows=None, ncols=None, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    '''Showing samples and their corresponding predictions for regression tasks.'''
-
-    if ctxs is None: ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
+def show_results(x: MedImage, y: torch.Tensor, samples, outs, ctxs=None, max_n: int = 6,
+                 nrows: int = None, ncols: int = None, figsize=None, channel: int = 0,
+                 indices: int = None, anatomical_plane: int = 0, **kwargs):
+    """Showing samples and their corresponding predictions for regression tasks."""
+
+    if ctxs is None:
+        ctxs = get_grid(min(len(samples), max_n), nrows=nrows,
+                        ncols=ncols, figsize=figsize)
 
     for i in range(len(samples[0])):
-        ctxs = [b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) for b,c,_ in zip(samples.itemgot(i),ctxs,range(max_n))]
+        ctxs = [
+            b.show(ctx=c, channel=channel, indices=indices,
+                   anatomical_plane=anatomical_plane, **kwargs)
+            for b, c, _ in zip(samples.itemgot(i), ctxs, range(max_n))
+        ]
+
     for i in range(len(outs[0])):
-        ctxs = [b.show(ctx=c, **kwargs) for b,c,_ in zip(outs.itemgot(i),ctxs,range(max_n))]
+        ctxs = [
+            b.show(ctx=c, **kwargs)
+            for b, c, _ in zip(outs.itemgot(i), ctxs, range(max_n))
+        ]
+
     return ctxs
 
-# %% ../nbs/02_vision_data.ipynb 23
+# %% ../nbs/02_vision_data.ipynb 20
 @typedispatch
-def show_results(x:MedImage, y:TensorCategory, samples, outs, ctxs=None, max_n=6, nrows=None, ncols=None, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    '''Showing samples and their corresponding predictions for classification tasks.'''
-
-    if ctxs is None: ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
+def show_results(x: MedImage, y: TensorCategory, samples, outs, ctxs=None, 
+                 max_n: int = 6, nrows: int = None, ncols: int = None, figsize=None, channel: int = 0, 
+                 indices: int = None, anatomical_plane: int = 0, **kwargs):
+    """Showing samples and their corresponding predictions for classification tasks."""
+
+    if ctxs is None: 
+        ctxs = get_grid(min(len(samples), max_n), nrows=nrows, 
+                        ncols=ncols, figsize=figsize)
+    
     for i in range(2):
-        ctxs = [b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) for b,c,_ in zip(samples.itemgot(i),ctxs,range(max_n))]
-    ctxs = [r.show(ctx=c, color='green' if b==r else 'red', **kwargs) for b,r,c,_ in zip(samples.itemgot(1),outs.itemgot(0),ctxs,range(max_n))]
+        ctxs = [b.show(ctx=c, channel=channel, indices=indices, 
+                       anatomical_plane=anatomical_plane, **kwargs) 
+                for b, c, _ in zip(samples.itemgot(i), ctxs, range(max_n))]
+
+    ctxs = [r.show(ctx=c, color='green' if b == r else 'red', **kwargs) 
+            for b, r, c, _ in zip(samples.itemgot(1), outs.itemgot(0), ctxs, range(max_n))]
+
     return ctxs
 
-# %% ../nbs/02_vision_data.ipynb 24
+# %% ../nbs/02_vision_data.ipynb 21
 @typedispatch
-def show_results(x:MedImage, y:MedMask, samples, outs, ctxs=None, max_n=6, nrows=None, ncols=1, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    ''' Showing decoded samples and their corresponding predictions for segmentation tasks.'''
+def show_results(x: MedImage, y: MedMask, samples, outs, ctxs=None, max_n: int = 6, 
+                 nrows: int = None, ncols: int = 1, figsize=None, channel: int = 0, 
+                 indices: int = None, anatomical_plane: int = 0, **kwargs):
+    """Showing decoded samples and their corresponding predictions for segmentation tasks."""
+
+    if ctxs is None: 
+        ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, 
+                        figsize=figsize, double=True, title='Target/Prediction')
 
-    if ctxs is None: ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize, double=True, title='Target/Prediction')
     for i in range(2):
-        ctxs[::2] = [b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) for b,c,_ in zip(samples.itemgot(i),ctxs[::2],range(2*max_n))]
-    for o in [samples,outs]:
-        ctxs[1::2] = [b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) for b,c,_ in zip(o.itemgot(0),ctxs[1::2],range(2*max_n))]
+        ctxs[::2] = [b.show(ctx=c, channel=channel, indices=indices, 
+                            anatomical_plane=anatomical_plane, **kwargs) 
+                     for b, c, _ in zip(samples.itemgot(i), ctxs[::2], range(2 * max_n))]
+
+    for o in [samples, outs]:
+        ctxs[1::2] = [b.show(ctx=c, channel=channel, indices=indices, 
+                             anatomical_plane=anatomical_plane, **kwargs) 
+                      for b, c, _ in zip(o.itemgot(0), ctxs[1::2], range(2 * max_n))]
+
     return ctxs
 
-# %% ../nbs/02_vision_data.ipynb 26
+# %% ../nbs/02_vision_data.ipynb 23
 @typedispatch
-def plot_top_losses(x: MedImage, y, samples, outs, raws, losses, nrows=None, ncols=None, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    '''Show images in top_losses along with their prediction, actual, loss, and probability of actual class.'''
+def plot_top_losses(x: MedImage, y, samples, outs, raws, losses, nrows: int = None, 
+                    ncols: int = None, figsize=None, channel: int = 0, indices: int = None, 
+                    anatomical_plane: int = 0, **kwargs):
+    """Show images in top_losses along with their prediction, actual, loss, and probability of actual class."""
 
-    title = 'Prediction/Actual/Loss' if type(y) == torch.Tensor else 'Prediction/Actual/Loss/Probability'
+    title = 'Prediction/Actual/Loss' if isinstance(y, torch.Tensor) else 'Prediction/Actual/Loss/Probability'
     axs = get_grid(len(samples), nrows=nrows, ncols=ncols, figsize=figsize, title=title)
-    for ax,s,o,r,l in zip(axs, samples, outs, raws, losses):
+
+    for ax, s, o, r, l in zip(axs, samples, outs, raws, losses):
         s[0].show(ctx=ax, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs)
-        if type(y) == torch.Tensor: ax.set_title(f'{r.max().item():.2f}/{s[1]} / {l.item():.2f}')
-        else: ax.set_title(f'{o[0]}/{s[1]} / {l.item():.2f} / {r.max().item():.2f}')
 
-# %% ../nbs/02_vision_data.ipynb 27
+        if isinstance(y, torch.Tensor): 
+            ax.set_title(f'{r.max().item():.2f}/{s[1]} / {l.item():.2f}')
+        else: 
+            ax.set_title(f'{o[0]}/{s[1]} / {l.item():.2f} / {r.max().item():.2f}')
+
+# %% ../nbs/02_vision_data.ipynb 24
 @typedispatch
-def plot_top_losses(x: MedImage, y:TensorMultiCategory, samples, outs, raws, losses, nrows=None, ncols=None, figsize=None, channel=0, indices=None, anatomical_plane=0, **kwargs):
-    #TODO: not tested yet
+def plot_top_losses(x: MedImage, y: TensorMultiCategory, samples, outs, raws, 
+                    losses, nrows: int = None, ncols: int = None, figsize=None, 
+                    channel: int = 0, indices: int = None, 
+                    anatomical_plane: int = 0, **kwargs):
+    # TODO: not tested yet
     axs = get_grid(len(samples), nrows=nrows, ncols=ncols, figsize=figsize)
-    for i,(ax,s) in enumerate(zip(axs, samples)): s[0].show(ctx=ax, title=f'Image {i}', channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs)
+
+    for i, (ax, s) in enumerate(zip(axs, samples)):
+        s[0].show(ctx=ax, title=f'Image {i}', channel=channel, 
+                  indices=indices, anatomical_plane=anatomical_plane, **kwargs)
+
     rows = get_empty_df(len(samples))
-    outs = L(s[1:] + o + (TitledStr(r), TitledFloat(l.item())) for s,o,r,l in zip(samples, outs, raws, losses))
-    for i,l in enumerate(["target", "predicted", "probabilities", "loss"]):
-        rows = [b.show(ctx=r, label=l, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) for b,r in zip(outs.itemgot(i),rows)]
+    outs = L(s[1:] + o + (TitledStr(r), TitledFloat(l.item())) 
+             for s, o, r, l in zip(samples, outs, raws, losses))
+
+    for i, l in enumerate(["target", "predicted", "probabilities", "loss"]):
+        rows = [b.show(ctx=r, label=l, channel=channel, indices=indices, 
+                       anatomical_plane=anatomical_plane, **kwargs) 
+                for b, r in zip(outs.itemgot(i), rows)]
+
     display_df(pd.DataFrame(rows))
```

### Comparing `fastMONAI-0.3.1/fastMONAI/vision_inference.py` & `fastMONAI-0.3.2/fastMONAI/vision_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,64 +20,78 @@
     
     orientation_itk = DICOMOrient(input_img, org_orientation)
     reoriented_array =  GetArrayFromImage(orientation_itk).transpose()
     
     return reoriented_array[None]
 
 # %% ../nbs/06_vision_inference.ipynb 4
-def _do_resize(o, target_shape, image_interpolation='linear', label_interpolation='nearest'):
-    '''Resample images so the output shape matches the given target shape.'''
+def _do_resize(o, target_shape, image_interpolation='linear', 
+               label_interpolation='nearest'):
+    """
+    Resample images so the output shape matches the given target shape.
+    """
 
-    resize = Resize(target_shape, image_interpolation=image_interpolation, label_interpolation=label_interpolation)
+    resize = Resize(
+        target_shape, 
+        image_interpolation=image_interpolation, 
+        label_interpolation=label_interpolation
+    )
+    
     return resize(o)
 
 # %% ../nbs/06_vision_inference.ipynb 5
-def inference(learn_inf, reorder, resample, fn:(Path,str)='', save_path:(str,Path)=None, org_img=None, input_img=None, org_size=None): 
-    '''Predict on new data using exported model'''         
+def inference(learn_inf, reorder, resample, fn: (str, Path) = '',
+              save_path: (str, Path) = None, org_img=None, input_img=None,
+              org_size=None): 
+    """Predict on new data using exported model."""         
+    
     if None in [org_img, input_img, org_size]: 
-        org_img, input_img, org_size = med_img_reader(fn, reorder, resample, only_tensor=False)
-    else: org_img, input_img = copy(org_img), copy(input_img)
+        org_img, input_img, org_size = med_img_reader(fn, reorder, resample, 
+                                                      only_tensor=False)
+    else: 
+        org_img, input_img = copy(org_img), copy(input_img)
     
-    pred, *_ = learn_inf.predict(input_img.data);
+    pred, *_ = learn_inf.predict(input_img.data)
     
-    pred_mask = do_pad_or_crop(pred.float(), input_img.shape[1:], padding_mode=0, mask_name=None)
+    pred_mask = do_pad_or_crop(pred.float(), input_img.shape[1:], padding_mode=0, 
+                               mask_name=None)
     input_img.set_data(pred_mask)
     
     input_img = _do_resize(input_img, org_size, image_interpolation='nearest')
     
-    reoriented_array = _to_original_orientation(input_img.as_sitk(), ('').join(org_img.orientation))
+    reoriented_array = _to_original_orientation(input_img.as_sitk(), 
+                                                ('').join(org_img.orientation))
     
     org_img.set_data(reoriented_array)
 
     if save_path:
         save_fn = Path(save_path)/('pred_' + Path(fn).parts[-1])
         org_img.save(save_fn)
         return save_fn
     
     return org_img
 
 # %% ../nbs/06_vision_inference.ipynb 7
-def refine_binary_pred_mask(
-        pred_mask,
-        remove_size: (int, float) = None,
-        percentage: float = 0.2,
-        verbose: bool = False
-):
+def refine_binary_pred_mask(pred_mask, 
+                            remove_size: (int, float) = None,
+                            percentage: float = 0.2,
+                            verbose: bool = False) -> np.ndarray:
     """Removes small objects from the predicted binary mask.
 
     Args:
         pred_mask: The predicted mask from which small objects are to be removed.
         remove_size: The size under which objects are considered 'small'.
         percentage: The percentage of the remove_size to be used as threshold. 
             Defaults to 0.2.
         verbose: If True, print the number of components. Defaults to False.
 
     Returns:
         The processed mask with small objects removed.
     """
+                                
     labeled_mask, n_components = label(pred_mask)
 
     if verbose:
         print(n_components)
 
     if remove_size is None:
         sizes = np.bincount(labeled_mask.ravel())
```

### Comparing `fastMONAI-0.3.1/fastMONAI/vision_loss.py` & `fastMONAI-0.3.2/fastMONAI/vision_loss.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,91 +8,100 @@
 from .vision_core import *
 from .vision_data import pred_to_binary_mask, batch_pred_to_multiclass_mask
 from monai.losses import TverskyLoss, FocalLoss
 from torch.nn.modules.loss import _Loss
 
 # %% ../nbs/04_vision_loss_functions.ipynb 3
 class CustomLoss:
-    '''Wrapper to get show_results to work.'''
+    """A custom loss wrapper class for loss functions to allow them to work with
+    the 'show_results' method in fastai. 
+    """
 
     def __init__(self, loss_func):
+        """Constructs CustomLoss object."""
+        
         self.loss_func = loss_func
 
     def __call__(self, pred, targ):
-        if isinstance(pred, MedBase): pred, targ = torch.Tensor(pred.cpu()), torch.Tensor(targ.cpu().float())
+        """Computes the loss for given predictions and targets."""
+        
+        if isinstance(pred, MedBase):
+            pred, targ = torch.Tensor(pred.cpu()), torch.Tensor(targ.cpu().float())
+            
         return self.loss_func(pred, targ)
 
     def activation(self, x):
         return x
     
-    def decodes(self, x):
-        '''Converts model output to target format.
-
+    def decodes(self, x) -> torch.Tensor:
+        """Converts model output to target format.
+        
         Args:
-            x: Activations for each class [B, C, W, H, D]
+            x: Activations for each class with dimensions [B, C, W, H, D].
 
         Returns:
-            torch.Tensor: Predicted mask.
-        '''
-
+            The predicted mask.
+        """
+        
         n_classes = x.shape[1]
-        if n_classes == 1: x = pred_to_binary_mask(x)
-        else: x,_ = batch_pred_to_multiclass_mask(x)
+        if n_classes == 1: 
+            x = pred_to_binary_mask(x)
+        else: 
+            x,_ = batch_pred_to_multiclass_mask(x)
 
         return x
 
 # %% ../nbs/04_vision_loss_functions.ipynb 4
 class TverskyFocalLoss(_Loss):
     """
-    Compute both Dice loss and Focal Loss, and return the weighted sum of these two losses.
-    The details of Dice loss is shown in ``monai.losses.DiceLoss``.
-    The details of Focal Loss is shown in ``monai.losses.FocalLoss``.
+    Compute Tversky loss with a focus parameter, gamma, applied.
+    The details of Tversky loss is shown in ``monai.losses.TverskyLoss``.
     """
 
     def __init__(
         self,
         include_background: bool = True,
         to_onehot_y: bool = False,
         sigmoid: bool = False,
         softmax: bool = False,
-        reduction: str = "mean",
         gamma: float = 2,
-        #focal_weight: (float, int, torch.Tensor) = None,
-        #lambda_dice: float = 1.0,
-        #lambda_focal: float = 1.0,
-        alpha = 0.5, 
-        beta = 0.99
-    ) -> None:
-
+        alpha: float = 0.5, 
+        beta: float = 0.99):
+        """
+        Args:
+            include_background: if to calculate loss for the background class.
+            to_onehot_y: whether to convert `y` into one-hot format.
+            sigmoid: if True, apply a sigmoid function to the prediction.
+            softmax: if True, apply a softmax function to the prediction.
+            gamma: the focal parameter, it modulates the loss with regards to 
+                how far the prediction is from target.
+            alpha: the weight of false positive in Tversky loss calculation.
+            beta: the weight of false negative in Tversky loss calculation.
+        """
+            
         super().__init__()
-        self.tversky = TverskyLoss(to_onehot_y=to_onehot_y, include_background=include_background, sigmoid=sigmoid, softmax=softmax, alpha=alpha, beta=beta)
-        #self.focal = FocalLoss(to_onehot_y=to_onehot_y, include_background=include_background, gamma=gamma, weight=focal_weight, reduction=reduction)
-        
-        #if lambda_dice < 0.0: raise ValueError("lambda_dice should be no less than 0.0.")
-        #if lambda_focal < 0.0: raise ValueError("lambda_focal should be no less than 0.0.")
-        #self.lambda_dice = lambda_dice
-        #self.lambda_focal = lambda_focal
-        self.to_onehot_y = to_onehot_y
+        self.tversky = TverskyLoss(
+            to_onehot_y=to_onehot_y, 
+            include_background=include_background, 
+            sigmoid=sigmoid, 
+            softmax=softmax, 
+            alpha=alpha, 
+            beta=beta
+        )
         self.gamma = gamma
-        self.include_background = include_background
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         """
         Args:
-            input: the shape should be BNH[WD]. The input should be the original logits
-                due to the restriction of ``monai.losses.FocalLoss``.
-            target: the shape should be BNH[WD] or B1H[WD].
+            input: the shape should be [B, C, W, H, D]. The input should be the original logits.
+            target: the shape should be[B, C, W, H, D].
+
         Raises:
             ValueError: When number of dimensions for input and target are different.
-            ValueError: When number of channels for target is neither 1 nor the same as input.
         """
         if len(input.shape) != len(target.shape):
-            raise ValueError("the number of dimensions for input and target should be the same.")
-
-        n_pred_ch = input.shape[1]
+            raise ValueError("The number of dimensions for input and target should be the same.")
 
         tversky_loss = self.tversky(input, target)
-        #focal_loss = self.focal(input, target)
-        total_loss: torch.Tensor = 1 - ((1 - tversky_loss)**self.gamma) #tversky_loss
-        #print(total_loss,total_loss.shape)
-        #tversky_loss +  focal_loss
+        total_loss: torch.Tensor = 1 - ((1 - tversky_loss)**self.gamma)
+
         return total_loss
```

### Comparing `fastMONAI-0.3.1/fastMONAI/vision_plot.py` & `fastMONAI-0.3.2/fastMONAI/vision_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 # %% ../nbs/00_vision_plot.ipynb 1
 from fastai.data.all import *
 from torchio.visualization import rotate
 
 # %% ../nbs/00_vision_plot.ipynb 3
 def _get_slice(image, channel: int, indices: (int, list), anatomical_plane: int, voxel_size: (int, list)):
-    """
-    A private method to get a 2D tensor and aspect ratio for plotting.
+    """A private method to get a 2D tensor and aspect ratio for plotting.
     This is modified code from the torchio function `plot_volume`.
 
     Args:
         image: The input image.
         channel: Channel of the image.
         indices: Index of the 2D slice.
         anatomical_plane: Anatomical plane of the image.
@@ -49,19 +48,17 @@
         sliced_img = rotate(data[i, :, :], radiological=True, n=1)
         aspect = ss / sa
 
     return sliced_img, aspect
 
 # %% ../nbs/00_vision_plot.ipynb 4
 @delegates(plt.Axes.imshow, keep=True, but=['shape', 'imlim'])
-def show_med_img(
-    im, ctx, channel: int, indices: (int, list), anatomical_plane: int,
-    voxel_size: (int, list), ax=None, figsize=None, title=None, **kwargs):
-    """
-    Show an image on `ax`. This is a modified code from the fastai function `show_image`.
+def show_med_img(im, ctx, channel: int, indices: (int, list), anatomical_plane: int,
+                 voxel_size: (int, list), ax=None, figsize=None, title=None, **kwargs):
+    """Show an image on `ax`. This is a modified code from the fastai function `show_image`.
 
     Args:
         im: The input image.
         ctx: The context.
         channel: Channel of the image.
         indices: Index of the 2D slice.
         anatomical_plane: Anatomical plane of the image.
@@ -70,25 +67,30 @@
         figsize: Figure size for the plot.
         title: Title for the plot.
         kwargs: Additional parameters for plt.Axes.imshow method.
 
     Returns:
         Axis with the plot.
     """
-    if hasattrs(im, ('data', 'cpu', 'permute')):
+    if hasattrs(im, ('data', 'cpu', 'permute')): # Check if `im` has the necessary attributes
         im = im.data.cpu()
         im, aspect = _get_slice(
-            im, channel=channel, anatomical_plane=anatomical_plane,
-            voxel_size=voxel_size, indices=indices
+            im, 
+            channel=channel, 
+            anatomical_plane=anatomical_plane,
+            voxel_size=voxel_size, 
+            indices=indices
         )
 
-    ax = ifnone(ax, ctx)
-    if ax is None:
-        _, ax = plt.subplots(figsize=figsize)  # ax is only None when .show() is used.
+    ax = ax if ax is not None else ctx 
+
+    if ax is None: # ax is only None when .show() is used.
+        _, ax = plt.subplots(figsize=figsize)
 
     ax.imshow(im, aspect=aspect, **kwargs)
+
     if title is not None:
         ax.set_title(title)
 
     ax.axis('off')
 
     return ax
```

### Comparing `fastMONAI-0.3.1/fastMONAI.egg-info/PKG-INFO` & `fastMONAI-0.3.2/fastMONAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.1
+Version: 0.3.2
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.1/fastMONAI.egg-info/SOURCES.txt` & `fastMONAI-0.3.2/fastMONAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.1/settings.ini` & `fastMONAI-0.3.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = fastMONAI
 min_python = 3.7
-version = 0.3.1
+version = 0.3.2
 ### OPTIONAL ###
 
 requirements = fastai==2.7.12 monai==1.2.0 torchio==0.18.91 xlrd>=1.2.0 scikit-image==0.19.3 huggingface-hub gdown
 dev_requirements = ipywidgets nbdev tabulate
 
 ### nbdev ###
 nbs_path = nbs
```

### Comparing `fastMONAI-0.3.1/setup.py` & `fastMONAI-0.3.2/setup.py`

 * *Files identical despite different names*

