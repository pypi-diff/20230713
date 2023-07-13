# Comparing `tmp/cjm-yolox-pytorch-0.0.90.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.90.tar", last modified: Thu Jul 13 18:23:27 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.91.tar", last modified: Thu Jul 13 20:15:23 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.90.tar` & `cjm-yolox-pytorch-0.0.91.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 18:23:27.944970 cjm-yolox-pytorch-0.0.90/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.90/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.90/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 18:23:27.944781 cjm-yolox-pytorch-0.0.90/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-04 21:34:25.000000 cjm-yolox-pytorch-0.0.90/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 18:23:27.941295 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-13 18:23:04.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12403 2023-07-13 18:23:04.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    17314 2023-07-13 18:23:04.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-13 18:23:04.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    14772 2023-07-13 18:23:04.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2614 2023-07-13 18:23:04.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 18:23:27.944353 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 18:23:27.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-13 18:23:27.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-13 18:23:27.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-13 18:23:27.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-13 18:23:27.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-13 18:23:27.000000 cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-13 18:21:54.000000 cjm-yolox-pytorch-0.0.90/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-13 18:23:27.945032 cjm-yolox-pytorch-0.0.90/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.90/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 20:15:23.709344 cjm-yolox-pytorch-0.0.91/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.91/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.91/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 20:15:23.709175 cjm-yolox-pytorch-0.0.91/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-04 21:34:25.000000 cjm-yolox-pytorch-0.0.91/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 20:15:23.706727 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-13 20:14:43.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12406 2023-07-13 20:14:43.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    17563 2023-07-13 20:14:43.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-13 20:14:43.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-13 20:14:43.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2618 2023-07-13 20:14:43.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 20:15:23.708854 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 20:15:23.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-13 20:15:23.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-13 20:15:23.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-13 20:15:23.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-13 20:15:23.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-13 20:15:23.000000 cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-13 20:07:44.000000 cjm-yolox-pytorch-0.0.91/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-13 20:15:23.709396 cjm-yolox-pytorch-0.0.91/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.91/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.90/LICENSE` & `cjm-yolox-pytorch-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.90/PKG-INFO` & `cjm-yolox-pytorch-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.90
+Version: 0.0.91
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.90/README.md` & `cjm-yolox-pytorch-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,10 +94,10 @@
                                                                                                 'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.assign': ( 'simota.html#simotaassigner.assign',
                                                                                               'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.dynamic_k_matching': ( 'simota.html#simotaassigner.dynamic_k_matching',
                                                                                                           'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.get_in_gt_and_in_center_info': ( 'simota.html#simotaassigner.get_in_gt_and_in_center_info',
                                                                                                                     'cjm_yolox_pytorch/simota.py')},
-            'cjm_yolox_pytorch.utils': { 'cjm_yolox_pytorch.utils.generate_grid_priors': ( 'utils.html#generate_grid_priors',
-                                                                                           'cjm_yolox_pytorch/utils.py'),
+            'cjm_yolox_pytorch.utils': { 'cjm_yolox_pytorch.utils.generate_output_grids': ( 'utils.html#generate_output_grids',
+                                                                                            'cjm_yolox_pytorch/utils.py'),
                                          'cjm_yolox_pytorch.utils.multi_apply': ('utils.html#multi_apply', 'cjm_yolox_pytorch/utils.py')}}}
```

### Comparing `cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 import numpy as np
 
 import torch
 import torch.nn.functional as F
 import torchvision
 
 # %% ../nbs/02_loss.ipynb 5
-from .utils import multi_apply, generate_grid_priors
+from .utils import multi_apply, generate_output_grids
 from .simota import AssignResult, SimOTAAssigner
 
 # %% ../nbs/02_loss.ipynb 7
 @dataclass
 class SamplingResult:
     """
     Bounding box sampling result.
     
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/samplers/sampling_result.py#L7)
     """
-    positive_indices: np.array # Indices of the positive samples.
-    negative_indices: np.array # Indices of the negative samples.
-    bboxes: np.array # Array containing all bounding boxes.
+    positive_indices: np.ndarray # Indices of the positive samples.
+    negative_indices: np.ndarray # Indices of the negative samples.
+    bboxes: np.ndarray # Array containing all bounding boxes.
     ground_truth_bboxes: torch.Tensor # Tensor containing all ground truth bounding boxes.
     assignment_result: AssignResult # Object that contains the ground truth indices and labels corresponding to each sample.
