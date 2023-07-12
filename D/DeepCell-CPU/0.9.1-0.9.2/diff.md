# Comparing `tmp/DeepCell-CPU-0.9.1.tar.gz` & `tmp/DeepCell-CPU-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepCell-CPU-0.9.1.tar", last modified: Wed Jun 23 18:32:57 2021, max compression
+gzip compressed data, was "DeepCell-CPU-0.9.2.tar", last modified: Wed Aug 11 19:53:55 2021, max compression
```

## Comparing `DeepCell-CPU-0.9.1.tar` & `DeepCell-CPU-0.9.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.960466 DeepCell-CPU-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.952466 DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12895 2021-06-23 18:32:57.000000 DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2021-06-23 18:32:57.000000 DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-23 18:32:57.000000 DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-06-23 18:32:57.000000 DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-23 18:32:57.000000 DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11639 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12895 2021-06-23 18:32:57.960466 DeepCell-CPU-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10406 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.952466 DeepCell-CPU-0.9.1/deepcell/
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.956466 DeepCell-CPU-0.9.1/deepcell/applications/
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16595 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/application.py
--rw-r--r--   0 runner    (1001) docker     (121)     8761 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/application_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/cell_tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/cell_tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5418 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/cytoplasm_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/cytoplasm_segmentation_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7504 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/label_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3165 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/label_detection_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11279 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/mesmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8907 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/mesmer_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/multiplex_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5930 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/nuclear_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/nuclear_segmentation_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7390 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/scale_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/applications/scale_detection_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.956466 DeepCell-CPU-0.9.1/deepcell/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     5830 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/datasets/cytoplasm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4180 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/datasets/phase.py
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/datasets/tracked.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.956466 DeepCell-CPU-0.9.1/deepcell/image_generators/
--rw-r--r--   0 runner    (1001) docker     (121)    11983 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22206 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/cropping.py
--rw-r--r--   0 runner    (1001) docker     (121)    33547 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/fully_convolutional.py
--rw-r--r--   0 runner    (1001) docker     (121)    99236 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/image_generators_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    30933 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)    12688 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/scale.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    73011 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/semantic.py
--rw-r--r--   0 runner    (1001) docker     (121)    43940 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/image_generators/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.956466 DeepCell-CPU-0.9.1/deepcell/layers/
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22762 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/convolutional_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)     7728 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/convolutional_recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6745 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/location.py
--rw-r--r--   0 runner    (1001) docker     (121)     2774 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/location_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    18332 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/padding.py
--rw-r--r--   0 runner    (1001) docker     (121)     8178 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13966 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9437 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/tensor_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/tensor_product_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5913 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (121)     5259 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/layers/upsample_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13258 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/losses_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.956466 DeepCell-CPU-0.9.1/deepcell/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/model_zoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28692 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/model_zoo/featurenet.py
--rw-r--r--   0 runner    (1001) docker     (121)    20527 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/model_zoo/featurenet_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    22941 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/model_zoo/fpn.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13472 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/model_zoo/panopticnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    15145 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/model_zoo/panopticnet_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8423 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/running.py
--rw-r--r--   0 runner    (1001) docker     (121)     7324 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/running_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)    23250 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/training.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 18:32:57.960466 DeepCell-CPU-0.9.1/deepcell/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18849 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/backbone_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5490 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/backbone_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    20762 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    23301 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/data_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5610 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/export_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4182 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/io_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/misc_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10076 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4842 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/plot_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/tracking_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/train_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3030 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/train_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16579 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/transform_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    20219 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/deepcell/utils/transform_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-23 18:32:57.960466 DeepCell-CPU-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2021-06-23 18:32:56.000000 DeepCell-CPU-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.219977 DeepCell-CPU-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.211977 DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12895 2021-08-11 19:53:55.000000 DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2021-08-11 19:53:55.000000 DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 19:53:55.000000 DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2021-08-11 19:53:55.000000 DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-11 19:53:55.000000 DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11639 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12895 2021-08-11 19:53:55.219977 DeepCell-CPU-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10406 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.211977 DeepCell-CPU-0.9.2/deepcell/
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.211977 DeepCell-CPU-0.9.2/deepcell/applications/
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16595 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/application.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8761 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/application_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5061 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/cell_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/cell_tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5418 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/cytoplasm_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2549 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/cytoplasm_segmentation_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7504 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/label_detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3165 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/label_detection_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11279 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/mesmer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8907 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/mesmer_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1543 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/multiplex_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5930 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/nuclear_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/nuclear_segmentation_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7390 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/scale_detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/applications/scale_detection_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.215978 DeepCell-CPU-0.9.2/deepcell/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)     5830 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5392 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/datasets/cytoplasm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4180 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/datasets/phase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/datasets/tracked.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.215978 DeepCell-CPU-0.9.2/deepcell/image_generators/
+-rw-r--r--   0 runner    (1001) docker     (121)    11983 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22206 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33547 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/fully_convolutional.py
+-rw-r--r--   0 runner    (1001) docker     (121)    99236 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/image_generators_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30933 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12688 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/scale.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    73011 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/semantic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43940 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/image_generators/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.215978 DeepCell-CPU-0.9.2/deepcell/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22762 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/convolutional_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7728 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/convolutional_recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6745 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2774 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/location_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18332 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/padding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8178 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13966 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9437 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/tensor_product.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4188 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/tensor_product_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5913 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5259 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/layers/upsample_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13258 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/losses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2641 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/losses_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.219977 DeepCell-CPU-0.9.2/deepcell/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/model_zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28692 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/model_zoo/featurenet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20527 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/model_zoo/featurenet_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22941 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/model_zoo/fpn.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13472 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/model_zoo/panopticnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15145 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/model_zoo/panopticnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8423 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/running.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7324 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/running_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23250 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/training.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 19:53:55.219977 DeepCell-CPU-0.9.2/deepcell/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18849 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/backbone_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5490 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/backbone_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20762 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23301 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/data_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5610 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/export_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4182 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4593 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/io_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2250 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2220 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/misc_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10076 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4842 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/plot_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/tracking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3757 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3030 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/train_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16579 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20219 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/deepcell/utils/transform_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 19:53:55.219977 DeepCell-CPU-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3404 2021-08-11 19:53:54.000000 DeepCell-CPU-0.9.2/setup.py
```

### Comparing `DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/PKG-INFO` & `DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DeepCell-CPU
-Version: 0.9.1
+Version: 0.9.2
 Summary: Deep learning for single cell image segmentation
 Home-page: https://github.com/vanvalenlab/deepcell-tf
 Author: The Van Valen Lab
 Author-email: vanvalen@caltech.edu
 License: LICENSE
