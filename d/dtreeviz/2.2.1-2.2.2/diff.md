# Comparing `tmp/dtreeviz-2.2.1.tar.gz` & `tmp/dtreeviz-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtreeviz-2.2.1.tar", last modified: Sun Apr 16 16:37:49 2023, max compression
+gzip compressed data, was "dtreeviz-2.2.2.tar", last modified: Thu Jul 13 17:21:05 2023, max compression
```

## Comparing `dtreeviz-2.2.1.tar` & `dtreeviz-2.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.908134 dtreeviz-2.2.1/
--rw-r--r--   0 parrt      (501) staff       (20)     1069 2021-12-03 22:37:44.000000 dtreeviz-2.2.1/LICENSE
--rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-04-16 16:37:49.908216 dtreeviz-2.2.1/PKG-INFO
--rw-r--r--   0 parrt      (501) staff       (20)    16124 2023-04-16 16:36:09.000000 dtreeviz-2.2.1/README.md
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.899041 dtreeviz-2.2.1/dtreeviz/
--rw-r--r--   0 parrt      (501) staff       (20)      596 2022-12-27 19:55:14.000000 dtreeviz-2.2.1/dtreeviz/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)    24724 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/classifiers.py
--rw-r--r--   0 parrt      (501) staff       (20)     4174 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/colors.py
--rw-r--r--   0 parrt      (501) staff       (20)    35384 2023-04-16 16:35:55.000000 dtreeviz-2.2.1/dtreeviz/compatibility.py
--rw-r--r--   0 parrt      (501) staff       (20)     6498 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/interpretation.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.901026 dtreeviz-2.2.1/dtreeviz/models/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2020-07-11 17:37:37.000000 dtreeviz-2.2.1/dtreeviz/models/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)     8271 2023-02-09 18:22:21.000000 dtreeviz-2.2.1/dtreeviz/models/lightgbm_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)    22221 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/dtreeviz/models/shadow_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     5254 2023-04-16 16:35:55.000000 dtreeviz-2.2.1/dtreeviz/models/sklearn_decision_trees.py
--rw-r--r--   0 parrt      (501) staff       (20)     8735 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/models/spark_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     8460 2023-02-09 18:22:21.000000 dtreeviz-2.2.1/dtreeviz/models/tensorflow_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     8979 2023-02-09 18:22:21.000000 dtreeviz-2.2.1/dtreeviz/models/xgb_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     3780 2023-01-29 18:56:38.000000 dtreeviz-2.2.1/dtreeviz/t3.py
--rw-r--r--   0 parrt      (501) staff       (20)    90581 2023-04-16 16:35:55.000000 dtreeviz-2.2.1/dtreeviz/trees.py
--rw-r--r--   0 parrt      (501) staff       (20)    17511 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/dtreeviz/utils.py
--rw-r--r--   0 parrt      (501) staff       (20)     1099 2023-04-16 16:36:09.000000 dtreeviz-2.2.1/dtreeviz/version.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.899726 dtreeviz-2.2.1/dtreeviz.egg-info/
--rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/PKG-INFO
--rw-r--r--   0 parrt      (501) staff       (20)     1659 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/SOURCES.txt
--rw-r--r--   0 parrt      (501) staff       (20)        1 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/dependency_links.txt
--rw-r--r--   0 parrt      (501) staff       (20)      243 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/requires.txt
--rw-r--r--   0 parrt      (501) staff       (20)       17 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/top_level.txt
--rw-r--r--   0 parrt      (501) staff       (20)       79 2023-04-16 16:37:49.908602 dtreeviz-2.2.1/setup.cfg
--rw-r--r--   0 parrt      (501) staff       (20)     2579 2023-04-16 16:36:09.000000 dtreeviz-2.2.1/setup.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.906061 dtreeviz-2.2.1/testing/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)     1878 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/animate_rtree_bivar_3D.py
--rw-r--r--   0 parrt      (501) staff       (20)     1754 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/cancer.py
--rw-r--r--   0 parrt      (501) staff       (20)     7263 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/gen_feature_space_samples.py
--rw-r--r--   0 parrt      (501) staff       (20)    13771 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/gen_samples.py
--rw-r--r--   0 parrt      (501) staff       (20)     1973 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/iris.py
--rw-r--r--   0 parrt      (501) staff       (20)     1861 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/paper_examples.py
--rw-r--r--   0 parrt      (501) staff       (20)      703 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_ctree.py
--rw-r--r--   0 parrt      (501) staff       (20)      724 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_ctree_bivar.py
--rw-r--r--   0 parrt      (501) staff       (20)     2247 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/play_lightgbm.py
--rw-r--r--   0 parrt      (501) staff       (20)      550 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_rtree.py
--rw-r--r--   0 parrt      (501) staff       (20)      817 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_rtree_bivar_3D.py
--rw-r--r--   0 parrt      (501) staff       (20)      565 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_rtree_bivar_heatmap.py
--rw-r--r--   0 parrt      (501) staff       (20)     3068 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/play_spark.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.906225 dtreeviz-2.2.1/testing/testlib/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/testlib/__init__.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.907968 dtreeviz-2.2.1/testing/testlib/models/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/testlib/models/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)     1129 2022-09-25 19:55:25.000000 dtreeviz-2.2.1/testing/testlib/models/conftest.py
--rw-r--r--   0 parrt      (501) staff       (20)     3879 2021-03-30 18:20:29.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_lightgbm_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     7608 2022-09-25 19:55:25.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_spark_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     4051 2022-12-27 19:55:15.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_tensorflow_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     2161 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_xgb_regressor.py
--rw-r--r--   0 parrt      (501) staff       (20)     7565 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     2467 2022-12-27 19:55:15.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_pipeline.py
--rw-r--r--   0 parrt      (501) staff       (20)     3887 2022-02-24 22:21:33.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_xgb_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     7207 2023-02-20 19:59:16.000000 dtreeviz-2.2.1/testing/testone.py
--rw-r--r--   0 parrt      (501) staff       (20)     2412 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf-catvars.py
--rw-r--r--   0 parrt      (501) staff       (20)     1897 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf_catvars2.py
--rw-r--r--   0 parrt      (501) staff       (20)     1788 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf_catvars3.py
--rw-r--r--   0 parrt      (501) staff       (20)     1941 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf_regr_catvars.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.978103 dtreeviz-2.2.2/
+-rw-r--r--   0 parrt      (501) staff       (20)     1069 2021-12-03 22:37:44.000000 dtreeviz-2.2.2/LICENSE
+-rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-07-13 17:21:05.978189 dtreeviz-2.2.2/PKG-INFO
+-rw-r--r--   0 parrt      (501) staff       (20)    16354 2023-07-13 17:11:52.000000 dtreeviz-2.2.2/README.md
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.971814 dtreeviz-2.2.2/dtreeviz/
+-rw-r--r--   0 parrt      (501) staff       (20)      596 2022-12-27 19:55:14.000000 dtreeviz-2.2.2/dtreeviz/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)    24724 2023-01-16 21:32:12.000000 dtreeviz-2.2.2/dtreeviz/classifiers.py
+-rw-r--r--   0 parrt      (501) staff       (20)     4174 2023-01-16 21:32:12.000000 dtreeviz-2.2.2/dtreeviz/colors.py
+-rw-r--r--   0 parrt      (501) staff       (20)    35384 2023-04-16 16:35:55.000000 dtreeviz-2.2.2/dtreeviz/compatibility.py
+-rw-r--r--   0 parrt      (501) staff       (20)     6498 2023-01-16 21:32:12.000000 dtreeviz-2.2.2/dtreeviz/interpretation.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.973907 dtreeviz-2.2.2/dtreeviz/models/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2020-07-11 17:37:37.000000 dtreeviz-2.2.2/dtreeviz/models/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8271 2023-02-09 18:22:21.000000 dtreeviz-2.2.2/dtreeviz/models/lightgbm_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)    22739 2023-07-13 17:11:16.000000 dtreeviz-2.2.2/dtreeviz/models/shadow_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     5255 2023-07-13 17:11:16.000000 dtreeviz-2.2.2/dtreeviz/models/sklearn_decision_trees.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8735 2023-01-16 21:32:12.000000 dtreeviz-2.2.2/dtreeviz/models/spark_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8778 2023-07-13 17:11:16.000000 dtreeviz-2.2.2/dtreeviz/models/tensorflow_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8979 2023-02-09 18:22:21.000000 dtreeviz-2.2.2/dtreeviz/models/xgb_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3780 2023-01-29 18:56:38.000000 dtreeviz-2.2.2/dtreeviz/t3.py
+-rw-r--r--   0 parrt      (501) staff       (20)    90853 2023-07-13 17:11:16.000000 dtreeviz-2.2.2/dtreeviz/trees.py
+-rw-r--r--   0 parrt      (501) staff       (20)    17511 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/dtreeviz/utils.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1099 2023-07-13 17:11:16.000000 dtreeviz-2.2.2/dtreeviz/version.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.972625 dtreeviz-2.2.2/dtreeviz.egg-info/
+-rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-07-13 17:21:05.000000 dtreeviz-2.2.2/dtreeviz.egg-info/PKG-INFO
+-rw-r--r--   0 parrt      (501) staff       (20)     1659 2023-07-13 17:21:05.000000 dtreeviz-2.2.2/dtreeviz.egg-info/SOURCES.txt
+-rw-r--r--   0 parrt      (501) staff       (20)        1 2023-07-13 17:21:05.000000 dtreeviz-2.2.2/dtreeviz.egg-info/dependency_links.txt
+-rw-r--r--   0 parrt      (501) staff       (20)      243 2023-07-13 17:21:05.000000 dtreeviz-2.2.2/dtreeviz.egg-info/requires.txt
+-rw-r--r--   0 parrt      (501) staff       (20)       17 2023-07-13 17:21:05.000000 dtreeviz-2.2.2/dtreeviz.egg-info/top_level.txt
+-rw-r--r--   0 parrt      (501) staff       (20)       79 2023-07-13 17:21:05.978477 dtreeviz-2.2.2/setup.cfg
+-rw-r--r--   0 parrt      (501) staff       (20)     2579 2023-07-13 17:11:16.000000 dtreeviz-2.2.2/setup.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.976615 dtreeviz-2.2.2/testing/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1878 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/animate_rtree_bivar_3D.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1754 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/cancer.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7263 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/gen_feature_space_samples.py
+-rw-r--r--   0 parrt      (501) staff       (20)    13771 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/gen_samples.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1973 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/iris.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1861 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/paper_examples.py
+-rw-r--r--   0 parrt      (501) staff       (20)      703 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/play_ctree.py
+-rw-r--r--   0 parrt      (501) staff       (20)      724 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/play_ctree_bivar.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2247 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/play_lightgbm.py
+-rw-r--r--   0 parrt      (501) staff       (20)      550 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/play_rtree.py
+-rw-r--r--   0 parrt      (501) staff       (20)      817 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/play_rtree_bivar_3D.py
+-rw-r--r--   0 parrt      (501) staff       (20)      565 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/play_rtree_bivar_heatmap.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3068 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/play_spark.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.976743 dtreeviz-2.2.2/testing/testlib/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/testlib/__init__.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-07-13 17:21:05.977973 dtreeviz-2.2.2/testing/testlib/models/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/testlib/models/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1129 2022-09-25 19:55:25.000000 dtreeviz-2.2.2/testing/testlib/models/conftest.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3879 2021-03-30 18:20:29.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_lightgbm_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7608 2022-09-25 19:55:25.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_spark_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     4051 2022-12-27 19:55:15.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_tensorflow_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2161 2021-02-05 19:09:10.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_xgb_regressor.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7565 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_trees_sk_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2467 2022-12-27 19:55:15.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_trees_sk_pipeline.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3887 2022-02-24 22:21:33.000000 dtreeviz-2.2.2/testing/testlib/models/test_decision_trees_xgb_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7207 2023-02-20 19:59:16.000000 dtreeviz-2.2.2/testing/testone.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2412 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/tf-catvars.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1897 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/tf_catvars2.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1788 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/tf_catvars3.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1941 2023-02-20 21:19:16.000000 dtreeviz-2.2.2/testing/tf_regr_catvars.py
```

### Comparing `dtreeviz-2.2.1/LICENSE` & `dtreeviz-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/PKG-INFO` & `dtreeviz-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtreeviz
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Python 3 library for sci-kit learn, XGBoost, LightGBM, Spark, and TensorFlow decision tree visualization
 Home-page: https://github.com/parrt/dtreeviz
 Author: Terence Parr, Tudor Lapusan, and Prince Grover
 Author-email: parrt@antlr.org
 License: MIT
 Keywords: machine-learning data structures trees visualization
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dtreeviz-2.2.1/README.md` & `dtreeviz-2.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -252,18 +252,26 @@
 cmd = ["dot", "-V"]
 stdout, stderr = be.run(cmd, capture_output=True, check=True, quiet=False)
 print( stderr )
 ```
 
 If you are having issues with run command you can try copying the following files from: https://github.com/xflr6/graphviz/tree/master/graphviz.
 
-Place them in the AppData\Local\Continuum\anaconda3\Lib\site-packages\graphviz folder. 
+Place them in the AppData\Local\Continuum\anaconda3\Lib\site-packages\graphviz folder.  
 
 Clean out the __pycache__ directory too.
 
+For graphviz windows install 8.0.5 and python interface v0.18+ :  
+```python
+import graphviz.backend as be
+cmd = ["dot", "-V"]
+stdout = be.execute.run_check(cmd, capture_output=True, check=True, quiet=False)
+print( stdout )
+```
+
 Jupyter Lab and Jupyter notebook both show the inline .svg images well.
 
 ### Verify graphviz installation
 
 Try making text file `t.dot` with content `digraph T { A -> B }` (paste that into a text editor, for example) and then running this from the command line:
 
 ```