-    ground_truth_flags: np.array # Array indicating which samples are ground truth.
+    ground_truth_flags: np.ndarray # Array indicating which samples are ground truth.
 
     def __post_init__(self):
         # Indices of positive and negative samples
         self.positive_bboxes = self.bboxes[self.positive_indices]
         self.negative_bboxes = self.bboxes[self.negative_indices]
         
         # Bounding boxes for positive and negative samples
@@ -65,15 +65,15 @@
 # %% ../nbs/02_loss.ipynb 9
 class YOLOXLoss:
     """
     The callable YOLOXLoss class implements the loss function for training a YOLOX model.
     
     A YOLOXLoss instance takes the, class scores, predicted bounding boxes, objectness scores, ground truth bounding boxes, and ground truth labels. It then goes through the following steps:
 
-    1. Generate prior box coordinates for all anchors.
+    1. Generate box coordinates for the output grids based on the input dimensions and stride values.
     2. Flatten and concatenate class predictions, bounding box predictions, and objectness scores.
     3. Decode box predictions.
     4. Compute targets for each image in the batch.
     5. Concatenate all positive masks, class targets, objectness targets, and bounding box targets.
     6. Compute the bounding box loss, objectness loss, and classification loss, scale them by their respective weights, and normalize them by the total number of samples.
     7. If using L1 loss, concatenate L1 targets, computes the L1 loss, scale it by its weight, and normalize it by the total number of samples.
     8. Return a dictionary containing the computed losses.
@@ -110,28 +110,28 @@
         
         # Initialize the assigner
         self.assigner = SimOTAAssigner(center_radius=2.5)
         
         self.strides = strides
         
         
-    def bbox_decode(self, prior_boxes, predicted_boxes):
+    def bbox_decode(self, output_grid_boxes, predicted_boxes):
         """
         Decodes the predicted bounding boxes based on the prior boxes.
 
         Args:
-            prior_boxes (torch.Tensor): The prior bounding boxes.
+            output_grid_boxes (torch.Tensor): The output grid boxes.
             predicted_boxes (torch.Tensor): The predicted bounding boxes.
 
         Returns:
             torch.Tensor: The decoded bounding boxes.
         """
         # Calculate box centroids (geometric centers) and sizes
-        box_centroids = (predicted_boxes[..., :2] * prior_boxes[:, 2:]) + prior_boxes[:, :2]
-        box_sizes = torch.exp(predicted_boxes[..., 2:]) * prior_boxes[:, 2:]
+        box_centroids = (predicted_boxes[..., :2] * output_grid_boxes[:, 2:]) + output_grid_boxes[:, :2]
+        box_sizes = torch.exp(predicted_boxes[..., 2:]) * output_grid_boxes[:, 2:]
 
         # Calculate corners of bounding boxes
         top_left = box_centroids - box_sizes / 2
         bottom_right = box_centroids + box_sizes / 2
 
         # Stack coordinates to create decoded bounding boxes
         decoded_boxes = torch.cat((top_left, bottom_right), -1)
@@ -157,78 +157,78 @@
             assignment_result.ground_truth_box_indices == 0, as_tuple=False).squeeze(-1).unique()
         ground_truth_flags = bboxes.new_zeros(bboxes.shape[0], dtype=torch.uint8)
         sampling_result = SamplingResult(positive_indices, negative_indices, bboxes, ground_truth_boxes,
                                          assignment_result, ground_truth_flags)
         return sampling_result
 
 
-    def get_l1_target(self, l1_target, ground_truth_boxes, prior_boxes, epsilon=1e-8):
+    def get_l1_target(self, l1_target, ground_truth_boxes, output_grid_boxes, epsilon=1e-8):
         """
         Calculates the L1 target.
 
         Args:
             l1_target (torch.Tensor): The L1 target tensor.
             ground_truth_boxes (torch.Tensor): The ground truth boxes.
