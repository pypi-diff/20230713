# Comparing `tmp/cjm-yolox-pytorch-0.0.86.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.86.tar", last modified: Thu Jul 13 07:29:46 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.9.tar", last modified: Mon Jul  3 19:21:36 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.86.tar` & `cjm-yolox-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 07:29:46.252548 cjm-yolox-pytorch-0.0.86/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.86/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.86/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 07:29:46.252371 cjm-yolox-pytorch-0.0.86/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-04 21:34:25.000000 cjm-yolox-pytorch-0.0.86/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 07:29:46.249700 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-13 07:29:35.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12388 2023-07-13 07:29:35.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    18085 2023-07-13 07:29:35.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-13 07:29:35.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    16960 2023-07-13 07:29:35.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2614 2023-07-13 07:29:35.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 07:29:46.252042 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 07:29:46.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-13 07:29:46.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-13 07:29:46.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-13 07:29:46.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-13 07:29:46.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-13 07:29:46.000000 cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-13 07:27:56.000000 cjm-yolox-pytorch-0.0.86/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-13 07:29:46.252612 cjm-yolox-pytorch-0.0.86/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.86/setup.py
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

### Comparing `cjm-yolox-pytorch-0.0.86/LICENSE` & `cjm-yolox-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.86/PKG-INFO` & `cjm-yolox-pytorch-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.86
+Version: 0.0.9
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.86/README.md` & `cjm-yolox-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/cjm-yolox-pytorch',
                 'doc_host': 'https://cj-mills.github.io',
                 'git_url': 'https://github.com/cj-mills/cjm-yolox-pytorch',
                 'lib_path': 'cjm_yolox_pytorch'},