@@ -282,15 +290,15 @@
 
 To push the `dtreeviz` library to your local egg cache (force updates) during development, do this (from anaconda prompt on Windows):
  
 ```bash 
 python setup.py install -f
 ```
 
-E.g., on Terence's box, it add `/Users/parrt/anaconda3/lib/python3.6/site-packages/dtreeviz-2.2.1-py3.6.egg`.
+E.g., on Terence's box, it add `/Users/parrt/anaconda3/lib/python3.6/site-packages/dtreeviz-2.2.2-py3.6.egg`.
 
 ## Feedback
 
 We welcome info from users on how they use dtreeviz, what features they'd like, etc... via [email (to parrt)](mailto:parrt@antlr.org) or via an [issue](https://github.com/parrt/dtreeviz/issues).
 
 ## Useful Resources
```

### Comparing `dtreeviz-2.2.1/dtreeviz/__init__.py` & `dtreeviz-2.2.2/dtreeviz/__init__.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/classifiers.py` & `dtreeviz-2.2.2/dtreeviz/classifiers.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/colors.py` & `dtreeviz-2.2.2/dtreeviz/colors.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/compatibility.py` & `dtreeviz-2.2.2/dtreeviz/compatibility.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/interpretation.py` & `dtreeviz-2.2.2/dtreeviz/interpretation.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/models/lightgbm_decision_tree.py` & `dtreeviz-2.2.2/dtreeviz/models/lightgbm_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/models/shadow_decision_tree.py` & `dtreeviz-2.2.2/dtreeviz/models/shadow_decision_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,23 +453,25 @@
             from dtreeviz.models import spark_decision_tree
             return spark_decision_tree.ShadowSparkTree(tree_model, X_train, y_train,
                                                        feature_names, target_name, class_names)
         elif "lightgbm.basic.Booster" in str(type(tree_model)):
             from dtreeviz.models import lightgbm_decision_tree
             return lightgbm_decision_tree.ShadowLightGBMTree(tree_model, tree_index, X_train, y_train,
                                                              feature_names, target_name, class_names)