-            prior_boxes (torch.Tensor): The prior bounding boxes.
+            output_grid_boxes (torch.Tensor): The output grid boxes.
             epsilon (float, optional): A small value to prevent division by zero. Defaults to 1e-8.
 
         Returns:
             torch.Tensor: The updated L1 target.
         """
         ground_truth_centroid_and_wh = torchvision.ops.box_convert(ground_truth_boxes, 'xyxy', 'cxcywh')
-        l1_target[:, :2] = (ground_truth_centroid_and_wh[:, :2] - prior_boxes[:, :2]) / prior_boxes[:, 2:]
-        l1_target[:, 2:] = torch.log(ground_truth_centroid_and_wh[:, 2:] / prior_boxes[:, 2:] + epsilon)
+        l1_target[:, :2] = (ground_truth_centroid_and_wh[:, :2] - output_grid_boxes[:, :2]) / output_grid_boxes[:, 2:]
+        l1_target[:, 2:] = torch.log(ground_truth_centroid_and_wh[:, 2:] / output_grid_boxes[:, 2:] + epsilon)
         return l1_target
 
 
-    def get_target_single(self, class_preds, objectness_score, prior_boxes, decoded_bboxes,
+    def get_target_single(self, class_preds, objectness_score, output_grid_boxes, decoded_bboxes,
                            ground_truth_bboxes, ground_truth_labels):
         """
         Calculates the targets for a single image.
 
         Args:
             class_preds (torch.Tensor): The predicted class probabilities.
             objectness_score (torch.Tensor): The predicted objectness scores.
-            prior_boxes (torch.Tensor): The prior bounding boxes.
+            output_grid_boxes (torch.Tensor): The output grid boxes.
             decoded_bboxes (torch.Tensor): The decoded bounding boxes.
             ground_truth_bboxes (torch.Tensor): The ground truth boxes.
             ground_truth_labels (torch.Tensor): The ground truth labels.
 
         Returns:
             Tuple: The targets for classification, objectness, bounding boxes, and L1 (if applicable), along with
             the foreground mask and the number of positive samples.
         """
         # Get the number of prior boxes and ground truth labels
-        num_prior_boxes = prior_boxes.size(0)
+        num_output_grid_boxes = output_grid_boxes.size(0)
         num_ground_truths = ground_truth_labels.size(0)
 
         # Match dtype of ground truth bounding boxes to the dtype of decoded bounding boxes
         ground_truth_bboxes = ground_truth_bboxes.to(decoded_bboxes.dtype)
 
         # Check if there are no ground truth labels (objects) in the image
         if num_ground_truths == 0:
             # Initialize targets as zero tensors, and foreground_mask as a boolean tensor with False values
             class_targets = class_preds.new_zeros((0, self.num_classes))
             bbox_targets = class_preds.new_zeros((0, 4))
             l1_targets = class_preds.new_zeros((0, 4))
-            objectness_targets = class_preds.new_zeros((num_prior_boxes, 1))
-            foreground_mask = class_preds.new_zeros(num_prior_boxes).bool()
+            objectness_targets = class_preds.new_zeros((num_output_grid_boxes, 1))
+            foreground_mask = class_preds.new_zeros(num_output_grid_boxes).bool()
             return (foreground_mask, class_targets, objectness_targets, bbox_targets,
                     l1_targets, 0)  # Return zero for num_positive_per_image
 
         # Calculate the offset for the prior boxes
-        offset_prior_boxes = torch.cat([prior_boxes[:, :2] + prior_boxes[:, 2:] * 0.5, prior_boxes[:, 2:]], dim=-1)
+        offset_output_grid_boxes = torch.cat([output_grid_boxes[:, :2] + output_grid_boxes[:, 2:] * 0.5, output_grid_boxes[:, 2:]], dim=-1)
 
         # Assign ground truth objects to prior boxes and get assignment results
         assignment_result = self.assigner.assign(
             class_preds.sigmoid() * objectness_score.unsqueeze(1).sigmoid(),
-            offset_prior_boxes, decoded_bboxes, ground_truth_bboxes, ground_truth_labels)
+            offset_output_grid_boxes, decoded_bboxes, ground_truth_bboxes, ground_truth_labels)
 
         # Use assignment results to sample prior boxes
-        sampling_result = self.sample(assignment_result, prior_boxes, ground_truth_bboxes)
+        sampling_result = self.sample(assignment_result, output_grid_boxes, ground_truth_bboxes)
         
         # Get the indices of positive (object-containing) samples
         positive_indices = sampling_result.positive_indices
         num_positive_per_image = positive_indices.size(0)
 
         # Get the maximum IoU values for the positive samples
         positive_ious = assignment_result.max_iou_values[positive_indices]
@@ -244,15 +244,15 @@
         bbox_targets = sampling_result.positive_ground_truth_bboxes
 
         # Initialize L1 targets as zeros
         l1_targets = class_preds.new_zeros((num_positive_per_image, 4))
 
         # If use_l1 is True, calculate L1 targets
         if self.use_l1:
-            l1_targets = self.get_l1_target(l1_targets, bbox_targets, prior_boxes[positive_indices])
+            l1_targets = self.get_l1_target(l1_targets, bbox_targets, output_grid_boxes[positive_indices])
 
         # Initialize foreground_mask as zeros and set the values at positive_indices to True
         foreground_mask = torch.zeros_like(objectness_score).to(torch.bool)
         foreground_mask[positive_indices] = 1
 
         # Return the computed targets, the foreground mask, and the number of positive samples per image
         return (foreground_mask, class_targets, objectness_targets, bbox_targets, l1_targets, num_positive_per_image)
@@ -277,34 +277,34 @@
         Returns:
             Dict: A dictionary with the classification, bounding box, objectness, and optionally, L1 loss.
         """
         
         # Get the number of images in the batch
         batch_size = class_scores[0].shape[0]
         
