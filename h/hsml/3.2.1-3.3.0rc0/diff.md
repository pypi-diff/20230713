# Comparing `tmp/hsml-3.2.1.tar.gz` & `tmp/hsml-3.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsml-3.2.1.tar", last modified: Thu Jul 13 09:10:20 2023, max compression
+gzip compressed data, was "hsml-3.3.0rc0.tar", last modified: Mon Jul  3 12:07:27 2023, max compression
```

## Comparing `hsml-3.2.1.tar` & `hsml-3.3.0rc0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/
--rw-r--r--   0     1006     1006       40 2023-06-27 14:44:06.000000 hsml-3.2.1/MANIFEST.in
--rw-r--r--   0     1006     1006     5172 2023-07-13 09:10:20.341163 hsml-3.2.1/PKG-INFO
--rw-r--r--   0     1006     1006     3399 2023-07-13 09:10:19.000000 hsml-3.2.1/README.md
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.325163 hsml-3.2.1/hsml/
--rw-r--r--   0     1006     1006     1016 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.329163 hsml-3.2.1/hsml/client/
--rw-r--r--   0     1006     1006     3685 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/client/__init__.py
--rw-r--r--   0     1006     1006     1876 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/auth.py
--rw-r--r--   0     1006     1006     3946 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/base.py
--rw-r--r--   0     1006     1006     2456 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/exceptions.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.329163 hsml-3.2.1/hsml/client/hopsworks/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     3985 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/hopsworks/base.py
--rw-r--r--   0     1006     1006     2846 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/hopsworks/external.py
--rw-r--r--   0     1006     1006     7088 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/hopsworks/internal.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.333163 hsml-3.2.1/hsml/client/istio/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/istio/__init__.py
--rw-r--r--   0     1006     1006     3455 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/istio/base.py
--rw-r--r--   0     1006     1006     1663 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/istio/external.py
--rw-r--r--   0     1006     1006     6650 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/client/istio/internal.py
--rw-r--r--   0     1006     1006    10216 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/connection.py
--rw-r--r--   0     1006     1006     2627 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/constants.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.333163 hsml-3.2.1/hsml/core/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/core/__init__.py
--rw-r--r--   0     1006     1006    15187 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/core/dataset_api.py
--rw-r--r--   0     1006     1006     7327 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/core/model_api.py
--rw-r--r--   0     1006     1006     2745 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/core/model_registry_api.py
--rw-r--r--   0     1006     1006     5810 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/core/model_serving_api.py
--rw-r--r--   0     1006     1006     1188 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/core/native_hdfs_api.py
--rw-r--r--   0     1006     1006    11463 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/core/serving_api.py
--rw-r--r--   0     1006     1006     1656 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/decorators.py
--rw-r--r--   0     1006     1006     2899 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/deployable_component.py
--rw-r--r--   0     1006     1006     2936 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/deployable_component_logs.py
--rw-r--r--   0     1006     1006    14408 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/deployment.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.337163 hsml-3.2.1/hsml/engine/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/engine/__init__.py
--rw-r--r--   0     1006     1006     1536 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/engine/hopsworks_engine.py
--rw-r--r--   0     1006     1006      934 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/engine/local_engine.py
--rw-r--r--   0     1006     1006    14766 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/engine/model_engine.py
--rw-r--r--   0     1006     1006    23120 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/engine/serving_engine.py
--rw-r--r--   0     1006     1006     4387 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/inference_batcher.py
--rw-r--r--   0     1006     1006     4668 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/inference_endpoint.py
--rw-r--r--   0     1006     1006     4034 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/inference_logger.py
--rw-r--r--   0     1006     1006     4700 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/kafka_topic.py
--rw-r--r--   0     1006     1006    14300 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/model.py
--rw-r--r--   0     1006     1006     6574 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/model_registry.py
--rw-r--r--   0     1006     1006     1861 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/model_schema.py
--rw-r--r--   0     1006     1006    12706 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/model_serving.py
--rw-r--r--   0     1006     1006    15504 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/predictor.py
--rw-r--r--   0     1006     1006     5164 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/predictor_state.py
--rw-r--r--   0     1006     1006     2618 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/predictor_state_condition.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.337163 hsml-3.2.1/hsml/python/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/python/__init__.py
--rw-r--r--   0     1006     1006     2223 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/python/model.py
--rw-r--r--   0     1006     1006     1151 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/python/predictor.py
--rw-r--r--   0     1006     1006     2515 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/python/signature.py
--rw-r--r--   0     1006     1006    11756 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/resources.py
--rw-r--r--   0     1006     1006     2540 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/schema.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.337163 hsml-3.2.1/hsml/sklearn/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/sklearn/__init__.py
--rw-r--r--   0     1006     1006     2218 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/sklearn/model.py
--rw-r--r--   0     1006     1006      977 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/sklearn/predictor.py
--rw-r--r--   0     1006     1006     2510 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/sklearn/signature.py
--rw-r--r--   0     1006     1006     1937 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/tag.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/hsml/tensorflow/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/tensorflow/__init__.py
--rw-r--r--   0     1006     1006     2223 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/tensorflow/model.py
--rw-r--r--   0     1006     1006     1169 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/tensorflow/predictor.py
--rw-r--r--   0     1006     1006     2515 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/tensorflow/signature.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/hsml/torch/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/torch/__init__.py
--rw-r--r--   0     1006     1006     2213 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/torch/model.py
--rw-r--r--   0     1006     1006     1142 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/torch/predictor.py
--rw-r--r--   0     1006     1006     2505 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/torch/signature.py
--rw-r--r--   0     1006     1006     2968 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/transformer.py
--rw-r--r--   0     1006     1006     9842 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/util.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/hsml/utils/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/utils/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/hsml/utils/schema/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/utils/schema/__init__.py
--rw-r--r--   0     1006     1006      936 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/utils/schema/column.py
--rw-r--r--   0     1006     1006     3570 2023-06-27 14:44:06.000000 hsml-3.2.1/hsml/utils/schema/columnar_schema.py
--rw-r--r--   0     1006     1006      976 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/utils/schema/tensor.py
--rw-r--r--   0     1006     1006     2396 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/utils/schema/tensor_schema.py
--rw-r--r--   0     1006     1006      628 2023-07-13 09:10:12.000000 hsml-3.2.1/hsml/version.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.329163 hsml-3.2.1/hsml.egg-info/
--rw-r--r--   0     1006     1006     5172 2023-07-13 09:10:20.000000 hsml-3.2.1/hsml.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2009 2023-07-13 09:10:20.000000 hsml-3.2.1/hsml.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-07-13 09:10:20.000000 hsml-3.2.1/hsml.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      306 2023-07-13 09:10:20.000000 hsml-3.2.1/hsml.egg-info/requires.txt
--rw-r--r--   0     1006     1006       11 2023-07-13 09:10:20.000000 hsml-3.2.1/hsml.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-07-13 09:10:20.341163 hsml-3.2.1/setup.cfg
--rw-r--r--   0     1006     1006     2478 2023-06-27 14:44:06.000000 hsml-3.2.1/setup.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/tests/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/tests/hsml/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/tests/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-07-13 09:10:20.341163 hsml-3.2.1/tests/hsml/core/
--rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.2.1/tests/hsml/core/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/
+-rw-r--r--   0     1006     1006       40 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     5178 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     3399 2023-07-03 12:07:26.000000 hsml-3.3.0rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.908037 hsml-3.3.0rc0/hsml/
+-rw-r--r--   0     1006     1006     1016 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.908037 hsml-3.3.0rc0/hsml/client/
+-rw-r--r--   0     1006     1006     3896 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/client/__init__.py
+-rw-r--r--   0     1006     1006     1876 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/auth.py
+-rw-r--r--   0     1006     1006     3946 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/base.py
+-rw-r--r--   0     1006     1006     2456 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/exceptions.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.912037 hsml-3.3.0rc0/hsml/client/hopsworks/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     3985 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/hopsworks/base.py
+-rw-r--r--   0     1006     1006     2846 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/hopsworks/external.py
+-rw-r--r--   0     1006     1006     7088 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/hopsworks/internal.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.912037 hsml-3.3.0rc0/hsml/client/istio/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/istio/__init__.py
+-rw-r--r--   0     1006     1006     3455 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/istio/base.py
+-rw-r--r--   0     1006     1006     1663 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/istio/external.py
+-rw-r--r--   0     1006     1006     6650 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/client/istio/internal.py
+-rw-r--r--   0     1006     1006    10216 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/connection.py
+-rw-r--r--   0     1006     1006     2627 2023-06-30 15:35:13.000000 hsml-3.3.0rc0/hsml/constants.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.916036 hsml-3.3.0rc0/hsml/core/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/core/__init__.py
+-rw-r--r--   0     1006     1006    15186 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7327 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/core/model_api.py
+-rw-r--r--   0     1006     1006     2745 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/core/model_registry_api.py
+-rw-r--r--   0     1006     1006     5950 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/core/model_serving_api.py
+-rw-r--r--   0     1006     1006     1188 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/core/native_hdfs_api.py
+-rw-r--r--   0     1006     1006    11830 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/core/serving_api.py
+-rw-r--r--   0     1006     1006     1656 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/decorators.py
+-rw-r--r--   0     1006     1006     2899 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/deployable_component.py
+-rw-r--r--   0     1006     1006     2936 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/deployable_component_logs.py
+-rw-r--r--   0     1006     1006    14408 2023-06-30 15:35:13.000000 hsml-3.3.0rc0/hsml/deployment.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.916036 hsml-3.3.0rc0/hsml/engine/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/engine/__init__.py
+-rw-r--r--   0     1006     1006     1536 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/engine/hopsworks_engine.py
+-rw-r--r--   0     1006     1006      934 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/engine/local_engine.py
+-rw-r--r--   0     1006     1006    14765 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/engine/model_engine.py
+-rw-r--r--   0     1006     1006    23119 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/engine/serving_engine.py
+-rw-r--r--   0     1006     1006     4387 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/inference_batcher.py
+-rw-r--r--   0     1006     1006     4668 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/inference_endpoint.py
+-rw-r--r--   0     1006     1006     4034 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/inference_logger.py
+-rw-r--r--   0     1006     1006     4700 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/kafka_topic.py
+-rw-r--r--   0     1006     1006    14300 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/model.py
+-rw-r--r--   0     1006     1006     6574 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/model_registry.py
+-rw-r--r--   0     1006     1006     1861 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/model_schema.py
+-rw-r--r--   0     1006     1006    12706 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/model_serving.py
+-rw-r--r--   0     1006     1006    15504 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/predictor.py
+-rw-r--r--   0     1006     1006     5164 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/predictor_state.py
+-rw-r--r--   0     1006     1006     2618 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/predictor_state_condition.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.920037 hsml-3.3.0rc0/hsml/python/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/python/__init__.py
+-rw-r--r--   0     1006     1006     2223 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/python/model.py
+-rw-r--r--   0     1006     1006     1150 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/python/predictor.py
+-rw-r--r--   0     1006     1006     2515 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/python/signature.py
+-rw-r--r--   0     1006     1006    11754 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/resources.py
+-rw-r--r--   0     1006     1006     2540 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/schema.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.920037 hsml-3.3.0rc0/hsml/sklearn/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/sklearn/__init__.py
+-rw-r--r--   0     1006     1006     2218 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/sklearn/model.py
+-rw-r--r--   0     1006     1006      976 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/sklearn/predictor.py
+-rw-r--r--   0     1006     1006     2510 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/sklearn/signature.py
+-rw-r--r--   0     1006     1006     1937 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/tag.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.920037 hsml-3.3.0rc0/hsml/tensorflow/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/tensorflow/__init__.py
+-rw-r--r--   0     1006     1006     2223 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/tensorflow/model.py
+-rw-r--r--   0     1006     1006     1168 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/tensorflow/predictor.py
+-rw-r--r--   0     1006     1006     2515 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/tensorflow/signature.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.920037 hsml-3.3.0rc0/hsml/torch/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/torch/__init__.py
+-rw-r--r--   0     1006     1006     2213 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/torch/model.py
+-rw-r--r--   0     1006     1006     1141 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/torch/predictor.py
+-rw-r--r--   0     1006     1006     2505 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/torch/signature.py
+-rw-r--r--   0     1006     1006     2968 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/transformer.py
+-rw-r--r--   0     1006     1006     9842 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/util.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.920037 hsml-3.3.0rc0/hsml/utils/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/utils/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/hsml/utils/schema/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/utils/schema/__init__.py
+-rw-r--r--   0     1006     1006      935 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/utils/schema/column.py
+-rw-r--r--   0     1006     1006     3570 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/hsml/utils/schema/columnar_schema.py
+-rw-r--r--   0     1006     1006      975 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/utils/schema/tensor.py
+-rw-r--r--   0     1006     1006     2395 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/utils/schema/tensor_schema.py
+-rw-r--r--   0     1006     1006      631 2023-07-03 12:07:22.000000 hsml-3.3.0rc0/hsml/version.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.908037 hsml-3.3.0rc0/hsml.egg-info/
+-rw-r--r--   0     1006     1006     5178 2023-07-03 12:07:27.000000 hsml-3.3.0rc0/hsml.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2009 2023-07-03 12:07:27.000000 hsml-3.3.0rc0/hsml.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-07-03 12:07:27.000000 hsml-3.3.0rc0/hsml.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      306 2023-07-03 12:07:27.000000 hsml-3.3.0rc0/hsml.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       11 2023-07-03 12:07:27.000000 hsml-3.3.0rc0/hsml.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/setup.cfg
+-rw-r--r--   0     1006     1006     2478 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/tests/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/tests/hsml/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/tests/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:07:27.924037 hsml-3.3.0rc0/tests/hsml/core/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:44:06.000000 hsml-3.3.0rc0/tests/hsml/core/__init__.py
```

### Comparing `hsml-3.2.1/PKG-INFO` & `hsml-3.3.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.2.1
+Version: 3.3.0rc0
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.1
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.3.0rc0
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.2.1 Summary: HSML: An environment
-independent client to interact with the Hopsworks Model Registry Home-page:
-https://github.com/logicalclocks/machine-learning-api Author: Logical Clocks AB
-Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.1
-Description: # Hopsworks Model Management
+Metadata-Version: 2.1 Name: hsml Version: 3.3.0rc0 Summary: HSML: An
+environment independent client to interact with the Hopsworks Model Registry
+Home-page: https://github.com/logicalclocks/machine-learning-api Author:
+Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
+2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
+releases/tag/3.3.0rc0 Description: # Hopsworks Model Management
 [Hopsworks_Community] [Hopsworks_Model_Management_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
```

### Comparing `hsml-3.2.1/README.md` & `hsml-3.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/__init__.py` & `hsml-3.3.0rc0/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/__init__.py` & `hsml-3.3.0rc0/hsml/client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 _hopsworks_client = None
 _istio_client = None
 
 _kserve_installed = None
 _serving_resource_limits = None
 _serving_num_instances_limits = None
+_knative_domain = None
 
 
 def init(
     client_type,
     host=None,
     port=None,
     project=None,
@@ -126,12 +127,22 @@
 
 
 def get_serving_num_instances_limits():
     global _serving_num_instances_limits
     return _serving_num_instances_limits
 
 
+def get_knative_domain():
+    global _knative_domain
+    return _knative_domain
+
+
+def set_knative_domain(knative_domain):
+    global _knative_domain
+    _knative_domain = knative_domain
+
+
 def stop():
     global _hopsworks_client, _istio_client
     _hopsworks_client._close()
     _istio_client._close()
     _hopsworks_client = _istio_client = None
```

### Comparing `hsml-3.2.1/hsml/client/auth.py` & `hsml-3.3.0rc0/hsml/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/base.py` & `hsml-3.3.0rc0/hsml/client/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/exceptions.py` & `hsml-3.3.0rc0/hsml/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/hopsworks/__init__.py` & `hsml-3.3.0rc0/hsml/client/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/hopsworks/base.py` & `hsml-3.3.0rc0/hsml/client/hopsworks/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/hopsworks/external.py` & `hsml-3.3.0rc0/hsml/client/hopsworks/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/hopsworks/internal.py` & `hsml-3.3.0rc0/hsml/client/hopsworks/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/istio/__init__.py` & `hsml-3.3.0rc0/hsml/client/istio/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/istio/base.py` & `hsml-3.3.0rc0/hsml/client/istio/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/istio/external.py` & `hsml-3.3.0rc0/hsml/client/istio/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/client/istio/internal.py` & `hsml-3.3.0rc0/hsml/client/istio/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/connection.py` & `hsml-3.3.0rc0/hsml/connection.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/constants.py` & `hsml-3.3.0rc0/hsml/constants.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/core/__init__.py` & `hsml-3.3.0rc0/hsml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/core/dataset_api.py` & `hsml-3.3.0rc0/hsml/core/dataset_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
             "flowIdentifier": str(size) + "_" + file_name,
             "flowFilename": file_name,
             "flowRelativePath": file_name,
             "flowTotalChunks": num_chunks,
         }
 
     def _upload_request(self, params, path, file_name, chunk):
-
         _client = client.get_instance()
         path_params = ["project", _client._project_id, "dataset", "upload", path]
 
         # Flow configuration params are sent as form data
         _client._send_request(
             "POST", path_params, data=params, files={"file": (file_name, chunk)}
         )
```

### Comparing `hsml-3.2.1/hsml/core/model_api.py` & `hsml-3.3.0rc0/hsml/core/model_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/core/model_registry_api.py` & `hsml-3.3.0rc0/hsml/core/model_registry_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/core/model_serving_api.py` & `hsml-3.3.0rc0/hsml/core/model_serving_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         max_resources = self._serving_api.get_resource_limits()
         client.set_serving_resource_limits(max_resources)
 
         # num instances limits
         num_instances_range = self._serving_api.get_num_instances_limits()
         client.set_serving_num_instances_limits(num_instances_range)
 
+        # Knative domain
+        knative_domain = self._serving_api.get_knative_domain()
+        client.set_knative_domain(knative_domain)
+
     def _set_istio_client_if_available(self):
         """Set istio client if available"""
 
         if client.is_kserve_installed():
             # check existing istio client
             try:
                 if client.get_istio_instance() is not None:
```

### Comparing `hsml-3.2.1/hsml/core/native_hdfs_api.py` & `hsml-3.3.0rc0/hsml/core/native_hdfs_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/core/serving_api.py` & `hsml-3.3.0rc0/hsml/core/serving_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,17 @@
         else:
             _client = client.get_istio_instance()
             if _client is not None:
                 # use istio client
                 path_params = self._get_istio_inference_path(deployment_instance)
                 # - add host header
                 headers["host"] = self._get_inference_request_host_header(
-                    _client._project_name, deployment_instance.name
+                    _client._project_name,
+                    deployment_instance.name,
+                    client.get_knative_domain(),
                 )
             else:
                 # fallback to Hopsworks client
                 _client = client.get_instance()
                 path_params = self._get_hopsworks_inference_path(
                     _client._project_id, deployment_instance
                 )
@@ -277,14 +279,24 @@
         max_instances = _client._send_request("GET", path_params)
 
         return [
             int(min_instances["successMessage"]),
             int(max_instances["successMessage"]),
         ]
 
+    def get_knative_domain(self):
+        """Get the domain used by knative"""
+
+        _client = client.get_instance()
+
+        path_params = ["variables", "kube_knative_domain_name"]
+        domain = _client._send_request("GET", path_params)
+
+        return domain["successMessage"]
+
     def get_logs(self, deployment_instance, component, tail):
         """Get the logs of a deployment
 
         :param deployment_instance: metadata object of the deployment to get logs from
         :type deployment_instance: Deployment
         :param component: deployment component (e.g., predictor or transformer)
         :type component: str
@@ -307,18 +319,18 @@
             "GET", path_params, query_params=query_params
         )
         return deployable_component_logs.DeployableComponentLogs.from_response_json(
             server_logs
         )
 
     def _get_inference_request_host_header(
-        self, project_name: str, deployment_name: str
+        self, project_name: str, deployment_name: str, domain: str
     ):
-        return "{}.{}.hopsworks.ai".format(
-            deployment_name, project_name.replace("_", "-")
+        return "{}.{}.{}".format(
+            deployment_name, project_name.replace("_", "-"), domain
         ).lower()
 
     def _get_hopsworks_inference_path(self, project_id: int, deployment_instance):
         return [
             "project",
             project_id,
             "inference",
```

### Comparing `hsml-3.2.1/hsml/decorators.py` & `hsml-3.3.0rc0/hsml/decorators.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/deployable_component.py` & `hsml-3.3.0rc0/hsml/deployable_component.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/deployable_component_logs.py` & `hsml-3.3.0rc0/hsml/deployable_component_logs.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/deployment.py` & `hsml-3.3.0rc0/hsml/deployment.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/engine/__init__.py` & `hsml-3.3.0rc0/hsml/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/engine/hopsworks_engine.py` & `hsml-3.3.0rc0/hsml/engine/hopsworks_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/engine/local_engine.py` & `hsml-3.3.0rc0/hsml/engine/local_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/engine/model_engine.py` & `hsml-3.3.0rc0/hsml/engine/model_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,14 @@
         return model_instance
 
     def _build_resource_path(self, model_instance, artifact):
         artifact_path = "{}/{}".format(model_instance.version_path, artifact)
         return artifact_path
 
     def save(self, model_instance, model_path, await_registration=480):
-
         _client = client.get_instance()
 
         is_shared_registry = model_instance.shared_registry_project_name is not None
 
         if is_shared_registry:
             dataset_models_root_path = "{}::{}".format(
                 model_instance.shared_registry_project_name,
```

### Comparing `hsml-3.2.1/hsml/engine/serving_engine.py` & `hsml-3.3.0rc0/hsml/engine/serving_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from hsml.constants import DEPLOYMENT, PREDICTOR, PREDICTOR_STATE
 from hsml.core import serving_api, dataset_api
 
 from hsml.client.exceptions import ModelServingException, RestAPIError
 
 
 class ServingEngine:
-
     START_STEPS = [
         PREDICTOR_STATE.CONDITION_TYPE_STOPPED,
         PREDICTOR_STATE.CONDITION_TYPE_SCHEDULED,
         PREDICTOR_STATE.CONDITION_TYPE_INITIALIZED,
         PREDICTOR_STATE.CONDITION_TYPE_STARTED,
         PREDICTOR_STATE.CONDITION_TYPE_READY,
     ]
```

### Comparing `hsml-3.2.1/hsml/inference_batcher.py` & `hsml-3.3.0rc0/hsml/inference_batcher.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/inference_endpoint.py` & `hsml-3.3.0rc0/hsml/inference_endpoint.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/inference_logger.py` & `hsml-3.3.0rc0/hsml/inference_logger.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/kafka_topic.py` & `hsml-3.3.0rc0/hsml/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/model.py` & `hsml-3.3.0rc0/hsml/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/model_registry.py` & `hsml-3.3.0rc0/hsml/model_registry.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/model_schema.py` & `hsml-3.3.0rc0/hsml/model_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/model_serving.py` & `hsml-3.3.0rc0/hsml/model_serving.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/predictor.py` & `hsml-3.3.0rc0/hsml/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/predictor_state.py` & `hsml-3.3.0rc0/hsml/predictor_state.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/predictor_state_condition.py` & `hsml-3.3.0rc0/hsml/predictor_state_condition.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/python/__init__.py` & `hsml-3.3.0rc0/hsml/python/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/python/model.py` & `hsml-3.3.0rc0/hsml/python/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/python/predictor.py` & `hsml-3.3.0rc0/hsml/python/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from hsml.predictor import Predictor
 
 
 class Predictor(Predictor):
     """Configuration for a predictor running a python model."""
 
     def __init__(self, **kwargs):
-
         kwargs["model_framework"] = MODEL.FRAMEWORK_PYTHON
         kwargs["model_server"] = PREDICTOR.MODEL_SERVER_PYTHON
 
         if kwargs["script_file"] is None:
             raise ValueError(
                 "Predictor scripts are required in deployments for custom Python models"
             )
```

### Comparing `hsml-3.2.1/hsml/python/signature.py` & `hsml-3.3.0rc0/hsml/python/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/resources.py` & `hsml-3.3.0rc0/hsml/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,14 @@
         self._limits = limits
 
     def __repr__(self):
         return f"ComponentResources(num_instances: {self._num_instances!r}, requests: {self._requests is not None!r}, limits: {self._limits is not None!r})"
 
 
 class PredictorResources(ComponentResources):
-
     RESOURCES_CONFIG_KEY = "predictor_resources"
     NUM_INSTANCES_KEY = "requested_instances"
 
     def __init__(
         self,
         num_instances: int,
         requests: Optional[Union[Resources, dict]] = None,
@@ -329,15 +328,14 @@
                 else None,
                 "limits": self._limits.to_dict() if self._limits is not None else None,
             },
         }
 
 
 class TransformerResources(ComponentResources):
-
     RESOURCES_CONFIG_KEY = "transformer_resources"
     NUM_INSTANCES_KEY = "requested_transformer_instances"
 
     def __init__(
         self,
         num_instances: int,
         requests: Optional[Union[Resources, dict]] = None,
```

### Comparing `hsml-3.2.1/hsml/schema.py` & `hsml-3.3.0rc0/hsml/schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/sklearn/__init__.py` & `hsml-3.3.0rc0/hsml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/sklearn/model.py` & `hsml-3.3.0rc0/hsml/sklearn/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/sklearn/predictor.py` & `hsml-3.3.0rc0/hsml/torch/predictor.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 #
 
 from hsml.constants import PREDICTOR, MODEL
 from hsml.predictor import Predictor
 
 
 class Predictor(Predictor):
-    """Configuration for a predictor running a sklearn model."""
+    """Configuration for a predictor running a torch model."""
 
     def __init__(self, **kwargs):
-
-        kwargs["model_framework"] = MODEL.FRAMEWORK_SKLEARN
+        kwargs["model_framework"] = MODEL.FRAMEWORK_PYTHON
         kwargs["model_server"] = PREDICTOR.MODEL_SERVER_PYTHON
 
+        if kwargs["script_file"] is None:
+            raise ValueError(
+                "Predictor scripts are required in deployments for Torch models"
+            )
+
         super().__init__(**kwargs)
```

### Comparing `hsml-3.2.1/hsml/sklearn/signature.py` & `hsml-3.3.0rc0/hsml/sklearn/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/tag.py` & `hsml-3.3.0rc0/hsml/tag.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/tensorflow/__init__.py` & `hsml-3.3.0rc0/hsml/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/tensorflow/model.py` & `hsml-3.3.0rc0/hsml/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/tensorflow/predictor.py` & `hsml-3.3.0rc0/hsml/tensorflow/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from hsml.predictor import Predictor
 
 
 class Predictor(Predictor):
     """Configuration for a predictor running a tensorflow model."""
 
     def __init__(self, **kwargs):
-
         kwargs["model_framework"] = MODEL.FRAMEWORK_TENSORFLOW
         kwargs["model_server"] = PREDICTOR.MODEL_SERVER_TF_SERVING
 
         if kwargs["script_file"] is not None:
             raise ValueError(
                 "Predictor scripts are not supported in deployments for Tensorflow models"
             )
```

### Comparing `hsml-3.2.1/hsml/tensorflow/signature.py` & `hsml-3.3.0rc0/hsml/tensorflow/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/torch/__init__.py` & `hsml-3.3.0rc0/hsml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/torch/model.py` & `hsml-3.3.0rc0/hsml/torch/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/torch/predictor.py` & `hsml-3.3.0rc0/hsml/sklearn/predictor.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,20 +15,14 @@
 #
 
 from hsml.constants import PREDICTOR, MODEL
 from hsml.predictor import Predictor
 
 
 class Predictor(Predictor):
-    """Configuration for a predictor running a torch model."""
+    """Configuration for a predictor running a sklearn model."""
 
     def __init__(self, **kwargs):
-
-        kwargs["model_framework"] = MODEL.FRAMEWORK_PYTHON
+        kwargs["model_framework"] = MODEL.FRAMEWORK_SKLEARN
         kwargs["model_server"] = PREDICTOR.MODEL_SERVER_PYTHON
 
-        if kwargs["script_file"] is None:
-            raise ValueError(
-                "Predictor scripts are required in deployments for Torch models"
-            )
-
         super().__init__(**kwargs)
```

### Comparing `hsml-3.2.1/hsml/torch/signature.py` & `hsml-3.3.0rc0/hsml/torch/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/transformer.py` & `hsml-3.3.0rc0/hsml/transformer.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/util.py` & `hsml-3.3.0rc0/hsml/util.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/utils/__init__.py` & `hsml-3.3.0rc0/hsml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/utils/schema/__init__.py` & `hsml-3.3.0rc0/hsml/utils/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/utils/schema/column.py` & `hsml-3.3.0rc0/hsml/utils/schema/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 
 
 class Column:
     """Metadata object representing a column in the schema for a model."""
 
     def __init__(self, type, name=None, description=None):
-
         self.type = str(type)
 
         if name is not None:
             self.name = str(name)
 
         if description is not None:
             self.description = str(description)
```

### Comparing `hsml-3.2.1/hsml/utils/schema/columnar_schema.py` & `hsml-3.3.0rc0/hsml/utils/schema/columnar_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/hsml/utils/schema/tensor.py` & `hsml-3.3.0rc0/hsml/utils/schema/tensor.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 
 
 class Tensor:
     """Metadata object representing a tensor in the schema for a model."""
 
     def __init__(self, type, shape, name=None, description=None):
-
         self.type = str(type)
 
         self.shape = str(shape)
 
         if name is not None:
             self.name = str(name)
```

### Comparing `hsml-3.2.1/hsml/utils/schema/tensor_schema.py` & `hsml-3.3.0rc0/hsml/utils/schema/tensor_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import numpy
 
 
 class TensorSchema:
     """Metadata object representing a tensor schema for a model."""
 
     def __init__(self, tensor_obj=None):
-
         if isinstance(tensor_obj, list):
             self.tensors = self._convert_list_to_schema(tensor_obj)
         elif isinstance(tensor_obj, numpy.ndarray):
             self.tensors = self._convert_tensor_to_schema(tensor_obj)
         else:
             raise TypeError(
                 "{} is not supported in a tensor schema.".format(type(tensor_obj))
```

### Comparing `hsml-3.2.1/hsml/version.py` & `hsml-3.3.0rc0/hsml/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.2.1"
+__version__ = "3.3.0rc0"
```

### Comparing `hsml-3.2.1/hsml.egg-info/PKG-INFO` & `hsml-3.3.0rc0/hsml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.2.1
+Version: 3.3.0rc0
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.1
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.3.0rc0
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.2.1 Summary: HSML: An environment
-independent client to interact with the Hopsworks Model Registry Home-page:
-https://github.com/logicalclocks/machine-learning-api Author: Logical Clocks AB
-Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.1
-Description: # Hopsworks Model Management
+Metadata-Version: 2.1 Name: hsml Version: 3.3.0rc0 Summary: HSML: An
+environment independent client to interact with the Hopsworks Model Registry
+Home-page: https://github.com/logicalclocks/machine-learning-api Author:
+Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
+2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
+releases/tag/3.3.0rc0 Description: # Hopsworks Model Management
 [Hopsworks_Community] [Hopsworks_Model_Management_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
```

### Comparing `hsml-3.2.1/hsml.egg-info/SOURCES.txt` & `hsml-3.3.0rc0/hsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/setup.py` & `hsml-3.3.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/tests/__init__.py` & `hsml-3.3.0rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/tests/hsml/__init__.py` & `hsml-3.3.0rc0/tests/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.1/tests/hsml/core/__init__.py` & `hsml-3.3.0rc0/tests/hsml/core/__init__.py`

 * *Files identical despite different names*

