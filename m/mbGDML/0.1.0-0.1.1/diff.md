# Comparing `tmp/mbGDML-0.1.0.tar.gz` & `tmp/mbGDML-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbGDML-0.1.0.tar", last modified: Fri Apr 21 03:33:57 2023, max compression
+gzip compressed data, was "mbGDML-0.1.1.tar", last modified: Thu Jul 13 13:34:40 2023, max compression
```

## Comparing `mbGDML-0.1.0.tar` & `mbGDML-0.1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 03:33:41.000000 mbGDML-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 03:33:41.000000 mbGDML-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-21 03:33:41.000000 mbGDML-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-21 03:33:57.311221 mbGDML-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 03:33:41.000000 mbGDML-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.303221 mbGDML-0.1.0/mbGDML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 03:33:57.000000 mbGDML-0.1.0/mbGDML.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.315221 mbGDML-0.1.0/mbgdml/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/_gdml/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/desc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20028 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/perm.py
--rw-r--r--   0 runner    (1001) docker     (123)    43148 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/_gdml/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/solvers/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23584 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/solvers/iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)    37575 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/torchtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    56038 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/_gdml/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 03:33:57.315221 mbGDML-0.1.0/mbgdml/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/active_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/active_learning/drive_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/active_learning/sample_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/alchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.307221 mbGDML-0.1.0/mbgdml/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/problematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/analysis/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/basedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/data/predictset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/interfaces/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    47240 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/mbe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/models/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/gap_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/gdml_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/models/schnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/gap_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/gdml_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/predictors/schnet_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/stress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/mbgdml/structure_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/structure_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/structure_gen/packmol_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/structure_gen/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/switching.py
--rw-r--r--   0 runner    (1001) docker     (123)    42748 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-04-21 03:33:41.000000 mbGDML-0.1.0/mbgdml/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-21 03:33:57.311221 mbGDML-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-04-21 03:33:41.000000 mbGDML-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:33:57.311221 mbGDML-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_mbe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_packmol_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_predictsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_structure_gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-21 03:33:41.000000 mbGDML-0.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-21 03:33:41.000000 mbGDML-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.790778 mbGDML-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 13:34:27.000000 mbGDML-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 13:34:27.000000 mbGDML-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-13 13:34:27.000000 mbGDML-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-13 13:34:40.790778 mbGDML-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-13 13:34:27.000000 mbGDML-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.782777 mbGDML-0.1.1/mbGDML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-13 13:34:40.000000 mbGDML-0.1.1/mbGDML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-13 13:34:40.000000 mbGDML-0.1.1/mbGDML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:34:40.000000 mbGDML-0.1.1/mbGDML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:34:40.000000 mbGDML-0.1.1/mbGDML.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 13:34:40.000000 mbGDML-0.1.1/mbGDML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 13:34:40.000000 mbGDML-0.1.1/mbGDML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.790778 mbGDML-0.1.1/mbgdml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/_gdml/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20028 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43148 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/_gdml/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/solvers/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23584 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/solvers/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37575 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/torchtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56038 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/_gdml/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 13:34:40.790778 mbGDML-0.1.1/mbgdml/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/active_learning/drive_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/active_learning/sample_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/alchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/analysis/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/analysis/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/analysis/problematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/analysis/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/data/basedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/data/predictset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/interfaces/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47240 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/mbe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/models/gap_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/models/gdml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/models/schnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.786777 mbGDML-0.1.1/mbgdml/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/predictors/gap_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/predictors/gdml_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/predictors/schnet_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/stress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.790778 mbGDML-0.1.1/mbgdml/structure_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/structure_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/structure_gen/packmol_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/structure_gen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/switching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43086 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-07-13 13:34:27.000000 mbGDML-0.1.1/mbgdml/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-07-13 13:34:40.790778 mbGDML-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-13 13:34:27.000000 mbGDML-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:34:40.790778 mbGDML-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_mbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_packmol_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_predictsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_structure_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 13:34:27.000000 mbGDML-0.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-07-13 13:34:27.000000 mbGDML-0.1.1/versioneer.py
```

### Comparing `mbGDML-0.1.0/LICENSE` & `mbGDML-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/NOTICE` & `mbGDML-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/PKG-INFO` & `mbGDML-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: mbGDML
-Version: 0.1.0
-Summary: Create, use, and analyze machine learning potentials within the many-body expansion framework
-Home-page: https://github.com/keithgroup/mbGDML
-Author: Alex M. Maldonado
-Author-email: aalexmmaldonado@gmail.com
-License: MIT license
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 <h1 align="center">mbGDML</h1>
 
 <h4 align="center">Create, use, and analyze machine learning potentials within the many-body expansion framework.</h4>
 
 <h4 align="center" style="padding-bottom: 0.5em;"><a href="https://keithgroup.github.io/mbGDML">Documentation</a></h4>
 
 <p align="center">