-        # Generate prior box coordinates for all anchors.
-        grid_priors = generate_grid_priors(*[s*self.strides[0] for s in class_scores[0].shape[-2:]], self.strides)
-        grid_priors[:, :2] *= grid_priors[:, 2].unsqueeze(1)
-        flatten_prior_boxes = torch.cat([grid_priors, grid_priors[:, 2:].clone()], dim=1)
+        # Generate box coordinates for all grid priors.
+        output_grid_boxes = generate_output_grid_boxes(*[s*self.strides[0] for s in class_scores[0].shape[-2:]], self.strides)
+        output_grid_boxes[:, :2] *= output_grid_boxes[:, 2].unsqueeze(1)
+        flatten_output_grid_boxes = torch.cat([output_grid_boxes, output_grid_boxes[:, 2:].clone()], dim=1)
         
         # Flatten and concatenate class predictions, bounding box predictions, and objectness scores
         flatten_class_preds = self.flatten_and_concat(class_scores, batch_size, self.num_classes)
         flatten_bbox_preds = self.flatten_and_concat(predicted_bboxes, batch_size, 4)
         flatten_objectness_scores = self.flatten_and_concat(objectness_scores, batch_size)
                     
         # Concatenate and decode box predictions
-        flatten_prior_boxes = flatten_prior_boxes.to(flatten_bbox_preds.device)
-        flatten_decoded_bboxes = self.bbox_decode(flatten_prior_boxes, flatten_bbox_preds)
+        flatten_output_grid_boxes = flatten_output_grid_boxes.to(flatten_bbox_preds.device)
+        flatten_decoded_bboxes = self.bbox_decode(flatten_output_grid_boxes, flatten_bbox_preds)
 
         # Compute targets
         (positive_masks, class_targets, objectness_targets, bbox_targets, l1_targets,
          num_positive_images) = multi_apply(
              self.get_target_single, flatten_class_preds.detach(),
              flatten_objectness_scores.detach(),
-             flatten_prior_boxes.unsqueeze(0).repeat(batch_size, 1, 1),
+             flatten_output_grid_boxes.unsqueeze(0).repeat(batch_size, 1, 1),
              flatten_decoded_bboxes.detach(), ground_truth_bboxes, ground_truth_labels)
 
         # Concatenate all positive masks, class targets, objectness targets, and bounding box targets
         positive_masks = torch.cat(positive_masks, 0)
         class_targets = torch.cat(class_targets, 0)
         objectness_targets = torch.cat(objectness_targets, 0)
         bbox_targets = torch.cat(bbox_targets, 0)