-Download-URL: https://github.com/vanvalenlab/deepcell-tf/tarball/0.9.1
+Download-URL: https://github.com/vanvalenlab/deepcell-tf/tarball/0.9.2
 Description: # ![DeepCell Banner](https://raw.githubusercontent.com/vanvalenlab/deepcell-tf/master/docs/images/DeepCell_tf_Banner.png)
         [![Build Status](https://github.com/vanvalenlab/deepcell-tf/workflows/build/badge.svg)](https://github.com/vanvalenlab/deepcell-tf/actions)
         [![Coverage Status](https://coveralls.io/repos/github/vanvalenlab/deepcell-tf/badge.svg?branch=master)](https://coveralls.io/github/vanvalenlab/deepcell-tf?branch=master)
         [![Documentation Status](https://readthedocs.org/projects/deepcell/badge/?version=master)](https://deepcell.readthedocs.io/en/master/?badge=master)
         [![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/vanvalenlab/deepcell-tf/blob/master/LICENSE)
         [![PyPI version](https://badge.fury.io/py/DeepCell.svg)](https://badge.fury.io/py/deepcell)
         [![Python Versions](https://img.shields.io/pypi/pyversions/deepcell.svg)](https://pypi.org/project/deepcell/)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: DeepCell-CPU Version: 0.9.1 Summary: Deep learning
+Metadata-Version: 2.1 Name: DeepCell-CPU Version: 0.9.2 Summary: Deep learning
 for single cell image segmentation Home-page: https://github.com/vanvalenlab/
 deepcell-tf Author: The Van Valen Lab Author-email: vanvalen@caltech.edu
 License: LICENSE Download-URL: https://github.com/vanvalenlab/deepcell-tf/
-tarball/0.9.1 Description: # ![DeepCell Banner](https://
+tarball/0.9.2 Description: # ![DeepCell Banner](https://
 raw.githubusercontent.com/vanvalenlab/deepcell-tf/master/docs/images/
 DeepCell_tf_Banner.png) [![Build Status](https://github.com/vanvalenlab/
 deepcell-tf/workflows/build/badge.svg)](https://github.com/vanvalenlab/
 deepcell-tf/actions) [![Coverage Status](https://coveralls.io/repos/github/
 vanvalenlab/deepcell-tf/badge.svg?branch=master)](https://coveralls.io/github/
 vanvalenlab/deepcell-tf?branch=master) [![Documentation Status](https://
 readthedocs.org/projects/deepcell/badge/?version=master)](https://
```

### Comparing `DeepCell-CPU-0.9.1/DeepCell_CPU.egg-info/SOURCES.txt` & `DeepCell-CPU-0.9.2/DeepCell_CPU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/LICENSE` & `DeepCell-CPU-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/PKG-INFO` & `DeepCell-CPU-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DeepCell-CPU
-Version: 0.9.1
+Version: 0.9.2
 Summary: Deep learning for single cell image segmentation
 Home-page: https://github.com/vanvalenlab/deepcell-tf
 Author: The Van Valen Lab
 Author-email: vanvalen@caltech.edu
 License: LICENSE
-Download-URL: https://github.com/vanvalenlab/deepcell-tf/tarball/0.9.1
+Download-URL: https://github.com/vanvalenlab/deepcell-tf/tarball/0.9.2
 Description: # ![DeepCell Banner](https://raw.githubusercontent.com/vanvalenlab/deepcell-tf/master/docs/images/DeepCell_tf_Banner.png)
         [![Build Status](https://github.com/vanvalenlab/deepcell-tf/workflows/build/badge.svg)](https://github.com/vanvalenlab/deepcell-tf/actions)
         [![Coverage Status](https://coveralls.io/repos/github/vanvalenlab/deepcell-tf/badge.svg?branch=master)](https://coveralls.io/github/vanvalenlab/deepcell-tf?branch=master)
         [![Documentation Status](https://readthedocs.org/projects/deepcell/badge/?version=master)](https://deepcell.readthedocs.io/en/master/?badge=master)
         [![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/vanvalenlab/deepcell-tf/blob/master/LICENSE)
         [![PyPI version](https://badge.fury.io/py/DeepCell.svg)](https://badge.fury.io/py/deepcell)
         [![Python Versions](https://img.shields.io/pypi/pyversions/deepcell.svg)](https://pypi.org/project/deepcell/)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: DeepCell-CPU Version: 0.9.1 Summary: Deep learning
+Metadata-Version: 2.1 Name: DeepCell-CPU Version: 0.9.2 Summary: Deep learning
 for single cell image segmentation Home-page: https://github.com/vanvalenlab/
 deepcell-tf Author: The Van Valen Lab Author-email: vanvalen@caltech.edu
 License: LICENSE Download-URL: https://github.com/vanvalenlab/deepcell-tf/
-tarball/0.9.1 Description: # ![DeepCell Banner](https://
+tarball/0.9.2 Description: # ![DeepCell Banner](https://
 raw.githubusercontent.com/vanvalenlab/deepcell-tf/master/docs/images/
 DeepCell_tf_Banner.png) [![Build Status](https://github.com/vanvalenlab/
 deepcell-tf/workflows/build/badge.svg)](https://github.com/vanvalenlab/
 deepcell-tf/actions) [![Coverage Status](https://coveralls.io/repos/github/
 vanvalenlab/deepcell-tf/badge.svg?branch=master)](https://coveralls.io/github/
 vanvalenlab/deepcell-tf?branch=master) [![Documentation Status](https://
 readthedocs.org/projects/deepcell/badge/?version=master)](https://
```

### Comparing `DeepCell-CPU-0.9.1/README.md` & `DeepCell-CPU-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/_version.py` & `DeepCell-CPU-0.9.2/deepcell/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 __title__ = 'DeepCell-CPU'
 __description__ = 'Deep learning for single cell image segmentation'
 __url__ = 'https://github.com/vanvalenlab/deepcell-tf'
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __download_url__ = '{}/tarball/{}'.format(__url__, __version__)
 __author__ = 'The Van Valen Lab'
 __author_email__ = 'vanvalen@caltech.edu'
 __license__ = 'LICENSE'
 __copyright__ = 'Copyright 2016-2021 The Van Valen Lab at the ' \
     'California Institute of Technology (Caltech)'
```

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/application.py` & `DeepCell-CPU-0.9.2/deepcell/applications/application.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/application_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/application_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/cell_tracking.py` & `DeepCell-CPU-0.9.2/deepcell/applications/cell_tracking.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/cell_tracking_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/cell_tracking_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/cytoplasm_segmentation.py` & `DeepCell-CPU-0.9.2/deepcell/applications/cytoplasm_segmentation.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/cytoplasm_segmentation_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/cytoplasm_segmentation_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/label_detection.py` & `DeepCell-CPU-0.9.2/deepcell/applications/label_detection.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/label_detection_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/label_detection_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/mesmer.py` & `DeepCell-CPU-0.9.2/deepcell/applications/mesmer.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/mesmer_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/mesmer_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/multiplex_segmentation.py` & `DeepCell-CPU-0.9.2/deepcell/applications/multiplex_segmentation.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/nuclear_segmentation.py` & `DeepCell-CPU-0.9.2/deepcell/applications/nuclear_segmentation.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/nuclear_segmentation_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/nuclear_segmentation_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/scale_detection.py` & `DeepCell-CPU-0.9.2/deepcell/applications/scale_detection.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/applications/scale_detection_test.py` & `DeepCell-CPU-0.9.2/deepcell/applications/scale_detection_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/datasets/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/datasets/cytoplasm.py` & `DeepCell-CPU-0.9.2/deepcell/datasets/cytoplasm.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/datasets/phase.py` & `DeepCell-CPU-0.9.2/deepcell/datasets/phase.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/datasets/tracked.py` & `DeepCell-CPU-0.9.2/deepcell/datasets/tracked.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/cropping.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/cropping.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/fully_convolutional.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/fully_convolutional.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/image_generators_test.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/image_generators_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/sample.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/sample.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/scale.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/scale.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/semantic.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/semantic.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/image_generators/tracking.py` & `DeepCell-CPU-0.9.2/deepcell/image_generators/tracking.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/convolutional_recurrent.py` & `DeepCell-CPU-0.9.2/deepcell/layers/convolutional_recurrent.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/convolutional_recurrent_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/convolutional_recurrent_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/location.py` & `DeepCell-CPU-0.9.2/deepcell/layers/location.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/location_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/location_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/normalization.py` & `DeepCell-CPU-0.9.2/deepcell/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/normalization_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/normalization_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/padding.py` & `DeepCell-CPU-0.9.2/deepcell/layers/padding.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/padding_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/padding_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/pooling.py` & `DeepCell-CPU-0.9.2/deepcell/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/pooling_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/pooling_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/tensor_product.py` & `DeepCell-CPU-0.9.2/deepcell/layers/tensor_product.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/tensor_product_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/tensor_product_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/upsample.py` & `DeepCell-CPU-0.9.2/deepcell/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/layers/upsample_test.py` & `DeepCell-CPU-0.9.2/deepcell/layers/upsample_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/losses.py` & `DeepCell-CPU-0.9.2/deepcell/losses.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/losses_test.py` & `DeepCell-CPU-0.9.2/deepcell/losses_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/metrics.py` & `DeepCell-CPU-0.9.2/deepcell/metrics.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/model_zoo/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/model_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/model_zoo/featurenet.py` & `DeepCell-CPU-0.9.2/deepcell/model_zoo/featurenet.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/model_zoo/featurenet_test.py` & `DeepCell-CPU-0.9.2/deepcell/model_zoo/featurenet_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/model_zoo/fpn.py` & `DeepCell-CPU-0.9.2/deepcell/model_zoo/fpn.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/model_zoo/panopticnet.py` & `DeepCell-CPU-0.9.2/deepcell/model_zoo/panopticnet.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/model_zoo/panopticnet_test.py` & `DeepCell-CPU-0.9.2/deepcell/model_zoo/panopticnet_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/running.py` & `DeepCell-CPU-0.9.2/deepcell/running.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/running_test.py` & `DeepCell-CPU-0.9.2/deepcell/running_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/tracking.py` & `DeepCell-CPU-0.9.2/deepcell/tracking.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/training.py` & `DeepCell-CPU-0.9.2/deepcell/training.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/__init__.py` & `DeepCell-CPU-0.9.2/deepcell/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/backbone_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/backbone_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/backbone_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/backbone_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/data_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/data_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/data_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/export_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/io_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/io_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/io_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/misc_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/misc_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/misc_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/plot_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/plot_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/plot_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/tracking_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/train_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/train_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/transform_utils.py` & `DeepCell-CPU-0.9.2/deepcell/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/deepcell/utils/transform_utils_test.py` & `DeepCell-CPU-0.9.2/deepcell/utils/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `DeepCell-CPU-0.9.1/setup.py` & `DeepCell-CPU-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     long_description=readme,
     long_description_content_type='text/markdown',
     install_requires=[
         'numpy>=1.16.6,<1.20.0',
         'scipy>=1.2.3,<2',
         'scikit-image>=0.14.5',
         'scikit-learn>=0.20.4',
-        'tensorflow-cpu~=2.4.2',
+        'tensorflow-cpu~=2.4.3',
         'jupyter>=1.0.0,<2',
         'opencv-python-headless<5',
         'deepcell-tracking>=0.3.1,<0.4.0',
         'deepcell-toolbox>=0.9.0,<0.10.0'
     ],
     extras_require={
         'tests': [
```