@@ -119,10 +99,33 @@
 
 ```text
 git clone https://github.com/keithgroup/mbGDML
 cd mbGDML
 pip install .
 ```
 
+## Citing this work
+
+If you find this code helpful in your research or project, please consider citing the following paper:
+
+Maldonado, A. M.; Poltavsky, I.; Vassilev-Galindo, V.; Tkatchenko, A.; Keith, J. A. Modeling molecular ensembles with gradient-domain machine learning force fields. *Digital Discovery* **2023**, *2* (3), 871-880. DOI: [10.1039/D3DD00011G](https://doi.org/10.1039/D3DD00011G).
+
+```bibtex
+@article{maldonado2023modeling,
+  title={Modeling molecular ensembles with gradient-domain machine learning force fields},
+  author={Maldonado, Alex M and Poltavsky, Igor and Vassilev-Galindo, Valentin and Tkatchenko, Alexandre and Keith, John A},
+  journal={Digital Discovery},
+  volume={2},
+  number={3},
+  pages={871--880},
+  year={2023},
+  publisher={Royal Society of Chemistry},
+  doi={10.1039/D3DD00011G}
+}
+```
+
+Citing the paper helps acknowledge the effort put into developing and maintaining this codebase, and it provides a way to support further research and development.
+Thank you for your support!
+
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: mbGDML Version: 0.1.0 Summary: Create, use, and
-analyze machine learning potentials within the many-body expansion framework
-Home-page: https://github.com/keithgroup/mbGDML Author: Alex M. Maldonado
-Author-email: aalexmmaldonado@gmail.com License: MIT license Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
-Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Chemistry Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE License-File: NOTICE
                              ****** mbGDML ******
  *** Create, use, and analyze machine learning potentials within the many-body
                            expansion framework. ***
                              *** Documentation ***
   [Build_Status_] [Codecov] [DOI] [License] [Repo_size] [Black_style] [Black
                                     style]
        Motivation â¢ Approach â¢ Features â¢ Installation â¢ License
@@ -56,9 +46,22 @@
 learn.org/stable/index.html). ### Interfaces - [Atomic Simulation Environment]
 (https://wiki.fysik.dtu.dk/ase/) (ASE) for geometry optimizations, molecular
 dynamics simulations, and more. ## Installation You can install mbGDML from
 [PyPI](https://pypi.org/project/mbGDML/) by using `pip install mbGDML`. Or, the
 latest development version can be installed directly from the [GitHub
 repository](https://github.com/keithgroup/mbGDML) or from [TestPyPI](https://
 test.pypi.org/project/mbGDML/). ```text git clone https://github.com/
-keithgroup/mbGDML cd mbGDML pip install . ``` ## License Distributed under the
-MIT License. See `LICENSE` for more information.
+keithgroup/mbGDML cd mbGDML pip install . ``` ## Citing this work If you find
+this code helpful in your research or project, please consider citing the
+following paper: Maldonado, A. M.; Poltavsky, I.; Vassilev-Galindo, V.;
+Tkatchenko, A.; Keith, J. A. Modeling molecular ensembles with gradient-domain
+machine learning force fields. *Digital Discovery* **2023**, *2* (3), 871-880.
+DOI: [10.1039/D3DD00011G](https://doi.org/10.1039/D3DD00011G). ```bibtex
+@article{maldonado2023modeling, title={Modeling molecular ensembles with
+gradient-domain machine learning force fields}, author={Maldonado, Alex M and
+Poltavsky, Igor and Vassilev-Galindo, Valentin and Tkatchenko, Alexandre and
+Keith, John A}, journal={Digital Discovery}, volume={2}, number={3}, pages=
+{871--880}, year={2023}, publisher={Royal Society of Chemistry}, doi={10.1039/
+D3DD00011G} } ``` Citing the paper helps acknowledge the effort put into
+developing and maintaining this codebase, and it provides a way to support
+further research and development. Thank you for your support! ## License
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `mbGDML-0.1.0/README.md` & `mbGDML-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: mbGDML
+Version: 0.1.1
+Summary: Create, use, and analyze machine learning potentials within the many-body expansion framework
+Home-page: https://github.com/keithgroup/mbGDML
+Author: Alex M. Maldonado
+Author-email: aalexmmaldonado@gmail.com
+License: MIT license
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 <h1 align="center">mbGDML</h1>
 
 <h4 align="center">Create, use, and analyze machine learning potentials within the many-body expansion framework.</h4>
 
 <h4 align="center" style="padding-bottom: 0.5em;"><a href="https://keithgroup.github.io/mbGDML">Documentation</a></h4>
 
 <p align="center">
@@ -99,10 +119,33 @@
 
 ```text
 git clone https://github.com/keithgroup/mbGDML
 cd mbGDML
 pip install .
 ```
 
+## Citing this work
+
+If you find this code helpful in your research or project, please consider citing the following paper:
+
+Maldonado, A. M.; Poltavsky, I.; Vassilev-Galindo, V.; Tkatchenko, A.; Keith, J. A. Modeling molecular ensembles with gradient-domain machine learning force fields. *Digital Discovery* **2023**, *2* (3), 871-880. DOI: [10.1039/D3DD00011G](https://doi.org/10.1039/D3DD00011G).
+
+```bibtex
+@article{maldonado2023modeling,
+  title={Modeling molecular ensembles with gradient-domain machine learning force fields},
+  author={Maldonado, Alex M and Poltavsky, Igor and Vassilev-Galindo, Valentin and Tkatchenko, Alexandre and Keith, John A},
+  journal={Digital Discovery},
+  volume={2},
+  number={3},
+  pages={871--880},
+  year={2023},
+  publisher={Royal Society of Chemistry},
+  doi={10.1039/D3DD00011G}
+}
+```
+
+Citing the paper helps acknowledge the effort put into developing and maintaining this codebase, and it provides a way to support further research and development.
+Thank you for your support!
+
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: mbGDML Version: 0.1.1 Summary: Create, use, and
+analyze machine learning potentials within the many-body expansion framework
+Home-page: https://github.com/keithgroup/mbGDML Author: Alex M. Maldonado
+Author-email: aalexmmaldonado@gmail.com License: MIT license Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
+Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Chemistry Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE License-File: NOTICE
                              ****** mbGDML ******
  *** Create, use, and analyze machine learning potentials within the many-body
                            expansion framework. ***
                              *** Documentation ***
   [Build_Status_] [Codecov] [DOI] [License] [Repo_size] [Black_style] [Black
                                     style]
        Motivation â¢ Approach â¢ Features â¢ Installation â¢ License
@@ -46,9 +56,22 @@
 learn.org/stable/index.html). ### Interfaces - [Atomic Simulation Environment]
 (https://wiki.fysik.dtu.dk/ase/) (ASE) for geometry optimizations, molecular
 dynamics simulations, and more. ## Installation You can install mbGDML from
 [PyPI](https://pypi.org/project/mbGDML/) by using `pip install mbGDML`. Or, the
 latest development version can be installed directly from the [GitHub
 repository](https://github.com/keithgroup/mbGDML) or from [TestPyPI](https://
 test.pypi.org/project/mbGDML/). ```text git clone https://github.com/
-keithgroup/mbGDML cd mbGDML pip install . ``` ## License Distributed under the
-MIT License. See `LICENSE` for more information.
+keithgroup/mbGDML cd mbGDML pip install . ``` ## Citing this work If you find
+this code helpful in your research or project, please consider citing the
+following paper: Maldonado, A. M.; Poltavsky, I.; Vassilev-Galindo, V.;
+Tkatchenko, A.; Keith, J. A. Modeling molecular ensembles with gradient-domain
+machine learning force fields. *Digital Discovery* **2023**, *2* (3), 871-880.
+DOI: [10.1039/D3DD00011G](https://doi.org/10.1039/D3DD00011G). ```bibtex
+@article{maldonado2023modeling, title={Modeling molecular ensembles with
+gradient-domain machine learning force fields}, author={Maldonado, Alex M and
+Poltavsky, Igor and Vassilev-Galindo, Valentin and Tkatchenko, Alexandre and
+Keith, John A}, journal={Digital Discovery}, volume={2}, number={3}, pages=
+{871--880}, year={2023}, publisher={Royal Society of Chemistry}, doi={10.1039/
+D3DD00011G} } ``` Citing the paper helps acknowledge the effort put into
+developing and maintaining this codebase, and it provides a way to support
+further research and development. Thank you for your support! ## License
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `mbGDML-0.1.0/mbGDML.egg-info/PKG-INFO` & `mbGDML-0.1.1/mbGDML.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbGDML
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create, use, and analyze machine learning potentials within the many-body expansion framework
 Home-page: https://github.com/keithgroup/mbGDML
 Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -119,10 +119,33 @@
 
 ```text
 git clone https://github.com/keithgroup/mbGDML
 cd mbGDML
 pip install .
 ```
 
+## Citing this work
+
+If you find this code helpful in your research or project, please consider citing the following paper:
+
+Maldonado, A. M.; Poltavsky, I.; Vassilev-Galindo, V.; Tkatchenko, A.; Keith, J. A. Modeling molecular ensembles with gradient-domain machine learning force fields. *Digital Discovery* **2023**, *2* (3), 871-880. DOI: [10.1039/D3DD00011G](https://doi.org/10.1039/D3DD00011G).
+
+```bibtex
+@article{maldonado2023modeling,
+  title={Modeling molecular ensembles with gradient-domain machine learning force fields},
+  author={Maldonado, Alex M and Poltavsky, Igor and Vassilev-Galindo, Valentin and Tkatchenko, Alexandre and Keith, John A},
+  journal={Digital Discovery},
+  volume={2},
+  number={3},
+  pages={871--880},
+  year={2023},
+  publisher={Royal Society of Chemistry},
+  doi={10.1039/D3DD00011G}
+}
+```
+
+Citing the paper helps acknowledge the effort put into developing and maintaining this codebase, and it provides a way to support further research and development.
+Thank you for your support!
+
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mbGDML Version: 0.1.0 Summary: Create, use, and
+Metadata-Version: 2.1 Name: mbGDML Version: 0.1.1 Summary: Create, use, and
 analyze machine learning potentials within the many-body expansion framework
 Home-page: https://github.com/keithgroup/mbGDML Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com License: MIT license Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
@@ -56,9 +56,22 @@
 learn.org/stable/index.html). ### Interfaces - [Atomic Simulation Environment]
 (https://wiki.fysik.dtu.dk/ase/) (ASE) for geometry optimizations, molecular
 dynamics simulations, and more. ## Installation You can install mbGDML from
 [PyPI](https://pypi.org/project/mbGDML/) by using `pip install mbGDML`. Or, the
 latest development version can be installed directly from the [GitHub
 repository](https://github.com/keithgroup/mbGDML) or from [TestPyPI](https://
 test.pypi.org/project/mbGDML/). ```text git clone https://github.com/
-keithgroup/mbGDML cd mbGDML pip install . ``` ## License Distributed under the
-MIT License. See `LICENSE` for more information.
+keithgroup/mbGDML cd mbGDML pip install . ``` ## Citing this work If you find
+this code helpful in your research or project, please consider citing the
+following paper: Maldonado, A. M.; Poltavsky, I.; Vassilev-Galindo, V.;
+Tkatchenko, A.; Keith, J. A. Modeling molecular ensembles with gradient-domain
+machine learning force fields. *Digital Discovery* **2023**, *2* (3), 871-880.
+DOI: [10.1039/D3DD00011G](https://doi.org/10.1039/D3DD00011G). ```bibtex
+@article{maldonado2023modeling, title={Modeling molecular ensembles with
+gradient-domain machine learning force fields}, author={Maldonado, Alex M and
+Poltavsky, Igor and Vassilev-Galindo, Valentin and Tkatchenko, Alexandre and
+Keith, John A}, journal={Digital Discovery}, volume={2}, number={3}, pages=
+{871--880}, year={2023}, publisher={Royal Society of Chemistry}, doi={10.1039/
+D3DD00011G} } ``` Citing the paper helps acknowledge the effort put into
+developing and maintaining this codebase, and it provides a way to support
+further research and development. Thank you for your support! ## License
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `mbGDML-0.1.0/mbGDML.egg-info/SOURCES.txt` & `mbGDML-0.1.1/mbGDML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/desc.py` & `mbGDML-0.1.1/mbgdml/_gdml/desc.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/perm.py` & `mbGDML-0.1.1/mbgdml/_gdml/perm.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/predict.py` & `mbGDML-0.1.1/mbgdml/_gdml/predict.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/sample.py` & `mbGDML-0.1.1/mbgdml/_gdml/sample.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/solvers/analytic.py` & `mbGDML-0.1.1/mbgdml/_gdml/solvers/analytic.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/solvers/iterative.py` & `mbGDML-0.1.1/mbgdml/_gdml/solvers/iterative.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/torchtools.py` & `mbGDML-0.1.1/mbgdml/_gdml/torchtools.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/_gdml/train.py` & `mbGDML-0.1.1/mbgdml/_gdml/train.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/active_learning/drive_md.py` & `mbGDML-0.1.1/mbgdml/active_learning/drive_md.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/active_learning/sample_md.py` & `mbGDML-0.1.1/mbgdml/active_learning/sample_md.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/alchemy.py` & `mbGDML-0.1.1/mbgdml/alchemy.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/analysis/clustering.py` & `mbGDML-0.1.1/mbgdml/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/analysis/models.py` & `mbGDML-0.1.1/mbgdml/analysis/models.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/analysis/problematic.py` & `mbGDML-0.1.1/mbgdml/analysis/problematic.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/analysis/rdf.py` & `mbGDML-0.1.1/mbgdml/analysis/rdf.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/data/basedata.py` & `mbGDML-0.1.1/mbgdml/data/basedata.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/data/dataset.py` & `mbGDML-0.1.1/mbgdml/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/data/predictset.py` & `mbGDML-0.1.1/mbgdml/data/predictset.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/descriptors.py` & `mbGDML-0.1.1/mbgdml/descriptors.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/interfaces/ase.py` & `mbGDML-0.1.1/mbgdml/interfaces/ase.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/logger.py` & `mbGDML-0.1.1/mbgdml/logger.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/losses.py` & `mbGDML-0.1.1/mbgdml/losses.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/mbe.py` & `mbGDML-0.1.1/mbgdml/mbe.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/models/base.py` & `mbGDML-0.1.1/mbgdml/models/base.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/models/gap_model.py` & `mbGDML-0.1.1/mbgdml/models/gap_model.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/models/gdml_model.py` & `mbGDML-0.1.1/mbgdml/models/gdml_model.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/models/schnet_model.py` & `mbGDML-0.1.1/mbgdml/models/schnet_model.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/periodic.py` & `mbGDML-0.1.1/mbgdml/periodic.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/predictors/gap_predict.py` & `mbGDML-0.1.1/mbgdml/predictors/gap_predict.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/predictors/gdml_predict.py` & `mbGDML-0.1.1/mbgdml/predictors/gdml_predict.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/predictors/schnet_predict.py` & `mbGDML-0.1.1/mbgdml/predictors/schnet_predict.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/stress.py` & `mbGDML-0.1.1/mbgdml/stress.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/structure_gen/packmol_gen.py` & `mbGDML-0.1.1/mbgdml/structure_gen/packmol_gen.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/structure_gen/utils.py` & `mbGDML-0.1.1/mbgdml/structure_gen/utils.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/switching.py` & `mbGDML-0.1.1/mbgdml/switching.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/mbgdml/train.py` & `mbGDML-0.1.1/mbgdml/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -686,18 +686,24 @@
         if is_final:
             if self.bayes_opt_params_final is not None:
                 gp_params = self.bayes_opt_params_final
             else:
                 gp_params = self.bayes_opt_params
         else:
             gp_params = self.bayes_opt_params
-        if gp_params is not None and "init_points" in gp_params:
-            init_points = gp_params["init_points"]
-        else:
-            init_points = 5  # BayesianOptimization default.
+        # Addressing way of handling gp_params
+        # https://github.com/bayesian-optimization/BayesianOptimization/commit/ac435483f24e666866a395423aa3eb4d65278fea
+        if gp_params is not None:
+            init_points = gp_params.get("init_points", 5)
+            init_points = gp_params.get("n_iter", 25)
+        del_keys = ["init_points", "n_iter"]
+        for key in del_keys:
+            if key in gp_params.keys():  # pylint: disable=consider-iterating-dictionary
+                del gp_params[key]
+
         sigma_grid = self.sigma_grid
         if sigma_grid is not None:
             log.info("#   Initial grid search   #")
             sigma_grid.sort()
 
             def probe_sigma(sigma):
                 optimizer.probe({"sigma": sigma}, lazy=False)
@@ -773,20 +779,20 @@
                         # we have already checked.
                         sigma_bounds = (sigma_bounds[0], np.max(valid_json["sigmas"]))
                         optimizer.set_bounds({"sigma": sigma_bounds})
 
                         # We stop grid search and start Bayesian optimization.
                         break
 
-        if init_points < 0:
-            init_points = 0
-            gp_params["init_points"] = init_points
+        # Ensure init_points cannot be negative
+        init_points = max(init_points, 0)
 
         log.info("#   Bayesian optimization   #")
-        optimizer.maximize(**gp_params)
+        optimizer.set_gp_params(**gp_params)
+        optimizer.maximize()
 
         results = optimizer.res
         losses = np.array([-res["target"] for res in results])
         min_idxs = np.argsort(losses)
 
         for idx in min_idxs:
             sigma_best = results[idx]["params"]["sigma"]
```

### Comparing `mbGDML-0.1.0/mbgdml/utils.py` & `mbGDML-0.1.1/mbgdml/utils.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/setup.cfg` & `mbGDML-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/setup.py` & `mbGDML-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "matplotlib",
     "numpy",
     "scipy",
     "psutil",
     "bayesian-optimization>=1.4.0",
     "pandas",
     "qcelemental>=0.25.1",
+    "pydantic<2.0.0",  # See https://github.com/MolSSI/QCElemental/issues/312
     "ray>=2.0.0",
 ]
 setup_requirements = []
 test_requirements = requirements.append(["pytest"])
 
 setup(
     packages=find_packages(include=["mbgdml", "mbgdml.*"]),
```

### Comparing `mbGDML-0.1.0/tests/test_datasets.py` & `mbGDML-0.1.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_descriptors.py` & `mbGDML-0.1.1/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_mbe.py` & `mbGDML-0.1.1/tests/test_mbe.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_packmol_gen.py` & `mbGDML-0.1.1/tests/test_packmol_gen.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_predict.py` & `mbGDML-0.1.1/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_predictsets.py` & `mbGDML-0.1.1/tests/test_predictsets.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_rdf.py` & `mbGDML-0.1.1/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_structure_gen_utils.py` & `mbGDML-0.1.1/tests/test_structure_gen_utils.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_train.py` & `mbGDML-0.1.1/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/tests/test_utils.py` & `mbGDML-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mbGDML-0.1.0/versioneer.py` & `mbGDML-0.1.1/versioneer.py`

 * *Files identical despite different names*