```

### Comparing `cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/simota.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     Based on OpenMMLab's implementation in the mmdetection library:
     
     - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/bbox/assigners/sim_ota_assigner.py#L14)
     
     
     #### Pseudocode
 
-    1. Receive as input: predicted_scores, priors, decoded_bounding_boxes, ground_truth_bounding_boxes, and ground_truth_labels. These are all tensors.
+    1. Receive as input: predicted_scores, output_grid_boxes, decoded_bounding_boxes, ground_truth_bounding_boxes, and ground_truth_labels. These are all tensors.
     2. Initialize a large value for HIGH_COST_VALUE.
     3. Calculate the number of ground truth bounding boxes and predicted bounding boxes.
     4. Create a tensor `assigned_gt_inds` with the same size as the number of predicted bounding boxes and fill it with zeros. 
     5. If there are no ground truth bounding boxes or predicted bounding boxes, return an `AssignResult` with no assignments.
     6. If there are no ground truth bounding boxes, assign all predicted bounding boxes to the background.
-    7. Calculate which priors are within a ground truth bounding box and which priors are in the center of a ground truth bounding box.
+    7. Calculate which output_grid_boxes are within a ground truth bounding box and which output_grid_boxes are in the center of a ground truth bounding box.
     8. Extract the valid decoded bounding boxes and valid predicted scores, i.e., those that are inside a ground truth bounding box and at the center.
     9. Compute the IoU between valid bounding boxes and ground truth bounding boxes. 
         - Calculate the IoU cost by taking the negative logarithm of this IoU.
     10. Convert the ground truth labels to one-hot format and calculate the classification cost using the valid predicted scores and one-hot ground truth labels.
     11. Calculate the total cost matrix by adding up the classification cost, the IoU cost and, if not within a ground truth bounding box and at the center, a high cost.
     12. Use the dynamic_k_matching method on the cost matrix to perform a dynamic matching between the ground truth bounding boxes and valid bounding boxes.
         - Obtain the matched ground truth indices and IoU scores.