-        elif "tensorflow_decision_forests.keras.RandomForestModel" in str(type(tree_model)):
+        elif any(tf_model in str(type(tree_model)) for tf_model in ["tensorflow_decision_forests.keras.RandomForestModel",
+                                                                    "tensorflow_decision_forests.keras.GradientBoostedTreesModel"]):
             from dtreeviz.models import tensorflow_decision_tree
             return tensorflow_decision_tree.ShadowTensorflowTree(tree_model, tree_index, X_train, y_train,
                                                                  feature_names, target_name, class_names)
         else:
             raise ValueError(
                 f"Tree model must be in (DecisionTreeRegressor, DecisionTreeClassifier, "
                 "xgboost.core.Booster, lightgbm.basic.Booster, pyspark DecisionTreeClassificationModel, "
-                f"pyspark DecisionTreeClassificationModel, tensorflow_decision_forests.keras.RandomForestModel) "
+                f"pyspark DecisionTreeClassificationModel, tensorflow_decision_forests.keras.RandomForestModel, "
+                f"tensorflow_decision_forests.keras.GradientBoostedTreesModel) "
                 f"but you passed a {tree_model.__class__.__name__}!")
 
 
 class ShadowDecTreeNode():
     """
     A node in a shadow tree. Each node has left and right pointers to child nodes, if any.
     As part of tree construction process, the samples examined at each decision node or at each leaf node are
@@ -556,14 +558,17 @@
         """
         If the tree model is a classifier and we know the class names, return the class name associated with the
         prediction for this leaf node.
 
         Return prediction class or value otherwise.
         """
         if self.isclassifier():
+            # In a GBT model, the trees are always regressive trees (even if the GBT is a classifier).
+            if "tensorflow_decision_forests.keras.GradientBoostedTreesModel" in str(type(self.shadow_tree.tree_model)):
+                return round(self.prediction(), 6)
             if self.shadow_tree.class_names is not None:
                 return self.shadow_tree.class_names[self.prediction()]
         return self.prediction()
 
     def class_counts(self) -> (List[int], None):
         """
         If this tree model is a classifier, return a list with the count associated with each class.
