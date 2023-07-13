# Comparing `tmp/prolog_primitives-1.1.0.tar.gz` & `tmp/prolog_primitives-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-1.1.0.tar", last modified: Thu Jul 13 16:18:16 2023, max compression
+gzip compressed data, was "prolog_primitives-1.1.1.tar", last modified: Thu Jul 13 17:47:00 2023, max compression
```

## Comparing `prolog_primitives-1.1.0.tar` & `prolog_primitives-1.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.830978 prolog_primitives-1.1.0/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.830978 prolog_primitives-1.1.0/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/basic/nt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.834978 prolog_primitives-1.1.0/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 16:17:40.000000 prolog_primitives-1.1.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.834978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.834978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.838978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.838978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.838978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:16.830978 prolog_primitives-1.1.0/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 16:18:16.000000 prolog_primitives-1.1.0/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:18:16.842978 prolog_primitives-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-13 16:16:09.000000 prolog_primitives-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.935640 prolog_primitives-1.1.1/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.943640 prolog_primitives-1.1.1/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/nt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.935640 prolog_primitives-1.1.1/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/setup.py
```

### Comparing `prolog_primitives-1.1.0/LICENSE` & `prolog_primitives-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/PKG-INFO` & `prolog_primitives-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 1.1.0
+Version: 1.1.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/Session.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/basic/nt.py` & `prolog_primitives-1.1.1/prolog_primitives/basic/nt.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-1.1.1/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-1.1.1/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-1.1.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/launcher.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,17 @@
 
         else:
             yield request.replyFail()
             
 class __Mse(__AssessTemplate):
     
     def evaluator(self, y_true, y_pred):
-        return tf.keras.metrics.mean_squared_error(y_true, y_pred)
+        m = tf.keras.metrics.MeanSquaredError()
+        m.update_state(y_true, y_pred)
+        return m.result().numpy()
                  
 msePrimitive = DistributedElements.DistributedPrimitiveWrapper("mse", 3, __Mse())
 
 
 class __Mae(__AssessTemplate):
     
     def evaluator(self, y_true, y_pred):
```

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/train.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.1.1/prolog_primitives.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 1.1.0
+Version: 1.1.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.1.0/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.1.1/prolog_primitives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.0/setup.py` & `prolog_primitives-1.1.1/setup.py`

 * *Files identical despite different names*