-  'syms': { 'cjm_yolox_pytorch.loss': { 'cjm_yolox_pytorch.loss.SamplingResult': ('loss.html#samplingresult', 'cjm_yolox_pytorch/loss.py'),
+  'syms': { 'cjm_yolox_pytorch.loss': { 'cjm_yolox_pytorch.loss.MlvlPointGenerator': ( 'loss.html#mlvlpointgenerator',
+                                                                                       'cjm_yolox_pytorch/loss.py'),
+                                        'cjm_yolox_pytorch.loss.MlvlPointGenerator.__init__': ( 'loss.html#mlvlpointgenerator.__init__',
+                                                                                                'cjm_yolox_pytorch/loss.py'),
+                                        'cjm_yolox_pytorch.loss.MlvlPointGenerator.grid_priors': ( 'loss.html#mlvlpointgenerator.grid_priors',
+                                                                                                   'cjm_yolox_pytorch/loss.py'),
+                                        'cjm_yolox_pytorch.loss.MlvlPointGenerator.num_levels': ( 'loss.html#mlvlpointgenerator.num_levels',
+                                                                                                  'cjm_yolox_pytorch/loss.py'),
+                                        'cjm_yolox_pytorch.loss.MlvlPointGenerator.single_level_grid_priors': ( 'loss.html#mlvlpointgenerator.single_level_grid_priors',
+                                                                                                                'cjm_yolox_pytorch/loss.py'),
+                                        'cjm_yolox_pytorch.loss.SamplingResult': ('loss.html#samplingresult', 'cjm_yolox_pytorch/loss.py'),
                                         'cjm_yolox_pytorch.loss.SamplingResult.__init__': ( 'loss.html#samplingresult.__init__',
                                                                                             'cjm_yolox_pytorch/loss.py'),
                                         'cjm_yolox_pytorch.loss.YOLOXLoss': ('loss.html#yoloxloss', 'cjm_yolox_pytorch/loss.py'),
                                         'cjm_yolox_pytorch.loss.YOLOXLoss.__call__': ( 'loss.html#yoloxloss.__call__',
                                                                                        'cjm_yolox_pytorch/loss.py'),
                                         'cjm_yolox_pytorch.loss.YOLOXLoss.__init__': ( 'loss.html#yoloxloss.__init__',
                                                                                        'cjm_yolox_pytorch/loss.py'),
@@ -74,30 +84,29 @@
                                          'cjm_yolox_pytorch.model.YOLOXHead.forward': ( 'model.html#yoloxhead.forward',
                                                                                         'cjm_yolox_pytorch/model.py'),
                                          'cjm_yolox_pytorch.model.YOLOXHead.forward_single': ( 'model.html#yoloxhead.forward_single',
                                                                                                'cjm_yolox_pytorch/model.py'),
                                          'cjm_yolox_pytorch.model.YOLOXPAFPN': ('model.html#yoloxpafpn', 'cjm_yolox_pytorch/model.py'),
                                          'cjm_yolox_pytorch.model.YOLOXPAFPN.__init__': ( 'model.html#yoloxpafpn.__init__',
                                                                                           'cjm_yolox_pytorch/model.py'),
-                                         'cjm_yolox_pytorch.model.YOLOXPAFPN._bottom_up': ( 'model.html#yoloxpafpn._bottom_up',
-                                                                                            'cjm_yolox_pytorch/model.py'),
-                                         'cjm_yolox_pytorch.model.YOLOXPAFPN._top_down': ( 'model.html#yoloxpafpn._top_down',
-                                                                                           'cjm_yolox_pytorch/model.py'),
                                          'cjm_yolox_pytorch.model.YOLOXPAFPN.forward': ( 'model.html#yoloxpafpn.forward',
                                                                                          'cjm_yolox_pytorch/model.py'),
                                          'cjm_yolox_pytorch.model.build_model': ('model.html#build_model', 'cjm_yolox_pytorch/model.py'),
-                                         'cjm_yolox_pytorch.model.init_head': ('model.html#init_head', 'cjm_yolox_pytorch/model.py')},
+                                         'cjm_yolox_pytorch.model.init_head': ('model.html#init_head', 'cjm_yolox_pytorch/model.py'),
+                                         'cjm_yolox_pytorch.model.kaiming_init': ('model.html#kaiming_init', 'cjm_yolox_pytorch/model.py')},
             'cjm_yolox_pytorch.simota': { 'cjm_yolox_pytorch.simota.AssignResult': ( 'simota.html#assignresult',
                                                                                      'cjm_yolox_pytorch/simota.py'),
+                                          'cjm_yolox_pytorch.simota.AssignResult.__init__': ( 'simota.html#assignresult.__init__',
+                                                                                              'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner': ( 'simota.html#simotaassigner',
                                                                                        'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.__init__': ( 'simota.html#simotaassigner.__init__',
                                                                                                 'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.assign': ( 'simota.html#simotaassigner.assign',
                                                                                               'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.dynamic_k_matching': ( 'simota.html#simotaassigner.dynamic_k_matching',
                                                                                                           'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.get_in_gt_and_in_center_info': ( 'simota.html#simotaassigner.get_in_gt_and_in_center_info',
                                                                                                                     'cjm_yolox_pytorch/simota.py')},
-            'cjm_yolox_pytorch.utils': { 'cjm_yolox_pytorch.utils.generate_grid_priors': ( 'utils.html#generate_grid_priors',
-                                                                                           'cjm_yolox_pytorch/utils.py'),
+            'cjm_yolox_pytorch.utils': { 'cjm_yolox_pytorch.utils.download_file': ( 'utils.html#download_file',
+                                                                                    'cjm_yolox_pytorch/utils.py'),
                                          'cjm_yolox_pytorch.utils.multi_apply': ('utils.html#multi_apply', 'cjm_yolox_pytorch/utils.py')}}}
```

### Comparing `cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/loss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,95 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_loss.ipynb.
 
 # %% auto 0
-__all__ = ['SamplingResult', 'YOLOXLoss']
+__all__ = ['MlvlPointGenerator', 'SamplingResult', 'YOLOXLoss']
 
 # %% ../nbs/02_loss.ipynb 3
 from typing import Any, Type, List, Optional, Callable, Tuple, Union
 from functools import partial
 
 # %% ../nbs/02_loss.ipynb 4
 import numpy as np
 
 import torch
 import torch.nn.functional as F
 import torchvision
 
 # %% ../nbs/02_loss.ipynb 5
-from .utils import multi_apply, generate_grid_priors
+from .utils import multi_apply
 from .simota import SimOTAAssigner
 
 # %% ../nbs/02_loss.ipynb 7
+class MlvlPointGenerator:
+    """Standard points generator for multi-level (Mlvl) feature maps in 2D points-based detectors.
+    
+    Based on OpenMMLab's implementation in the mmdetection library:
+    
+    - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/anchor/point_generator.py#L44)
+    
+    """
+
+    def __init__(self, 
+                 strides:List[Union[int, Tuple[int, int]]], # Strides of anchors in multiple feature levels in order (w, h).
+                 offset:float = 0.5 # The offset of points, the value is normalized with corresponding stride.
+                ):
+        self.strides = strides
+        self.offset = offset
+
+    @property
+    def num_levels(self) -> int:
+        """int: number of feature levels that the generator will be applied."""
+        return len(self.strides)
+
+    def grid_priors(self, featmap_sizes: List[Tuple[int, int]], device: str = 'cuda', with_stride: bool = False) -> List[torch.Tensor]:
+        """Generate grid points of multiple feature levels.
+
+        Args:
+            featmap_sizes (List[Tuple[int, int]]): List of feature map sizes in multiple feature levels, each size arrange as as (h, w).
+            device (str): The device where the anchors will be put on.
+            with_stride (bool): Whether to concatenate the stride to the last dimension of points.
+
+        Return:
+            list[torch.Tensor]: Points of multiple feature levels.
+        """
+        assert self.num_levels == len(featmap_sizes)
+        multi_level_priors = [self.single_level_grid_priors(featmap_sizes[i], i, device, with_stride) for i in range(self.num_levels)]
+        return multi_level_priors
+
+    def single_level_grid_priors(self,
+                                 featmap_size: Tuple[int, int],
+                                 level_idx: int,
+                                 device: str = 'cuda',
+                                 with_stride: bool = False) -> torch.Tensor:
+        """Generate grid Points of a single level.
+
+        Args:
+            featmap_size (Tuple[int, int]): Size of the feature maps, arrange as (h, w).
+            level_idx (int): The index of corresponding feature map level.
+            device (str, optional): The device the tensor will be put on. Defaults to 'cuda'.
+            with_stride (bool): Concatenate the stride to the last dimension of points.
+
+        Return:
+            torch.Tensor: Points of single feature levels.
+        """
+        feat_h, feat_w = featmap_size
+        stride = self.strides[level_idx]
+        shift_x = (torch.arange(0., feat_w, device=device) + self.offset) * stride
+        shift_y = (torch.arange(0., feat_h, device=device) + self.offset) * stride
+        shift_xx, shift_yy = torch.meshgrid(shift_x, shift_y, indexing='xy')
+        shift_xx, shift_yy = shift_xx.flatten(), shift_yy.flatten()
+
+        if with_stride:
+            shifts = torch.stack([shift_xx, shift_yy, torch.full_like(shift_xx, stride), torch.full_like(shift_yy, stride)], dim=-1)
+        else:
+            shifts = torch.stack([shift_xx, shift_yy], dim=-1)
+        
+        return shifts.to(device)
+
+# %% ../nbs/02_loss.ipynb 9
 class SamplingResult:
     """
     Bounding box sampling result.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/samplers/sampling_result.py#L7)
@@ -65,40 +132,42 @@
 
         # If labels are assigned, assign labels for positive samples. Otherwise, set it as None
         if assignment_result.category_labels is not None:
             self.positive_ground_truth_labels = assignment_result.category_labels[positive_indices]
         else:
             self.positive_ground_truth_labels = None
 
-# %% ../nbs/02_loss.ipynb 9
+# %% ../nbs/02_loss.ipynb 11
 class YOLOXLoss:
     """
     YOLOXLoss class implements the loss function used in the YOLOX model. 
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/dense_heads/yolox_head.py#L321)
 
     #### Pseudocode
-    1. Generate the grid of prior boxes by calling the `generate_grid_priors` function with arguments based on the shape of class scores and strides.
-    2. Update the centroids of the prior boxes based on their widths and heights.
-    3. Flatten the predicted class scores, bounding box predictions, and objectness scores across all scales and concatenate them. This is done by calling the `flatten_and_concat` method for each of these predictions.
-    4. Decode the predicted bounding boxes by calling the `bbox_decode` method, which calculates the actual coordinates of the predicted boxes based on the prior boxes and the predicted bounding box transformations.
-    5. For each image in the batch, compute the targets for classification, bounding box regression, objectness, and optionally, L1 regression. This is done by calling the `get_target_single` method, which matches prior boxes to ground truth boxes, samples positive and negative boxes, and then computes the targets. 
-    6. Concatenate all the computed targets across all images.
-    7. Compute the bounding box, objectness, and class losses by comparing the predictions with the targets. 
-    8. Calculate the total number of positive samples across all images in the batch.
-    9. Scale the computed losses using their respective weights and the total number of samples.
-    10. Create a dictionary to store the computed losses.
-    11. If use_l1 is True, concatenate l1 targets, compute L1 loss and add it to the loss dictionary.
-        
+    1. Receive class_scores, predicted_bboxes, objectness_scores, ground_truth_bboxes, and ground_truth_labels as input. These are all tensors.
+    2. Calculate the size of the feature maps from class scores.
+    3. Create multi-level prior boxes using the feature map sizes.
+    4. Reshape and flatten class predictions, bounding box predictions, and objectness scores. 
+    5. Combine the class predictions, bounding box predictions, and objectness scores from different levels into one tensor respectively.
+    6. Combine the prior boxes from different levels into one tensor and decode the bounding boxes using these prior boxes and bounding box predictions.
+    7. For each image, calculate the targets for classification, bounding box, objectness, and optionally, L1 loss.
+    8. Determine the total number of positive samples.
+    9. Combine the masks, class targets, objectness targets, and bounding box targets from different images into one tensor respectively.
+    10. Calculate the bounding box loss, objectness loss, and class loss using the respective targets and predictions.
+        - If L1 loss is enabled, calculate the L1 loss using the bounding box predictions and L1 targets.
+    11. Return a dictionary containing the classification, bounding box, objectness, and optionally, L1 loss.
+    
+    
     """
     def __init__(self, 
                  num_classes:int, # The number of target classes.
-                 bbox_loss_weight:float=5.0, # The weight for the loss function to calculate the bounding box regression loss.
+                 bbox_loss_weight:float=2.0, # The weight for the loss function to calculate the bounding box regression loss.
                  class_loss_weight:float=1.0, # The weight for the loss function to calculate the classification loss.
                  objectness_loss_weight:float=1.0, # The weight for the loss function to calculate the objectness loss.
                  l1_loss_weight:float=1.0, # The weight for the loss function to calculate the L1 loss.
                  use_l1:bool=False, # Whether to use L1 loss in the calculation.
                  strides:List[int]=[8,16,32] # The list of strides.
                 ):
         
@@ -106,27 +175,27 @@
         
         giou_loss_partial = partial(torchvision.ops.generalized_box_iou_loss, reduction='none', eps=1e-16)
         self.bbox_loss_func = lambda bx1, bx2 : (1-(1-giou_loss_partial(boxes1=bx1, boxes2=bx2))**2).sum()
         self.class_loss_func = partial(F.binary_cross_entropy_with_logits, reduction='sum')
         self.objectness_loss_func = partial(F.binary_cross_entropy_with_logits, reduction='sum')
         self.l1_loss_func = partial(F.l1_loss, reduction='sum')
         
+        
         self.bbox_loss_weight = bbox_loss_weight
         self.class_loss_weight = class_loss_weight
         self.objectness_loss_weight = objectness_loss_weight
         self.l1_loss_weight = l1_loss_weight
         
+        
         self.use_l1 = use_l1
         
-        # Initialize the assigner
+        # Initialize the prior box generator and assigner
+        self.prior_generator = MlvlPointGenerator(strides, offset=0)
         self.assigner = SimOTAAssigner(center_radius=2.5)
         
-        self.strides = strides
-        
-        
     def bbox_decode(self, prior_boxes, predicted_boxes):
         """
         Decodes the predicted bounding boxes based on the prior boxes.
 
         Args:
             prior_boxes (torch.Tensor): The prior bounding boxes.
             predicted_boxes (torch.Tensor): The predicted bounding boxes.
@@ -283,66 +352,76 @@
             objectness_scores (List[torch.Tensor]): A list of objectness scores for each scale.
             ground_truth_bboxes (List[torch.Tensor]): A list of ground truth bounding boxes for each image.
             ground_truth_labels (List[torch.Tensor]): A list of ground truth labels for each image.
 
         Returns:
             Dict: A dictionary with the classification, bounding box, objectness, and optionally, L1 loss.
         """
-        
-        # Generate prior box coordinates for all anchors.
-        grid_priors = generate_grid_priors(*[s*self.strides[0] for s in class_scores[0].shape[-2:]], self.strides)
-        grid_priors[:, :2] *= grid_priors[:, 2].unsqueeze(1)
-        flatten_prior_boxes = torch.cat([grid_priors, grid_priors[:, 2:].clone()], dim=1)
+        # Compute feature map sizes from class scores
+        feature_map_sizes = [class_score.shape[2:] for class_score in class_scores]
+
+        # Generate multi-level priors
+        multilevel_prior_boxes = self.prior_generator.grid_priors(
+            feature_map_sizes, class_scores[0].device, with_stride=True)
         
         # Flatten and concatenate class predictions, bounding box predictions, and objectness scores
         flatten_class_preds = self.flatten_and_concat(class_scores, num_images, self.num_classes)
         flatten_bbox_preds = self.flatten_and_concat(predicted_bboxes, num_images, 4)
         flatten_objectness_scores = self.flatten_and_concat(objectness_scores, num_images)
                     
-        # Concatenate and decode box predictions
-        flatten_prior_boxes = flatten_prior_boxes.to(flatten_bbox_preds.device)
+        # Concatenate and decode prior boxes
+        flatten_prior_boxes = torch.cat(multilevel_prior_boxes)
         flatten_decoded_bboxes = self.bbox_decode(flatten_prior_boxes, flatten_bbox_preds)
 
         # Compute targets
         (positive_masks, class_targets, objectness_targets, bbox_targets, l1_targets,
          num_positive_images) = multi_apply(
              self.get_target_single, flatten_class_preds.detach(),
              flatten_objectness_scores.detach(),
              flatten_prior_boxes.unsqueeze(0).repeat(num_images, 1, 1),
              flatten_decoded_bboxes.detach(), ground_truth_bboxes, ground_truth_labels)
 
+        # Calculate total number of samples
+        num_total_samples = max(sum(num_positive_images), 1)
+
         # Concatenate all positive masks, class targets, objectness targets, and bounding box targets
         positive_masks = torch.cat(positive_masks, 0)
         class_targets = torch.cat(class_targets, 0)
         objectness_targets = torch.cat(objectness_targets, 0)
         bbox_targets = torch.cat(bbox_targets, 0)
 
+        # If use_l1 is True, concatenate l1 targets
+        if self.use_l1:
+            l1_targets = torch.cat(l1_targets, 0)
+
         # Compute bounding box loss
-        loss_bbox = self.bbox_loss_func(flatten_decoded_bboxes.view(-1, 4)[positive_masks], bbox_targets)
+        loss_bbox = self.bbox_loss_func(
+            flatten_decoded_bboxes.view(-1, 4)[positive_masks],
+            bbox_targets) / num_total_samples
 
         # Compute objectness loss
-        loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1), objectness_targets)
+        loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1),
+                                 objectness_targets) / num_total_samples
 
         # Compute class loss
-        loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks],class_targets)
-        
-        # Calculate total number of samples
-        num_total_samples = max(sum(num_positive_images), 1)
-        
+        loss_cls = self.class_loss_func(
+            flatten_class_preds.view(-1, self.num_classes)[positive_masks],
+            class_targets) / num_total_samples
+                
         # Scale losses
-        loss_bbox = (loss_bbox * self.bbox_loss_weight) / num_total_samples
-        loss_obj = (loss_obj * self.objectness_loss_weight) / num_total_samples
-        loss_cls = (loss_cls * self.class_loss_weight) / num_total_samples
+        loss_bbox *= self.bbox_loss_weight
+        loss_obj *= self.objectness_loss_weight
+        loss_cls *= self.class_loss_weight
         
+
         # Initialize loss dictionary
         loss_dict = dict(loss_cls=loss_cls, loss_bbox=loss_bbox, loss_obj=loss_obj)
 
-        # If use_l1 is True, concatenate l1 targets, compute L1 loss and add it to the loss dictionary
+        # If use_l1 is True, compute L1 loss and add it to the loss dictionary
         if self.use_l1:
-            l1_targets = torch.cat(l1_targets, 0)
             loss_l1 = self.l1_loss_func(
                 flatten_bbox_preds.view(-1, 4)[positive_masks],
                 l1_targets) / num_total_samples
             loss_l1 *= self.l1_loss_weight
             loss_dict.update(loss_l1=loss_l1)
 
         # Return loss dictionary
```

### Comparing `cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_model.ipynb.
 
 # %% auto 0
 __all__ = ['MODEL_TYPES', 'CSP_DARKNET_CFGS', 'PAFPN_CFGS', 'HEAD_CFGS', 'OPENMMLAB_CKPT_URL', 'PRETRAINED_URLS', 'NORM_CFG',
-           'NORM_STATS', 'MODEL_CFGS', 'ConvModule', 'DarknetBottleneck', 'CSPLayer', 'Focus', 'SPPBottleneck',
-           'CSPDarknet', 'YOLOXPAFPN', 'YOLOXHead', 'YOLOX', 'init_head', 'build_model']
+           'ConvModule', 'DarknetBottleneck', 'CSPLayer', 'Focus', 'SPPBottleneck', 'CSPDarknet', 'YOLOXPAFPN',
+           'YOLOXHead', 'YOLOX', 'kaiming_init', 'init_head', 'build_model']
 
 # %% ../nbs/00_model.ipynb 4
 import os
 from typing import Any, Type, List, Optional, Callable, Tuple
 from functools import partial
 
 from pathlib import Path
@@ -15,15 +15,15 @@
 # %% ../nbs/00_model.ipynb 5
 import torch
 import torch.nn as nn
 
 import torch.nn.init as init
 
 # %% ../nbs/00_model.ipynb 6
-from .utils import multi_apply
+from .utils import download_file, multi_apply
 
 # %% ../nbs/00_model.ipynb 8
 MODEL_TYPES = ['yolox_tiny', 'yolox_s', 'yolox_m', 'yolox_l', 'yolox_x']
 
 CSP_DARKNET_CFGS = {
     MODEL_TYPES[0]:dict(deepen_factor=0.33, widen_factor=0.375),
     MODEL_TYPES[1]:dict(deepen_factor=0.33, widen_factor=0.5),
@@ -56,23 +56,14 @@
     MODEL_TYPES[2]:None,
     MODEL_TYPES[3]:f'{OPENMMLAB_CKPT_URL}/yolox_l_8x8_300e_coco/yolox_l_8x8_300e_coco_20211126_140236-d3bd2b23.pth',
     MODEL_TYPES[4]:f'{OPENMMLAB_CKPT_URL}/yolox_x_8x8_300e_coco/yolox_x_8x8_300e_coco_20211126_140254-1ef88d67.pth',
 }
 
 NORM_CFG = dict(momentum=0.03, eps=0.001)
 
-
-NORM_STATS = dict(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
-
-MODEL_CFGS = {model_type: {**CSP_DARKNET_CFGS[model_type], 
-                            **{'neck_'+k: v for k, v in PAFPN_CFGS[model_type].items()}, 
-                            **{'head_'+k: v for k, v in HEAD_CFGS[model_type].items()}, 
-                            **{k:{"pretrained": v != None} for k,v in PRETRAINED_URLS.items()}[model_type]} 
-               for model_type in MODEL_TYPES}
-
 # %% ../nbs/00_model.ipynb 11
 class ConvModule(nn.Module):
     """
     Configurable block used for Convolution2d-Normalization-Activation blocks.
     
     #### Pseudocode
     Function forward(input x):
@@ -101,16 +92,14 @@
 
         # Convolutional layer
         self.conv = nn.Conv2d(in_channels, out_channels, kernel_size, stride, padding, bias=bias)
         # Batch normalization layer
         self.bn = nn.BatchNorm2d(out_channels, eps=eps, momentum=momentum, affine=affine, track_running_stats=track_running_stats)
         # Activation function
         self.activate = activation_function()
-        
-        init.kaiming_normal_(self.conv.weight.data, mode='fan_out', nonlinearity='relu')
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         
         # Pass input through convolutional layer
         x = self.conv(x)
         # Pass output from convolutional layer through batch normalization
         x = self.bn(x)
@@ -118,128 +107,186 @@
         return self.activate(x)
 
 # %% ../nbs/00_model.ipynb 13
 class DarknetBottleneck(nn.Module):
     """
     Basic Darknet bottleneck block used in Darknet.
     
-    This class represents a basic bottleneck block used in Darknet, which consists of two convolutional layers with a possible identity shortcut.
-    
     Based on OpenMMLab's implementation in the mmdetection library:
     
-     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/utils/csp_layer.py#L8)
+    - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/utils/csp_layer.py#L8)
+    
+    #### Pseudocode
+    Function forward(input_tensor x):
+    
+    1. Store x as identity.
+    2. Pass x through the first convolutional layer (conv1), and then the result through the second convolutional layer (conv2). Store the output as 'out'.
+    3. Check if add_identity is True:
+       a. If True, check if identity_conv exists (i.e., when the input and output channels do not match).
+          i. If identity_conv exists, pass identity through the identity_conv layer and update the identity.
+       b. Add the updated identity to the 'out'.
+    4. Return 'out' as the final output.
+
     """
     
     def __init__(self, 
                  in_channels: int, # The number of input channels to the block.
                  out_channels: int, # The number of output channels from the block.
                  eps: float = 0.001, # A value added to the denominator for numerical stability in the ConvModule's BatchNorm layer.
                  momentum: float = 0.03, # The value used for the running_mean and running_var computation in the ConvModule's BatchNorm layer.
                  affine: bool = True, # A flag that when set to True, gives the ConvModule's BatchNorm layer learnable affine parameters.
                  track_running_stats: bool = True, # If True, the ConvModule's BatchNorm layer will track the running mean and variance.
                  add_identity: bool = True # If True, add an identity shortcut (also known as skip connection) to the output.
-                ) -> None:
+                ):
         super(DarknetBottleneck, self).__init__()
 
         self.add_identity = add_identity
-
-        # The first conv layer reduces the dimensionality with a 1x1 kernel, 
-        # and the second conv layer restores it with a 3x3 kernel.
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        
+        # First convolutional layer with 1x1 kernel size
         self.conv1 = ConvModule(in_channels, out_channels, kernel_size=1, stride=1, padding=0, 
                                 bias=False, eps=eps, momentum=momentum, affine=affine, 
                                 track_running_stats=track_running_stats)
+        
+        # Second convolutional layer with 3x3 kernel size
         self.conv2 = ConvModule(out_channels, out_channels, kernel_size=3, stride=1, padding=1, 
                                 bias=False, eps=eps, momentum=momentum, affine=affine, 
                                 track_running_stats=track_running_stats)
         
-        # If add_identity is True and in_channels do not match out_channels, 
-        # introduce a conv layer on the identity shortcut to match the dimensions.
-        # If not, use nn.Identity() for a cleaner forward method.
-        if self.add_identity and in_channels != out_channels:
+        # Add a 1x1 conv on shortcut when in and out channels don't match
+        if self.add_identity and self.in_channels != self.out_channels:
             self.identity_conv = ConvModule(in_channels, out_channels, kernel_size=1, stride=1, padding=0, 
                                             bias=False, eps=eps, momentum=momentum, affine=affine, 
                                             track_running_stats=track_running_stats)
         else:
-            self.identity_conv = nn.Identity()
+            self.identity_conv = None
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
+                
+        # Store the input tensor as identity tensor for possible use in shortcut connection
         identity = x
+        # Pass the input tensor through two conv layers in sequence
         out = self.conv2(self.conv1(x))
         
-        # If add_identity is True, add the transformed (if necessary) identity to the output
+        # If add_identity is True, then add the original input (identity) to the output of the conv layers
         if self.add_identity:
-            out += self.identity_conv(identity)
+            # Apply a conv layer to the identity tensor if the in and out channels don't match
+            if self.identity_conv is not None:
+                identity = self.identity_conv(identity)
+            # Add the identity tensor to the output tensor
+            out += identity
 
         return out
 
 # %% ../nbs/00_model.ipynb 15
 class CSPLayer(nn.Module):
-    """
-    Cross Stage Partial Layer (CSPLayer).
     
-    This layer consists of a series of convolutions, blocks of transformations, and a final convolution. 
-    The inputs are processed via two paths: a main path with blocks and a shortcut path. The results from 
-    both paths are concatenated and further processed before returning the final output.
-
-    The blocks are instances of the DarknetBottleneck class which perform additional transformations.
+    """
+    Cross Stage Partial Layer
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
-    - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/)
+    - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/utils/csp_layer.py#L75)
+    
+    #### Pseudocode
+    1. Start with input `x`
+    2. Apply `main_conv` layer on `x` and store the output in `x1`
+    3. Apply `short_conv` layer on `x` and store the output in `x2`
+    4. For each `block` in the `blocks` list:
+        - Pass `x1` through the `block` and store the result back in `x1`
+    5. Concatenate `x1` and `x2` along dimension 1 to form a new tensor called `out`
+    6. Pass `out` through the `final_conv` layer and store the result back in `out`
+    7. Return `out` as the final output of the forward function
+    
+    Notes:
+    
+    - The `main_conv`, `short_conv`, and `final_conv` are convolution layers which apply a series of transformations (including convolution, batch normalization, and non-linear activation) on the input tensor.
+    - The `blocks` list contains a number of "bottleneck" layers that perform additional transformations on the `x1` tensor. Each bottleneck layer has a specific structure, with two convolution layers and an optional identity shortcut.
+    - The concatenation operation combines the results of the `main_conv` layers processed through `blocks` and the `short_conv` layer, preparing the tensor for the final transformations in `final_conv`.
     """
+        
     def __init__(self, 
-                 in_channels: int, # Number of input channels.
-                 out_channels: int, # Number of output channels.
-                 num_blocks: int, # Number of blocks in the bottleneck.
-                 kernel_size: int = 1, # Size of the convolving kernel.
-                 stride: int = 1, # Stride of the convolution.
-                 padding: int = 0, # Zero-padding added to both sides of the input.
-                 eps: float = 0.001, # A value added to the denominator for numerical stability.
-                 momentum: float = 0.03, # The value used for the running_mean and running_var computation.
-                 affine: bool = True, # A flag that when set to True, gives the layer learnable affine parameters.
-                 track_running_stats: bool = True, # Whether or not to track the running mean and variance during training.
-                 add_identity: bool = True # Whether or not to add an identity shortcut connection if the input and output are the same size.
-                ) -> None:
+                 in_channels, # Number of input channels.
+                 out_channels, # Number of output channels.
+                 num_blocks, # Number of blocks in the bottleneck.
+                 kernel_size=1, # Size of the convolving kernel.
+                 stride=1, # Stride of the convolution.
+                 padding=0, # Zero-padding added to both sides of the input.
+                 eps=0.001, # A value added to the denominator for numerical stability in the ConvModule's BatchNorm layer.
+                 momentum=0.03, # The value used for the running_mean and running_var computation in the ConvModule's BatchNorm layer.
+                 affine=True, # A flag that when set to True, gives the ConvModule's BatchNorm layer learnable affine parameters.
+                 track_running_stats=True, # Whether or not to track the running mean and variance during training.
+                 add_identity=True # Whether or not to add an identity shortcut connection if the input and output are the same size.
+                ):
         
-        super().__init__()
+        super(CSPLayer, self).__init__()
 
+        # Define the number of hidden_channels as half the number of out_channels
         hidden_channels = out_channels // 2
 
+        # Define the main convolution layer
         self.main_conv = ConvModule(in_channels, hidden_channels, kernel_size, stride, padding, 
                                     bias=False, eps=eps, momentum=momentum, affine=affine, 
                                     track_running_stats=track_running_stats)
 
+        # Define the short convolution layer
         self.short_conv = ConvModule(in_channels, hidden_channels, kernel_size, stride, padding, 
                                      bias=False, eps=eps, momentum=momentum, affine=affine, 
                                      track_running_stats=track_running_stats)
 
+        # Define the final convolution layer, which takes in the concatenated output from main_conv 
+        # and short_conv and outputs to the final output layer
         self.final_conv = ConvModule(2 * hidden_channels, out_channels, kernel_size, stride, padding, 
                                      bias=False, eps=eps, momentum=momentum, affine=affine, 
                                      track_running_stats=track_running_stats)
         
+        # Define a list of blocks using the DarknetBottleneck structure
         self.blocks = nn.ModuleList([DarknetBottleneck(hidden_channels, hidden_channels, eps, momentum, affine, track_running_stats, add_identity) for _ in range(num_blocks)])
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
+    def forward(self, x):
         
-        main_path = self.main_conv(x)
+        # Pass the input through the main_conv layer
+        x1 = self.main_conv(x)
+
+        # Pass the input through the short_conv layer
+        x2 = self.short_conv(x)
+
+        # Pass the output of main_conv through each block in the blocks list
         for block in self.blocks:
-            main_path = block(main_path)
+            x1 = block(x1)
 
-        shortcut_path = self.short_conv(x)
+        # Concatenate the outputs of the blocks and the short_conv along dimension 1
+        out = torch.cat((x1, x2), dim=1)
 
-        return self.final_conv(torch.cat((main_path, shortcut_path), dim=1))
+        # Pass the concatenated output through the final_conv layer
+        out = self.final_conv(out)
+
+        # Returning the final output
+        return out
 
 # %% ../nbs/00_model.ipynb 17
 class Focus(nn.Module):
+    
     """
     Focus width and height information into channel space.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/backbones/csp_darknet.py#L14)
+    
+    
+    #### Pseudocode
+    Function forward(input_tensor x):
+
+    1. Split the input tensor x into four patches (patch_top_left, patch_top_right, patch_bot_left, patch_bot_right) based on their spatial positions in the last two dimensions of x.
+    2. Concatenate these four patches along the channel dimension and store the output back into 'x'.
+    3. Pass 'x' through the convolutional layer (self.conv) and store the result as 'out'.
+    4. Return 'out' as the final output.
+
     """
     
     def __init__(self,
                  in_channels: int, # Number of input channels.
                  out_channels: int, # Number of output channels.
                  kernel_size: int = 1, # Size of the convolving kernel.
                  stride: int = 1, # Stride of the convolution.
@@ -267,80 +314,112 @@
                 
         # Split the input tensor into 4 patches
         patch_top_left = x[..., ::2, ::2]   # Top left patch
         patch_top_right = x[..., ::2, 1::2]  # Top right patch
         patch_bot_left = x[..., 1::2, ::2]  # Bottom left patch
         patch_bot_right = x[..., 1::2, 1::2]  # Bottom right patch
         
-        # Concatenate the patches along the channel dimension in order respecting the spatial locality
+        # Concatenate the patches along the channel dimension
         x = torch.cat(
             (
                 patch_top_left,
-                patch_top_right,
                 patch_bot_left,
+                patch_top_right,
                 patch_bot_right,
             ),
             dim=1,
         )
         return self.conv(x)
 
-
 # %% ../nbs/00_model.ipynb 19
 class SPPBottleneck(nn.Module):
     """
     Spatial Pyramid Pooling layer used in YOLOv3-SPP
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/backbones/csp_darknet.py#L67)
+    
+    #### Pseudocode
+    Function forward(input_tensor x):
+
+    1. Pass x through the first convolutional layer (conv1) and assign the output back to x.
+    2. Create an empty list called pooling_results and add x to it.
+    3. For each pooling layer in the poolings list, do the following:
+       a. Apply the pooling layer on x and append the output to the pooling_results list.
+    4. Concatenate all tensors in the pooling_results list along the channel dimension (dimension 1) and assign the output back to x.
+    5. Pass x through the second convolutional layer (conv2) to combine the features from all pooling layers and project them to the desired number of output channels.
+    6. Return the final output tensor.
+
     """
+
     def __init__(self, 
                  in_channels: int, # The number of input channels.
                  out_channels: int, # The number of output channels.
-                 pool_sizes: List[int] = [5, 9, 13], # The sizes of the pooling areas.
-                 eps: float = 0.001, # A value added to the denominator for numerical stability in the BatchNorm layer.
-                 momentum: float = 0.03, #  The value used for the running_mean and running_var computation in the BatchNorm layer.
-                 affine: bool = True, # A flag that when set to True, gives the BatchNorm layer learnable affine parameters.
-                 track_running_stats: bool = True # Whether to keep track of running mean and variance in BatchNorm.
-                ) -> None:
+                 pool_sizes: List[int]=[5, 9, 13], # The sizes of the pooling areas.
+                 eps: float=0.001, # A value added to the denominator for numerical stability in the BatchNorm layer.
+                 momentum: float=0.03, #  The value used for the running_mean and running_var computation in the BatchNorm layer.
+                 affine: bool=True, # A flag that when set to True, gives the BatchNorm layer learnable affine parameters.
+                 track_running_stats: bool=True # Whether to keep track of running mean and variance in BatchNorm.
+                ):
         
         super(SPPBottleneck, self).__init__()
-
+        
+        # Reducing the number of channels by a factor of 2
         hidden_channels = in_channels // 2
 
+        # Convolution layer to reduce the number of channels
         self.conv1 = ConvModule(in_channels, hidden_channels, kernel_size=1, stride=1, padding=0, 
                                 bias=False, eps=eps, momentum=momentum, affine=affine, 
                                 track_running_stats=track_running_stats)
 
-        self.pooling_layers = nn.ModuleList([nn.MaxPool2d(kernel_size=ps, stride=1, padding=ps//2) for ps in pool_sizes])
+        # List of pooling layers with different window sizes
+        self.poolings = nn.ModuleList([nn.MaxPool2d(kernel_size=ps, stride=1, padding=ps//2) for ps in pool_sizes])
 
-        self.conv2 = ConvModule(hidden_channels * (len(pool_sizes) + 1), out_channels, kernel_size=1, stride=1, padding=0, 
+        # Convolution layer to combine the features from the pooling layers and project them to the desired number of output channels
+        self.conv2 = ConvModule(hidden_channels*(len(pool_sizes)+1), out_channels, kernel_size=1, stride=1, padding=0, 
                                 bias=False, eps=eps, momentum=momentum, affine=affine, 
                                 track_running_stats=track_running_stats)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
                 
+        # Reducing the number of channels by a factor of 2 using the convolution layer
         x = self.conv1(x)
 
+        # Applying max pooling with different window sizes and collecting the results
         pooling_results = [x]
-        for pooling in self.pooling_layers:
+        for pooling in self.poolings:
             pooling_results.append(pooling(x))
 
+        # Concatenating the results of pooling along the channel dimension
         x = torch.cat(pooling_results, dim=1)
 
+        # Combining the features and projecting them to the desired number of output channels using the convolution layer
         return self.conv2(x)
 
 # %% ../nbs/00_model.ipynb 21
 class CSPDarknet(nn.Module):
     """
-    The `CSPDarknet` class implements a CSPDarknet backbone, a convolutional neural network (CNN) used in various image recognition tasks. The CSPDarknet backbone forms an integral part of the YOLOX object detection model.
+    CSP-Darknet backbone
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/backbones/csp_darknet.py#L124)
+    
+    #### Pseudocode
+    Function forward(input_tensor x):
+
+    1. Initialize an empty list 'outs' to store intermediate outputs.
+    2. For each index and layer name in the model's layers:
+       a. Retrieve the layer corresponding to the current layer name.
+       b. Pass 'x' through the retrieved layer and update 'x' with the output.
+       c. If the current index is in the set of output indices:
+          i. Append 'x' to 'outs'.
+    3. Convert 'outs' to a tuple and return it as the final output.
+
     """
 
     # Architecture settings for P5 and P6
     ARCH_SETTINGS = {
         'P5': [[64, 128, 3, True, False], [128, 256, 9, True, False],
                [256, 512, 9, True, False], [512, 1024, 3, False, True]],
         'P6': [[64, 128, 3, True, False], [128, 256, 9, True, False],
@@ -433,244 +512,319 @@
         return tuple(outs)
 
 # %% ../nbs/00_model.ipynb 24
 class YOLOXPAFPN(nn.Module):
     """
     Path Aggregation Feature Pyramid Network (PAFPN) used in YOLOX.
     
-    In object detection tasks, this class merges the feature maps from different layers of the backbone network. It helps in aggregating multi-scale feature maps to enhance the detection of objects of various sizes.
-    
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/necks/yolox_pafpn.py#L14)
-    """
     
+    
+    #### Pseudocode
+    Function forward(list inputs):
+
+    1. Assert that the length of inputs equals the length of in_channels.
+    2. Initialize inner_outs with the last feature map in inputs.
+    3. For each index in in_channels in reverse (exclude first):
+       a. Set feature_high to the first feature map in inner_outs.
+       b. Set feature_low to the corresponding input feature map.
+       c. Reduce the channels of feature_high using the corresponding reduce_layer. Update feature_high in inner_outs.
+       d. Upsample feature_high to the spatial size of feature_low.
+       e. Concatenate upsampled feature_high and feature_low, and pass the result through the corresponding CSPLayer. The output is inner_out.
+       f. Add inner_out to the beginning of inner_outs.
+    4. Initialize outs with the first feature map from inner_outs.
+    5. For each index in in_channels (exclude last):
+       a. Set feature_low to the last feature map in outs.
+       b. Set feature_high to the corresponding feature map in inner_outs.
+       c. Downsample feature_low to the spatial size of feature_high.
+       d. Concatenate downsampled feature_low and feature_high, and pass the result through the corresponding CSPLayer. The output is out.
+       e. Add out to the end of outs.
+    6. For each convolutional layer (conv) in out_convs:
+       a. Apply conv to the corresponding feature map in outs.
+    7. Return the tuple of feature maps in outs as the final output.
+    """
     def __init__(self,
-                 in_channels,
-                 out_channels,
-                 num_csp_blocks=3,
-                 upsample_cfg=dict(scale_factor=2, mode='nearest'),
-                 momentum=0.03,
-                 eps=0.001):
+                 in_channels, # The number of input channels for each level of the feature pyramid.
+                 out_channels, # The number of output channels for each level of the feature pyramid.
+                 num_csp_blocks=3, # The number of bottlenecks in each CSPLayer.
+                 upsample_cfg=dict(scale_factor=2, mode='nearest'), # The configuration for the upsampling operation.
+                 momentum=0.03, # The momentum for the batch normalization in the ConvModule.
+                 eps=0.001 # The epsilon for the batch normalization in the ConvModule.
+                ):
         super(YOLOXPAFPN, self).__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
-        self.upsample = nn.Upsample(**upsample_cfg)
 
         # build top-down blocks, which includes reduce layers and CSP blocks
-        self.reduce_layers = nn.ModuleList([
-            ConvModule(
-                in_channels[idx],
-                in_channels[idx - 1],
-                kernel_size=(1, 1),
-                stride=(1, 1),
-                padding=0,
-                bias=False,
-                momentum=momentum,
-                eps=eps,
-                affine=True,
-                track_running_stats=True
-            ) for idx in range(len(in_channels) - 1, 0, -1)
-        ])
-        self.top_down_blocks = nn.ModuleList([
-            CSPLayer(
-                in_channels[idx - 1] * 2,
-                in_channels[idx - 1],
-                num_blocks=num_csp_blocks,
-                add_identity=False
-            ) for idx in range(len(in_channels) - 1, 0, -1)
-        ])
+        self.upsample = nn.Upsample(**upsample_cfg)
+        self.reduce_layers = nn.ModuleList()
+        self.top_down_blocks = nn.ModuleList()
+        for idx in range(len(in_channels) - 1, 0, -1):
+            # add reducing layers for channel-wise feature reduction
+            self.reduce_layers.append(
+                ConvModule(
+                    in_channels[idx],
+                    in_channels[idx - 1],
+                    kernel_size=(1, 1), 
+                    stride=(1, 1),
+                    padding=0,
+                    bias=False,
+                    momentum=momentum,
+                    eps=eps,
+                    affine=True, 
+                    track_running_stats=True
+                ))
+            # add CSP layers for feature learning
+            self.top_down_blocks.append(
+                CSPLayer(
+                    in_channels[idx - 1] * 2,
+                    in_channels[idx - 1],
+                    num_blocks=num_csp_blocks,
+                    add_identity=False))
 
         # build bottom-up blocks, which includes downsampling layers and CSP blocks
-        self.downsamples = nn.ModuleList([
-            ConvModule(
-                in_channels[idx],
-                in_channels[idx],
-                3,
-                stride=2,
-                padding=1,
-                bias=False,
-                momentum=momentum,
-                eps=eps,
-                affine=True,
-                track_running_stats=True
-            ) for idx in range(len(in_channels) - 1)
-        ])
-        self.bottom_up_blocks = nn.ModuleList([
-            CSPLayer(
-                in_channels[idx] * 2,
-                in_channels[idx + 1],
-                num_blocks=num_csp_blocks,
-                add_identity=False
-            ) for idx in range(len(in_channels) - 1)
-        ])
+        self.downsamples = nn.ModuleList()
+        self.bottom_up_blocks = nn.ModuleList()
+        for idx in range(len(in_channels) - 1):
+            # add downsampling layers for spatial reduction
+            self.downsamples.append(
+                ConvModule(
+                    in_channels[idx],
+                    in_channels[idx],
+                    3,
+                    stride=2,
+                    padding=1,
+                    bias=False,
+                    momentum=momentum,
+                    eps=eps,
+                    affine=True, 
+                    track_running_stats=True
+                ))
+            # add CSP layers for feature learning
+            self.bottom_up_blocks.append(
+                CSPLayer(
+                    in_channels[idx] * 2,
+                    in_channels[idx + 1],
+                    num_blocks=num_csp_blocks,
+                    add_identity=False))
 
         # build output convolutions for each level
-        self.out_convs = nn.ModuleList([
-            ConvModule(
-                in_channels[i],
-                out_channels,
-                1,
-                stride=(1, 1),
-                padding=0,
-                bias=False,
-                momentum=momentum,
-                eps=eps,
-                affine=True,
-                track_running_stats=True
-            ) for i in range(len(in_channels))
-        ])
+        self.out_convs = nn.ModuleList()
+        for i in range(len(in_channels)):
+            self.out_convs.append(
+                ConvModule(
+                    in_channels[i],
+                    out_channels,
+                    1,
+                    stride=(1, 1),
+                    padding=0,
+                    bias=False,
+                    momentum=momentum,
+                    eps=eps,
+                    affine=True, 
+                    track_running_stats=True))
 
     def forward(self, inputs):
+        
         assert len(inputs) == len(self.in_channels)
 
         # top-down path
-        inner_outs = self._top_down(inputs)
+        inner_outs = [inputs[-1]]
+        for idx in range(len(self.in_channels) - 1, 0, -1):
+            feat_heigh = inner_outs[0]
+            feat_low = inputs[idx - 1]
+            # reduce the channel dimension of the higher feature map
+            feat_heigh = self.reduce_layers[len(self.in_channels) - 1 - idx](feat_heigh)
+            inner_outs[0] = feat_heigh
+
+            # upsample the higher feature map to the same spatial size as the lower one
+            upsample_feat = self.upsample(feat_heigh)
+
+            # concatenate the upsampled higher feature map and the lower one, and feed them into the CSPLayer
+            inner_out = self.top_down_blocks[len(self.in_channels) - 1 - idx](
+                torch.cat([upsample_feat, feat_low], 1))
+            # collect the output feature maps
+            inner_outs.insert(0, inner_out)
 
         # bottom-up path
-        outs = self._bottom_up(inner_outs)
+        outs = [inner_outs[0]]
+        for idx in range(len(self.in_channels) - 1):
+            feat_low = outs[-1]
+            feat_height = inner_outs[idx + 1]
+            # downsample the lower feature map to the same spatial size as the higher one
+            downsample_feat = self.downsamples[idx](feat_low)
+            # concatenate the downsampled lower feature map and the higher one, and feed them into the CSPLayer
+            out = self.bottom_up_blocks[idx](
+                torch.cat([downsample_feat, feat_height], 1))
+            # collect the output feature maps
+            outs.append(out)
 
         # apply the output convolutions to the feature maps
-        outs = [conv(out) for out, conv in zip(outs, self.out_convs)]
+        for idx, conv in enumerate(self.out_convs):
+            outs[idx] = conv(outs[idx])
 
         return tuple(outs)
 
-    def _top_down(self, inputs):
-        inner_outs = [inputs[-1]]
-        for idx, (reduce_layer, block) in enumerate(zip(self.reduce_layers, self.top_down_blocks)):
-            feat_high = reduce_layer(inner_outs[0])
-            inner_outs[0] = feat_high
-            upsample_feat = self.upsample(feat_high)
-            inner_out = block(torch.cat([upsample_feat, inputs[len(inputs) - 2 - idx]], 1))
-            inner_outs.insert(0, inner_out)
-        return inner_outs
-
-    def _bottom_up(self, inner_outs):
-        outs = [inner_outs[0]]
-        for idx, (downsample, block) in enumerate(zip(self.downsamples, self.bottom_up_blocks)):
-            downsample_feat = downsample(outs[-1])
-            out = block(torch.cat([downsample_feat, inner_outs[idx + 1]], 1))
-            outs.append(out)
-        return outs
-
 # %% ../nbs/00_model.ipynb 27
 class YOLOXHead(nn.Module):
     """
-    The `YOLOXHead` class is a PyTorch module that implements the head of a YOLOX model <https://arxiv.org/abs/2107.08430>, used for bounding box prediction.
-    
-    The head takes as input feature maps at multiple scale levels (e.g., from a feature pyramid network) and outputs predicted class scores, bounding box coordinates, and objectness scores for each scale level.
+    The head of YOLOX model <https://arxiv.org/abs/2107.08430>, used for bounding box prediction.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/models/dense_heads/yolox_head.py#L20)
-    """
     
+    #### Pseudocode
+    Function forward(feats):
+
+    1. For each scale level in feats, perform the following steps:
+        a. Pass the scale level feature through the classification convolutions (cls_convs) to produce a feature map (cls_feat).
+        b. Pass the same scale level feature through the regression convolutions (reg_convs) to produce another feature map (reg_feat).
+        c. Apply the classification predictor convolution (conv_cls) on the classification feature map (cls_feat) to get the classification scores (cls_score).
+        d. Apply the regression predictor convolution (conv_reg) on the regression feature map (reg_feat) to get bounding box predictions (bbox_pred).
+        e. Apply the objectness predictor convolution (conv_obj) on the regression feature map (reg_feat) to get objectness scores (objectness).
+    2. Collect the classification scores, bounding box predictions, and objectness scores for each scale level and store them in a tuple.
+    3. Return the tuple as the final output.
+
+    """
+
     BBOX_DIM = 4
     OBJECTNESS_DIM = 1
 
     def __init__(self,
                  num_classes:int, # The number of target classes.
                  in_channels:int, # The number of input channels.
                  feat_channels=256, # The number of feature channels.
                  stacked_convs=2, # The number of convolution layers to stack.
                  strides=[8, 16, 32], # The stride of each scale level in the feature pyramid.
                  momentum=0.03, # The momentum for the moving average in batch normalization.
                  eps=0.001 # The epsilon to avoid division by zero in batch normalization.
                 ):
 
         super().__init__()
-        # Store various configurations as instance variables
         self.num_classes = num_classes
         self.cls_out_channels = num_classes
         self.in_channels = in_channels
         self.feat_channels = feat_channels
         self.stacked_convs = stacked_convs
         self.strides = strides
         self.momentum = momentum
         self.eps = eps
-        
-        # Initialize the layers of the model
-        self._init_layers()
+        self._init_layers()  # initialize layers
 
     def _init_layers(self):
         """
         Initialize layers for the head module, includes classification 
         convolutions, regression convolutions and prediction convolutions 
         for each scale level.
         """
-        # Initialize multi-level lists for each type of layer
         self.multi_level_cls_convs = nn.ModuleList()
         self.multi_level_reg_convs = nn.ModuleList()
         self.multi_level_conv_cls = nn.ModuleList()
         self.multi_level_conv_reg = nn.ModuleList()
         self.multi_level_conv_obj = nn.ModuleList()
-        
-        # For each stride level, create layers and add them to their respective lists
         for _ in self.strides:
             self.multi_level_cls_convs.append(self._build_stacked_convs())
             self.multi_level_reg_convs.append(self._build_stacked_convs())
             conv_cls, conv_reg, conv_obj = self._build_predictor()
             self.multi_level_conv_cls.append(conv_cls)
             self.multi_level_conv_reg.append(conv_reg)
             self.multi_level_conv_obj.append(conv_obj)
 
     def _build_stacked_convs(self):
         """
         Build stacked convolution layers.
+
+        Returns
+        -------
+        nn.Sequential
+            A sequential container of stacked conv layers.
         """
         conv = ConvModule
         stacked_convs = []
-        # Create a series of convolution layers
         for i in range(self.stacked_convs):
             chn = self.in_channels if i == 0 else self.feat_channels
             stacked_convs.append(
                 conv(
                     chn,
                     self.feat_channels,
                     3,
                     stride=1,
                     padding=1,
                     momentum=self.momentum,
                     eps=self.eps,
                     affine=True, 
                     track_running_stats=True,
                     bias=False))
-        # Return the layers as a sequential model
         return nn.Sequential(*stacked_convs)
 
     def _build_predictor(self):
         """
         Build predictor layers for classification, regression, and objectness.
+
+        Returns
+        -------
+        tuple
+            The classification, regression, and objectness convolutional layers.
         """
-        # Create convolution layers for each type of prediction
         conv_cls = nn.Conv2d(self.feat_channels, self.cls_out_channels, 1)
         conv_reg = nn.Conv2d(self.feat_channels, self.BBOX_DIM, 1)
         conv_obj = nn.Conv2d(self.feat_channels, self.OBJECTNESS_DIM, 1)
         return conv_cls, conv_reg, conv_obj
 
-    def forward_single(self, x, cls_convs, reg_convs, conv_cls, conv_reg, conv_obj):
+    def forward_single(self, x, cls_convs, reg_convs, conv_cls, conv_reg,
+                       conv_obj):
         """
         Forward feature of a single scale level.
+
+        Parameters
+        ----------
+        x : tensor
+            The input tensor.
+        cls_convs : nn.Module
+            The classification convolutions.
+        reg_convs : nn.Module
+            The regression convolutions.
+        conv_cls : nn.Module
+            The classification predictor convolution.
+        conv_reg : nn.Module
+            The regression predictor convolution.
+        conv_obj : nn.Module
+            The objectness predictor convolution.
+
+        Returns
+        -------
+        tuple
+            The classification scores, bounding box predictions, and objectness.
         """
-        # Pass input through classification and regression convolutions
         cls_feat = cls_convs(x)
         reg_feat = reg_convs(x)
 
-        # Apply predictors to get scores and predictions
         cls_score = conv_cls(cls_feat)
         bbox_pred = conv_reg(reg_feat)
         objectness = conv_obj(reg_feat)
 
         return cls_score, bbox_pred, objectness
 
     def forward(self, feats):
         """
         Forward pass for the head.
+
+        Parameters
+        ----------
+        feats : list
+            A list of multi-level features.
+
+        Returns
+        -------
+        tuple
+            The results of applying the forward_single function to each scale level.
         """
-        # Apply the forward_single function to each scale level
         return multi_apply(self.forward_single, feats,
                            self.multi_level_cls_convs,
                            self.multi_level_reg_convs,
                            self.multi_level_conv_cls,
                            self.multi_level_conv_reg,
                            self.multi_level_conv_obj)
 
@@ -710,14 +864,38 @@
 
         # Forward through bbox_head
         x = self.bbox_head(x)
 
         return x
 
 # %% ../nbs/00_model.ipynb 33
+def kaiming_init(model:torch.nn.Module # The model to be initialized.
+                ) -> None:
+    """
+    Initializes the weights of the Conv2d layers of the given model using the [Kaiming Normal initialization](https://pytorch.org/docs/stable/nn.init.html#torch.nn.init.kaiming_normal_).
+    """
+    
+    # Iterating through each module in the model
+    for module in model.modules():
+
+        # If the module is a 2d convolutional layer
+        if isinstance(module, nn.Conv2d):
+            
+            # Apply Kaiming Normal initialization to the weights of the module
+            # We use 'fan_out' mode as this preserves the magnitude of the variance of the weights
+            # in the forward pass. The nonlinearity is set to 'relu' as the network uses ReLU activation functions.
+            nn.init.kaiming_normal_(module.weight, mode='fan_out', nonlinearity='relu')
+            
+            # If the module has a bias term
+            if module.bias is not None:
+                
+                # Initialize the bias term to 0 for this module
+                nn.init.constant_(module.bias, 0)
+
+# %% ../nbs/00_model.ipynb 37
 def init_head(head: YOLOXHead, # The YOLOX head to be initialized.
               num_classes: int # The number of classes in the dataset.
              ) -> None:
     """
     Initialize the `YOLOXHead` with appropriate class outputs and convolution layers.
 
     This function configures the output channels in the YOLOX head to match the
@@ -727,27 +905,22 @@
 
     # Set the number of output channels in the head to be equal to the number of classes
     head.cls_out_channels = num_classes
 
     # Create a list of 2D convolutional layers, one for each stride in the head.
     # Each convolutional layer will have a number of output channels equal to the number of classes
     # and a kernel size of 1 (i.e., it will perform a 1x1 convolution).
+    head.multi_level_conv_cls = nn.ModuleList(
+        [nn.Conv2d(head.feat_channels, head.cls_out_channels, 1) for _ in head.strides]
+    )
     
-    conv_layers = [nn.Conv2d(head.feat_channels, head.cls_out_channels, 1) for _ in head.strides]
-    
-    for conv in conv_layers:
-        # Use Kaiming initialization to initialize the weights of the convolutional layers. 
-        init.kaiming_normal_(conv.weight.data, mode='fan_out', nonlinearity='relu')
-    
-    head.multi_level_conv_cls = nn.ModuleList(conv_layers)
+    # Use Kaiming initialization to initialize the weights of the convolutional layers. 
+    kaiming_init(head.multi_level_conv_cls)
 
-# %% ../nbs/00_model.ipynb 37
-from cjm_psl_utils.core import download_file
-
-# %% ../nbs/00_model.ipynb 38
+# %% ../nbs/00_model.ipynb 41
 def build_model(model_type:str, # Type of the model to be built.
                 num_classes:int, # Number of classes for the model.
                 pretrained:bool=True, # Whether to load pretrained weights.
                 checkpoint_dir:str='./pretrained_checkpoints/' # Directory to store checkpoints.
                ) -> YOLOX: # The built YOLOX model.
     """
     Builds a YOLOX model based on the given parameters.
@@ -758,35 +931,33 @@
     backbone_cfg = CSP_DARKNET_CFGS[model_type]
     neck_cfg = PAFPN_CFGS[model_type]
     head_cfg = HEAD_CFGS[model_type]
     
     backbone = CSPDarknet(**backbone_cfg)
     neck = YOLOXPAFPN(**neck_cfg)
 
-    if pretrained and PRETRAINED_URLS[model_type] == None:
-        print("The selected model type does not have a pretrained checkpoint. Initializing model with untrained weights.")
-        pretrained = False
-    
     try:
         if pretrained:
             url = PRETRAINED_URLS[model_type]
             checkpoint_path = os.path.join(checkpoint_dir, Path(url).name)
-            download_file(url, checkpoint_dir)
+            download_file(url, checkpoint_path)
             
             pretrained_ckpt = torch.load(checkpoint_path)['state_dict']
             num_pretrained_classes = pretrained_ckpt['bbox_head.multi_level_conv_cls.0.weight'].shape[0]
             
             head = YOLOXHead(num_classes=num_pretrained_classes, **head_cfg)
         else:
             head = YOLOXHead(num_classes=num_classes, **head_cfg)
         
         yolox = YOLOX(backbone, neck, head)
         
         if pretrained:
             yolox.load_state_dict(pretrained_ckpt)
             init_head(head, num_classes)
+        else:
+            kaiming_init(yolox)
             
     except Exception as e:
         print(f"Error occurred while building the model: {str(e)}")
         return None
 
     return yolox
```

### Comparing `cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch/simota.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_simota.ipynb.
 
 # %% auto 0
 __all__ = ['AssignResult', 'SimOTAAssigner']
 
 # %% ../nbs/03_simota.ipynb 4
-from dataclasses import dataclass, field
 from typing import Any, Type, List, Optional, Callable, Tuple, Union
 from functools import partial
 
 # %% ../nbs/03_simota.ipynb 5
 import torch
 import torch.nn.functional as F
 import torchvision
 
 # %% ../nbs/03_simota.ipynb 7
-@dataclass
-class AssignResult:
+class AssignResult():
     """
     Stores assignments between predicted bounding boxes and actual truth bounding boxes.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/assigners/assign_result.py#L7)
 
     """
-    num_ground_truth_boxes: int # The number of actual truth boxes considered when computing this assignment
-    ground_truth_box_indices: torch.LongTensor # For each predicted bounding box, this indicates the 1-based index of the assigned actual truth box. 0 means unassigned and -1 means ignore.
-    max_iou_values: torch.FloatTensor # The Intersection over Union (IoU) between the predicted bounding box and its assigned actual truth box.
-    category_labels: torch.LongTensor = field(default=None) # If specified, for each predicted bounding box, this indicates the category label of the assigned actual truth box.
+
+    def __init__(self, 
+                 num_ground_truth_boxes:int, # The number of actual truth boxes considered when computing this assignment
+                 ground_truth_box_indices:torch.LongTensor, # For each predicted bounding box, this indicates the 1-based index of the assigned actual truth box. 0 means unassigned and -1 means ignore.
+                 max_iou_values:torch.FloatTensor, # The Intersection over Union (IoU) between the predicted bounding box and its assigned actual truth box.
+                 category_labels:torch.LongTensor=None # If specified, for each predicted bounding box, this indicates the category label of the assigned actual truth box.
+                ):
+        self.num_ground_truth_boxes = num_ground_truth_boxes
+        self.ground_truth_box_indices = ground_truth_box_indices
+        self.max_iou_values = max_iou_values
+        self.category_labels = category_labels
 
 # %% ../nbs/03_simota.ipynb 9
 class SimOTAAssigner():
     """
     Computes matching between predictions and ground truth.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/assigners/sim_ota_assigner.py#L14)
     
     
     #### Pseudocode
 
     1. Receive as input: predicted_scores, priors, decoded_bounding_boxes, ground_truth_bounding_boxes, and ground_truth_labels. These are all tensors.
-    2. Initialize a large value for HIGH_COST_VALUE.
+    2. Initialize a large value for INF.
     3. Calculate the number of ground truth bounding boxes and predicted bounding boxes.
     4. Create a tensor `assigned_gt_inds` with the same size as the number of predicted bounding boxes and fill it with zeros. 
     5. If there are no ground truth bounding boxes or predicted bounding boxes, return an `AssignResult` with no assignments.
     6. If there are no ground truth bounding boxes, assign all predicted bounding boxes to the background.
     7. Calculate which priors are within a ground truth bounding box and which priors are in the center of a ground truth bounding box.
     8. Extract the valid decoded bounding boxes and valid predicted scores, i.e., those that are inside a ground truth bounding box and at the center.
     9. Compute the IoU between valid bounding boxes and ground truth bounding boxes. 
@@ -54,15 +59,15 @@
     10. Convert the ground truth labels to one-hot format and calculate the classification cost using the valid predicted scores and one-hot ground truth labels.
     11. Calculate the total cost matrix by adding up the classification cost, the IoU cost and, if not within a ground truth bounding box and at the center, a high cost.
     12. Use the dynamic_k_matching method on the cost matrix to perform a dynamic matching between the ground truth bounding boxes and valid bounding boxes.
         - Obtain the matched ground truth indices and IoU scores.
     13. Update the `assigned_gt_inds` with the matched ground truth indices.
     14. Create a tensor `assigned_labels` of the same size as `assigned_gt_inds`, and fill it with -1.
         - Update `assigned_labels` with the labels of the matched ground truth boxes.
-    15. Create a tensor `max_overlaps` of the same size as `assigned_gt_inds`, and fill it with -HIGH_COST_VALUE.
+    15. Create a tensor `max_overlaps` of the same size as `assigned_gt_inds`, and fill it with -INF.
         - Update `max_overlaps` with the IoU scores of the matched ground truth boxes.
     16. Return an instance of `AssignResult` with the number of ground truth boxes, the `assigned_gt_inds`, `max_overlaps`, and `assigned_labels`.
     
     """
 
     def __init__(self,
                  center_radius:float=2.5, # Ground truth center size to judge whether a prior is in center.
@@ -106,15 +111,15 @@
                 stability. Default 1e-7.
 
         Returns:
             :obj:`AssignResult`: The assigned result. This includes information about the index 
                 of the ground truth box each prediction is assigned to, the IoU between the 
                 predictions and their assigned ground truth, and the category labels for each prediction.
         """
-        HIGH_COST_VALUE = 100000000
+        INF = 100000000
         num_gt = gt_bboxes.size(0)
         num_bboxes = decoded_bboxes.size(0)
 
         # assign 0 by default
         assigned_gt_inds = decoded_bboxes.new_full((num_bboxes, ), 0, dtype=torch.long)
         if num_gt == 0 or num_bboxes == 0:
             # No ground truth or boxes, return empty assignment
@@ -143,123 +148,83 @@
 
         # Convert gt_labels to one-hot format and calculate classification cost
         gt_onehot_label = F.one_hot(gt_labels.to(torch.int64), pred_scores.shape[-1]).float().unsqueeze(0).repeat(num_valid, 1, 1)
         valid_pred_scores = valid_pred_scores.unsqueeze(1).repeat(1, num_gt, 1)
         cls_cost = F.binary_cross_entropy(valid_pred_scores.sqrt_(), gt_onehot_label, reduction='none').sum(-1)
 
         # Calculate total cost matrix by combining classification and IoU costs, 
-        # and assign a high cost (HIGH_COST_VALUE) for bboxes not in both boxes and centers
-        cost_matrix = cls_cost * self.cls_weight + iou_cost * self.iou_weight + (~is_in_boxes_and_center) * HIGH_COST_VALUE
+        # and assign a high cost (INF) for bboxes not in both boxes and centers
+        cost_matrix = cls_cost * self.cls_weight + iou_cost * self.iou_weight + (~is_in_boxes_and_center) * INF
 
         # Perform matching between ground truth and valid bounding boxes based on the cost matrix
         matched_pred_ious, matched_gt_inds = self.dynamic_k_matching(cost_matrix, pairwise_ious, num_gt, valid_mask)
 
         # Convert to AssignResult format: assign matched gt indices, labels and IoU scores
         assigned_gt_inds[valid_mask] = matched_gt_inds + 1
         assigned_labels = assigned_gt_inds.new_full((num_bboxes, ), -1)
         assigned_labels[valid_mask] = gt_labels[matched_gt_inds].long()
-        max_overlaps = assigned_gt_inds.new_full((num_bboxes, ), -HIGH_COST_VALUE, dtype=torch.float32)
+        max_overlaps = assigned_gt_inds.new_full((num_bboxes, ), -INF, dtype=torch.float32)
         max_overlaps[valid_mask] = matched_pred_ious
         return AssignResult(num_gt, assigned_gt_inds, max_overlaps, category_labels=assigned_labels)
 
-#     def get_in_gt_and_in_center_info(self, priors, gt_bboxes):
-#         """Get the information about whether priors are in ground truth boxes or center.
-
-#         Args:
-#             priors (Tensor): All priors of one image, a 2D-Tensor with shape [num_priors, 4]
-#                 in [cx, xy, stride_w, stride_y] format.
-#             gt_bboxes (Tensor): Ground truth bboxes of one image, a 2D-Tensor
-#                 with shape [num_gts, 4] in [tl_x, tl_y, br_x, br_y] format.
-
-#         Returns:
-#             Tuple[Tensor, Tensor]: The first tensor indicates if the prior is in any ground truth box or center, 
-#             the second tensor specifies if the prior is in both the ground truth box and center.
-#         """
-
-#         # Calculate the centers of the ground truth boxes
-#         gt_cxs = (gt_bboxes[:, 0] + gt_bboxes[:, 2]) / 2.0
-#         gt_cys = (gt_bboxes[:, 1] + gt_bboxes[:, 3]) / 2.0
-
-#         # Calculate the boundaries for the ground truth boxes
-#         gt_bounds = torch.stack([
-#             priors[:, 0, None] - gt_bboxes[:, 0], 
-#             priors[:, 1, None] - gt_bboxes[:, 1], 
-#             gt_bboxes[:, 2] - priors[:, 0, None], 
-#             gt_bboxes[:, 3] - priors[:, 1, None]
-#         ], dim=1)
-
-#         # Check if priors are inside the ground truth boxes
-#         is_in_gts = gt_bounds.min(dim=1).values > 0
-#         is_in_gts_all = is_in_gts.any(dim=1)
-
-#         # Prepare the boundaries for the center boxes
-#         ct_bounds = torch.stack([
-#             priors[:, 0, None] - (gt_cxs - self.center_radius * priors[:, 2, None]),
-#             priors[:, 1, None] - (gt_cys - self.center_radius * priors[:, 3, None]),
-#             (gt_cxs + self.center_radius * priors[:, 2, None]) - priors[:, 0, None],
-#             (gt_cys + self.center_radius * priors[:, 3, None]) - priors[:, 1, None]
-#         ], dim=1)
-
-#         # Check if priors are inside the center boxes
-#         is_in_cts = ct_bounds.min(dim=1).values > 0
-#         is_in_cts_all = is_in_cts.any(dim=1)
-
-#         # Check if priors are in either any ground truth box or any center box
-#         is_in_gts_or_centers = is_in_gts_all | is_in_cts_all
-
-#         # Check if priors are in both ground truth boxes and centers
-#         is_in_boxes_and_centers = is_in_gts[is_in_gts_or_centers, :] & is_in_cts[is_in_gts_or_centers, :]
-
-#         return is_in_gts_or_centers, is_in_boxes_and_centers
-    
-    
     def get_in_gt_and_in_center_info(self, priors, gt_bboxes):
         """Get the information about whether priors are in ground truth boxes or center.
 
         Args:
             priors (Tensor): All priors of one image, a 2D-Tensor with shape [num_priors, 4]
                 in [cx, xy, stride_w, stride_y] format.
             gt_bboxes (Tensor): Ground truth bboxes of one image, a 2D-Tensor
                 with shape [num_gts, 4] in [tl_x, tl_y, br_x, br_y] format.
 
         Returns:
             Tuple[Tensor, Tensor]: The first tensor indicates if the prior is in any ground truth box or center, 
             the second tensor specifies if the prior is in both the ground truth box and center.
         """
 
+        # Repeat the prior values across the new dimension to facilitate the calculations
+        repeated_x = priors[:, 0, None]
+        repeated_y = priors[:, 1, None]
+        repeated_stride_x = priors[:, 2, None]
+        repeated_stride_y = priors[:, 3, None]
+
+        # Calculate deltas (distances from priors to the boundaries of the ground truth boxes)
+        deltas = torch.stack([
+            repeated_x - gt_bboxes[:, 0], 
+            repeated_y - gt_bboxes[:, 1], 
+            gt_bboxes[:, 2] - repeated_x, 
+            gt_bboxes[:, 3] - repeated_y], dim=1)
+
+        # Check if any value of deltas is positive, which means the prior is within the ground truth box
+        is_in_gts = deltas.min(dim=1).values > 0
+        # Check if a prior is in any ground truth box
+        is_in_gts_all = is_in_gts.any(dim=1)
+
         # Calculate the centers of the ground truth boxes
         gt_cxs = (gt_bboxes[:, 0] + gt_bboxes[:, 2]) / 2.0
         gt_cys = (gt_bboxes[:, 1] + gt_bboxes[:, 3]) / 2.0
 
-        # Prepare the boundaries for both the ground truth boxes and the center boxes
-        bounds = torch.stack([
-            priors[:, 0, None] - gt_bboxes[:, 0], 
-            priors[:, 1, None] - gt_bboxes[:, 1], 
-            gt_bboxes[:, 2] - priors[:, 0, None], 
-            gt_bboxes[:, 3] - priors[:, 1, None],
-            priors[:, 0, None] - (gt_cxs - self.center_radius * priors[:, 2, None]),
-            priors[:, 1, None] - (gt_cys - self.center_radius * priors[:, 3, None]),
-            (gt_cxs + self.center_radius * priors[:, 2, None]) - priors[:, 0, None],
-            (gt_cys + self.center_radius * priors[:, 3, None]) - priors[:, 1, None]
-        ], dim=1)
-
-        # Check if priors are inside the boxes or centers
-        is_in_bounds = bounds.min(dim=1).values > 0
-        is_in_gts_or_centers = is_in_bounds.any(dim=1)
-
-        # Check if priors are in both ground truth boxes and centers
-        is_in_gts = is_in_bounds[:, :4].any(dim=1)
-        is_in_cts = is_in_bounds[:, 4:].any(dim=1)
-        is_in_boxes_and_centers = is_in_gts & is_in_cts
-        is_in_boxes_and_centers = is_in_boxes_and_centers[is_in_gts_or_centers]
+        # Calculate deltas for center boxes (distances from priors to the boundaries of the center boxes)
+        ct_deltas = torch.stack([
+            repeated_x - (gt_cxs - self.center_radius * repeated_stride_x),
+            repeated_y - (gt_cys - self.center_radius * repeated_stride_y),
+            (gt_cxs + self.center_radius * repeated_stride_x) - repeated_x,
+            (gt_cys + self.center_radius * repeated_stride_y) - repeated_y], dim=1)
+
+        # Check if any value of ct_deltas is positive, which means the prior is within the center box
+        is_in_cts = ct_deltas.min(dim=1).values > 0
+        # Check if a prior is in any center box
+        is_in_cts_all = is_in_cts.any(dim=1)
+
+        # Check if a prior is in either any ground truth box or any center box
+        is_in_gts_or_centers = is_in_gts_all | is_in_cts_all
+        # Check if a prior is in both any ground truth box and any center box
+        is_in_boxes_and_centers = (is_in_gts[is_in_gts_or_centers, :] & is_in_cts[is_in_gts_or_centers, :])
 
         return is_in_gts_or_centers, is_in_boxes_and_centers
-
-
-
+    
     def dynamic_k_matching(self, cost, pairwise_ious, num_gt, valid_mask):
         """
         This method performs dynamic k-matching. This is a core part of the SimOTA assignment
         where each ground truth object dynamically chooses k bounding box predictions that best 
         match itself according to the cost matrix. Then, if there are any conflicts (i.e., one 
         prediction is selected by multiple ground truths), the conflicts are resolved by choosing 
         the pair with the smallest cost.
@@ -273,15 +238,14 @@
             valid_mask (Tensor): A 1D tensor representing which predicted boxes are valid based 
                 on being in gt bboxes and in centers. Shape is [num_priors].
 
         Returns:
             matched_pred_ious (Tensor): IoU scores for matched pairs. Shape is [num_priors].
             matched_gt_inds (Tensor): The indices of the ground truth for each prior. Shape is [num_priors].
         """
-
         # Initialize the matching matrix with zeros
         matching_matrix = torch.zeros_like(cost)
 
         # Select the top k IoUs for dynamic-k calculation
         topk_ious, _ = torch.topk(pairwise_ious, self.candidate_topk, dim=0)
 
         # Calculate dynamic k for each ground truth
@@ -292,15 +256,15 @@
         for gt_idx in range(num_gt):
             matching_matrix[pos_idx[:dynamic_ks[gt_idx], gt_idx], gt_idx] = 1
 
         # If a prior matches multiple ground truths, keep only the one with smallest cost
         prior_match_gt_mask = matching_matrix.sum(1) > 1
         if prior_match_gt_mask.any():
             _, cost_argmin = cost[prior_match_gt_mask].min(dim=1)
-            matching_matrix[prior_match_gt_mask].zero_()
+            matching_matrix[prior_match_gt_mask] *= 0
             matching_matrix[prior_match_gt_mask, cost_argmin] = 1
 
         # Update the valid mask based on final matches
         valid_mask[valid_mask.clone()] = matching_matrix.sum(1) > 0
 
         # Get the final matched ground truth indices and IoUs for valid predicted boxes
         fg_mask_inboxes = matching_matrix.sum(1) > 0
```

### Comparing `cjm-yolox-pytorch-0.0.86/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.9/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.86
+Version: 0.0.9
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.86/settings.ini` & `cjm-yolox-pytorch-0.0.9/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.86
+version = 0.0.9
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
@@ -34,10 +34,10 @@
 description = A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 keywords = nbdev jupyter notebook python torch
 language = English
 status = 3
 user = cj-mills
 
 ### Optional ###
-requirements = torch numpy torchvision cjm_psl_utils
+requirements = torch numpy torchvision
 # dev_requirements = 
 # console_scripts =
```

### Comparing `cjm-yolox-pytorch-0.0.86/setup.py` & `cjm-yolox-pytorch-0.0.9/setup.py`

 * *Files identical despite different names*