```

### Comparing `dtreeviz-2.2.1/dtreeviz/models/sklearn_decision_trees.py` & `dtreeviz-2.2.2/dtreeviz/models/sklearn_decision_trees.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,8 +143,8 @@
     def get_score(self):
         return self.tree_model.score(self.X_train, self.y_train)
 
     def get_min_samples_leaf(self):
         return self.tree_model.min_samples_leaf
 
     def shouldGoLeftAtSplit(self, id, x):
-        return x < self.get_node_split(id)
+        return x <= self.get_node_split(id)
```

### Comparing `dtreeviz-2.2.1/dtreeviz/models/spark_decision_tree.py` & `dtreeviz-2.2.2/dtreeviz/models/spark_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/models/tensorflow_decision_tree.py` & `dtreeviz-2.2.2/dtreeviz/models/tensorflow_decision_tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -156,14 +156,18 @@
         all_nodes = self.internal + self.leaves
         if self.is_classifier():
             node_value = [node.n_sample_classes() for node in all_nodes if node.id == id]
             return node_value[0]
 
     def get_prediction(self, id):
         if self.is_classifier():
+            # In a GBT model, the trees are always regressive trees (even if the GBT is a classifier). So we don't
+            # have the probability attribute
+            if "tensorflow_decision_forests.keras.GradientBoostedTreesModel" in str(type(self.model)):
+                return self.tree_nodes[id].value.value
             return np.argmax(self.tree_nodes[id].value.probability)
         else:
             return self.tree_nodes[id].value.value
 
     def is_categorical_split(self, id) -> bool:
         node_condition = self.tree_nodes[id].condition
