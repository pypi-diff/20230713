# Comparing `tmp/pypaz-0.2.4.tar.gz` & `tmp/pypaz-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaz-0.2.4.tar", last modified: Sat Jun 10 13:40:05 2023, max compression
+gzip compressed data, was "pypaz-0.2.5.tar", last modified: Thu Jul 13 09:32:54 2023, max compression
```

## Comparing `pypaz-0.2.4.tar` & `pypaz-0.2.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-10 13:39:55.000000 pypaz-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-10 13:40:05.403826 pypaz-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-10 13:39:55.000000 pypaz-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/abstract/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/applications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/camera.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.391826 pypaz-0.2.4/paz/backend/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/SE3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/SO3.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/groups/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/heatmaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/backend/image/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/opencv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/image/tensorflow_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    23479 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/munkres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/backend/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/CMU_poanoptic.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/fat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/fer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/ferplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/human36m.py
--rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/omniglot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/open_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/evaluation/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/classification/protonet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/classification/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.395826 pypaz-0.2.4/paz/models/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/detection/efficientdet/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/efficientdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/efficientdet_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/efficientdet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/haar_cascade.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/ssd300.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/ssd512.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/detection/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/keypoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/detnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/iknet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/keypointnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/keypoint/simplebaselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/pose_estimation/higher_hrnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/models/segmentation/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/optimization/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/keypointnet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/multi_box_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.399826 pypaz-0.2.4/paz/optimization/losses/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/jaccard_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/optimization/losses/segmentation/weighted_reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/paz/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    34146 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    21416 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/pipelines/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/paz/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    18276 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/munkres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/processors/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/paz/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/utils/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-10 13:39:55.000000 pypaz-0.2.4/paz/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:40:05.403826 pypaz-0.2.4/pypaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-10 13:40:05.000000 pypaz-0.2.4/pypaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:40:05.403826 pypaz-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-10 13:39:55.000000 pypaz-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.354881 pypaz-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 09:32:44.000000 pypaz-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-13 09:32:54.354881 pypaz-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-07-13 09:32:44.000000 pypaz-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.338881 pypaz-0.2.5/paz/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.342881 pypaz-0.2.5/paz/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/abstract/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/abstract/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/abstract/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/applications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.342881 pypaz-0.2.5/paz/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28821 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/camera.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.342881 pypaz-0.2.5/paz/backend/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/groups/SE3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/groups/SO3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/groups/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/heatmaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.342881 pypaz-0.2.5/paz/backend/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/image/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/image/opencv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/image/tensorflow_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23479 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/munkres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/backend/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.346881 pypaz-0.2.5/paz/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/CMU_poanoptic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/fer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/ferplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/human36m.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/omniglot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/open_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.346881 pypaz-0.2.5/paz/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/evaluation/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.346881 pypaz-0.2.5/paz/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.346881 pypaz-0.2.5/paz/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/classification/protonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/classification/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.346881 pypaz-0.2.5/paz/models/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.346881 pypaz-0.2.5/paz/models/detection/efficientdet/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/efficientdet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/efficientdet/efficientdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/efficientdet/efficientdet_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/efficientdet/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/efficientdet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/haar_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/ssd300.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/ssd512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/detection/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/models/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/detnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/iknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/keypointnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/keypoint/simplebaselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/models/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/pose_estimation/higher_hrnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/models/segmentation/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/optimization/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/keypointnet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/multi_box_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/optimization/losses/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/segmentation/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/segmentation/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/segmentation/jaccard_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/optimization/losses/segmentation/weighted_reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.350881 pypaz-0.2.5/paz/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34149 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21416 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/pipelines/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.354881 pypaz-0.2.5/paz/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18276 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/munkres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/processors/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.354881 pypaz-0.2.5/paz/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/utils/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-13 09:32:44.000000 pypaz-0.2.5/paz/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:54.354881 pypaz-0.2.5/pypaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-13 09:32:54.000000 pypaz-0.2.5/pypaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-13 09:32:54.000000 pypaz-0.2.5/pypaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:32:54.000000 pypaz-0.2.5/pypaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 09:32:54.000000 pypaz-0.2.5/pypaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 09:32:54.000000 pypaz-0.2.5/pypaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:32:54.354881 pypaz-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-13 09:32:44.000000 pypaz-0.2.5/setup.py
```

### Comparing `pypaz-0.2.4/LICENSE` & `pypaz-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/PKG-INFO` & `pypaz-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypaz
-Version: 0.2.4
+Version: 0.2.5
 Summary: Perception for Autonomous Systems
 Home-page: https://github.com/oarriaga/paz/
 Author: Octavio Arriaga
 Author-email: octavio.arriaga@dfki.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `pypaz-0.2.4/README.md` & `pypaz-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/abstract/loader.py` & `pypaz-0.2.5/paz/abstract/loader.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/abstract/messages.py` & `pypaz-0.2.5/paz/abstract/messages.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/abstract/processor.py` & `pypaz-0.2.5/paz/abstract/processor.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/abstract/sequence.py` & `pypaz-0.2.5/paz/abstract/sequence.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/applications.py` & `pypaz-0.2.5/paz/applications.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/anchors.py` & `pypaz-0.2.5/paz/backend/anchors.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/angles.py` & `pypaz-0.2.5/paz/backend/angles.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/boxes.py` & `pypaz-0.2.5/paz/backend/boxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
             `(num_nms_boxes, 4 + num_classes)` and an array
             of corresponding class labels of shape `(num_nms_boxes, )`.
     """
     decoded_boxes = box_data[:, :4]
     class_predictions = box_data[:, 4:]
     num_classes = class_predictions.shape[1]
     nms_boxes = np.array([], dtype=float).reshape(0, box_data.shape[1])
-    class_labels = np.array([], dtype=np.int)
+    class_labels = np.array([], dtype=int)
     args = (decoded_boxes, class_predictions, epsilon, nms_thresh, top_k)
     for class_arg in range(num_classes):
         nms_boxes, class_labels = _nms_per_class(
             nms_boxes, class_labels, class_arg, *args)
     return nms_boxes, class_labels
```