@@ -61,45 +61,45 @@
     15. Create a tensor `max_overlaps` of the same size as `assigned_gt_inds`, and fill it with -HIGH_COST_VALUE.
         - Update `max_overlaps` with the IoU scores of the matched ground truth boxes.
     16. Return an instance of `AssignResult` with the number of ground truth boxes, the `assigned_gt_inds`, `max_overlaps`, and `assigned_labels`.
     
     """
 
     def __init__(self,
-                 center_radius:float=2.5, # Ground truth center size to judge whether a prior is in center.
+                 center_radius:float=2.5, # Ground truth center size to judge whether a output_grid_box is in center.
                  candidate_topk:int=10, # The candidate top-k which used to get top-k ious to calculate dynamic-k.
                  iou_weight:float=3.0, # The scale factor for regression iou cost.
                  cls_weight:float=1.0 # The scale factor for classification cost.
                 ):
         self.center_radius = center_radius
         self.candidate_topk = candidate_topk
         self.iou_weight = iou_weight
         self.cls_weight = cls_weight
 
     def assign(self,
            pred_scores,
-           priors,
+           output_grid_boxes,
            decoded_bboxes,
            gt_bboxes,
            gt_labels,
            gt_bboxes_ignore=None,
            eps=1e-7):
-        """Assign ground truth to priors using SimOTA (Similarity-Overlap-Training-Assignment).
+        """Assign ground truth to output_grid_boxes using SimOTA (Similarity-Overlap-Training-Assignment).
 
-        This method finds the best assignment of predicted bounding boxes (priors) to 
+        This method finds the best assignment of predicted bounding boxes (output_grid_boxes) to 
         the ground truth bounding boxes (gt) based on a combination of classification and 
         regression (IoU) costs.
 
         Args:
-            pred_scores (Tensor): Classification scores of each prior box across all classes. 
-                It is a 2D-Tensor with shape [num_priors, num_classes].
-            priors (Tensor): Prior bounding boxes of one image in format [cx, xy, stride_w, stride_y].
-                It is a 2D-Tensor with shape [num_priors, 4].
+            pred_scores (Tensor): Classification scores of each output grid box across all classes. 
+                It is a 2D-Tensor with shape [num_output_grid_boxes, num_classes].
+            output_grid_boxes (Tensor): Output grid bounding boxes of one image in format [cx, xy, stride_w, stride_y].
+                It is a 2D-Tensor with shape [num_output_grid_boxes, 4].
             decoded_bboxes (Tensor): Predicted bounding boxes of one image in format [tl_x, tl_y, br_x, br_y].
-                It is a 2D-Tensor with shape [num_priors, 4].
+                It is a 2D-Tensor with shape [num_output_grid_boxes, 4].
             gt_bboxes (Tensor): Ground truth bounding boxes of one image in format [tl_x, tl_y, br_x, br_y].
                 It is a 2D-Tensor with shape [num_gts, 4].
             gt_labels (Tensor): Ground truth labels of one image, 
                 It is a Tensor with shape [num_gts].
             gt_bboxes_ignore (Tensor, optional): Ground truth bounding boxes that are
                 labelled as `ignored`, e.g., crowd boxes in COCO.
             eps (float): A value added to the denominator for numerical
@@ -124,16 +124,16 @@
                 assigned_gt_inds[:] = 0
             if gt_labels is None:
                 assigned_labels = None
             else:
                 assigned_labels = decoded_bboxes.new_full((num_bboxes, ), -1, dtype=torch.long)
             return AssignResult(num_gt, assigned_gt_inds, max_overlaps, category_labels=assigned_labels)
 
-        # Get info whether a prior is in gt bounding box and also the center of gt bounding box
-        valid_mask, is_in_boxes_and_center = self.get_in_gt_and_in_center_info(priors, gt_bboxes)
+        # Get info whether a output_grid_box is in gt bounding box and also the center of gt bounding box
+        valid_mask, is_in_boxes_and_center = self.get_in_gt_and_in_center_info(output_grid_boxes, gt_bboxes)
 
         # Extract valid bounding boxes and scores (i.e., those in ground truth boxes and centers)
         valid_decoded_bbox = decoded_bboxes[valid_mask]
         valid_pred_scores = pred_scores[valid_mask]
         num_valid = valid_decoded_bbox.size(0)
 
         # Compute IoU between valid decoded bounding boxes and gt bounding boxes
@@ -157,106 +157,106 @@
         assigned_gt_inds[valid_mask] = matched_gt_inds + 1
         assigned_labels = assigned_gt_inds.new_full((num_bboxes, ), -1)
         assigned_labels[valid_mask] = gt_labels[matched_gt_inds].long()
         max_overlaps = assigned_gt_inds.new_full((num_bboxes, ), -HIGH_COST_VALUE, dtype=torch.float32)
         max_overlaps[valid_mask] = matched_pred_ious
         return AssignResult(num_gt, assigned_gt_inds, max_overlaps, category_labels=assigned_labels)
 
-    def get_in_gt_and_in_center_info(self, priors, gt_bboxes):
-        """Get the information about whether priors are in ground truth boxes or center.
+    def get_in_gt_and_in_center_info(self, output_grid_boxes, gt_bboxes):
+        """Get the information about whether output_grid_boxes are in ground truth boxes or center.
 
         Args:
-            priors (Tensor): All priors of one image, a 2D-Tensor with shape [num_priors, 4]
+            output_grid_boxes (Tensor): All output_grid_boxes of one image, a 2D-Tensor with shape [num_output_grid_boxes, 4]
                 in [cx, xy, stride_w, stride_y] format.
             gt_bboxes (Tensor): Ground truth bboxes of one image, a 2D-Tensor
                 with shape [num_gts, 4] in [tl_x, tl_y, br_x, br_y] format.
 
         Returns:
-            Tuple[Tensor, Tensor]: The first tensor indicates if the prior is in any ground truth box or center, 
-            the second tensor specifies if the prior is in both the ground truth box and center.
+            Tuple[Tensor, Tensor]: The first tensor indicates if the output_grid_box is in any ground truth box or center, 
+            the second tensor specifies if the output_grid_box is in both the ground truth box and center.
         """
 
         # Calculate the centers of the ground truth boxes
         gt_cxs = (gt_bboxes[:, 0] + gt_bboxes[:, 2]) / 2.0
         gt_cys = (gt_bboxes[:, 1] + gt_bboxes[:, 3]) / 2.0
 
         # Calculate the boundaries for the ground truth boxes
         gt_bounds = torch.stack([
-            priors[:, 0, None] - gt_bboxes[:, 0], 
-            priors[:, 1, None] - gt_bboxes[:, 1], 
-            gt_bboxes[:, 2] - priors[:, 0, None], 
-            gt_bboxes[:, 3] - priors[:, 1, None]
+            output_grid_boxes[:, 0, None] - gt_bboxes[:, 0], 
+            output_grid_boxes[:, 1, None] - gt_bboxes[:, 1], 
+            gt_bboxes[:, 2] - output_grid_boxes[:, 0, None], 
+            gt_bboxes[:, 3] - output_grid_boxes[:, 1, None]
         ], dim=1)
 
