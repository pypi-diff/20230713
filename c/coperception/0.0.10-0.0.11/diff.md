# Comparing `tmp/coperception-0.0.10.tar.gz` & `tmp/coperception-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coperception-0.0.10.tar", last modified: Sat Jul  9 18:59:23 2022, max compression
+gzip compressed data, was "dist\coperception-0.0.11.tar", last modified: Thu Jul 13 05:10:19 2023, max compression
```

## Comparing `coperception-0.0.10.tar` & `coperception-0.0.11.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    11549 2022-05-06 23:48:53.000000 coperception-0.0.10/LICENSE
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      907 2022-07-09 18:59:23.000000 coperception-0.0.10/PKG-INFO
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     3321 2022-07-09 18:43:16.000000 coperception-0.0.10/README.md
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       94 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/configs/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     7009 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/configs/Config.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     6239 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/configs/ConfigGlobal.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       68 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/configs/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/datasets/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    10990 2022-05-07 01:30:33.000000 coperception-0.0.10/coperception/datasets/NuscenesDataset.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    16032 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/datasets/V2XSimDet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     9095 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/datasets/V2XSimSeg.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      114 2022-05-07 01:30:33.000000 coperception-0.0.10/coperception/datasets/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/models/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       17 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/models/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/models/det/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     2715 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/AgentWiseWeightedFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     1285 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/CatFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     6181 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/DiscoNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     1373 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/FaFNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      574 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/MaxFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      486 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/MeanFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      567 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/SumFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      482 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/TeacherNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     4221 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/V2VNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    16032 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/When2com.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      356 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/models/det/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/models/det/backbone/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    14197 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/backbone/Backbone.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       32 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/models/det/backbone/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/models/det/base/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    12152 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/base/DetModelBase.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     2572 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/base/FusionBase.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      814 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/base/IntermediateModelBase.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      719 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/det/base/NonIntermediateModelBase.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      198 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/models/det/base/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/models/seg/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     3026 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/AgentWiseWeightedFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     1163 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/CatFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     4516 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/DiscoNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     2911 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/FusionBase.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      451 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/MaxFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      446 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/MeanFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     5161 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/SegModelBase.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      444 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/SumFusion.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     1156 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/UNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     3552 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/V2VNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    19290 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/models/seg/When2Com_UNet.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      402 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/models/seg/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/utils/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      639 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/AverageMeter.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    33304 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/utils/CoDetModule.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     2392 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/SegMetrics.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     6464 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/SegModule.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       57 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/__init__.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception/utils/convolutional_rnn/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      862 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/convolutional_rnn/__init__.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    11970 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/convolutional_rnn/functional.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    36180 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/convolutional_rnn/module.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      358 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/convolutional_rnn/utils.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    52024 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/utils/data_util.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    41909 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/utils/detection_util.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    20050 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/loss.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)   150776 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/mapping.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      346 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/mapping.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    16063 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/utils/mean_ap.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     9008 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/min_norm_solvers.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    18076 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/utils/nuscenes_pc_util.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)    33229 2022-05-06 23:48:53.000000 coperception-0.0.10/coperception/utils/obj_util.py
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     9182 2022-07-09 15:11:09.000000 coperception-0.0.10/coperception/utils/postprocess.py
-drwxr-xr-x   0 dekunma   (1000) dekunma   (1000)        0 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception.egg-info/
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      907 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception.egg-info/PKG-INFO
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)     2440 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception.egg-info/SOURCES.txt
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)        1 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception.egg-info/dependency_links.txt
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      127 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception.egg-info/requires.txt
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       13 2022-07-09 18:59:23.000000 coperception-0.0.10/coperception.egg-info/top_level.txt
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)      170 2022-05-06 23:48:53.000000 coperception-0.0.10/pyproject.toml
--rw-r--r--   0 dekunma   (1000) dekunma   (1000)       38 2022-07-09 18:59:23.000000 coperception-0.0.10/setup.cfg
--rwxr-xr-x   0 dekunma   (1000) dekunma   (1000)     2076 2022-07-09 15:11:09.000000 coperception-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:19.000000 coperception-0.0.11/
+-rw-rw-rw-   0        0        0    11549 2023-07-13 04:51:22.000000 coperception-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0      895 2023-07-13 05:10:19.000000 coperception-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     4776 2023-07-13 04:53:19.000000 coperception-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/
+-rw-rw-rw-   0        0        0       94 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/configs/
+-rw-rw-rw-   0        0        0     6953 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/configs/Config.py
+-rw-rw-rw-   0        0        0     6239 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/configs/ConfigGlobal.py
+-rw-rw-rw-   0        0        0       68 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/datasets/
+-rw-rw-rw-   0        0        0    10990 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/datasets/NuscenesDataset.py
+-rw-rw-rw-   0        0        0    16032 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/datasets/V2XSimDet.py
+-rw-rw-rw-   0        0        0     9145 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/datasets/V2XSimSeg.py
+-rw-rw-rw-   0        0        0      114 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/models/
+-rw-rw-rw-   0        0        0       17 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/models/det/
+-rw-rw-rw-   0        0        0     2715 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/AgentWiseWeightedFusion.py
+-rw-rw-rw-   0        0        0     1285 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/CatFusion.py
+-rw-rw-rw-   0        0        0     6181 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/DiscoNet.py
+-rw-rw-rw-   0        0        0     1373 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/FaFNet.py
+-rw-rw-rw-   0        0        0      574 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/MaxFusion.py
+-rw-rw-rw-   0        0        0      486 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/MeanFusion.py
+-rw-rw-rw-   0        0        0      567 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/SumFusion.py
+-rw-rw-rw-   0        0        0      482 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/TeacherNet.py
+-rw-rw-rw-   0        0        0     4221 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/V2VNet.py
+-rw-rw-rw-   0        0        0    16032 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/When2com.py
+-rw-rw-rw-   0        0        0      356 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/models/det/backbone/
+-rw-rw-rw-   0        0        0    14197 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/backbone/Backbone.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/backbone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception/models/det/base/
+-rw-rw-rw-   0        0        0    12152 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/base/DetModelBase.py
+-rw-rw-rw-   0        0        0     2572 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/base/FusionBase.py
+-rw-rw-rw-   0        0        0      814 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/base/IntermediateModelBase.py
+-rw-rw-rw-   0        0        0      719 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/base/NonIntermediateModelBase.py
+-rw-rw-rw-   0        0        0      198 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/det/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:19.000000 coperception-0.0.11/coperception/models/seg/
+-rw-rw-rw-   0        0        0     3026 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/AgentWiseWeightedFusion.py
+-rw-rw-rw-   0        0        0     1163 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/CatFusion.py
+-rw-rw-rw-   0        0        0     2513 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/DiscoNet.py
+-rw-rw-rw-   0        0        0     2911 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/FusionBase.py
+-rw-rw-rw-   0        0        0      451 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/MaxFusion.py
+-rw-rw-rw-   0        0        0      446 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/MeanFusion.py
+-rw-rw-rw-   0        0        0     5161 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/SegModelBase.py
+-rw-rw-rw-   0        0        0      444 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/SumFusion.py
+-rw-rw-rw-   0        0        0     1156 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/UNet.py
+-rw-rw-rw-   0        0        0     3552 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/V2VNet.py
+-rw-rw-rw-   0        0        0    19290 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/When2Com_UNet.py
+-rw-rw-rw-   0        0        0      402 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/models/seg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:19.000000 coperception-0.0.11/coperception/utils/
+-rw-rw-rw-   0        0        0      639 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/AverageMeter.py
+-rw-rw-rw-   0        0        0    33304 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/CoDetModule.py
+-rw-rw-rw-   0        0        0     2392 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/SegMetrics.py
+-rw-rw-rw-   0        0        0     6464 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/SegModule.py
+-rw-rw-rw-   0        0        0       85 2023-07-13 05:02:13.000000 coperception-0.0.11/coperception/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:19.000000 coperception-0.0.11/coperception/utils/convolutional_rnn/
+-rw-rw-rw-   0        0        0      862 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/convolutional_rnn/__init__.py
+-rw-rw-rw-   0        0        0    11970 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/convolutional_rnn/functional.py
+-rw-rw-rw-   0        0        0    36180 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/convolutional_rnn/module.py
+-rw-rw-rw-   0        0        0      358 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/convolutional_rnn/utils.py
+-rw-rw-rw-   0        0        0    52024 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/data_util.py
+-rw-rw-rw-   0        0        0    41909 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/detection_util.py
+-rw-rw-rw-   0        0        0    20050 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/loss.py
+-rw-rw-rw-   0        0        0    16063 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/mean_ap.py
+-rw-rw-rw-   0        0        0     9008 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/min_norm_solvers.py
+-rw-rw-rw-   0        0        0    18076 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/nuscenes_pc_util.py
+-rw-rw-rw-   0        0        0    33229 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/obj_util.py
+-rw-rw-rw-   0        0        0     9182 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/postprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:19.000000 coperception-0.0.11/coperception/utils/v2x_sim_scene_split/
+-rw-rw-rw-   0        0        0       15 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/v2x_sim_scene_split/__init__.py
+-rw-rw-rw-   0        0        0      454 2023-07-13 04:51:22.000000 coperception-0.0.11/coperception/utils/v2x_sim_scene_split/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception.egg-info/
+-rw-rw-rw-   0        0        0      895 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2451 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 05:10:18.000000 coperception-0.0.11/coperception.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      170 2023-07-13 04:51:22.000000 coperception-0.0.11/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 05:10:19.000000 coperception-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0     2076 2023-07-13 05:09:34.000000 coperception-0.0.11/setup.py
```

### Comparing `coperception-0.0.10/LICENSE` & `coperception-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/PKG-INFO` & `coperception-0.0.11/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-Metadata-Version: 2.1
-Name: coperception
-Version: 0.0.10
-Summary: A library for collaborative perception.
-Home-page: https://ai4ce.github.io/
-Download-URL: https://github.com/coperception/coperception/archive/refs/tags/v0.0.1-alpha.tar.gz
-Author: AI4CE Lab @NYU
-Author-email: dm4524@nyu.edu
-License: apache-2.0
-Keywords: computer-vision,deep-learning,autonomous-driving,collaborative-learning,knowledge-distillation,communication-networks,multi-agent-learning,multi-agent-system,3d-object-detection,graph-learning,point-cloud-processing,v2x-communication,multi-agent-perception,3d-scene-understanding
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: coperception
+Version: 0.0.11
+Summary: A library for collaborative perception.
+Home-page: https://ai4ce.github.io/
+Download-URL: https://github.com/coperception/coperception/archive/refs/tags/v0.0.1-alpha.tar.gz
+Author: AI4CE Lab @NYU
+Author-email: dm4524@nyu.edu
+License: apache-2.0
+Keywords: computer-vision,deep-learning,autonomous-driving,collaborative-learning,knowledge-distillation,communication-networks,multi-agent-learning,multi-agent-system,3d-object-detection,graph-learning,point-cloud-processing,v2x-communication,multi-agent-perception,3d-scene-understanding
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
```

### Comparing `coperception-0.0.10/coperception/configs/Config.py` & `coperception-0.0.11/coperception/configs/Config.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     def __init__(
         self,
         split,
         binary=True,
         only_det=True,
         code_type="faf",
         loss_type="faf_loss",
-        savepath="",
         root="",
         is_cross_road=False,
         use_vis=False,
     ):
         # for segmentaion task only
         # =========================
         self.num_class = 8
