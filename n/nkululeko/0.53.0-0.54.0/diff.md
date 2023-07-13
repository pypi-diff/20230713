# Comparing `tmp/nkululeko-0.53.0.tar.gz` & `tmp/nkululeko-0.54.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.53.0.tar", last modified: Tue Jul 11 17:20:59 2023, max compression
+gzip compressed data, was "nkululeko-0.54.0.tar", last modified: Thu Jul 13 17:31:00 2023, max compression
```

## Comparing `nkululeko-0.53.0.tar` & `nkululeko-0.54.0.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-11 17:20:59.162757 nkululeko-0.53.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7166 2023-07-11 17:19:19.000000 nkululeko-0.53.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.53.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18965 2023-07-11 17:20:59.162757 nkululeko-0.53.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.53.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-11 17:20:59.158756 nkululeko-0.53.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.53.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.53.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.53.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.53.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.53.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-11 17:19:50.000000 nkululeko-0.53.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.53.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.53.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.53.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.53.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.53.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21808 2023-07-11 17:10:58.000000 nkululeko-0.53.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.53.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.53.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.53.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.53.0/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.53.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.53.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.53.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.53.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.53.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.53.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.53.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.53.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.53.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.53.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.53.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3510 2023-07-11 17:13:59.000000 nkululeko-0.53.0/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6717 2023-07-11 16:16:04.000000 nkululeko-0.53.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.53.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.53.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.53.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.53.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.53.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.53.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.53.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.53.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.53.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.53.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.53.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.53.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.53.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.53.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.53.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.53.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.53.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.53.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.53.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.53.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.53.0/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.53.0/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.53.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.53.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.53.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.53.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.53.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.53.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.53.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10463 2023-07-06 09:40:02.000000 nkululeko-0.53.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-11 17:20:59.162757 nkululeko-0.53.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18965 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1675 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-11 17:20:59.000000 nkululeko-0.53.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.53.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-11 17:20:59.162757 nkululeko-0.53.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.53.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-13 17:31:00.682561 nkululeko-0.54.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7285 2023-07-13 17:27:18.000000 nkululeko-0.54.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.54.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19069 2023-07-13 17:31:00.682561 nkululeko-0.54.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11232 2023-07-12 17:10:33.000000 nkululeko-0.54.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-13 17:31:00.682561 nkululeko-0.54.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.54.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.54.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.54.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.54.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.54.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-13 17:01:55.000000 nkululeko-0.54.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.54.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.54.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.54.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.54.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.54.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21808 2023-07-11 17:10:58.000000 nkululeko-0.54.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.54.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2751 2023-07-13 17:19:32.000000 nkululeko-0.54.0/nkululeko/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2832 2023-07-13 17:19:11.000000 nkululeko-0.54.0/nkululeko/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.54.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2750 2023-07-13 17:19:46.000000 nkululeko-0.54.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2741 2023-07-13 17:20:04.000000 nkululeko-0.54.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.54.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.54.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.54.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.54.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.54.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.54.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.54.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.54.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3935 2023-07-13 17:17:52.000000 nkululeko-0.54.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.54.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.54.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3510 2023-07-11 17:13:59.000000 nkululeko-0.54.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6717 2023-07-11 16:16:04.000000 nkululeko-0.54.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.54.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.54.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.54.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.54.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.54.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.54.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.54.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.54.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.54.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.54.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.54.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.54.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.54.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.54.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.54.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.54.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.54.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.54.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.54.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.54.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.54.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.54.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.54.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.54.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.54.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.54.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.54.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.54.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.54.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10463 2023-07-06 09:40:02.000000 nkululeko-0.54.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-13 17:31:00.682561 nkululeko-0.54.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19069 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1737 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.54.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-13 17:31:00.682561 nkululeko-0.54.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.54.0/setup.py
```

### Comparing `nkululeko-0.53.0/CHANGELOG.md` & `nkululeko-0.54.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.54.0
+--------------
+* added audeering public age and gender model embeddings and age and gender predictions
+
 Version 0.53.0
 --------------
 * added file checks: size in bytes and voice activity detection with silero
 
 Version 0.52.1
 --------------
 * bugfix: min/max duration_of_sample was not working