-        # Check if priors are inside the ground truth boxes
+        # Check if output_grid_boxes are inside the ground truth boxes
         is_in_gts = gt_bounds.min(dim=1).values > 0
         is_in_gts_all = is_in_gts.any(dim=1)
 
         # Prepare the boundaries for the center boxes
         ct_bounds = torch.stack([
-            priors[:, 0, None] - (gt_cxs - self.center_radius * priors[:, 2, None]),
-            priors[:, 1, None] - (gt_cys - self.center_radius * priors[:, 3, None]),
-            (gt_cxs + self.center_radius * priors[:, 2, None]) - priors[:, 0, None],
-            (gt_cys + self.center_radius * priors[:, 3, None]) - priors[:, 1, None]
+            output_grid_boxes[:, 0, None] - (gt_cxs - self.center_radius * output_grid_boxes[:, 2, None]),
+            output_grid_boxes[:, 1, None] - (gt_cys - self.center_radius * output_grid_boxes[:, 3, None]),
+            (gt_cxs + self.center_radius * output_grid_boxes[:, 2, None]) - output_grid_boxes[:, 0, None],
+            (gt_cys + self.center_radius * output_grid_boxes[:, 3, None]) - output_grid_boxes[:, 1, None]
         ], dim=1)
 
-        # Check if priors are inside the center boxes
+        # Check if output_grid_boxes are inside the center boxes
         is_in_cts = ct_bounds.min(dim=1).values > 0
         is_in_cts_all = is_in_cts.any(dim=1)
 
-        # Check if priors are in either any ground truth box or any center box
+        # Check if output_grid_boxes are in either any ground truth box or any center box
         is_in_gts_or_centers = is_in_gts_all | is_in_cts_all
 
-        # Check if priors are in both ground truth boxes and centers
+        # Check if output_grid_boxes are in both ground truth boxes and centers
         is_in_boxes_and_centers = is_in_gts[is_in_gts_or_centers, :] & is_in_cts[is_in_gts_or_centers, :]
 
         return is_in_gts_or_centers, is_in_boxes_and_centers
     
     def dynamic_k_matching(self, cost, pairwise_ious, num_gt, valid_mask):
         """
         This method performs dynamic k-matching. This is a core part of the SimOTA assignment
         where each ground truth object dynamically chooses k bounding box predictions that best 
         match itself according to the cost matrix. Then, if there are any conflicts (i.e., one 
         prediction is selected by multiple ground truths), the conflicts are resolved by choosing 
         the pair with the smallest cost.
 
         Args:
             cost (Tensor): A 2D tensor representing the cost matrix calculated from both 
-                classification cost and regression IoU cost. Shape is [num_priors, num_gts].
+                classification cost and regression IoU cost. Shape is [num_output_grid_boxes, num_gts].
             pairwise_ious (Tensor): A 2D tensor representing IoU scores between predictions and 
-                ground truths. Shape is [num_priors, num_gts].
+                ground truths. Shape is [num_output_grid_boxes, num_gts].
             num_gt (int): The number of ground truth boxes.
             valid_mask (Tensor): A 1D tensor representing which predicted boxes are valid based 
-                on being in gt bboxes and in centers. Shape is [num_priors].
+                on being in gt bboxes and in centers. Shape is [num_output_grid_boxes].
 
         Returns:
-            matched_pred_ious (Tensor): IoU scores for matched pairs. Shape is [num_priors].
-            matched_gt_inds (Tensor): The indices of the ground truth for each prior. Shape is [num_priors].
+            matched_pred_ious (Tensor): IoU scores for matched pairs. Shape is [num_output_grid_boxes].
+            matched_gt_inds (Tensor): The indices of the ground truth for each output_grid_box. Shape is [num_output_grid_boxes].
         """
 
         # Initialize the matching matrix with zeros
         matching_matrix = torch.zeros_like(cost)
 
         # Select the top k IoUs for dynamic-k calculation
         topk_ious, _ = torch.topk(pairwise_ious, self.candidate_topk, dim=0)
 
         # Calculate dynamic k for each ground truth
         dynamic_ks = topk_ious.sum(0).int().clamp(min=1)
 