@@ -62,15 +61,14 @@
             6: "Pedestrian",
             7: "Vegetation",
         }
         # =========================
 
         self.device = None
         self.split = split
-        self.savepath = savepath
         self.binary = binary
         self.only_det = only_det
         self.code_type = code_type
         self.loss_type = loss_type  # corner_loss faf_loss
 
         # The specifications for BEV maps
         self.voxel_size = (0.25, 0.25, 0.4)
```

### Comparing `coperception-0.0.10/coperception/configs/ConfigGlobal.py` & `coperception-0.0.11/coperception/configs/ConfigGlobal.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/datasets/NuscenesDataset.py` & `coperception-0.0.11/coperception/datasets/NuscenesDataset.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/datasets/V2XSimDet.py` & `coperception-0.0.11/coperception/datasets/V2XSimDet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/datasets/V2XSimSeg.py` & `coperception-0.0.11/coperception/datasets/V2XSimSeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         if idx in self.cache[agent_id]:
             gt_dict = self.cache[agent_id][idx]
         else:
             seq_file = self.seq_files[agent_id][idx]
             gt_data_handle = np.load(seq_file, allow_pickle=True)
             if gt_data_handle == 0:
                 empty_flag = True
-                if self.com != 'lowerbound' and self.com != 'upperbound':
+                if self.com != 'lowerbound' and self.com != 'upperbound' and self.bound != 'both':
                     return (
                         torch.zeros((256, 256, 13)).bool(),
                         torch.zeros((256, 256, 13)).bool(),
                         torch.zeros((256, 256)).int(),
                         torch.zeros((self.num_agent, 4, 4)),
                         0,
                         0,
@@ -165,15 +165,15 @@
                 indices_teacher[:, 0], indices_teacher[:, 1], indices_teacher[:, 2]
             ] = 1
             curr_voxels_teacher = np.rot90(curr_voxels_teacher, 3)
             padded_voxel_points_teacher.append(curr_voxels_teacher)
             padded_voxel_points_teacher = np.stack(padded_voxel_points_teacher, 0)
             padded_voxel_points_teacher = np.squeeze(padded_voxel_points_teacher, 0)
 