```

### Comparing `dtreeviz-2.2.1/dtreeviz/models/xgb_decision_tree.py` & `dtreeviz-2.2.2/dtreeviz/models/xgb_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/t3.py` & `dtreeviz-2.2.2/dtreeviz/t3.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/trees.py` & `dtreeviz-2.2.2/dtreeviz/trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,64 +334,68 @@
         """
 
         def node_name(node: ShadowDecTreeNode) -> str:
             return f"node{node.id}"
 
         def split_node(name, node_name, split):
             if fancy:
+                filepath = os.path.join(tmp, f"node{node.id}_{os.getpid()}.svg")
                 labelgraph = node_label(node) if show_node_labels else ''
                 html = f"""<table border="0">
                     {labelgraph}
                     <tr>
-                            <td><img src="{tmp}/node{node.id}_{os.getpid()}.svg"/></td>
+                            <td><img src="{filepath}"/></td>
                     </tr>
                     </table>"""
             else:
                 html = f"""<font face="{fontname}" color="{colors["text"]}" point-size="12">{name}@{split}</font>"""
             if node.id in highlight_path:
                 gr_node = f'{node_name} [margin="0" shape=box penwidth=".5" color="{colors["highlight"]}" style="dashed" label=<{html}>]'
             else:
                 gr_node = f'{node_name} [margin="0" shape=none label=<{html}>]'
             return gr_node
 
         def regr_leaf_node(node, label_fontsize: int = 12):
             # always generate fancy regr leaves for now but shrink a bit for nonfancy.
             labelgraph = node_label(node) if show_node_labels else ''
+            filepath = os.path.join(tmp, f"leaf{node.id}_{os.getpid()}.svg")
             html = f"""<table border="0">
                 {labelgraph}
                 <tr>