### Comparing `pypaz-0.2.4/paz/backend/camera.py` & `pypaz-0.2.5/paz/backend/camera.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/groups/SE3.py` & `pypaz-0.2.5/paz/backend/groups/SE3.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/groups/SO3.py` & `pypaz-0.2.5/paz/backend/groups/SO3.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/groups/quaternion.py` & `pypaz-0.2.5/paz/backend/groups/quaternion.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/heatmaps.py` & `pypaz-0.2.5/paz/backend/heatmaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         k: Int. Maximum number of instances to return.
 
     # Returns
         values: Numpy array. Value of heatmaps at top k keypoints
         indices: Numpy array. Indices of top k keypoints.
     """
     num_of_objects, num_of_keypoints = heatmaps.shape[:2]
-    indices = np.zeros((num_of_objects, num_of_keypoints, k), dtype=np.int)
+    indices = np.zeros((num_of_objects, num_of_keypoints, k), dtype=int)
     values = np.zeros((num_of_objects, num_of_keypoints, k))
     for object_arg in range(num_of_objects):
         for keypoint_arg in range(num_of_keypoints):
             top_k_indices = np.argsort(heatmaps[object_arg][keypoint_arg])[-k:]
             top_k_values = heatmaps[object_arg][keypoint_arg][top_k_indices]
             indices[object_arg][keypoint_arg] = top_k_indices
             values[object_arg][keypoint_arg] = top_k_values
```

### Comparing `pypaz-0.2.4/paz/backend/image/draw.py` & `pypaz-0.2.5/paz/backend/image/draw.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/image/image.py` & `pypaz-0.2.5/paz/backend/image/image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/image/opencv_image.py` & `pypaz-0.2.5/paz/backend/image/opencv_image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/image/tensorflow_image.py` & `pypaz-0.2.5/paz/backend/image/tensorflow_image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/keypoints.py` & `pypaz-0.2.5/paz/backend/keypoints.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/munkres.py` & `pypaz-0.2.5/paz/backend/munkres.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/render.py` & `pypaz-0.2.5/paz/backend/render.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/backend/standard.py` & `pypaz-0.2.5/paz/backend/standard.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/CMU_poanoptic.py` & `pypaz-0.2.5/paz/datasets/CMU_poanoptic.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/__init__.py` & `pypaz-0.2.5/paz/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/cityscapes.py` & `pypaz-0.2.5/paz/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/coco.py` & `pypaz-0.2.5/paz/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/fat.py` & `pypaz-0.2.5/paz/datasets/fat.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/fer.py` & `pypaz-0.2.5/paz/datasets/fer.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/ferplus.py` & `pypaz-0.2.5/paz/datasets/ferplus.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/human36m.py` & `pypaz-0.2.5/paz/datasets/human36m.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/omniglot.py` & `pypaz-0.2.5/paz/datasets/omniglot.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/open_images.py` & `pypaz-0.2.5/paz/datasets/open_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.load_class_names()
         self.class_distribution = dict()
         for class_name in self.class_names:
             self.class_distribution[class_name] = 0
 
     def load_class_names(self):
         classes_file = os.path.join(self.path, CLASS_DESCRIPTIONS_FILE)
-        class_data = np.loadtxt(classes_file, delimiter=",", dtype=np.str)
+        class_data = np.loadtxt(classes_file, delimiter=",", dtype=str)
 
         # class ID zero is background
         self.machine_to_arg['background'] = 0
         self.machine_to_human_name['background'] = 'background'
         class_names, class_arg = [], 1
         class_names.append('background')
         for machine_name, human_name in class_data:
```

### Comparing `pypaz-0.2.4/paz/datasets/shapes.py` & `pypaz-0.2.5/paz/datasets/shapes.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/utils.py` & `pypaz-0.2.5/paz/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/datasets/voc.py` & `pypaz-0.2.5/paz/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/evaluation/detection.py` & `pypaz-0.2.5/paz/evaluation/detection.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/__init__.py` & `pypaz-0.2.5/paz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/classification/protonet.py` & `pypaz-0.2.5/paz/models/classification/protonet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/classification/xception.py` & `pypaz-0.2.5/paz/models/classification/xception.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/efficientdet/efficientdet.py` & `pypaz-0.2.5/paz/models/detection/efficientdet/efficientdet.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,18 +72,19 @@
     if ((base_weights == 'VOC') and (head_weights == 'VOC')):
         model_filename = '-'.join([model_name, str(base_weights),
                                    str(head_weights) + '_weights.hdf5'])
     elif ((base_weights == 'COCO') and (head_weights is None)):
         model_filename = '-'.join([model_name, str(base_weights),
                                    str(head_weights) + '_weights.hdf5'])
 
-    weights_path = get_file(model_filename, WEIGHT_PATH + model_filename,
-                            cache_subdir='paz/models')
-    print('Loading %s model weights' % weights_path)
-    model.load_weights(weights_path)
+    if not ((base_weights is None) and (head_weights is None)):
+        weights_path = get_file(model_filename, WEIGHT_PATH + model_filename,
+                                cache_subdir='paz/models')
+        print('Loading %s model weights' % weights_path)
+        model.load_weights(weights_path)
 
     image_shape = image.shape[1:3].as_list()
     model.prior_boxes = build_anchors(
         image_shape, branches, num_scales, aspect_ratios, anchor_scale)
     return model
```

### Comparing `pypaz-0.2.4/paz/models/detection/efficientdet/efficientdet_blocks.py` & `pypaz-0.2.5/paz/models/detection/efficientdet/efficientdet_blocks.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/efficientdet/efficientnet.py` & `pypaz-0.2.5/paz/models/detection/efficientdet/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/efficientdet/layers.py` & `pypaz-0.2.5/paz/models/detection/efficientdet/layers.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/haar_cascade.py` & `pypaz-0.2.5/paz/models/detection/haar_cascade.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/ssd300.py` & `pypaz-0.2.5/paz/models/detection/ssd300.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/ssd512.py` & `pypaz-0.2.5/paz/models/detection/ssd512.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/detection/utils.py` & `pypaz-0.2.5/paz/models/detection/utils.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/keypoint/detnet.py` & `pypaz-0.2.5/paz/models/keypoint/detnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/keypoint/hrnet.py` & `pypaz-0.2.5/paz/models/keypoint/hrnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/keypoint/iknet.py` & `pypaz-0.2.5/paz/models/keypoint/iknet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/keypoint/keypointnet.py` & `pypaz-0.2.5/paz/models/keypoint/keypointnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/keypoint/projector.py` & `pypaz-0.2.5/paz/models/keypoint/projector.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/keypoint/simplebaselines.py` & `pypaz-0.2.5/paz/models/keypoint/simplebaselines.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/layers.py` & `pypaz-0.2.5/paz/models/layers.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/pose_estimation/higher_hrnet.py` & `pypaz-0.2.5/paz/models/pose_estimation/higher_hrnet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/models/segmentation/unet.py` & `pypaz-0.2.5/paz/models/segmentation/unet.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/callbacks.py` & `pypaz-0.2.5/paz/optimization/callbacks.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/losses/keypointnet_loss.py` & `pypaz-0.2.5/paz/optimization/losses/keypointnet_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/losses/multi_box_loss.py` & `pypaz-0.2.5/paz/optimization/losses/multi_box_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/losses/segmentation/dice_loss.py` & `pypaz-0.2.5/paz/optimization/losses/segmentation/dice_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/losses/segmentation/focal_loss.py` & `pypaz-0.2.5/paz/optimization/losses/segmentation/focal_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/losses/segmentation/jaccard_loss.py` & `pypaz-0.2.5/paz/optimization/losses/segmentation/jaccard_loss.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/optimization/losses/segmentation/weighted_reconstruction.py` & `pypaz-0.2.5/paz/optimization/losses/segmentation/weighted_reconstruction.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/__init__.py` & `pypaz-0.2.5/paz/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/angles.py` & `pypaz-0.2.5/paz/pipelines/angles.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/classification.py` & `pypaz-0.2.5/paz/pipelines/classification.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/detection.py` & `pypaz-0.2.5/paz/pipelines/detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # Arguments
         mean: List of three elements used to fill empty image spaces.
     """
     def __init__(self, mean=pr.BGR_IMAGENET_MEAN):
         super(AugmentBoxes, self).__init__()
         self.add(pr.ToImageBoxCoordinates())
         self.add(pr.Expand(mean=mean))
