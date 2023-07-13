# Comparing `tmp/pykale-0.1.1.tar.gz` & `tmp/pykale-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pykale/pykale/dist/tmpe1rmbq96/pykale-0.1.1.tar", last modified: Sun Aug 21 21:17:53 2022, max compression
+gzip compressed data, was "pykale-0.1.2.tar", last modified: Thu Jul 13 11:38:42 2023, max compression
```

## Comparing `pykale-0.1.1.tar` & `pykale-0.1.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2022-08-21 21:17:40.000000 pykale-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     9962 2022-08-21 21:17:53.000000 pykale-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8657 2022-08-21 21:17:40.000000 pykale-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/action_dann/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/action_dann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3111 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/action_dann/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     4471 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/action_dann/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     4263 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/action_dann/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     2648 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/action_dann/test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/bindingdb_deepdta/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/bindingdb_deepdta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1602 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/bindingdb_deepdta/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2357 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/bindingdb_deepdta/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/bindingdb_deepdta/model.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/cifar_cnntransformer/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_cnntransformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2441 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_cnntransformer/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2407 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_cnntransformer/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     3155 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_cnntransformer/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     4709 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_cnntransformer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/cifar_isonet/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_isonet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2009 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_isonet/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_isonet/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     2477 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_isonet/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     5950 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cifar_isonet/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/cmri_mpca/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cmri_mpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2383 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cmri_mpca/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     7046 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/cmri_mpca/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/digits_dann/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/digits_dann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2408 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/digits_dann/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     3015 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/digits_dann/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     3659 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/digits_dann/model.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/landmark_uncertainty_qbin/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/landmark_uncertainty_qbin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/multisite_neuroimg_adapt/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/multisite_neuroimg_adapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1457 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/multisite_neuroimg_adapt/config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/office_multisource_adapt/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/office_multisource_adapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2654 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/office_multisource_adapt/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     3300 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/office_multisource_adapt/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     2942 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/office_multisource_adapt/model.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/polypharmacy_gripnet/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/polypharmacy_gripnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1485 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/polypharmacy_gripnet/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2503 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/polypharmacy_gripnet/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     2704 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/polypharmacy_gripnet/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     5771 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/polypharmacy_gripnet/trainer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3523 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/polypharmacy_gripnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/examples/toy_domain_adaptation/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/toy_domain_adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3112 2022-08-21 21:17:40.000000 pykale-0.1.1/examples/toy_domain_adaptation/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/embed/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6713 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/attention_cnn.py
--rw-r--r--   0 runner    (1001) docker     (116)    16963 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/factorization.py
--rw-r--r--   0 runner    (1001) docker     (116)     9936 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/gcn.py
--rw-r--r--   0 runner    (1001) docker     (116)    23709 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/gripnet.py
--rw-r--r--   0 runner    (1001) docker     (116)    10481 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/image_cnn.py
--rw-r--r--   0 runner    (1001) docker     (116)     2016 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     3304 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/seq_nn.py
--rw-r--r--   0 runner    (1001) docker     (116)     5307 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/video_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (116)    19368 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/video_i3d.py
--rw-r--r--   0 runner    (1001) docker     (116)    16133 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/video_res3d.py
--rw-r--r--   0 runner    (1001) docker     (116)    13501 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/video_se_i3d.py
--rw-r--r--   0 runner    (1001) docker     (116)    13619 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/video_se_res3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     6505 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/embed/video_selayer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/evaluate/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      680 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/evaluate/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/interpret/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1273 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/interpret/model_weights.py
--rw-r--r--   0 runner    (1001) docker     (116)     7319 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/interpret/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/loaddata/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3096 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/dataset_access.py
--rw-r--r--   0 runner    (1001) docker     (116)    17847 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/image_access.py
--rw-r--r--   0 runner    (1001) docker     (116)     5735 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/mnistm.py
--rw-r--r--   0 runner    (1001) docker     (116)    27118 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/multi_domain.py
--rw-r--r--   0 runner    (1001) docker     (116)    12769 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/sampler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1952 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/tdc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     3984 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/usps.py
--rw-r--r--   0 runner    (1001) docker     (116)    13525 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/video_access.py
--rw-r--r--   0 runner    (1001) docker     (116)     5731 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)    11775 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/video_multi_domain.py
--rw-r--r--   0 runner    (1001) docker     (116)    11476 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/loaddata/videos.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/pipeline/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4248 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/pipeline/deepdta.py
--rw-r--r--   0 runner    (1001) docker     (116)    42734 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/pipeline/domain_adapter.py
--rw-r--r--   0 runner    (1001) docker     (116)     8614 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/pipeline/mpca_trainer.py
--rw-r--r--   0 runner    (1001) docker     (116)    17937 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/pipeline/multi_domain_adapter.py
--rw-r--r--   0 runner    (1001) docker     (116)    29966 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/pipeline/video_domain_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/predict/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7219 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/predict/class_domain_nets.py
--rw-r--r--   0 runner    (1001) docker     (116)     1118 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/predict/decode.py
--rw-r--r--   0 runner    (1001) docker     (116)    13422 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/predict/isonet.py
--rw-r--r--   0 runner    (1001) docker     (116)    10553 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/predict/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/prepdata/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/prepdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3762 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/prepdata/chem_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)     7385 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/prepdata/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)    10814 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/prepdata/supergraph_construct.py
--rw-r--r--   0 runner    (1001) docker     (116)     2738 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/prepdata/tensor_reshape.py
--rw-r--r--   0 runner    (1001) docker     (116)     5030 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/prepdata/video_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/kale/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4346 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (116)     1374 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)      668 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (116)     1382 2022-08-21 21:17:40.000000 pykale-0.1.1/kale/utils/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/pykale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9962 2022-08-21 21:17:53.000000 pykale-0.1.1/pykale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3275 2022-08-21 21:17:53.000000 pykale-0.1.1/pykale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-21 21:17:53.000000 pykale-0.1.1/pykale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      866 2022-08-21 21:17:53.000000 pykale-0.1.1/pykale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2022-08-21 21:17:53.000000 pykale-0.1.1/pykale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      464 2022-08-21 21:17:40.000000 pykale-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      572 2022-08-21 21:17:53.000000 pykale-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4563 2022-08-21 21:17:40.000000 pykale-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:53.000000 pykale-0.1.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-21 21:17:40.000000 pykale-0.1.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      562 2022-08-21 21:17:40.000000 pykale-0.1.1/tests/helpers/boring_model.py
--rw-r--r--   0 runner    (1001) docker     (116)      562 2022-08-21 21:17:40.000000 pykale-0.1.1/tests/helpers/pipe_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.619943 pykale-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-13 11:38:28.000000 pykale-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-13 11:38:42.619943 pykale-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-13 11:38:28.000000 pykale-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.587941 pykale-0.1.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.595941 pykale-0.1.2/examples/action_dann/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/action_dann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/action_dann/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/action_dann/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/action_dann/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/action_dann/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.595941 pykale-0.1.2/examples/bindingdb_deepdta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/bindingdb_deepdta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/bindingdb_deepdta/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/bindingdb_deepdta/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/bindingdb_deepdta/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.599942 pykale-0.1.2/examples/cifar_cnntransformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_cnntransformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_cnntransformer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_cnntransformer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_cnntransformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.599942 pykale-0.1.2/examples/cifar_isonet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_isonet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_isonet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_isonet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_isonet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cifar_isonet/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.599942 pykale-0.1.2/examples/cmri_mpca/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cmri_mpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cmri_mpca/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/cmri_mpca/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.603942 pykale-0.1.2/examples/digits_dann/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/digits_dann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/digits_dann/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/digits_dann/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/digits_dann/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.603942 pykale-0.1.2/examples/landmark_uncertainty_qbin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/landmark_uncertainty_qbin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.603942 pykale-0.1.2/examples/multisite_neuroimg_adapt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/multisite_neuroimg_adapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/multisite_neuroimg_adapt/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.603942 pykale-0.1.2/examples/office_multisource_adapt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/office_multisource_adapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/office_multisource_adapt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/office_multisource_adapt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/office_multisource_adapt/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.607942 pykale-0.1.2/examples/polypharmacy_gripnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/polypharmacy_gripnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/polypharmacy_gripnet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/polypharmacy_gripnet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/polypharmacy_gripnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.607942 pykale-0.1.2/examples/toy_domain_adaptation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/toy_domain_adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-13 11:38:28.000000 pykale-0.1.2/examples/toy_domain_adaptation/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.607942 pykale-0.1.2/kale/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.611943 pykale-0.1.2/kale/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/attention_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/gripnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/image_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/seq_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/video_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/video_i3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/video_res3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/video_se_i3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/video_se_res3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/embed/video_selayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.611943 pykale-0.1.2/kale/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/evaluate/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.611943 pykale-0.1.2/kale/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/interpret/model_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/interpret/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.615943 pykale-0.1.2/kale/loaddata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/dataset_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/image_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/mnistm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27118 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/multi_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/polypharmacy_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/tdc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/usps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/video_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/video_multi_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/loaddata/videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.615943 pykale-0.1.2/kale/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/base_nn_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/deepdta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42735 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/domain_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/mpca_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/multi_domain_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29966 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/pipeline/video_domain_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.615943 pykale-0.1.2/kale/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/predict/class_domain_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/predict/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/predict/isonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/predict/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.615943 pykale-0.1.2/kale/prepdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/chem_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/graph_negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/supergraph_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/tensor_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/prepdata/video_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.615943 pykale-0.1.2/kale/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-13 11:38:28.000000 pykale-0.1.2/kale/utils/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.619943 pykale-0.1.2/pykale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-13 11:38:42.000000 pykale-0.1.2/pykale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-13 11:38:42.000000 pykale-0.1.2/pykale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:38:42.000000 pykale-0.1.2/pykale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-13 11:38:42.000000 pykale-0.1.2/pykale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 11:38:42.000000 pykale-0.1.2/pykale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 11:38:28.000000 pykale-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 11:38:42.619943 pykale-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-13 11:38:28.000000 pykale-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.591941 pykale-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:42.619943 pykale-0.1.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:38:28.000000 pykale-0.1.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-13 11:38:28.000000 pykale-0.1.2/tests/helpers/boring_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-13 11:38:28.000000 pykale-0.1.2/tests/helpers/pipe_test_helper.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pykale-0.1.1/LICENSE` & `pykale-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/PKG-INFO` & `pykale-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykale
-Version: 0.1.1
+Version: 0.1.2
 Summary: Knowledge-aware machine learning from multiple sources in Python
 Home-page: https://github.com/pykale/pykale
 Author: The PyKale team
 Author-email: pykale-group@sheffield.ac.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pykale/pykale/issues
 Project-URL: Documentation, https://pykale.readthedocs.io
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: graph
 Provides-Extra: image
 Provides-Extra: example
 Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