-                        <td><img src="{tmp}/leaf{node.id}_{os.getpid()}.svg"/></td>
+                        <td><img src="{filepath}"/></td>
                 </tr>
                 </table>"""
             if node.id in highlight_path:
                 return f'leaf{node.id} [margin="0" shape=box penwidth=".5" color="{colors["highlight"]}" style="dashed" label=<{html}>]'
             else:
                 return f'leaf{node.id} [margin="0" shape=box penwidth="0" color="{colors["text"]}" label=<{html}>]'
 
         def class_leaf_node(node, label_fontsize: int = 12):
             labelgraph = node_label(node) if show_node_labels else ''
+            filepath = os.path.join(tmp, f"leaf{node.id}_{os.getpid()}.svg")
             html = f"""<table border="0" CELLBORDER="0">
                 {labelgraph}
                 <tr>
-                        <td><img src="{tmp}/leaf{node.id}_{os.getpid()}.svg"/></td>
+                        <td><img src="{filepath}"/></td>
                 </tr>
                 </table>"""
             if node.id in highlight_path:
                 return f'leaf{node.id} [margin="0" shape=box penwidth=".5" color="{colors["highlight"]}" style="dashed" label=<{html}>]'
             else:
                 return f'leaf{node.id} [margin="0" shape=box penwidth="0" color="{colors["text"]}" label=<{html}>]'
 
         def node_label(node):
             return f'<tr><td CELLPADDING="0" CELLSPACING="0"><font face="{fontname}" color="{colors["node_label"]}" point-size="14"><i>Node {node.id}</i></font></td></tr>'
 
         def class_legend_html():
+            filepath = os.path.join(tmp, f"legend_{os.getpid()}.svg")
             return f"""
                 <table border="0" cellspacing="0" cellpadding="0">
                     <tr>
