# Comparing `tmp/prolog_primitives-1.0.5.tar.gz` & `tmp/prolog_primitives-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-1.0.5.tar", last modified: Sun Jul  9 20:41:39 2023, max compression
+gzip compressed data, was "prolog_primitives-1.1.0.tar", last modified: Thu Jul 13 16:18:16 2023, max compression
```

## Comparing `prolog_primitives-1.0.5.tar` & `prolog_primitives-1.1.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.351453 prolog_primitives-1.0.5/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.355453 prolog_primitives-1.0.5/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/nt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.363453 prolog_primitives-1.0.5/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.363453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.367453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.371453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.371453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.375453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.351453 prolog_primitives-1.0.5/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.830978 prolog_primitives-1.1.0/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.830978 prolog_primitives-1.1.0/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/nt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.834978 prolog_primitives-1.1.0/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.834978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.834978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.838978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.838978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.838978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.830978 prolog_primitives-1.1.0/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/setup.py
```

### Comparing `prolog_primitives-1.0.5/LICENSE` & `prolog_primitives-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/PKG-INFO` & `prolog_primitives-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 1.0.5
+Version: 1.1.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/Session.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/Utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     else:   
         return msg.functor
        
 def parseArgumentMsgList(msg: basicMsg.ArgumentMsg) -> list:
     returnValue = list()
     currentValue = msg.struct
     while(len(currentValue.arguments) != 0):