@@ -41,15 +41,15 @@
 
 -----------------------------------------
 
 <!-- Keep badges to just ONE line, i.e. only the most important badges! -->
 [![tests](https://github.com/pykale/pykale/workflows/test/badge.svg)](https://github.com/pykale/pykale/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/pykale/pykale/branch/main/graph/badge.svg?token=jmIYPbA2le)](https://codecov.io/gh/pykale/pykale)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/optuna/optuna)
-[![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org)
 [![PyPI version](https://img.shields.io/pypi/v/pykale?color=blue)](https://pypi.org/project/pykale/)
 [![PyPI downloads](https://pepy.tech/badge/pykale)](https://pepy.tech/project/pykale)
 <!-- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5557244.svg)](https://doi.org/10.5281/zenodo.5557244) -->
 
 [Getting Started](https://github.com/pykale/pykale#how-to-use) |
 [Documentation](https://pykale.readthedocs.io/) |
 [Contributing](https://github.com/pykale/pykale/blob/main/.github/CONTRIBUTING.md) |
@@ -76,15 +76,15 @@
 
 - `examples` demonstrate real applications on specific datasets with a standardized structure.
 
 ## How to Use
 
 ### Step 0: Installation
 
-PyKale supports Python 3.7, 3.8, or 3.9. Before installing `pykale`, we suggest you to first [install PyTorch](https://pytorch.org/get-started/locally/) matching your hardware, and if graphs will be used, install [PyTorch Geometric](https://github.com/rusty1s/pytorch_geometric) following its [official instructions](https://github.com/rusty1s/pytorch_geometric#installation).
+PyKale supports Python 3.8, 3.9, or 3.10. Before installing `pykale`, we suggest you to first [install PyTorch](https://pytorch.org/get-started/locally/) matching your hardware, and if graphs will be used, install [PyTorch Geometric](https://github.com/rusty1s/pytorch_geometric) following its [official instructions](https://github.com/rusty1s/pytorch_geometric#installation).
 
 Simple installation of `pykale` from [PyPI](https://pypi.org/project/pykale/):
 
 ```bash
 pip install pykale
 ```
```

### Comparing `pykale-0.1.1/README.md` & `pykale-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 -----------------------------------------
 
 <!-- Keep badges to just ONE line, i.e. only the most important badges! -->
 [![tests](https://github.com/pykale/pykale/workflows/test/badge.svg)](https://github.com/pykale/pykale/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/pykale/pykale/branch/main/graph/badge.svg?token=jmIYPbA2le)](https://codecov.io/gh/pykale/pykale)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/optuna/optuna)
-[![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org)
 [![PyPI version](https://img.shields.io/pypi/v/pykale?color=blue)](https://pypi.org/project/pykale/)
 [![PyPI downloads](https://pepy.tech/badge/pykale)](https://pepy.tech/project/pykale)
 <!-- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5557244.svg)](https://doi.org/10.5281/zenodo.5557244) -->
 
 [Getting Started](https://github.com/pykale/pykale#how-to-use) |
 [Documentation](https://pykale.readthedocs.io/) |
 [Contributing](https://github.com/pykale/pykale/blob/main/.github/CONTRIBUTING.md) |
@@ -43,15 +43,15 @@
 
 - `examples` demonstrate real applications on specific datasets with a standardized structure.
 
 ## How to Use
 
 ### Step 0: Installation
 
-PyKale supports Python 3.7, 3.8, or 3.9. Before installing `pykale`, we suggest you to first [install PyTorch](https://pytorch.org/get-started/locally/) matching your hardware, and if graphs will be used, install [PyTorch Geometric](https://github.com/rusty1s/pytorch_geometric) following its [official instructions](https://github.com/rusty1s/pytorch_geometric#installation).
+PyKale supports Python 3.8, 3.9, or 3.10. Before installing `pykale`, we suggest you to first [install PyTorch](https://pytorch.org/get-started/locally/) matching your hardware, and if graphs will be used, install [PyTorch Geometric](https://github.com/rusty1s/pytorch_geometric) following its [official instructions](https://github.com/rusty1s/pytorch_geometric#installation).
 
 Simple installation of `pykale` from [PyPI](https://pypi.org/project/pykale/):
 
 ```bash
 pip install pykale
 ```
```

### Comparing `pykale-0.1.1/examples/action_dann/config.py` & `pykale-0.1.2/examples/action_dann/config.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/action_dann/main.py` & `pykale-0.1.2/examples/action_dann/main.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/action_dann/model.py` & `pykale-0.1.2/examples/action_dann/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     }
     return config_params
 
 
 # Based on https://github.com/criteo-research/pytorch-ada/blob/master/adalib/ada/utils/experimentation.py
 def get_model(cfg, dataset, num_classes):
     """
-    Builds and returns a model and associated hyper parameters according to the config object passed.
+    Builds and returns a model and associated hyperparameters according to the config object passed.
 
     Args:
         cfg: A YACS config object.
         dataset: A multi domain dataset consisting of source and target datasets.
         num_classes: The class number of specific dataset.
     """
```

### Comparing `pykale-0.1.1/examples/action_dann/test.py` & `pykale-0.1.2/examples/action_dann/test.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/bindingdb_deepdta/config.py` & `pykale-0.1.2/examples/bindingdb_deepdta/config.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/bindingdb_deepdta/main.py` & `pykale-0.1.2/examples/bindingdb_deepdta/main.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/bindingdb_deepdta/model.py` & `pykale-0.1.2/examples/bindingdb_deepdta/model.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/cifar_cnntransformer/config.py` & `pykale-0.1.2/examples/digits_dann/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,68 @@
 """
-Hyperparameter configuration file based on the YACS library.
+Default configurations for domain adaptation
 """
+
+import os
+
 from yacs.config import CfgNode as CN
 
+# -----------------------------------------------------------------------------
+# Config definition
+# -----------------------------------------------------------------------------
+
 _C = CN()
 
 # -----------------------------------------------------------------------------
 # Dataset
 # -----------------------------------------------------------------------------
 _C.DATASET = CN()
-_C.DATASET.ROOT = "../data"
-_C.DATASET.NAME = "CIFAR10"
+_C.DATASET.ROOT = "../data"  # Path to store data and results
+_C.DATASET.NAME = "digits"  # Name of datasets
+_C.DATASET.SOURCE = "mnist"  # The source dataset name
+_C.DATASET.TARGET = "usps"  # The target dataset name
 _C.DATASET.NUM_CLASSES = 10
-_C.DATASET.NUM_WORKERS = 0
-
+_C.DATASET.NUM_REPEAT = 10
+_C.DATASET.DIMENSION = 784
+_C.DATASET.WEIGHT_TYPE = "natural"
+_C.DATASET.SIZE_TYPE = "source"
+_C.DATASET.VALID_SPLIT_RATIO = 0.1
 # ---------------------------------------------------------------------------- #
 # Solver
 # ---------------------------------------------------------------------------- #
 _C.SOLVER = CN()
-_C.SOLVER.SEED = 42
-_C.SOLVER.BASE_LR = 0.05
-_C.SOLVER.LR_MILESTONES = [30, 60, 90]
-_C.SOLVER.LR_GAMMA = 0.1
-_C.SOLVER.WEIGHT_DECAY = 1e-4
+_C.SOLVER.SEED = 2020
+_C.SOLVER.BASE_LR = 0.001  # Initial learning rate
 _C.SOLVER.MOMENTUM = 0.9
-_C.SOLVER.NESTEROV = False
-
-_C.SOLVER.TRAIN_BATCH_SIZE = 128
-_C.SOLVER.TEST_BATCH_SIZE = 200
-
-_C.SOLVER.MAX_EPOCHS = 100
-
-_C.SOLVER.WARMUP = False
-_C.SOLVER.WARMUP_EPOCHS = 5
-
-# ---------------------------------------------------------------------------- #
-# CNN configs
-# ---------------------------------------------------------------------------- #
-_C.CNN = CN()
-_C.CNN.POOL_LOCATIONS = (0, 3)  # After which index of the below
-# convolutionial-layer list pooling
-# layers should be placed. (0,3) Applies
-# 2 pooling layers, resulting in an image
-# size of 8x8.
-
-# A tuple for each convolutional layer given as (num_channels, kernel_size)
-# (Nested lists log to file prettier than nested tuples do)
-_C.CNN.CONV_LAYERS = [[16, 3], [32, 3], [64, 3], [32, 1], [64, 3], [128, 3], [256, 3], [64, 1]]
-_C.CNN.USE_BATCHNORM = True
-_C.CNN.ACTIVATION_FUN = "relu"  # one of ('relu', 'elu', 'leaky_relu')
-_C.CNN.OUTPUT_SHAPE = (-1, 64, 8, 8)
-# ---------------------------------------------------------------------------- #
-# Transformer configs
-# ---------------------------------------------------------------------------- #
-_C.TRANSFORMER = CN()
-# Will not attach the Transformer on top of the CNN in the model if False
-_C.TRANSFORMER.USE_TRANSFORMER = True
-_C.TRANSFORMER.NUM_LAYERS = 3
-_C.TRANSFORMER.NUM_HEADS = 2
-_C.TRANSFORMER.DIM_FEEDFORWARD = 128
-_C.TRANSFORMER.DROPOUT = 0.1
-_C.TRANSFORMER.OUTPUT_TYPE = "spatial"
+_C.SOLVER.WEIGHT_DECAY = 0.0005  # 1e-4
+_C.SOLVER.NESTEROV = True
 
+_C.SOLVER.TYPE = "SGD"
+_C.SOLVER.MAX_EPOCHS = 120  # "nb_adapt_epochs": 100,
+# _C.SOLVER.WARMUP = True
+_C.SOLVER.MIN_EPOCHS = 20  # "nb_init_epochs": 20,
+_C.SOLVER.TRAIN_BATCH_SIZE = 150  # 150
+_C.SOLVER.TEST_BATCH_SIZE = 200  # No difference in ADA
+
+# Adaptation-specific solver config
+_C.SOLVER.AD_LAMBDA = True
+_C.SOLVER.AD_LR = True
+_C.SOLVER.INIT_LAMBDA = 1.0
+
+# ---------------------------------------------------------------------------- #
+# Domain Adaptation Net (DAN) configs
+# ---------------------------------------------------------------------------- #
+_C.DAN = CN()
+_C.DAN.METHOD = "CDAN"  # choices=['CDAN', 'CDAN-E', 'DANN']
+_C.DAN.USERANDOM = False
+_C.DAN.RANDOM_DIM = 1024
 # ---------------------------------------------------------------------------- #
 # Misc options
 # ---------------------------------------------------------------------------- #
-_C.OUTPUT_DIR = "./outputs"
+_C.OUTPUT = CN()
+_C.OUTPUT.VERBOSE = False  # To discuss, for HPC jobs
+_C.OUTPUT.PB_FRESH = 0  # 0 # 50 # 0 to disable  ; MAYBE make it a command line option
+_C.OUTPUT.TB_DIR = os.path.join("lightning_logs", _C.DATASET.SOURCE + "2" + _C.DATASET.TARGET)
 
 
 def get_cfg_defaults():
     return _C.clone()
```

### Comparing `pykale-0.1.1/examples/cifar_cnntransformer/main.py` & `pykale-0.1.2/examples/cifar_isonet/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,80 @@
-"""
-This example demonstrates the use of a CNN and a Transformer-Encoder
-for image classification on CIFAR10.
+"""ISONet (an extension of ResNet) on CIFAR image classification
 
-Reference: See kale.embed.attention_cnn for more details.
+Reference: https://github.com/HaozhiQi/ISONet/blob/master/train.py
 """
+
 import argparse
 import os
 
 import torch
 from config import get_cfg_defaults
 from model import get_model
-from torchsummary import summary
 from trainer import Trainer
 
-import kale.utils.logger as logging
-import kale.utils.seed as seed
 from kale.loaddata.image_access import get_cifar
+from kale.utils.logger import construct_logger
+from kale.utils.seed import set_seed
 
 
 def arg_parse():
+    """Parsing arguments"""
     parser = argparse.ArgumentParser(description="PyTorch CIFAR10 Training")
     parser.add_argument("--cfg", required=True, help="path to config file", type=str)
-    # parser.add_argument('--output', default='default', help='folder to save output', type=str)
+    parser.add_argument("--output", default="default", help="folder to save output", type=str)
     parser.add_argument("--resume", default="", type=str)
     args = parser.parse_args()
     return args
 
 
 def main():
+    """The main for this domain adapation example, showing the workflow"""
     args = arg_parse()
 
     # ---- setup device ----
     device = "cuda" if torch.cuda.is_available() else "cpu"
     print("==> Using device " + device)
 
-    # ---- setup config ----
+    # ---- setup configs ----
     cfg = get_cfg_defaults()
     cfg.merge_from_file(args.cfg)
     cfg.freeze()
-    seed.set_seed(cfg.SOLVER.SEED)
+    set_seed(cfg.SOLVER.SEED)
 
-    # ---- setup logger ----
-    os.makedirs(cfg.OUTPUT_DIR, exist_ok=True)
-    logger = logging.construct_logger("context_cnns", cfg.OUTPUT_DIR)
-    logger.info(f"Using {device}")
+    # ---- setup logger and output ----
+    output_dir = os.path.join(cfg.OUTPUT_DIR, cfg.DATASET.NAME, args.output)
+    os.makedirs(output_dir, exist_ok=True)
+    logger = construct_logger("isonet", output_dir)
+    logger.info("Using " + device)
     logger.info("\n" + cfg.dump())
 
     # ---- setup dataset ----
     train_loader, valid_loader = get_cifar(cfg)
 
-    # ---- setup model ----
     print("==> Building model..")
     net = get_model(cfg)
+    # print(net)
     net = net.to(device)
+    # model_stats = summary(net, (3, 32, 32))
+    # logger.info('\n'+str(model_stats))
 
-    model_stats = summary(net, (3, 32, 32))
-    logger.info("\n" + str(model_stats))
-
+    # Needed even for single GPU https://discuss.pytorch.org/t/attributeerror-net-object-has-no-attribute-module/45652
     if device == "cuda":
         net = torch.nn.DataParallel(net)
 
-    # ---- setup trainers ----
     optim = torch.optim.SGD(
-        net.parameters(), lr=cfg.SOLVER.BASE_LR, momentum=cfg.SOLVER.MOMENTUM, weight_decay=cfg.SOLVER.WEIGHT_DECAY
+        net.parameters(),
+        lr=cfg.SOLVER.BASE_LR,
+        momentum=cfg.SOLVER.MOMENTUM,
+        weight_decay=cfg.SOLVER.WEIGHT_DECAY,
+        dampening=cfg.SOLVER.DAMPENING,
+        nesterov=cfg.SOLVER.NESTEROV,
     )
 
-    trainer = Trainer(device, train_loader, valid_loader, net, optim, logger, cfg)
+    trainer = Trainer(device, train_loader, valid_loader, net, optim, logger, output_dir, cfg)
 
     if args.resume:
         # Load checkpoint
         print("==> Resuming from checkpoint..")
         cp = torch.load(args.resume)
         trainer.model.load_state_dict(cp["net"])
         trainer.optim.load_state_dict(cp["optim"])
```

### Comparing `pykale-0.1.1/examples/cifar_cnntransformer/trainer.py` & `pykale-0.1.2/examples/cifar_isonet/trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,171 @@
-# Created by Raivo Koot from modifying https://github.com/HaozhiQi/ISONet/blob/master/isonet/trainer.py
-# Under the MIT License
+"""A standard trainer for ISONet
+
+From: https://github.com/HaozhiQi/ISONet/blob/master/isonet/trainer.py
+"""
+
 import time
 
 import torch
 import torch.nn as nn
 
 from kale.utils.print import pprint_without_newline, tprint
 
 
 class Trainer(object):
-    def __init__(self, device, train_loader, valid_loader, model, optim, logger, cfg):
-        self.device = device
+    """Sets up a standard trainer
+
+    Args:
+        device: gpu or cpu
+        train_loader: the training data loader
+        valid_loader: the validation data loader
+        model: the (network) model
+        optim: the optimizer
+        logger:: the logger to log info
+        output_dir: the path to save info
+        cfg: a YACS config object.
+    """
 
+    def __init__(self, device, train_loader, valid_loader, model, optim, logger, output_dir, cfg):
+        # misc
+        self.device = device
+        self.output_dir = output_dir
+        # data loader
         self.train_loader = train_loader
         self.valid_loader = valid_loader
+        # nn setting
         self.model = model
         self.optim = optim
-        self.logger = logger
-        self.cfg = cfg
-
-        # ---- loss settings ----
-        self.criterion = nn.NLLLoss()
-        self.loss = 0
+        # lr setting
+        self.criterion = nn.CrossEntropyLoss()
+        # training loop settings
+        self.epochs = 1
+        # loss settings
         self.train_acc, self.valid_acc = [], []
         self.best_valid_acc = 0
-
-        # ---- others ----
+        self.ce_loss, self.ortho_loss = 0, 0
+        # others
         self.ave_time = 0
-        self.epochs = 1
+        self.logger = logger
+        self.cfg = cfg
 
     def train(self):
+        """The validation step"""
         while self.epochs <= self.cfg.SOLVER.MAX_EPOCHS:
             self.adjust_learning_rate()
             self.train_epoch()
             self.valid()
             self.epochs += 1
 
     def train_epoch(self):
+        """One training epoch"""
         self.model.train()
-        self.loss = 0
+        self.ce_loss = 0
+        self.ortho_loss = 0
         self.ave_time = 0
         correct = 0
         total = 0
         epoch_t = time.time()
-
         for batch_idx, (inputs, targets) in enumerate(self.train_loader):
             iter_t = time.time()
             inputs, targets = inputs.to(self.device), targets.to(self.device)
             self.optim.zero_grad()
             batch_size = inputs.shape[0]
 
             outputs = self.model(inputs)
-            loss = self.criterion(outputs, targets)
+            loss = self.loss(outputs, targets)
             loss.backward()
             self.optim.step()
 
             _, predicted = outputs.max(1)
-            self.loss += loss.item()
             total += batch_size
 
             correct += predicted.eq(targets).sum().item()
 
             self.ave_time += time.time() - iter_t
             tprint(
                 f"train Epoch: {self.epochs} | {batch_idx + 1} / {len(self.train_loader)} | "
-                f"Acc: {100. * correct / total:.3f} | Loss: {self.loss / (batch_idx + 1):.3f} | "
-                f"time: {self.ave_time / (batch_idx + 1):.3f}s"
-            )
-
-            info_str = (
-                f"train Epoch: {self.epochs} | Acc: {100. * correct / total:.3f} | "
-                f"Loss: {self.loss / (batch_idx + 1):.3f} | "
-                f"time: {time.time() - epoch_t:.2f}s |"
+                f"Acc: {100. * correct / total:.3f} | CE: {self.ce_loss / (batch_idx + 1):.3f} | "
+                f"O: {self.ortho_loss / (batch_idx + 1):.3f} | time: {self.ave_time / (batch_idx + 1):.3f}s"
             )
 
+        info_str = (
+            f"train Epoch: {self.epochs} | Acc: {100. * correct / total:.3f} | "
+            f"CE: {self.ce_loss / (batch_idx + 1):.3f} | "
+            f"time: {time.time() - epoch_t:.2f}s |"
+        )
         self.logger.info(info_str)
         pprint_without_newline(info_str)
         self.train_acc.append(100.0 * correct / total)
 
     def valid(self):
+        """The validation step"""
         self.model.eval()
-        self.loss = 0
+        self.ce_loss = 0
+        self.ortho_loss = 0
         correct = 0
         total = 0
-
         with torch.no_grad():
             for batch_idx, (inputs, targets) in enumerate(self.valid_loader):
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
                 outputs = self.model(inputs)
-
-                loss = self.criterion(outputs, targets)
-                self.loss = loss
+                # loss = self.loss(outputs, targets)
 
                 _, predicted = outputs.max(1)
                 total += targets.size(0)
                 correct += predicted.eq(targets).sum().item()
 
         if 100.0 * correct / total > self.best_valid_acc:
             self.snapshot("best")
         self.snapshot("latest")
-
         self.best_valid_acc = max(self.best_valid_acc, 100.0 * correct / total)
         info_str = (
             f"valid | Acc: {100. * correct / total:.3f} | "
-            f"Loss: {self.loss / len(self.valid_loader):.3f} | "
+            f"CE: {self.ce_loss / len(self.valid_loader):.3f} | "
+            f"O: {self.ortho_loss / len(self.valid_loader):.3f} | "
             f"best: {self.best_valid_acc:.3f} | "
         )
-
         print(info_str)
         self.logger.info(info_str)
         self.valid_acc.append(100.0 * correct / total)
 
-    def adjust_learning_rate(self):
-        c = self.cfg
+    def loss(self, outputs, targets):
+        """Computes the loss between learning outputs and the targets (ground truth)"""
+        loss = self.criterion(outputs, targets)
+        self.ce_loss += loss.item()
+
+        if self.cfg.ISON.ORTHO_COEFF > 0:
+            o_loss = self.model.module.ortho(self.device)
+            self.ortho_loss += o_loss.item()
+            loss += o_loss * self.cfg.ISON.ORTHO_COEFF
+        return loss
 
-        # Linear warmup
-        if c.SOLVER.WARMUP and self.epochs < c.SOLVER.WARMUP_EPOCHS:
-            lr = c.SOLVER.BASE_LR * self.epochs / c.SOLVER.WARMUP_EPOCHS
+    def adjust_learning_rate(self):
+        """Adjust the learning rate according to the configuration"""
+        # if do linear warmup
+        if self.cfg.SOLVER.WARMUP and self.epochs < self.cfg.SOLVER.WARMUP_EPOCH:
+            lr = self.cfg.SOLVER.BASE_LR * self.epochs / self.cfg.SOLVER.WARMUP_EPOCH
         else:
             # normal (step) scheduling
-            lr = c.SOLVER.BASE_LR
-            for m_epoch in c.SOLVER.LR_MILESTONES:
+            lr = self.cfg.SOLVER.BASE_LR
+            for m_epoch in self.cfg.SOLVER.LR_MILESTONES:
                 if self.epochs > m_epoch:
-                    lr *= c.SOLVER.LR_GAMMA
+                    lr *= self.cfg.SOLVER.LR_GAMMA
 
         for param_group in self.optim.param_groups:
             param_group["lr"] = lr
             if "scaling" in param_group:
                 param_group["lr"] *= param_group["scaling"]
 
     def snapshot(self, name=None):
+        """Saves the current model"""
         state = {
             "net": self.model.state_dict(),
             "optim": self.optim.state_dict(),
             "epoch": self.epochs,
             "train_accuracy": self.train_acc,
             "test_accuracy": self.valid_acc,
         }
-
         if name is None:
-            torch.save(state, f"{self.cfg.OUTPUT_DIR}/epoch-{self.epochs}.pt")
+            torch.save(state, f"{self.output_dir}/{self.epochs}.pt")
         else:
-            torch.save(state, f"{self.cfg.OUTPUT_DIR}/{name}.pt")
+            torch.save(state, f"{self.output_dir}/{name}.pt")
```

### Comparing `pykale-0.1.1/examples/cifar_isonet/config.py` & `pykale-0.1.2/examples/cifar_isonet/config.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/cifar_isonet/model.py` & `pykale-0.1.2/examples/cifar_isonet/model.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/cmri_mpca/config.py` & `pykale-0.1.2/examples/cmri_mpca/config.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/cmri_mpca/main.py` & `pykale-0.1.2/examples/cmri_mpca/main.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/digits_dann/main.py` & `pykale-0.1.2/examples/digits_dann/main.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/digits_dann/model.py` & `pykale-0.1.2/examples/digits_dann/model.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/multisite_neuroimg_adapt/config.py` & `pykale-0.1.2/examples/multisite_neuroimg_adapt/config.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/office_multisource_adapt/config.py` & `pykale-0.1.2/examples/office_multisource_adapt/config.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/office_multisource_adapt/main.py` & `pykale-0.1.2/examples/office_multisource_adapt/main.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/office_multisource_adapt/model.py` & `pykale-0.1.2/examples/office_multisource_adapt/model.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/examples/toy_domain_adaptation/main.py` & `pykale-0.1.2/examples/toy_domain_adaptation/main.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/attention_cnn.py` & `pykale-0.1.2/kale/embed/attention_cnn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Any, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from kale.embed.positional_encoding import PositionalEncoding
 from kale.prepdata.tensor_reshape import seq_to_spatial, spatial_to_seq
 
@@ -11,25 +11,25 @@
     """
     A template to construct a feature extractor consisting of a CNN followed by a
     sequence-to-sequence contextualizer like a Transformer-Encoder. Before inputting the CNN output
     tensor to the contextualizer, the tensor's spatial dimensions are unrolled
     into a sequence.
 
     Args:
-        cnn: any convolutional neural network that takes in batches of images of
+        cnn (nn.Module): any convolutional neural network that takes in batches of images of
              shape (batch_size, channels, height, width) and outputs tensor
              representations of shape (batch_size, out_channels, out_height, out_width).
-        cnn_output_shape: A tuple of shape (batch_size, num_channels, height, width)
+        cnn_output_shape (tuple): A tuple of shape (batch_size, num_channels, height, width)
                            describing the output shape of the given CNN (required).
-        contextualizer: A sequence-to-sequence model that takes inputs of shape
+        contextualizer (nn.Module, optional): A sequence-to-sequence model that takes inputs of shape
                          (num_timesteps, batch_size, num_features) and uses
                          attention to contextualize the sequence and returns
                          a sequence of the exact same shape. This will mainly be
                          a Transformer-Encoder (required).
-        output_type: One of 'sequence' or 'spatial'. If Spatial then the final
+        output_type (string): One of 'sequence' or 'spatial'. If Spatial then the final
                       output of the model, which is a sequence, will be reshaped
                       to resemble the image-batch shape of the output of the CNN.
                       If Sequence then the output sequence is returned as is (required).
 
     Examples:
         >>> cnn = nn.Sequential(nn.Conv2d(3, 32, kernel_size=3),
         >>>                     nn.Conv2d(32, 64, kernel_size=3),
@@ -41,15 +41,19 @@
         >>> attention_cnn = ContextCNNGeneric(cnn, cnn_output_shape, contextualizer, output_type)
         >>> output = attention_cnn(torch.randn((32,3,16,16)))
         >>>
         >>> output.size() == cnn_output_shape # True
     """
 
     def __init__(
-        self, cnn: nn.Module, cnn_output_shape: Tuple[int, int, int, int], contextualizer: nn.Module, output_type: str
+        self,
+        cnn: nn.Module,
+        cnn_output_shape: Tuple[int, int, int, int],
+        contextualizer: Union[nn.Module, Any],
+        output_type: str,
     ):
         super(ContextCNNGeneric, self).__init__()
         assert output_type in ["spatial", "sequence"], (
             "parameter 'output_type' must be one of ('spatial', 'sequence')" + f" but is {output_type}"
         )
 
         self.cnn = cnn
@@ -80,29 +84,29 @@
 class CNNTransformer(ContextCNNGeneric):
     """
     A feature extractor consisting of a given CNN backbone followed by a standard
     Transformer-Encoder. See documentation of "ContextCNNGeneric" for more
     information.
 
     Args:
-        cnn: any convolutional neural network that takes in batches of images of
+        cnn (nn.Module): any convolutional neural network that takes in batches of images of
              shape (batch_size, channels, height, width) and outputs tensor
              representations of shape (batch_size, out_channels, out_height, out_width) (required).
-        cnn_output_shape: a tuple of shape (batch_size, num_channels, height, width)
+        cnn_output_shape (tuple): a tuple of shape (batch_size, num_channels, height, width)
                            describing the output shape of the given CNN (required).
-        num_layers: number of attention layers in the Transformer-Encoder (required).
-        num_heads: number of attention heads in each transformer block (required).
-        dim_feedforward: number of neurons in the intermediate dense layer of
+        num_layers (int): number of attention layers in the Transformer-Encoder (required).
+        num_heads (int): number of attention heads in each transformer block (required).
+        dim_feedforward (int): number of neurons in the intermediate dense layer of
                           each transformer feedforward block (required).
-        dropout: dropout rate of the transformer layers (required).
-        output_type: one of 'sequence' or 'spatial'. If Spatial then the final
+        dropout (float): dropout rate of the transformer layers (required).
+        output_type (string): one of 'sequence' or 'spatial'. If Spatial then the final
                       output of the model, which is the sequence output of the
                       Transformer-Encoder, will be reshaped to resemble the
                       image-batch shape of the output of the CNN (required).
-        positional_encoder: None or a nn.Module that expects inputs of
+        positional_encoder (nn.Module): None or a nn.Module that expects inputs of
                             shape (sequence_length, batch_size, embedding_dim)
                             and returns the same input after adding
                             some positional information to the embeddings. If
                             `None`, then the default and fixed sin-cos positional
                             encodings of base transformers are applied (optional).
 
     Examples:
```

### Comparing `pykale-0.1.1/kale/embed/factorization.py` & `pykale-0.1.2/kale/embed/factorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 import numpy as np
 from numpy.linalg import multi_dot
 from scipy import linalg
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.metrics.pairwise import pairwise_kernels
 from sklearn.preprocessing import KernelCenterer, LabelBinarizer
 from sklearn.utils.validation import check_is_fitted
-
-# import tensorly as tl
 from tensorly.base import fold, unfold
 from tensorly.tenalg import multi_mode_dot
 
 
 def _check_n_dim(x, n_dims):
     """Raise error if the number of dimensions of the input data is not consistent with the expected value.
 
@@ -85,15 +83,15 @@
     Reference:
         Haiping Lu, K.N. Plataniotis, and A.N. Venetsanopoulos, "MPCA: Multilinear Principal Component Analysis of
         Tensor Objects", IEEE Transactions on Neural Networks, Vol. 19, No. 1, Page: 18-39, January 2008. For initial
         Matlab implementation, please go to https://uk.mathworks.com/matlabcentral/fileexchange/26168.
 
     Examples:
         >>> import numpy as np
-        >>> from kale.embed.mpca import MPCA
+        >>> from kale.embed.factorization import MPCA
         >>> x = np.random.random((40, 20, 25, 20))
         >>> x.shape
         (40, 20, 25, 20)
         >>> mpca = MPCA()
         >>> x_projected = mpca.fit_transform(x)
         >>> x_projected.shape
         (40, 18, 23, 18)
@@ -373,15 +371,15 @@
             obj = multi_dot([kernel_x, self.mu * ctr_mat - multi_dot([ctr_mat, kernel_c, ctr_mat]), kernel_x.T])
 
         eig_values, eig_vectors = linalg.eigh(obj, subset_by_index=[n_samples - self.n_components, n_samples - 1])
         idx_sorted = eig_values.argsort()[::-1]
 
         self.eig_values_ = eig_values[idx_sorted]
         self.U = eig_vectors[:, idx_sorted]
-        self.U = np.asarray(self.U, dtype=np.float)
+        self.U = np.asarray(self.U, dtype=np.float64)
 
         return self
 
     def fit_transform(self, x, y=None, covariates=None):
         """
         Args:
             x : array-like, shape (n_samples, n_features)
```

### Comparing `pykale-0.1.1/kale/embed/gcn.py` & `pykale-0.1.2/kale/embed/gcn.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/image_cnn.py` & `pykale-0.1.2/kale/embed/image_cnn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-"""
-CNNs for extracting features from small images of size 32x32 (e.g. MNIST) and regular images of size 224x224 (e.g.
+"""CNNs for extracting features from small images of size 32x32 (e.g. MNIST) and regular images of size 224x224 (e.g.
 ImageNet). The code is based on https://github.com/criteo-research/pytorch-ada/blob/master/adalib/ada/models/modules.py,
  which is for domain adaptation.
 """
 
 import torch.nn as nn
 from torchvision import models
 
 
 # From FeatureExtractorDigits in adalib
 class SmallCNNFeature(nn.Module):
     """
     A feature extractor for small 32x32 images (e.g. CIFAR, MNIST) that outputs a feature vector of length 128.
 
     Args:
-        num_channels: the number of input channels (default=3).
-        kernel_size: the size of the convolution kernel (default=5).
+        num_channels (int): the number of input channels (default=3).
+        kernel_size (int): the size of the convolution kernel (default=5).
 
     Examples::
         >>> feature_network = SmallCNNFeature(num_channels)
     """
 
     def __init__(self, num_channels=3, kernel_size=5):
         super(SmallCNNFeature, self).__init__()
@@ -45,14 +44,61 @@
         x = x.view(x.size(0), -1)
         return x
 
     def output_size(self):
         return self._out_features
 
 
+class SimpleCNNBuilder(nn.Module):
+    """A builder for simple CNNs to experiment with different basic architectures.
+
+    Args:
+        num_channels (int, optional): the number of input channels. Defaults to 3.
+        conv_layers_spec (list): a list for each convolutional layer given as [num_channels, kernel_size].
+            For example, [[16, 3], [16, 1]] represents 2 layers with 16 filters and kernel sizes of 3 and 1 respectively.
+        activation_fun (str): a string specifying the activation function to use. one of ('relu', 'elu', 'leaky_relu').
+            Defaults to "relu".
+        use_batchnorm (boolean): a boolean flag indicating whether to use batch normalization. Defaults to True.
+        pool_locations (tuple): the index after which pooling layers should be placed in the convolutional layer list.
+            Defaults to (0,3). (0,3) means placing 2 pooling layers after the first and fourth convolutional layer.
+        num_channels (int): the number of input channels. Defaults to 3.
+    """
+
+    activations = {"relu": nn.ReLU(), "elu": nn.ELU(), "leaky_relu": nn.LeakyReLU()}
+
+    def __init__(
+        self, conv_layers_spec, activation_fun="relu", use_batchnorm=True, pool_locations=(0, 3), num_channels=3
+    ):
+        super(SimpleCNNBuilder, self).__init__()
+        self.layers = nn.ModuleList()
+        in_channels = num_channels
+        activation_fun = self.activations[activation_fun]
+
+        # Repetitively adds a convolution, batch-norm, activation Function, and max-pooling layer.
+        for layer_num, (num_kernels, kernel_size) in enumerate(conv_layers_spec):
+            conv = nn.Conv2d(in_channels, num_kernels, kernel_size, stride=1, padding=(kernel_size - 1) // 2)
+            self.layers.append(conv)
+
+            if use_batchnorm:
+                self.layers.append(nn.BatchNorm2d(num_kernels))
+
+            self.layers.append(activation_fun)
+
+            if layer_num in pool_locations:
+                self.layers.append(nn.MaxPool2d(kernel_size=2))
+
+            in_channels = num_kernels
+
+    def forward(self, x):
+        for block in self.layers:
+            x = block(x)
+
+        return x
+
+
 class _Bottleneck(nn.Module):
     """Simple bottleneck as domain specific feature extractor, used in multi-source domain adaptation method MFSAN only.
         Compared to the torchvision implementation, it accepts both 1D and 2D input, and the value of expansion is
         flexible and an average pooling layer is added.
 
         The code is based on:
             https://github.com/pytorch/vision/blob/main/torchvision/models/resnet.py#L86,
```

### Comparing `pykale-0.1.1/kale/embed/positional_encoding.py` & `pykale-0.1.2/kale/embed/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/seq_nn.py` & `pykale-0.1.2/kale/embed/seq_nn.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/video_feature_extractor.py` & `pykale-0.1.2/kale/embed/video_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/video_i3d.py` & `pykale-0.1.2/kale/embed/video_i3d.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/video_res3d.py` & `pykale-0.1.2/kale/embed/video_res3d.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/video_se_i3d.py` & `pykale-0.1.2/kale/embed/video_se_i3d.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/video_se_res3d.py` & `pykale-0.1.2/kale/embed/video_se_res3d.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/embed/video_selayer.py` & `pykale-0.1.2/kale/embed/video_selayer.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/interpret/model_weights.py` & `pykale-0.1.2/kale/interpret/model_weights.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/interpret/visualize.py` & `pykale-0.1.2/kale/interpret/visualize.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/dataset_access.py` & `pykale-0.1.2/kale/loaddata/dataset_access.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/image_access.py` & `pykale-0.1.2/kale/loaddata/image_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,18 @@
             return MultiDomainImageFolder(data_path, transform=transform, sub_domain_set=sub_domain_set, **kwargs)
 
 
 def get_cifar(cfg):
     """Gets training and validation data loaders for the CIFAR datasets
 
     Args:
-        cfg: A YACS config object.
+        cfg (CfgNode): hyperparameters from configure file
+
+    Examples:
+        >>> train_loader, valid_loader = get_cifar(cfg)
     """
     logging.info("==> Preparing to load data " + cfg.DATASET.NAME + " at " + cfg.DATASET.ROOT)
     cifar_train_transform = get_transform("cifar", augment=True)
     cifar_test_transform = get_transform("cifar", augment=False)
 
     if cfg.DATASET.NAME == "CIFAR10":
         train_set = datasets.CIFAR10(cfg.DATASET.ROOT, train=True, download=True, transform=cifar_train_transform)
@@ -348,14 +351,15 @@
         [list]: List of dicom dataset objects
     """
     dcm_phases = []  # list of dicom dataset objects (phases)
     # get all dicom files under the directory
     phase_files = glob.glob(dicom_path + "/**/*.dcm", recursive=True)
     for phase_file in phase_files:
         dataset = pydicom.dcmread(phase_file)
+        setattr(dataset, "FilePath", phase_file)
         dcm_phases.append(dataset)
     if sort_instance:
         dcm_phases.sort(key=lambda x: x.InstanceNumber, reverse=False)
 
     return dcm_phases
```

### Comparing `pykale-0.1.1/kale/loaddata/mnistm.py` & `pykale-0.1.2/kale/loaddata/mnistm.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/multi_domain.py` & `pykale-0.1.2/kale/loaddata/multi_domain.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/sampler.py` & `pykale-0.1.2/kale/loaddata/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             sum_w = np.sum(class_weights)
             if sum_w >= 1:
                 # normalize attributing equal weight to weighted part and remaining part
                 class_weights /= sum_w * k / n_classes + (n_classes - k) / n_classes
             krem = k - n_classes
             wrem = 1 - sum_w
             logging.warning(f"will assume uniform distribution for labels > {len(class_weights)}")
-            self._class_weights = np.ones(n_classes, dtype=np.float)
+            self._class_weights = np.ones(n_classes, dtype=np.float64)
             self._class_weights[:k] = class_weights
             self._class_weights[k:] = wrem / krem
         else:
             self._class_weights = class_weights[:n_classes]
 
         if np.sum(self._class_weights) != 1:
             self._class_weights = self._class_weights / np.sum(self._class_weights)
```

### Comparing `pykale-0.1.1/kale/loaddata/tdc_datasets.py` & `pykale-0.1.2/kale/loaddata/tdc_datasets.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/usps.py` & `pykale-0.1.2/kale/loaddata/usps.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/video_access.py` & `pykale-0.1.2/kale/loaddata/video_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 def generate_list(data_name, data_params_local, domain):
     """
 
     Args:
         data_name (string): name of dataset
-        data_params_local (dict): hyper parameters from configure file
+        data_params_local (dict): hyperparameters from configure file
         domain (string): domain type (source or target)
 
     Returns:
         data_path (string): image directory of dataset
         train_listpath (string): training list file directory of dataset
         test_listpath (string): test list file directory of dataset
     """
@@ -94,20 +94,20 @@
     def get_source_target(source: "VideoDataset", target: "VideoDataset", seed, params):
         """
         Gets data loaders for source and target datasets
         Sets channel_number as 3 for RGB, 2 for flow.
         Sets class_number as 8 for EPIC, 7 for ADL, 6 for both GTEA and KITCHEN.
 
         Args:
-            source: (VideoDataset): source dataset name
-            target: (VideoDataset): target dataset name
-            seed: (int): seed value set manually.
-            params: (CfgNode): hyper parameters from configure file
+            source (VideoDataset): source dataset name
+            target (VideoDataset): target dataset name
+            seed (int): seed value set manually
+            params (CfgNode): hyperparameters from configure file
 
-        Examples::
+        Examples:
             >>> source, target, num_classes = get_source_target(source, target, seed, params)
         """
         config_params = get_videodata_config(params)
         data_params = config_params["data_params"]
         data_params_local = deepcopy(data_params)
         data_src_name = data_params_local["dataset_src_name"].upper()
         src_data_path, src_tr_listpath, src_te_listpath = generate_list(data_src_name, data_params_local, domain="src")
@@ -205,15 +205,15 @@
         data_path (string): image directory of dataset
         train_list (string): training list file directory of dataset
         test_list (string): test list file directory of dataset
         image_modality (string): image type (RGB or Optical Flow)
         frames_per_segment (int): length of each action sample (the unit is number of frame)
         n_classes (int): number of class
         transform_kind (string): types of video transforms
-        seed: (int): seed value set manually.
+        seed (int): seed value set manually
     """
 
     def __init__(
         self, data_path, train_list, test_list, image_modality, frames_per_segment, n_classes, transform_kind, seed
     ):
         super().__init__(n_classes)
         self._data_path = data_path
```

### Comparing `pykale-0.1.1/kale/loaddata/video_datasets.py` & `pykale-0.1.2/kale/loaddata/video_datasets.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/video_multi_domain.py` & `pykale-0.1.2/kale/loaddata/video_multi_domain.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/loaddata/videos.py` & `pykale-0.1.2/kale/loaddata/videos.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/pipeline/deepdta.py` & `pykale-0.1.2/kale/pipeline/deepdta.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/pipeline/domain_adapter.py` & `pykale-0.1.2/kale/pipeline/domain_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Domain adaptation systems (pipelines) with three types of architectures
 
 This module takes individual modules as input and organises them into an architecture. This is taken directly from
 https://github.com/criteo-research/pytorch-ada/blob/master/adalib/ada/models/architectures.py with minor changes.
 
-This module uses `PyTorch Lightning <https://github.com/PyTorchLightning/pytorch-lightning>`_ to standardize the flow.
+This module uses `PyTorch Lightning <https://github.com/Lightning-AI/lightning>`_ to standardize the flow.
 """
 
 from enum import Enum
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
@@ -217,29 +217,30 @@
 
     :math:`\lambda_p = \frac{2}{1 + \exp{(-\gamma \cdot p)}} - 1` where :math:`p` the learning progress
     changes linearly from 0 to 1.
 
     Args:
         dataset (kale.loaddata.multi_domain): the multi-domain datasets to be used for train, validation, and tests.
         feature_extractor (torch.nn.Module): the feature extractor network (mapping inputs :math:`x\in\mathcal{X}`
-            to a latent space :math:`\mathcal{Z}`,)
+            to a latent space :math:`\mathcal{Z}`,).
         task_classifier (torch.nn.Module): the task classifier network that learns to predict labels
-            :math:`y \in \mathcal{Y}` from latent vectors,
+            :math:`y \in \mathcal{Y}` from latent vectors.
         method (Method, optional): the method implemented by the class. Defaults to None.
             Mostly useful when several methods may be implemented using the same class.
-        lambda_init (float, optional): Weight attributed to the adaptation part of the loss. Defaults to 1.0.
-        adapt_lambda (bool, optional): Whether to make lambda grow from 0 to 1 following the schedule from
+        lambda_init (float, optional): weight attributed to the adaptation part of the loss. Defaults to 1.0.
+        adapt_lambda (bool, optional): whether to make lambda grow from 0 to 1 following the schedule from
             the DANN paper. Defaults to True.
-        adapt_lr (bool, optional): Whether to use the schedule for the learning rate as defined
+        adapt_lr (bool, optional): whether to use the schedule for the learning rate as defined
             in the DANN paper. Defaults to True.
-        nb_init_epochs (int, optional): Number of warmup epochs (during which lambda=0, training only on the source). Defaults to 10.
-        nb_adapt_epochs (int, optional): Number of training epochs. Defaults to 50.
-        batch_size (int, optional): Defaults to 32.
-        init_lr (float, optional): Initial learning rate. Defaults to 1e-3.
-        optimizer (dict, optional): Optimizer parameters, a dictionary with 2 keys:
+        nb_init_epochs (int, optional): number of warmup epochs (during which lambda=0, training only on the source).
+            Defaults to 10.
+        nb_adapt_epochs (int, optional): number of training epochs. Defaults to 50.
+        batch_size (int, optional): defaults to 32.
+        init_lr (float, optional): initial learning rate. Defaults to 1e-3.
+        optimizer (dict, optional): optimizer parameters, a dictionary with 2 keys:
             "type": a string in ("SGD", "Adam", "AdamW")
             "optim_params": kwargs for the above PyTorch optimizer.
             Defaults to None.
     """
 
     def __init__(
         self,
```

### Comparing `pykale-0.1.1/kale/pipeline/mpca_trainer.py` & `pykale-0.1.2/kale/pipeline/mpca_trainer.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/pipeline/multi_domain_adapter.py` & `pykale-0.1.2/kale/pipeline/multi_domain_adapter.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/pipeline/video_domain_adapter.py` & `pykale-0.1.2/kale/pipeline/video_domain_adapter.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/predict/class_domain_nets.py` & `pykale-0.1.2/kale/predict/class_domain_nets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # =============================================================================
 # Author: Xianyuan Liu, xianyuan.liu@outlook.com
 #         Haiping Lu, h.lu@sheffield.ac.uk or hplu@ieee.org
 # =============================================================================
 
 """Classification of data or domain
 
-Modules for typical classification tasks (into class labels) and
-adversarial discrimination of source vs target domains, from
-https://github.com/criteo-research/pytorch-ada/blob/master/adalib/ada/models/modules.py
+Modules for typical classification tasks (into class labels) and adversarial discrimination of source vs target domains,
+from https://github.com/criteo-research/pytorch-ada/blob/master/adalib/ada/models/modules.py
 """
 
+import torch
 import torch.nn as nn
 
 from kale.embed.video_i3d import Unit3D
 
 
 # Previously FFSoftmaxClassifier
 class SoftmaxNet(nn.Module):
@@ -55,15 +55,35 @@
             return f"{self.name}: {self.hidden_sizes}x{self._activation_fn.__name__}xLin"
         return f"{self.name}: Linear"
 
     def n_classes(self):
         return self._n_classes
 
 
-# Previously DataClassifierDigits
+class ClassNet(nn.Module):
+    """Simple classification prediction-head block to plug ontop of the 4D output of a CNN.
+
+    Args:
+        n_class (int, optional): the number of different classes that can be predicted. Defaults to 10.
+        input_shape (tuples, optional): the shape that input to this head will have. Expected
+                      to be (batch_size, channels, height, width). Defaults to (-1, 64, 8, 8).
+    """
+
+    def __init__(self, n_class=10, input_shape=(-1, 64, 8, 8)):
+        super(ClassNet, self).__init__()
+        self.avgpool = nn.AvgPool2d(input_shape[2])
+        self.linear = nn.Linear(input_shape[1], n_class)
+
+    def forward(self, x):
+        x = self.avgpool(x)
+        x = torch.flatten(x, 1)
+        x = self.linear(x)
+        return x
+
+
 class ClassNetSmallImage(nn.Module):
     """Regular classifier network for small-size images
 
     Args:
         input_size (int, optional): the dimension of the final feature vector. Defaults to 128.
         n_class (int, optional): the number of classes. Defaults to 10.
     """
@@ -86,15 +106,14 @@
     def forward(self, input):
         x = self.dp1(self.relu1(self.bn1(self.fc1(input))))
         x = self.relu2(self.bn2(self.fc2(x)))
         x = self.fc3(x)
         return x
 
 
-# Previously DomainClassifierDigits
 class DomainNetSmallImage(nn.Module):
     """Domain classifier network for small-size images
 
     Args:
         input_size (int, optional): the dimension of the final feature vector. Defaults to 128.
         bigger_discrim (bool, optional): whether to use deeper network. Defaults to False.
     """
```

### Comparing `pykale-0.1.1/kale/predict/isonet.py` & `pykale-0.1.2/kale/predict/isonet.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/predict/losses.py` & `pykale-0.1.2/kale/predict/losses.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,39 +4,44 @@
 
 import torch
 import torch.nn as nn
 from torch.autograd import grad
 from torch.nn import functional as F
 
 
-def cross_entropy_logits(linear_output, label, weights=None):
+def cross_entropy_logits(output, target, weights=None):
     """Computes cross entropy with logits
 
+    Args:
+        output (Tensor): The output of the last layer of the network, before softmax.
+        target (Tensor): The ground truth label.
+        weights (Tensor, optional): The weight of each sample. Defaults to None.
+
     Examples:
         See DANN, WDGRL, and MMD trainers in kale.pipeline.domain_adapter
     """
 
-    class_output = F.log_softmax(linear_output, dim=1)
+    class_output = F.log_softmax(output, dim=1)
     max_class = class_output.max(1)
     y_hat = max_class[1]  # get the index of the max log-probability
-    correct = y_hat.eq(label.view(label.size(0)).type_as(y_hat))
+    correct = y_hat.eq(target.view(target.size(0)).type_as(y_hat))
     if weights is None:
-        loss = nn.NLLLoss()(class_output, label.type_as(y_hat).view(label.size(0)))
+        loss = nn.NLLLoss()(class_output, target.type_as(y_hat).view(target.size(0)))
     else:
-        losses = nn.NLLLoss(reduction="none")(class_output, label.type_as(y_hat).view(label.size(0)))
+        losses = nn.NLLLoss(reduction="none")(class_output, target.type_as(y_hat).view(target.size(0)))
         loss = torch.sum(weights * losses) / torch.sum(weights)
     return loss, correct
 
 
 def topk_accuracy(output, target, topk=(1,)):
     """Computes the top-k accuracy for the specified values of k.
 
     Args:
-        output (Tensor): Generated predictions. Shape: (batch_size, class_count).
-        target (Tensor): Ground truth. Shape: (batch_size)
+        output (Tensor): output (Tensor): The output of the last layer of the network, before softmax. Shape: (batch_size, class_count).
+        target (Tensor): The ground truth label. Shape: (batch_size)
         topk (tuple(int)): Compute accuracy at top-k for the values of k specified in this parameter.
     Returns:
         list(Tensor): A list of tensors of the same length as topk.
         Each tensor consists of boolean variables to show if this prediction ranks top k with each value of k.
         True means the prediction ranks top k and False means not.
         The shape of tensor is batch_size, i.e. the number of predictions.
```

### Comparing `pykale-0.1.1/kale/prepdata/chem_transform.py` & `pykale-0.1.2/kale/prepdata/chem_transform.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/prepdata/image_transform.py` & `pykale-0.1.2/kale/prepdata/image_transform.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/prepdata/supergraph_construct.py` & `pykale-0.1.2/kale/prepdata/supergraph_construct.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/prepdata/tensor_reshape.py` & `pykale-0.1.2/kale/prepdata/tensor_reshape.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/prepdata/video_transform.py` & `pykale-0.1.2/kale/prepdata/video_transform.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/utils/download.py` & `pykale-0.1.2/kale/utils/download.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/utils/logger.py` & `pykale-0.1.2/kale/utils/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,30 +12,49 @@
     Returns:
         string: A string to be used in a file name.
     """
     date = str(datetime.datetime.now().strftime("%Y%d%m_%H%M%S"))
     return f"log-{date}-{str(uuid.uuid4())}"
 
 
-def construct_logger(name, save_dir):
-    """Constructs a logger. Saves the output as a text file at a specified path. Also saves the output of `git diff HEAD` to the same folder.
+def construct_logger(name, save_dir, log_to_terminal=False):
+    """
+    Constructs a logger that saves the output as a text file and optionally logs to the terminal.
 
-    Reference: https://docs.python.org/3/library/logging.html
+    The logger is configured to output messages at the DEBUG level, and it saves the output as a text file with a name
+    based on the current timestamp and the specified name. It also saves the output of `git diff HEAD` to a file with
+    the same name and the extension `.gitdiff.patch`.
 
     Args:
-        name (str): the logger name, typically the method name
-        save_dir (str): the path to save the log file (.txt)
+        name (str): The name of the logger, typically the name of the method being logged.
+        save_dir (str): The directory where the log file and git diff file will be saved.
+        log_to_terminal (bool, optional): Whether to also log messages to the terminal. Defaults to False.
+
+    Returns:
+        logging.Logger: The constructed logger.
+
+    Reference:
+        https://docs.python.org/3/library/logging.html
+
+    Raises:
+        None.
     """
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
 
     file_no_ext = out_file_core()
 
     fh = logging.FileHandler(os.path.join(save_dir, file_no_ext + ".txt"), encoding="utf-8")
     fh.setLevel(logging.DEBUG)
     formatter = logging.Formatter("%(asctime)s %(name)s %(levelname)s: %(message)s")
     fh.setFormatter(formatter)
     logger.addHandler(fh)
     gitdiff_patch = os.path.join(save_dir, file_no_ext + ".gitdiff.patch")
     os.system(f"git diff HEAD > {gitdiff_patch}")
 
+    if log_to_terminal:
+        ch = logging.StreamHandler()
+        ch.setLevel(logging.INFO)
+        ch.setFormatter(formatter)
+        logger.addHandler(ch)
+
     return logger
```

### Comparing `pykale-0.1.1/kale/utils/print.py` & `pykale-0.1.2/kale/utils/print.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/kale/utils/seed.py` & `pykale-0.1.2/kale/utils/seed.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/pykale.egg-info/PKG-INFO` & `pykale-0.1.2/pykale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykale
-Version: 0.1.1
+Version: 0.1.2
 Summary: Knowledge-aware machine learning from multiple sources in Python
 Home-page: https://github.com/pykale/pykale
 Author: The PyKale team
 Author-email: pykale-group@sheffield.ac.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pykale/pykale/issues
 Project-URL: Documentation, https://pykale.readthedocs.io
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: graph
 Provides-Extra: image
 Provides-Extra: example
 Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
@@ -41,15 +41,15 @@
 
 -----------------------------------------
 
 <!-- Keep badges to just ONE line, i.e. only the most important badges! -->
 [![tests](https://github.com/pykale/pykale/workflows/test/badge.svg)](https://github.com/pykale/pykale/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/pykale/pykale/branch/main/graph/badge.svg?token=jmIYPbA2le)](https://codecov.io/gh/pykale/pykale)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/optuna/optuna)
-[![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org)
 [![PyPI version](https://img.shields.io/pypi/v/pykale?color=blue)](https://pypi.org/project/pykale/)
 [![PyPI downloads](https://pepy.tech/badge/pykale)](https://pepy.tech/project/pykale)
 <!-- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5557244.svg)](https://doi.org/10.5281/zenodo.5557244) -->
 
 [Getting Started](https://github.com/pykale/pykale#how-to-use) |
 [Documentation](https://pykale.readthedocs.io/) |
 [Contributing](https://github.com/pykale/pykale/blob/main/.github/CONTRIBUTING.md) |
@@ -76,15 +76,15 @@
 
 - `examples` demonstrate real applications on specific datasets with a standardized structure.
 
 ## How to Use
 
 ### Step 0: Installation
 
-PyKale supports Python 3.7, 3.8, or 3.9. Before installing `pykale`, we suggest you to first [install PyTorch](https://pytorch.org/get-started/locally/) matching your hardware, and if graphs will be used, install [PyTorch Geometric](https://github.com/rusty1s/pytorch_geometric) following its [official instructions](https://github.com/rusty1s/pytorch_geometric#installation).
+PyKale supports Python 3.8, 3.9, or 3.10. Before installing `pykale`, we suggest you to first [install PyTorch](https://pytorch.org/get-started/locally/) matching your hardware, and if graphs will be used, install [PyTorch Geometric](https://github.com/rusty1s/pytorch_geometric) following its [official instructions](https://github.com/rusty1s/pytorch_geometric#installation).
 
 Simple installation of `pykale` from [PyPI](https://pypi.org/project/pykale/):
 
 ```bash
 pip install pykale
 ```
```

### Comparing `pykale-0.1.1/pykale.egg-info/SOURCES.txt` & `pykale-0.1.2/pykale.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 examples/bindingdb_deepdta/config.py
 examples/bindingdb_deepdta/main.py
 examples/bindingdb_deepdta/model.py
 examples/cifar_cnntransformer/__init__.py
 examples/cifar_cnntransformer/config.py
 examples/cifar_cnntransformer/main.py
 examples/cifar_cnntransformer/model.py
-examples/cifar_cnntransformer/trainer.py
 examples/cifar_isonet/__init__.py
 examples/cifar_isonet/config.py
 examples/cifar_isonet/main.py
 examples/cifar_isonet/model.py
 examples/cifar_isonet/trainer.py
 examples/cmri_mpca/__init__.py
 examples/cmri_mpca/config.py
@@ -36,16 +35,14 @@
 examples/office_multisource_adapt/config.py
 examples/office_multisource_adapt/main.py
 examples/office_multisource_adapt/model.py
 examples/polypharmacy_gripnet/__init__.py
 examples/polypharmacy_gripnet/config.py
 examples/polypharmacy_gripnet/main.py
 examples/polypharmacy_gripnet/model.py
-examples/polypharmacy_gripnet/trainer.py
-examples/polypharmacy_gripnet/utils.py
 examples/toy_domain_adaptation/__init__.py
 examples/toy_domain_adaptation/main.py
 kale/__init__.py
 kale/embed/__init__.py
 kale/embed/attention_cnn.py
 kale/embed/factorization.py
 kale/embed/gcn.py
@@ -65,34 +62,37 @@
 kale/interpret/model_weights.py
 kale/interpret/visualize.py
 kale/loaddata/__init__.py
 kale/loaddata/dataset_access.py
 kale/loaddata/image_access.py
 kale/loaddata/mnistm.py
 kale/loaddata/multi_domain.py
+kale/loaddata/polypharmacy_datasets.py
 kale/loaddata/sampler.py
 kale/loaddata/tdc_datasets.py
 kale/loaddata/usps.py
 kale/loaddata/video_access.py
 kale/loaddata/video_datasets.py
 kale/loaddata/video_multi_domain.py
 kale/loaddata/videos.py
 kale/pipeline/__init__.py
+kale/pipeline/base_nn_trainer.py
 kale/pipeline/deepdta.py
 kale/pipeline/domain_adapter.py
 kale/pipeline/mpca_trainer.py
 kale/pipeline/multi_domain_adapter.py
 kale/pipeline/video_domain_adapter.py
 kale/predict/__init__.py
 kale/predict/class_domain_nets.py
 kale/predict/decode.py
 kale/predict/isonet.py
 kale/predict/losses.py
 kale/prepdata/__init__.py
 kale/prepdata/chem_transform.py
+kale/prepdata/graph_negative_sampling.py
 kale/prepdata/image_transform.py
 kale/prepdata/supergraph_construct.py
 kale/prepdata/tensor_reshape.py
 kale/prepdata/video_transform.py
 kale/utils/__init__.py
 kale/utils/download.py
 kale/utils/logger.py
```

### Comparing `pykale-0.1.1/pykale.egg-info/requires.txt` & `pykale-0.1.2/pykale.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 numpy>=1.18.0
 pandas
 pytorch-lightning<=1.6.5,>=1.3.0
 scikit-learn>=0.23.2
 scipy>=1.5.4
-tensorly>=0.5.1
+tensorly<=0.7.0,>=0.5.1
 torch>=1.11.0
 torchvision>=0.12.0
 
 [dev]
 networkx
-PyTDC
+PyTDC<=0.3.6
 glob2
 pydicom
 pylibjpeg
 python-gdcm
 scikit-image>=0.16.2
 ipykernel
-ipython
+ipython<=8.12.0
 matplotlib<=3.5.2
-nilearn
+nilearn>=0.7.0
 Pillow
 PyTDC
 seaborn
 torchsummary>=1.5.0
 yacs>=0.1.7
 black==19.10b0
 coverage
@@ -41,44 +41,44 @@
 pytest-cov
 recommonmark
 sphinx
 sphinx-rtd-theme
 
 [example]
 ipykernel
-ipython
+ipython<=8.12.0
 matplotlib<=3.5.2
-nilearn
+nilearn>=0.7.0
 Pillow
 PyTDC
 seaborn
 torchsummary>=1.5.0
 yacs>=0.1.7
 
 [full]
 networkx
-PyTDC
+PyTDC<=0.3.6
 glob2
 pydicom
 pylibjpeg
 python-gdcm
 scikit-image>=0.16.2
 ipykernel
-ipython
+ipython<=8.12.0
 matplotlib<=3.5.2
-nilearn
+nilearn>=0.7.0
 Pillow
 PyTDC
 seaborn
 torchsummary>=1.5.0
 yacs>=0.1.7
 
 [graph]
 networkx
-PyTDC
+PyTDC<=0.3.6
 
 [image]
 glob2
 pydicom
 pylibjpeg
 python-gdcm
 scikit-image>=0.16.2
```

### Comparing `pykale-0.1.1/setup.cfg` & `pykale-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/setup.py` & `pykale-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # Core dependencies frequently used in PyKale Core API
 install_requires = [
     "numpy>=1.18.0",  # sure
     "pandas",  # sure
     "pytorch-lightning>=1.3.0,<=1.6.5",  # in pipeline API only
     "scikit-learn>=0.23.2",  # sure
     "scipy>=1.5.4",  # in factorization API only
-    "tensorly>=0.5.1",  # in factorization and model_weights API only
+    "tensorly>=0.5.1,<=0.7.0",  # in factorization and model_weights API only
     "torch>=1.11.0",  # sure
     "torchvision>=0.12.0",  # in download, sampler (NON-ideal), and vision API only
 ]
 
 # Application-specific dependencies sorted alphabetically below
 
 # Dependencies for graph analysis, e.g., for drug discovery using Therapeutics Data Commons (TDC)
 graph_requires = [
     "networkx",
-    "PyTDC",
+    "PyTDC<=0.3.6",
 ]
 
 # Dependencies for image analysis
 image_requires = [
     "glob2",
     "pydicom",
     "pylibjpeg",
@@ -43,17 +43,17 @@
 ]
 
 # End application-specific dependencies
 
 # Dependencies for all examples and tutorials
 example_requires = [
     "ipykernel",
-    "ipython",
+    "ipython<=8.12.0",  # IPython 8.13+ support Python 3.9+ only and IPython 8.0-8.12 supports Python 3.8+.
     "matplotlib<=3.5.2",
-    "nilearn",
+    "nilearn>=0.7.0",
     "Pillow",
     "PyTDC",
     "seaborn",
     "torchsummary>=1.5.0",
     "yacs>=0.1.7",
 ]
 
@@ -96,15 +96,14 @@
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
 readme = open("README.md").read()
 version = find_version("kale", "__init__.py")
 
-
 # Run the setup
 setup(
     name="pykale",
     version=version,
     description="Knowledge-aware machine learning from multiple sources in Python",
     long_description=readme,
     long_description_content_type="text/markdown",
@@ -113,15 +112,15 @@
     author_email="pykale-group@sheffield.ac.uk",
     project_urls={
         "Bug Tracker": "https://github.com/pykale/pykale/issues",
         "Documentation": "https://pykale.readthedocs.io",
         "Source": "https://github.com/pykale/pykale",
     },
     packages=find_packages(exclude=("docs", "examples", "tests")),
-    python_requires=">=3.7,<3.10",
+    python_requires=">=3.8,<3.11",
     install_requires=install_requires,
     extras_require={
         "graph": graph_requires,
         "image": image_requires,
         "example": example_requires,
         "full": full_requires,
         "dev": dev_requires,
```

### Comparing `pykale-0.1.1/tests/helpers/boring_model.py` & `pykale-0.1.2/tests/helpers/boring_model.py`

 * *Files identical despite different names*

### Comparing `pykale-0.1.1/tests/helpers/pipe_test_helper.py` & `pykale-0.1.2/tests/helpers/pipe_test_helper.py`

 * *Files identical despite different names*