-        self.add(pr.RandomSampleCrop())
+        self.add(pr.RandomSampleCrop(1.0))
         self.add(pr.RandomFlipBoxesLeftRight())
         self.add(pr.ToNormalizedBoxCoordinates())
 
 
 class PreprocessBoxes(SequentialProcessor):
     """Preprocess bounding boxes
```

### Comparing `pypaz-0.2.4/paz/pipelines/heatmaps.py` & `pypaz-0.2.5/paz/pipelines/heatmaps.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/image.py` & `pypaz-0.2.5/paz/pipelines/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """Augments an RGB image by randomly changing contrast, brightness
         saturation and hue.
     """
     def __init__(self):
         super(AugmentImage, self).__init__()
         self.add(pr.RandomContrast())
         self.add(pr.RandomBrightness())
-        self.add(pr.RandomSaturation())
+        self.add(pr.RandomSaturation(0.7))
         self.add(pr.RandomHue())
 
 
 class PreprocessImage(SequentialProcessor):
     """Preprocess RGB image by resizing it to the given ``shape``. If a
     ``mean`` is given it is substracted from image and it not the image gets
     normalized.
```

### Comparing `pypaz-0.2.4/paz/pipelines/keypoints.py` & `pypaz-0.2.5/paz/pipelines/keypoints.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/masks.py` & `pypaz-0.2.5/paz/pipelines/masks.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/pose.py` & `pypaz-0.2.5/paz/pipelines/pose.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/pipelines/renderer.py` & `pypaz-0.2.5/paz/pipelines/renderer.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/__init__.py` & `pypaz-0.2.5/paz/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/angles.py` & `pypaz-0.2.5/paz/processors/angles.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/detection.py` & `pypaz-0.2.5/paz/processors/detection.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/draw.py` & `pypaz-0.2.5/paz/processors/draw.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/geometric.py` & `pypaz-0.2.5/paz/processors/geometric.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/groups.py` & `pypaz-0.2.5/paz/processors/groups.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/heatmaps.py` & `pypaz-0.2.5/paz/processors/heatmaps.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/image.py` & `pypaz-0.2.5/paz/processors/image.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/keypoints.py` & `pypaz-0.2.5/paz/processors/keypoints.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/munkres.py` & `pypaz-0.2.5/paz/processors/munkres.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/pose.py` & `pypaz-0.2.5/paz/processors/pose.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/processors/standard.py` & `pypaz-0.2.5/paz/processors/standard.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/paz/utils/logger.py` & `pypaz-0.2.5/paz/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/pypaz.egg-info/PKG-INFO` & `pypaz-0.2.5/pypaz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypaz
-Version: 0.2.4
+Version: 0.2.5
 Summary: Perception for Autonomous Systems
 Home-page: https://github.com/oarriaga/paz/
 Author: Octavio Arriaga
 Author-email: octavio.arriaga@dfki.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `pypaz-0.2.4/pypaz.egg-info/SOURCES.txt` & `pypaz-0.2.5/pypaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypaz-0.2.4/setup.py` & `pypaz-0.2.5/setup.py`

 * *Files identical despite different names*