-            if self.com != 'lowerbound' and self.com != 'upperbound':
+            if self.com != 'lowerbound' and self.com != 'upperbound' and self.bound != 'both':
                 if self.rsu:
                     trans_matrices = gt_dict["trans_matrices"]
                 else:
                     trans_matrices = gt_dict["trans_matrices_no_cross_road"]
 
                 target_agent_id = gt_dict["target_agent_id"]
                 num_sensor = gt_dict["num_sensor"]
```

### Comparing `coperception-0.0.10/coperception/models/det/AgentWiseWeightedFusion.py` & `coperception-0.0.11/coperception/models/det/AgentWiseWeightedFusion.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/CatFusion.py` & `coperception-0.0.11/coperception/models/det/CatFusion.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/DiscoNet.py` & `coperception-0.0.11/coperception/models/det/DiscoNet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/FaFNet.py` & `coperception-0.0.11/coperception/models/det/FaFNet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/MaxFusion.py` & `coperception-0.0.11/coperception/models/det/MaxFusion.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/SumFusion.py` & `coperception-0.0.11/coperception/models/det/SumFusion.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/V2VNet.py` & `coperception-0.0.11/coperception/models/det/V2VNet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/When2com.py` & `coperception-0.0.11/coperception/models/det/When2com.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/backbone/Backbone.py` & `coperception-0.0.11/coperception/models/det/backbone/Backbone.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/base/DetModelBase.py` & `coperception-0.0.11/coperception/models/det/base/DetModelBase.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/base/FusionBase.py` & `coperception-0.0.11/coperception/models/det/base/FusionBase.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/base/IntermediateModelBase.py` & `coperception-0.0.11/coperception/models/det/base/IntermediateModelBase.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/det/base/NonIntermediateModelBase.py` & `coperception-0.0.11/coperception/models/det/base/NonIntermediateModelBase.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/AgentWiseWeightedFusion.py` & `coperception-0.0.11/coperception/models/seg/AgentWiseWeightedFusion.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/CatFusion.py` & `coperception-0.0.11/coperception/models/seg/CatFusion.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/FusionBase.py` & `coperception-0.0.11/coperception/models/seg/FusionBase.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/SegModelBase.py` & `coperception-0.0.11/coperception/models/seg/SegModelBase.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/UNet.py` & `coperception-0.0.11/coperception/models/seg/UNet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/V2VNet.py` & `coperception-0.0.11/coperception/models/seg/V2VNet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/models/seg/When2Com_UNet.py` & `coperception-0.0.11/coperception/models/seg/When2Com_UNet.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/AverageMeter.py` & `coperception-0.0.11/coperception/utils/AverageMeter.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/CoDetModule.py` & `coperception-0.0.11/coperception/utils/CoDetModule.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/SegMetrics.py` & `coperception-0.0.11/coperception/utils/SegMetrics.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/SegModule.py` & `coperception-0.0.11/coperception/utils/SegModule.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/convolutional_rnn/__init__.py` & `coperception-0.0.11/coperception/utils/convolutional_rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/convolutional_rnn/functional.py` & `coperception-0.0.11/coperception/utils/convolutional_rnn/functional.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/convolutional_rnn/module.py` & `coperception-0.0.11/coperception/utils/convolutional_rnn/module.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/data_util.py` & `coperception-0.0.11/coperception/utils/data_util.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/detection_util.py` & `coperception-0.0.11/coperception/utils/detection_util.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/loss.py` & `coperception-0.0.11/coperception/utils/loss.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/mean_ap.py` & `coperception-0.0.11/coperception/utils/mean_ap.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/min_norm_solvers.py` & `coperception-0.0.11/coperception/utils/min_norm_solvers.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/nuscenes_pc_util.py` & `coperception-0.0.11/coperception/utils/nuscenes_pc_util.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/obj_util.py` & `coperception-0.0.11/coperception/utils/obj_util.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception/utils/postprocess.py` & `coperception-0.0.11/coperception/utils/postprocess.py`

 * *Files identical despite different names*

### Comparing `coperception-0.0.10/coperception.egg-info/PKG-INFO` & `coperception-0.0.11/coperception.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-Metadata-Version: 2.1
-Name: coperception
-Version: 0.0.10
-Summary: A library for collaborative perception.
-Home-page: https://ai4ce.github.io/
-Download-URL: https://github.com/coperception/coperception/archive/refs/tags/v0.0.1-alpha.tar.gz
-Author: AI4CE Lab @NYU
-Author-email: dm4524@nyu.edu
-License: apache-2.0
-Keywords: computer-vision,deep-learning,autonomous-driving,collaborative-learning,knowledge-distillation,communication-networks,multi-agent-learning,multi-agent-system,3d-object-detection,graph-learning,point-cloud-processing,v2x-communication,multi-agent-perception,3d-scene-understanding
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: coperception
+Version: 0.0.11
+Summary: A library for collaborative perception.
+Home-page: https://ai4ce.github.io/
+Download-URL: https://github.com/coperception/coperception/archive/refs/tags/v0.0.1-alpha.tar.gz
+Author: AI4CE Lab @NYU
+Author-email: dm4524@nyu.edu
+License: apache-2.0
+Keywords: computer-vision,deep-learning,autonomous-driving,collaborative-learning,knowledge-distillation,communication-networks,multi-agent-learning,multi-agent-system,3d-object-detection,graph-learning,point-cloud-processing,v2x-communication,multi-agent-perception,3d-scene-understanding
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
```

### Comparing `coperception-0.0.10/coperception.egg-info/SOURCES.txt` & `coperception-0.0.11/coperception.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 coperception/utils/CoDetModule.py
 coperception/utils/SegMetrics.py
 coperception/utils/SegModule.py
 coperception/utils/__init__.py
 coperception/utils/data_util.py
 coperception/utils/detection_util.py
 coperception/utils/loss.py
-coperception/utils/mapping.cpython-37m-x86_64-linux-gnu.so
-coperception/utils/mapping.py
 coperception/utils/mean_ap.py
 coperception/utils/min_norm_solvers.py
 coperception/utils/nuscenes_pc_util.py
 coperception/utils/obj_util.py
 coperception/utils/postprocess.py
 coperception/utils/convolutional_rnn/__init__.py
 coperception/utils/convolutional_rnn/functional.py
 coperception/utils/convolutional_rnn/module.py
-coperception/utils/convolutional_rnn/utils.py
+coperception/utils/convolutional_rnn/utils.py
+coperception/utils/v2x_sim_scene_split/__init__.py
+coperception/utils/v2x_sim_scene_split/parser.py
```

### Comparing `coperception-0.0.10/setup.py` & `coperception-0.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="coperception",
-    version="0.0.10",
+    version="0.0.11",
     package_data={
         "": ["*.so"],
     },
     packages=setuptools.find_packages(),
     license="apache-2.0",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description="A library for collaborative perception.",
     author="AI4CE Lab @NYU",
```