-        # For each ground truth, find top k matching priors based on smallest cost
+        # For each ground truth, find top k matching output_grid_boxes based on smallest cost
         _, pos_idx = cost.topk(k=dynamic_ks.max().item(), dim=0, largest=False)
         for gt_idx in range(num_gt):
             matching_matrix[pos_idx[:dynamic_ks[gt_idx], gt_idx], gt_idx] = 1
 
-        # If a prior matches multiple ground truths, keep only the one with smallest cost
-        prior_match_gt_mask = matching_matrix.sum(1) > 1
-        if prior_match_gt_mask.any():
-            _, cost_argmin = cost[prior_match_gt_mask].min(dim=1)
-            matching_matrix[prior_match_gt_mask].zero_()
-            matching_matrix[prior_match_gt_mask, cost_argmin] = 1
+        # If a output_grid_box matches multiple ground truths, keep only the one with smallest cost
+        output_grid_box_match_gt_mask = matching_matrix.sum(1) > 1
+        if output_grid_box_match_gt_mask.any():
+            _, cost_argmin = cost[output_grid_box_match_gt_mask].min(dim=1)
+            matching_matrix[output_grid_box_match_gt_mask].zero_()
+            matching_matrix[output_grid_box_match_gt_mask, cost_argmin] = 1
 
         # Update the valid mask based on final matches
         valid_mask[valid_mask.clone()] = matching_matrix.sum(1) > 0
 
         # Get the final matched ground truth indices and IoUs for valid predicted boxes
         fg_mask_inboxes = matching_matrix.sum(1) > 0
         matched_gt_inds = matching_matrix[fg_mask_inboxes].argmax(1)
```

### Comparing `cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_utils.ipynb.
 
 # %% auto 0
-__all__ = ['multi_apply', 'generate_grid_priors']
+__all__ = ['multi_apply', 'generate_output_grids']
 
 # %% ../nbs/01_utils.ipynb 4
 from pathlib import Path
 
 from typing import Any, Type, List, Optional, Callable, Tuple
 from functools import partial
 
@@ -31,15 +31,15 @@
         map_results = map(pfunc, *args)
         return tuple(map(list, zip(*map_results)))
     except Exception as e:
         print(f"Error occurred: {str(e)}")
         return ()
 
 # %% ../nbs/01_utils.ipynb 10
-def generate_grid_priors(height, width, strides=[8,16,32]):
+def generate_output_grids(height, width, strides=[8,16,32]):
         """
         Generate a tensor containing grid coordinates and strides for a given height and width.
 
         Args:
             height (int): The height of the image.
             width (int): The width of the image.
 
@@ -65,10 +65,10 @@
             # Stack the coordinates along with the stride
             coordinates = torch.stack((g0.flatten(), g1.flatten(), s.flatten()), dim=-1)
 
             # Append to the list
             all_coordinates.append(coordinates)
 
         # Concatenate all tensors in the list along the first dimension
-        grid_priors = torch.cat(all_coordinates, dim=0)
+        output_grids = torch.cat(all_coordinates, dim=0)
 
-        return grid_priors
+        return output_grids
```

### Comparing `cjm-yolox-pytorch-0.0.90/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.91/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.90
+Version: 0.0.91
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.90/settings.ini` & `cjm-yolox-pytorch-0.0.91/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.90
+version = 0.0.91
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.90/setup.py` & `cjm-yolox-pytorch-0.0.91/setup.py`

 * *Files identical despite different names*