-                        <td border="0" cellspacing="0" cellpadding="0"><img src="{tmp}/legend_{os.getpid()}.svg"/></td>
+                        <td border="0" cellspacing="0" cellpadding="0"><img src="{filepath}"/></td>
                     </tr>
                 </table>
                 """
 
         def class_legend_gr():
             if not self.shadow_tree.is_classifier():
                 return ""
@@ -523,15 +527,15 @@
 
         # Fix the mapping from target value to color for entire tree
         if self.shadow_tree.is_classifier():
             class_values = self.shadow_tree.classes()
             if np.max(class_values) >= n_classes:
                 raise ValueError(f"Target label values (for now) must be 0..{n_classes-1} for n={n_classes} labels")
             color_map = {v: color_values[i] for i, v in enumerate(class_values)}
-            _draw_legend(self.shadow_tree, self.shadow_tree.target_name, f"{tmp}/legend_{os.getpid()}.svg",
+            _draw_legend(self.shadow_tree, self.shadow_tree.target_name, os.path.join(tmp, f"legend_{os.getpid()}.svg"),
                          colors=colors,
                          fontname=fontname)
 
         X_train = self.shadow_tree.X_train
         y_train = self.shadow_tree.y_train
         if isinstance(X_train, pd.DataFrame):
             X_train = X_train.values
@@ -556,27 +560,27 @@
         for node in get_internal_nodes():
             if depth_range_to_display is not None:
                 if node.level not in range(depth_range_to_display[0], depth_range_to_display[1] + 1):
                     continue
             if fancy:
                 if self.shadow_tree.is_classifier():
                     _class_split_viz(node, X_train, y_train,
-                                     filename=f"{tmp}/node{node.id}_{os.getpid()}.svg",
+                                     filename=os.path.join(tmp, f"node{node.id}_{os.getpid()}.svg"),
                                      precision=precision,
                                      colors={**color_map, **colors},
                                      histtype=histtype,
                                      node_heights=node_heights,
                                      X=x,
                                      ticks_fontsize=ticks_fontsize,
                                      label_fontsize=label_fontsize,
                                      fontname=fontname,
                                      highlight_node=node.id in highlight_path)
                 else:
                     _regr_split_viz(node, X_train, y_train,
-                                    filename=f"{tmp}/node{node.id}_{os.getpid()}.svg",
+                                    filename=os.path.join(tmp, f"node{node.id}_{os.getpid()}.svg"),
                                     target_name=self.shadow_tree.target_name,
                                     y_range=y_range,
                                     X=x,
                                     ticks_fontsize=ticks_fontsize,
                                     label_fontsize=label_fontsize,
                                     fontname=fontname,
                                     highlight_node=node.id in highlight_path,
@@ -592,25 +596,25 @@
         leaves = []
         for node in get_leaves():
             if depth_range_to_display is not None:
                 if node.level not in range(depth_range_to_display[0], depth_range_to_display[1] + 1):
                     continue
             if self.shadow_tree.is_classifier():
                 _class_leaf_viz(node, colors=color_values,
-                                filename=f"{tmp}/leaf{node.id}_{os.getpid()}.svg",
+                                filename=os.path.join(tmp, f"leaf{node.id}_{os.getpid()}.svg"),
                                 graph_colors=colors,
                                 fontname=fontname,
                                 leaftype=leaftype)
                 leaves.append(class_leaf_node(node))
             else:
                 # for now, always gen leaf
                 _regr_leaf_viz(node,
                                y_train,
                                target_name=self.shadow_tree.target_name,
-                               filename=f"{tmp}/leaf{node.id}_{os.getpid()}.svg",
+                               filename=os.path.join(tmp, f"leaf{node.id}_{os.getpid()}.svg"),
                                y_range=y_range,
                                precision=precision,
                                ticks_fontsize=ticks_fontsize,
                                label_fontsize=label_fontsize,
                                fontname=fontname,
                                colors=colors)
                 leaves.append(regr_leaf_node(node))
@@ -1371,16 +1375,15 @@
 
     samples = node.samples()
     y = y[samples]
 
     figsize = (.75, .8)
 
     fig, ax = plt.subplots(1, 1, figsize=figsize)
-
-    m = np.mean(y)
+    m = node.prediction()
 
     _format_axes(ax, None, None, colors, fontsize=label_fontsize, fontname=fontname, ticks_fontsize=ticks_fontsize, grid=False)
     ax.set_ylim(y_range)
     ax.spines['bottom'].set_visible(False)
     ax.set_xticks([])
 
     ticklabelpad = plt.rcParams['xtick.major.pad']
@@ -1526,15 +1529,15 @@
     means = []
     means_range = []
     x_labels = []
     sigma = .05
     for i, node in enumerate(shadow_tree.leaves):
         leaf_index_sample = node.samples()
         leaf_target = shadow_tree.y_train[leaf_index_sample]
-        leaf_target_mean = np.mean(leaf_target)
+        leaf_target_mean = node.prediction()
         np.random.seed(0)  # generate the same list of random values for each call
         X = np.random.normal(i, sigma, size=len(leaf_target))
 
         x.extend(X)
         y.extend(leaf_target)
         means.append([leaf_target_mean, leaf_target_mean])
         means_range.append([i - (sigma * 3), i + (sigma * 3)])
```

### Comparing `dtreeviz-2.2.1/dtreeviz/utils.py` & `dtreeviz-2.2.2/dtreeviz/utils.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/dtreeviz/version.py` & `dtreeviz-2.2.2/dtreeviz/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = '2.2.1'
+__version__ = '2.2.2'
```

### Comparing `dtreeviz-2.2.1/dtreeviz.egg-info/PKG-INFO` & `dtreeviz-2.2.2/dtreeviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtreeviz
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Python 3 library for sci-kit learn, XGBoost, LightGBM, Spark, and TensorFlow decision tree visualization
 Home-page: https://github.com/parrt/dtreeviz
 Author: Terence Parr, Tudor Lapusan, and Prince Grover
 Author-email: parrt@antlr.org
 License: MIT
 Keywords: machine-learning data structures trees visualization
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dtreeviz-2.2.1/dtreeviz.egg-info/SOURCES.txt` & `dtreeviz-2.2.2/dtreeviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/setup.py` & `dtreeviz-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extra_pyspark = ['pyspark']
 extra_lightgbm = ['lightgbm']
 extra_tensorflow = ['tensorflow_decision_forests']
 
 
 setup(
     name='dtreeviz',
-    version='2.2.1',
+    version='2.2.2',
     url='https://github.com/parrt/dtreeviz',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'graphviz>=0.9',
         'pandas',
         'numpy',
```

### Comparing `dtreeviz-2.2.1/testing/animate_rtree_bivar_3D.py` & `dtreeviz-2.2.2/testing/animate_rtree_bivar_3D.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/cancer.py` & `dtreeviz-2.2.2/testing/cancer.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/gen_feature_space_samples.py` & `dtreeviz-2.2.2/testing/gen_feature_space_samples.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/gen_samples.py` & `dtreeviz-2.2.2/testing/gen_samples.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/iris.py` & `dtreeviz-2.2.2/testing/iris.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/paper_examples.py` & `dtreeviz-2.2.2/testing/paper_examples.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_ctree.py` & `dtreeviz-2.2.2/testing/play_ctree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_ctree_bivar.py` & `dtreeviz-2.2.2/testing/play_ctree_bivar.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_lightgbm.py` & `dtreeviz-2.2.2/testing/play_lightgbm.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_rtree.py` & `dtreeviz-2.2.2/testing/play_rtree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_rtree_bivar_3D.py` & `dtreeviz-2.2.2/testing/play_rtree_bivar_3D.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_rtree_bivar_heatmap.py` & `dtreeviz-2.2.2/testing/play_rtree_bivar_heatmap.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/play_spark.py` & `dtreeviz-2.2.2/testing/play_spark.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/conftest.py` & `dtreeviz-2.2.2/testing/testlib/models/conftest.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_lightgbm_classifier.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_lightgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_spark_classifier.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_spark_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_tensorflow_classifier.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_tensorflow_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_xgb_regressor.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_tree_xgb_regressor.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_classifier.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_trees_sk_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_pipeline.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_trees_sk_pipeline.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_xgb_classifier.py` & `dtreeviz-2.2.2/testing/testlib/models/test_decision_trees_xgb_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/testone.py` & `dtreeviz-2.2.2/testing/testone.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/tf-catvars.py` & `dtreeviz-2.2.2/testing/tf-catvars.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/tf_catvars2.py` & `dtreeviz-2.2.2/testing/tf_catvars2.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/tf_catvars3.py` & `dtreeviz-2.2.2/testing/tf_catvars3.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.1/testing/tf_regr_catvars.py` & `dtreeviz-2.2.2/testing/tf_regr_catvars.py`

 * *Files identical despite different names*