```

### Comparing `nkululeko-0.53.0/LICENSE` & `nkululeko-0.54.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/PKG-INFO` & `nkululeko-0.54.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.53.0
+Version: 0.54.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
  
 ## Overview
 A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
 The idea is to have a framework (based on e.g. sklearn and torch) that can be used to rapidly and automatically analyse and investigate audio data automatically.
 
 * New [We started a slack channel to discuss issues related to nkululeko](https://join.slack.com/t/nkululekoworkspace/shared_invite/zt-1wtvbxtwz-P5YoRJq8whxKSee86ebhJg). Please click the link if interested in contributing.
-* The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
+* The latest features can be seen in [the ini-file](./ini_file.md) options that are used to control Nkululeko
 * Below is a [Hello World example](#helloworld) that should set you up fastly, also on [Google Colab](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
@@ -62,15 +62,15 @@
 <img src="meta/images/tsne.png" width="500px"/>
 
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
 <img src="meta/images/data_plot.png" width="500px"/>
 
-## Installation
+## Installatione
 
 Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
 
 Some examples for *ini*-files (which you use to control nkululeko) are in the [tests folder](https://github.com/felixbur/nkululeko/tree/main/tests).
@@ -211,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.54.0
+--------------
+* added audeering public age and gender model embeddings and age and gender predictions
+
 Version 0.53.0
 --------------
 * added file checks: size in bytes and voice activity detection with silero
 
 Version 0.52.1
 --------------
 * bugfix: min/max duration_of_sample was not working
```

### Comparing `nkululeko-0.53.0/README.md` & `nkululeko-0.54.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  
 ## Overview
 A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
 The idea is to have a framework (based on e.g. sklearn and torch) that can be used to rapidly and automatically analyse and investigate audio data automatically.
 
 * New [We started a slack channel to discuss issues related to nkululeko](https://join.slack.com/t/nkululekoworkspace/shared_invite/zt-1wtvbxtwz-P5YoRJq8whxKSee86ebhJg). Please click the link if interested in contributing.
-* The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
+* The latest features can be seen in [the ini-file](./ini_file.md) options that are used to control Nkululeko
 * Below is a [Hello World example](#helloworld) that should set you up fastly, also on [Google Colab](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
@@ -46,15 +46,15 @@
 <img src="meta/images/tsne.png" width="500px"/>
 
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
 <img src="meta/images/data_plot.png" width="500px"/>
 
-## Installation
+## Installatione
 
 Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
 
 Some examples for *ini*-files (which you use to control nkululeko) are in the [tests folder](https://github.com/felixbur/nkululeko/tree/main/tests).
```

### Comparing `nkululeko-0.53.0/nkululeko/augment.py` & `nkululeko-0.54.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/augmenter.py` & `nkululeko-0.54.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/cacheddataset.py` & `nkululeko-0.54.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/dataset.py` & `nkululeko-0.54.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/dataset_csv.py` & `nkululeko-0.54.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.54.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/demo.py` & `nkululeko-0.54.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/demo_predictor.py` & `nkululeko-0.54.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/experiment.py` & `nkululeko-0.54.0/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/explore.py` & `nkululeko-0.54.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_analyser.py` & `nkululeko-0.54.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_audmodel.py` & `nkululeko-0.54.0/nkululeko/feats_audmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path('store')
         store_format = self.util.config_val('FEATS', 'store_format', 'pkl')
         storage = f'{store}{self.name}.{store_format}'
         extract = eval(self.util.config_val('FEATS', 'needs_feature_extraction', 'False'))
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
         if no_reuse or extract or not os.path.isfile(storage):
-            self.util.debug('extracting audmodel features, this might take a while...')
+            self.util.debug('extracting audmodel embeddings, this might take a while...')
             hidden_states = audinterface.Feature(
                 self.model.labels('hidden_states'),
                 process_func=self.model,
                 process_func_args={
                     'outputs': 'hidden_states',
                 },
                 sampling_rate=16000,
```

### Comparing `nkululeko-0.53.0/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.54.0/nkululeko/feats_audmodel_dim.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,14 @@
             self.df = logits.process_index(self.data_df.index)
             self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'False'
             except KeyError:
                 pass
         else:
-            self.util.debug('reusing extracted audmodel features.')
+            self.util.debug('reusing extracted audmodel dimensions.')
             self.df = self.util.get_store(storage, store_format)
 
 
     def extract_sample(self, signal, sr):
         result = self.model(signal, sr)
         return np.asarray(result['hidden_states'].flatten())
```

### Comparing `nkululeko-0.53.0/nkululeko/feats_clap.py` & `nkululeko-0.54.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_import.py` & `nkululeko-0.54.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_mld.py` & `nkululeko-0.54.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_opensmile.py` & `nkululeko-0.54.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_oxbow.py` & `nkululeko-0.54.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_praat.py` & `nkululeko-0.54.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_trill.py` & `nkululeko-0.54.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.54.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feature_extractor.py` & `nkululeko-0.54.0/nkululeko/feature_extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,20 @@
                 self.featExtractor = Wav2vec2(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='audmodel':
                 from nkululeko.feats_audmodel import AudModelSet
                 self.featExtractor = AudModelSet(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='auddim':
                 from nkululeko.feats_audmodel_dim import AudModelDimSet
                 self.featExtractor = AudModelDimSet(f'{store_name}_{self.feats_designation}', self.data_df)
+            elif feats_type=='agender':
+                from nkululeko.feats_agender import AudModelAgenderSet
+                self.featExtractor = AudModelAgenderSet(f'{store_name}_{self.feats_designation}', self.data_df)
+            elif feats_type=='agender_agender':
+                from nkululeko.feats_agender_agender import AgenderAgenderSet
+                self.featExtractor = AgenderAgenderSet(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='clap':
                 from nkululeko.feats_clap import Clap
                 self.featExtractor = Clap(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='praat':
                 from nkululeko.feats_praat import Praatset
                 self.featExtractor = Praatset(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='mld':
```

### Comparing `nkululeko-0.53.0/nkululeko/featureset.py` & `nkululeko-0.54.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/feinberg_praat.py` & `nkululeko-0.54.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/file_checker.py` & `nkululeko-0.54.0/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/filter_data.py` & `nkululeko-0.54.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/loss_ccc.py` & `nkululeko-0.54.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.54.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model.py` & `nkululeko-0.54.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_cnn.py` & `nkululeko-0.54.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_gmm.py` & `nkululeko-0.54.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_knn.py` & `nkululeko-0.54.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_knn_reg.py` & `nkululeko-0.54.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_mlp.py` & `nkululeko-0.54.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.54.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/model_svm.py` & `nkululeko-0.54.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/modelrunner.py` & `nkululeko-0.54.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/nkululeko.py` & `nkululeko-0.54.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/plots.py` & `nkululeko-0.54.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/randomsplicer.py` & `nkululeko-0.54.0/nkululeko/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/randomsplicing.py` & `nkululeko-0.54.0/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/reporter.py` & `nkululeko-0.54.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/runmanager.py` & `nkululeko-0.54.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/scaler.py` & `nkululeko-0.54.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.54.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/test.py` & `nkululeko-0.54.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/test_predictor.py` & `nkululeko-0.54.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko/util.py` & `nkululeko-0.54.0/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.53.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.54.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.53.0
+Version: 0.54.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
  
 ## Overview
 A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
 The idea is to have a framework (based on e.g. sklearn and torch) that can be used to rapidly and automatically analyse and investigate audio data automatically.
 
 * New [We started a slack channel to discuss issues related to nkululeko](https://join.slack.com/t/nkululekoworkspace/shared_invite/zt-1wtvbxtwz-P5YoRJq8whxKSee86ebhJg). Please click the link if interested in contributing.
-* The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
+* The latest features can be seen in [the ini-file](./ini_file.md) options that are used to control Nkululeko
 * Below is a [Hello World example](#helloworld) that should set you up fastly, also on [Google Colab](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
@@ -62,15 +62,15 @@
 <img src="meta/images/tsne.png" width="500px"/>
 
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
 <img src="meta/images/data_plot.png" width="500px"/>
 
-## Installation
+## Installatione
 
 Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
 
 Some examples for *ini*-files (which you use to control nkululeko) are in the [tests folder](https://github.com/felixbur/nkululeko/tree/main/tests).
@@ -211,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.54.0
+--------------
+* added audeering public age and gender model embeddings and age and gender predictions
+
 Version 0.53.0
 --------------
 * added file checks: size in bytes and voice activity detection with silero
 
 Version 0.52.1
 --------------
 * bugfix: min/max duration_of_sample was not working
```

### Comparing `nkululeko-0.53.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.54.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 nkululeko/dataset.py
 nkululeko/dataset_csv.py
 nkululeko/dataset_ravdess.py
 nkululeko/demo.py
 nkululeko/demo_predictor.py
 nkululeko/experiment.py
 nkululeko/explore.py
+nkululeko/feats_agender.py
+nkululeko/feats_agender_agender.py
 nkululeko/feats_analyser.py
 nkululeko/feats_audmodel.py
 nkululeko/feats_audmodel_dim.py
 nkululeko/feats_clap.py
 nkululeko/feats_import.py
 nkululeko/feats_mld.py
 nkululeko/feats_opensmile.py
```

### Comparing `nkululeko-0.53.0/setup.cfg` & `nkululeko-0.54.0/setup.cfg`

 * *Files identical despite different names*

