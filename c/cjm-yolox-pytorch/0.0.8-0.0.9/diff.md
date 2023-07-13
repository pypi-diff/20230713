# Comparing `tmp/cjm-yolox-pytorch-0.0.8.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.8.tar", last modified: Mon Jul  3 19:12:06 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.9.tar", last modified: Mon Jul  3 19:21:36 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.8.tar` & `cjm-yolox-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:12:06.956851 cjm-yolox-pytorch-0.0.8/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.8/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.8/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:12:06.956696 cjm-yolox-pytorch-0.0.8/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-03 18:20:50.000000 cjm-yolox-pytorch-0.0.8/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:12:06.954098 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    21379 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:12:06.956349 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-03 19:11:35.000000 cjm-yolox-pytorch-0.0.8/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-03 19:12:06.956927 cjm-yolox-pytorch-0.0.8/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.8/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:21:36.966369 cjm-yolox-pytorch-0.0.9/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.9/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.9/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:21:36.966214 cjm-yolox-pytorch-0.0.9/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-03 18:20:50.000000 cjm-yolox-pytorch-0.0.9/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:21:36.963734 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-03 19:21:23.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-03 19:21:23.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    21221 2023-07-03 19:21:23.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-03 19:21:23.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-03 19:21:23.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-03 19:21:23.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:21:36.965866 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:21:36.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-03 19:21:36.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-03 19:21:36.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-03 19:21:36.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-03 19:21:36.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-03 19:21:36.000000 cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-03 19:21:18.000000 cjm-yolox-pytorch-0.0.9/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-03 19:21:36.966417 cjm-yolox-pytorch-0.0.9/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.9/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.8/LICENSE` & `cjm-yolox-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.8/PKG-INFO` & `cjm-yolox-pytorch-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.8/README.md` & `cjm-yolox-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_loss.ipynb.
 
 # %% auto 0
 __all__ = ['MlvlPointGenerator', 'SamplingResult', 'YOLOXLoss']
 
-# %% ../nbs/02_loss.ipynb 4
+# %% ../nbs/02_loss.ipynb 3
 from typing import Any, Type, List, Optional, Callable, Tuple, Union
 from functools import partial
 
-# %% ../nbs/02_loss.ipynb 5
+# %% ../nbs/02_loss.ipynb 4
 import numpy as np
 
 import torch
-from torch.nn.modules.utils import _pair
 import torch.nn.functional as F
 import torchvision
 
-# %% ../nbs/02_loss.ipynb 6
+# %% ../nbs/02_loss.ipynb 5
 from .utils import multi_apply
 from .simota import SimOTAAssigner
 
-# %% ../nbs/02_loss.ipynb 8
+# %% ../nbs/02_loss.ipynb 7
 class MlvlPointGenerator:
     """Standard points generator for multi-level (Mlvl) feature maps in 2D points-based detectors.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/anchor/point_generator.py#L44)
     
     """
 
     def __init__(self, 
                  strides:List[Union[int, Tuple[int, int]]], # Strides of anchors in multiple feature levels in order (w, h).
                  offset:float = 0.5 # The offset of points, the value is normalized with corresponding stride.
                 ):
-        self.strides = [_pair(stride) for stride in strides]
         self.strides = strides
         self.offset = offset
 
     @property
     def num_levels(self) -> int:
         """int: number of feature levels that the generator will be applied."""
         return len(self.strides)
@@ -70,29 +68,28 @@
             device (str, optional): The device the tensor will be put on. Defaults to 'cuda'.
             with_stride (bool): Concatenate the stride to the last dimension of points.
 
         Return:
             torch.Tensor: Points of single feature levels.
         """
         feat_h, feat_w = featmap_size
-#         stride_w, stride_h = self.strides[level_idx]
         stride = self.strides[level_idx]
         shift_x = (torch.arange(0., feat_w, device=device) + self.offset) * stride
         shift_y = (torch.arange(0., feat_h, device=device) + self.offset) * stride
         shift_xx, shift_yy = torch.meshgrid(shift_x, shift_y, indexing='xy')
         shift_xx, shift_yy = shift_xx.flatten(), shift_yy.flatten()
 
         if with_stride:
             shifts = torch.stack([shift_xx, shift_yy, torch.full_like(shift_xx, stride), torch.full_like(shift_yy, stride)], dim=-1)
         else:
             shifts = torch.stack([shift_xx, shift_yy], dim=-1)
         
         return shifts.to(device)
 
-# %% ../nbs/02_loss.ipynb 10
+# %% ../nbs/02_loss.ipynb 9
 class SamplingResult:
     """
     Bounding box sampling result.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/samplers/sampling_result.py#L7)
@@ -135,15 +132,15 @@
 
         # If labels are assigned, assign labels for positive samples. Otherwise, set it as None
         if assignment_result.category_labels is not None:
             self.positive_ground_truth_labels = assignment_result.category_labels[positive_indices]
         else:
             self.positive_ground_truth_labels = None
 
-# %% ../nbs/02_loss.ipynb 12
+# %% ../nbs/02_loss.ipynb 11
 class YOLOXLoss:
     """
     YOLOXLoss class implements the loss function used in the YOLOX model. 
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/dense_heads/yolox_head.py#L321)
```

### Comparing `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.8/settings.ini` & `cjm-yolox-pytorch-0.0.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.8/setup.py` & `cjm-yolox-pytorch-0.0.9/setup.py`

 * *Files identical despite different names*