-        returnValue.append(parseArgumentMsg(currentValue.arguments[0]))
+        value = parseArgumentMsg(currentValue.arguments[0])
+        if(value != "[" and value != "]"):
+            returnValue.append(value)
         currentValue = currentValue.arguments[1].struct
     return returnValue 
 
 def fromListToArgumentMsg(elements: list) -> basicMsg.ArgumentMsg:
     last_element = buildConstantArgumentMsg(
         basicMsg.StructMsg(
                 functor = "[]"
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/basic/nt.py` & `prolog_primitives-1.1.0/prolog_primitives/basic/nt.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-1.1.0/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-1.1.0/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-1.1.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,11 +72,12 @@
         return self.__model.get(ref, None)
 
     def idGenerator(self) -> str:
         import random
         import string
         characters = string.ascii_lowercase# + string.digits
         id = ''.join(random.choice(characters) for i in range(10)) 
-        while(id in self.__schemas or id in self.__dataset):
+        while(id in self.__schemas or id in self.__dataset or id in self.__pipeline
+            or id in self.__topology or id in self. __model):
             id = ''.join(random.choice(characters) for i in range(10)) 
         return id
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from prolog_primitives.basic import DistributedElements
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 from sklearn.model_selection import KFold
+from datasets import Dataset
 
 class __FoldPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
         k = request.arguments[1]
         train_ref = request.arguments[2]
@@ -15,17 +16,16 @@
            train_ref.HasField("var") and val_ref.HasField("var")):
             datasetId = str(Utils.parseArgumentMsg(dataset_ref))
             schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
             dataset = SharedCollections().getDataset(datasetId)
             k = int(Utils.parseArgumentMsg(k))
             for kfold, (train, test) in enumerate(KFold(n_splits=k, 
                                 shuffle=True).split(dataset)):
-                train_ds = dataset[train]   
-                val_ds = dataset[test]
-                
+                train_ds = Dataset.from_dict(dataset[train]).with_format("tf")  
+                val_ds = Dataset.from_dict(dataset[test]).with_format("tf")  
                 
                 train_id = SharedCollections().addDataset(train_ds, schemaId)
                 val_id = SharedCollections().addDataset(val_ds, schemaId)
             
                 yield request.replySuccess(substitutions={
                     train_ref.var: Utils.buildConstantArgumentMsg(train_id),
                     val_ref.var: Utils.buildConstantArgumentMsg(val_id)
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
             datasetId = str(Utils.parseArgumentMsg(dataset_ref))
             schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
             dataset: Dataset = SharedCollections().getDataset(datasetId)
             ratio = float(Utils.parseArgumentMsg(ratio))
             train_size = int(ratio * len(list(dataset)))
         
             shuffled = dataset.shuffle()
-            train_ds = shuffled[:train_size]
-            val_ds = dataset[train_size:]
+            train_ds = Dataset.from_dict(shuffled[:train_size]).with_format("tf")
+            val_ds = Dataset.from_dict(dataset[train_size:]).with_format("tf")
             
             train_id = SharedCollections().addDataset(train_ds, schemaId)
             val_id = SharedCollections().addDataset(val_ds, schemaId)
             
             yield request.replySuccess(substitutions={
                 train_ref.var: Utils.buildConstantArgumentMsg(train_id),
                 val_ref.var: Utils.buildConstantArgumentMsg(val_id)
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class __TheoryToDatasetPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_name = request.arguments[0]
         dataset_ref = request.arguments[1]
         if(not schema_name.HasField("var") and dataset_ref.HasField("var")):
             schemaId = str(Utils.parseArgumentMsg(next(request.subSolve(
-                query = basicMsg.StructMsg(functor="theoryToSchema", arguments=[basicMsg.ArgumentMsg(var="X")]))
+                query = basicMsg.StructMsg(functor="theory_to_schema", arguments=[basicMsg.ArgumentMsg(var="X")]))
                  ).substitutions["X"]))         
             schema = SharedCollections().getSchema(schemaId)
             
             data = dict(list(map(lambda x: (x.name,[]), schema.attributes)))
             for i in request.inspectKb(
                 primitiveMsg.InspectKbMsg.STATIC,
                 [(primitiveMsg.InspectKbMsg.STARTS_WITH, str(Utils.parseArgumentMsg(schema_name)))]):
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .neuralNetwork.inputLayer import inputLayerPrimitive
 from .neuralNetwork.denseLayer import denseLayerPrimitive
 from .neuralNetwork.outputLayer import outputLayerPrimitive
 from .neuralNetwork.neuralNetwork import neuralNetworkPrimitive
 from .predictors.train import trainPrimitive
 from .predictors.predict import predictPrimitive
 from .predictors.classify import classifyPrimitive
-from .predictors.score import msePrimitive
+from .predictors.score import msePrimitive, maePrimitive, accuracyPrimitive, recallPrimitive, rPrimitive
 from ..basic import PrimitiveWrapper, DistributedElements
 from concurrent.futures import ThreadPoolExecutor
 
 def main():
     servers = []
     libraryName = "customLibrary"
 
@@ -36,15 +36,16 @@
     primitives = [schemaPrimitive, theoryToSchemaPrimitive,
                 theoryToDatasetPrimitive, randomSplitPrimitive,
                 rowPrimitive, columnPrimitive, cellPrimitive, foldPrimitive, 
                 theoryFromDatasetPrimitive, schemaTrasformation,
                 normalizePrimitive, one_hot_encodePrimitive, dropPrimitive,
                 fitPrimitive, transformPrimitive, inputLayerPrimitive,
                 denseLayerPrimitive, outputLayerPrimitive, neuralNetworkPrimitive,
-                trainPrimitive, predictPrimitive, classifyPrimitive, msePrimitive]
+                trainPrimitive, predictPrimitive, classifyPrimitive, msePrimitive,
+                maePrimitive, accuracyPrimitive, recallPrimitive, rPrimitive]
 
     initialport = 8080
     port = initialport
     executor = ThreadPoolExecutor(max_workers=len(primitives))
 
     for primitive in primitives:
         #future = executor.submit(launchPrimitive, primitive, port)
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,42 +19,36 @@
             data = None
             
             datasetId = Utils.parseArgumentMsg(dataset_ref)
             dataset: Dataset = SharedCollections().getDataset(datasetId)
             if(dataset != None):
                 schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
                 schema = SharedCollections().getSchema(schemaId)
+                data = list()
                 for attr in dataset.column_names:
                     if(not attr in schema.targets):
-                        if(data == None):
-                            data = tf.cast(dataset[attr], tf.float32)
-                        else:
-                            data = tf.stack([data, tf.cast(dataset[attr], tf.float32)], axis = 1)
-                            
-                
+                        data.append(tf.cast(dataset[attr], tf.float32))
+                data = tf.stack(data, axis = 1)
                 result = {}
                 for attr in schema.targets:
                     result[attr] = []
-                
                 for row in model.predict(x=data):
                     for attr, y in zip(schema.targets, row):
                         result[attr].append(y)
-
                 dataset = Dataset.from_dict(result).with_format("tf")
                 datasetId = SharedCollections().addDataset(dataset, schemaId)
             
                 yield request.replySuccess(substitutions={
                     prediction_ref.var: Utils.buildConstantArgumentMsg(datasetId)
                     }, hasNext=False)
             else:
                 row = [float(x) for x in Utils.parseArgumentMsg(dataset_ref).arguments]
                 data = tf.constant(value=[row], dtype=tf.float32)
             
                 result = model.predict(x=data)[0]
-                
                 yield request.replySuccess(substitutions={
                     prediction_ref.var: Utils.fromListToArgumentMsg(result.tolist())
                     }, hasNext=False)
         else:
             yield request.replyFail()
              
 predictPrimitive = DistributedElements.DistributedPrimitiveWrapper("predict", 3, __Predict())
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from prolog_primitives.basic import DistributedElements
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
+from ..schema.schemaClass import Schema
 from abc import ABC, abstractmethod
+import numpy as np
 
 
 
 class __AssessTemplate(DistributedElements.DistributedPrimitive, ABC):
     
     @abstractmethod
     def evaluator(self, y_true, y_pred):
@@ -20,40 +22,42 @@
         
         if(not y_true_ref.HasField('var') and not y_pred_ref.HasField('var') and
            score.HasField('var')):
             
             def parseY(input):
                 if(type(input) is str):
                     dataset = SharedCollections().getDataset(input)
+                    schema: Schema = SharedCollections().getSchema(SharedCollections().getSchemaIdFromDataset(input))
                     y = {}
                     for attr in dataset.column_names:
-                        y[attr] = list(tf.get_static_value(dataset[attr]))
+                        if(attr in schema.targets):
+                            y[attr] = list(tf.get_static_value(dataset[attr]))
                     return y
                 elif(type(input[0]) is list):
-                    y = []
-                    for x in range(len(input[0])):
-                        y.append([float(input[0][x])])
+                    y = {}
+                    lenght_1 = len(input[0])
+                    lenght_2 = len(input)
+                    input = np.reshape(input, (lenght_1, lenght_2))
+                    
+                    for x in range(len(input)):
+                        y[f"target{x}"] = list(input[x])
                         
-                    for row in input[1:]:
-                        for x in range(len(row)):
-                            y[x].append(float(row[x]))
                     return y
                 else:
                     return [float(x) for x in input]
                 
             y_true = parseY(Utils.parseArgumentMsg(y_true_ref))
                     
             y_pred = parseY(Utils.parseArgumentMsg(y_pred_ref))   
-                
             scores = []   
-            for (attr, y1), y2 in zip(y_true.items(), y_pred):
+            for (attr1, y1), (attr2, y2) in zip(y_true.items(), y_pred.items()):
                 scores.append(self.evaluator(y1, y2))
             
             totalscore = tf.get_static_value(sum(scores)/len(scores))
-                            
+            
             yield request.replySuccess(substitutions={
                 score.var:Utils.buildConstantArgumentMsg(totalscore)
             }, hasNext=False)
 
         else:
             yield request.replyFail()
             
@@ -64,15 +68,17 @@
                  
 msePrimitive = DistributedElements.DistributedPrimitiveWrapper("mse", 3, __Mse())
 
 
 class __Mae(__AssessTemplate):
     
     def evaluator(self, y_true, y_pred):
-        return tf.keras.metrics.mean_absolute_error(y_true, y_pred)
+        m = tf.keras.metrics.MeanAbsoluteError()
+        m.update_state(y_true, y_pred)
+        return m.result().numpy()
                  
 maePrimitive = DistributedElements.DistributedPrimitiveWrapper("mae", 3, __Mae())
 
 class __R(__AssessTemplate):
     
     def evaluator(self, y_true, y_pred):
         m = tf.keras.metrics.RootMeanSquaredError()
@@ -95,18 +101,8 @@
 class __Accuracy(__AssessTemplate):
     
     def evaluator(self, y_true, y_pred):
         m = tf.keras.metrics.Accuracy()
         m.update_state(y_true, y_pred)
         return m.result().numpy()
                  
-accuracyPrimitive = DistributedElements.DistributedPrimitiveWrapper("accuracy", 3, __Accuracy())
-
-#only available via pip install tf-nightly.
-class __F1Score(__AssessTemplate):
-    
-    def evaluator(self, y_true, y_pred):
-        m = tf.keras.metrics.F1Score()
-        m.update_state(y_true, y_pred)
-        return m.result().numpy()
-                 
-f1ScorePrimitive = DistributedElements.DistributedPrimitiveWrapper("f1_score", 3, __F1Score())
+accuracyPrimitive = DistributedElements.DistributedPrimitiveWrapper("accuracy", 3, __Accuracy())
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,38 +39,37 @@
         
         if(not predictor_in_ref.HasField('var') and not dataset_ref.HasField('var') and
            not params.HasField('var') and predictor_out_ref.HasField('var')):
             model: tf.keras.Model = SharedCollections().getModel(Utils.parseArgumentMsg(predictor_in_ref))
             datasetId = Utils.parseArgumentMsg(dataset_ref)
             dataset: Dataset = SharedCollections().getDataset(datasetId)
             schema = SharedCollections().getSchema(SharedCollections().getSchemaIdFromDataset(datasetId))
-            params = parseParams(Utils.parseArgumentMsg(params))
             
-            input = None
-            output = None
+            params = Utils.parseArgumentMsg(params)
+            if(type(params) is list[Utils.Struct]):
+                params = parseParams(params)
+            else:
+                params = parseParams(dict())
+            input = list()
+            output = list()
             for attr in dataset.column_names:
                 if(attr in schema.targets):
-                    if(output == None):
-                        output = tf.cast(dataset[attr], tf.float32)
-                    else:
-                        output = tf.stack([output, tf.cast(dataset[attr], tf.float32)], axis = 1)
+                    output.append(tf.cast(dataset[attr], tf.float32))
                 else:
-                    if(input == None):
-                        input = tf.cast(dataset[attr], tf.float32)
-                    else:
-                        input = tf.stack([input, tf.cast(dataset[attr], tf.float32)], axis = 1)
+                    input.append(tf.cast(dataset[attr], tf.float32))
+            output = tf.stack(output, axis = 1)
+            input = tf.stack(input, axis = 1)
             optimizer = tf.keras.optimizers.Adam(learning_rate=params["learning_rate"])
+            
             model.compile(
                 loss = params["loss"],
                 optimizer=optimizer,
-                metrics=[tf.keras.metrics.CategoricalAccuracy()],
+                metrics=["mse"],
             )
-            
             model.fit(x=input,y=output, batch_size=params["batch"], epochs=params["epoch"])
-            
             id = SharedCollections().addModel(model)
             yield request.replySuccess(substitutions={
                 predictor_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,8 +42,8 @@
                                                .addSchema(collections.Schema(schema_name, attributes, targets))) 
                 }
             yield request.replySuccess(substitutions, hasNext=False)
         else:
             request.replyFail()
             
             
-theoryToSchemaPrimitive = DistributedElements.DistributedPrimitiveWrapper("theoryToSchema", 1, __TheoryToSchemaPrimitive())
+theoryToSchemaPrimitive = DistributedElements.DistributedPrimitiveWrapper("theory_to_schema", 1, __TheoryToSchemaPrimitive())
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         transf_in_ref = request.arguments[0]
         dataset_ref = request.arguments[1]
         transf_out_ref = request.arguments[2]
         
         if(not transf_in_ref.HasField('var') and not dataset_ref.HasField('var') and transf_out_ref.HasField('var')):
             transf: Pipeline = SharedCollections().getPipeline(Utils.parseArgumentMsg(transf_in_ref))
             dataset: Dataset = SharedCollections().getDataset(Utils.parseArgumentMsg(dataset_ref))
-            
             id = SharedCollections().addPipeline(transf.adapt(dataset))
             yield request.replySuccess(substitutions={
                 transf_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,24 @@
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_ref = request.arguments[0]
         transf_ref = request.arguments[1]
         
         if(not schema_ref.HasField('var') and transf_ref.HasField('var')):
             schema_id = Utils.parseArgumentMsg(schema_ref)
-            
-            id = SharedCollections().addPipeline(Pipeline(schema_id))
+            pipeline = Pipeline(schema_id)
+            id = SharedCollections().addPipeline(pipeline)
             yield request.replySuccess(substitutions={
                 transf_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         elif(schema_ref.HasField('var') and not transf_ref.HasField('var')):
             transformation_id = Utils.parseArgumentMsg(transf_ref)
             transformation: Pipeline = SharedCollections().getPipeline(transformation_id)
-            
             id = SharedCollections().addSchema(transformation.computeFinalSchema())
             yield request.replySuccess(substitutions = {
                 schema_ref.var: Utils.buildConstantArgumentMsg(id)
             }, hasNext=False)            
         else:
             yield request.replyFail()
             
             
-schemaTrasformation = DistributedElements.DistributedPrimitiveWrapper("schema_trasformation", 2, __SchemaTrasformation())
+schemaTrasformation = DistributedElements.DistributedPrimitiveWrapper("schema_transformation", 2, __SchemaTrasformation())
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
 import tensorflow as tf
 from ..collections import SharedCollections
 from ..schema.schemaClass import Schema
 from datasets import Dataset
+import itertools
 
 class Transformation(ABC):
     applier = None
     inverter = None
     
     @abstractmethod
     def copy(self):
@@ -45,21 +46,22 @@
     
     def copy(self):
         return Dropper()      
     
 class Pipeline:   
     originalSchemaId: str = None
     originalSchema: Schema = None
-    __layers: dict = {}
+    __layers: dict
 
     def __init__(self,
                  originalSchema: str,
                  layers: dict = {}):
         self.originalSchemaId = originalSchema 
         self.originalSchema = SharedCollections().getSchema(originalSchema)
+        self.__layers = {}
         for attr in self.originalSchema.attributes:
             self.__layers[attr.name] = [] + layers.get(attr.name, [])
         
     def append(self, pipeline: dict):
         new_pipeline = {}
         for attr, layers in self.__layers.items():
             new_pipeline[attr] = layers + pipeline.get(attr, [])
@@ -80,14 +82,17 @@
         
     def apply(self, inputs):
         output = {}
         for attr, layers in self.__layers.items():
             output[attr] = tf.reshape(inputs[attr], (len(inputs[attr]), -1))
             for layer in layers:  
                 output[attr] = layer.applier(output[attr])
+
+            
+            
         return Dataset.from_dict(output)
         
     def invert(self, inputs):
         output = {}
         for attr, layers in self.__layers.items():
             reversedList = list(layers)
             reversedList.reverse()
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.1.0/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 1.0.5
+Version: 1.1.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.0.5/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.1.0/prolog_primitives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.5/setup.py` & `prolog_primitives-1.1.0/setup.py`

 * *Files identical despite different names*

