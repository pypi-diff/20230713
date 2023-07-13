# Comparing `tmp/seldon-core-1.9.0.tar.gz` & `tmp/seldon-core-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seldon-core-1.9.0.tar", last modified: Wed Jun 16 14:42:33 2021, max compression
+gzip compressed data, was "dist/seldon-core-1.9.1.tar", last modified: Fri Jul  2 12:22:10 2021, max compression
```

## Comparing `seldon-core-1.9.0.tar` & `seldon-core-1.9.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       11 2020-06-24 09:10:49.000000 seldon-core-1.9.0/.gitignore
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11354 2019-11-17 19:17:19.000000 seldon-core-1.9.0/LICENSE
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       89 2019-12-04 11:53:18.000000 seldon-core-1.9.0/MANIFEST.in
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3651 2021-06-14 15:53:23.000000 seldon-core-1.9.0/Makefile
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      351 2021-06-16 14:42:33.000000 seldon-core-1.9.0/PKG-INFO
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      191 2019-11-17 19:17:19.000000 seldon-core-1.9.0/README.md
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/conda.recipe/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1090 2021-05-19 08:53:51.000000 seldon-core-1.9.0/conda.recipe/meta.yaml
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/licenses/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)   318121 2021-06-16 14:40:39.000000 seldon-core-1.9.0/licenses/license.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2750 2021-06-16 14:40:39.000000 seldon-core-1.9.0/licenses/license_info.csv
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2167 2021-06-16 14:33:58.000000 seldon-core-1.9.0/licenses/license_info.no_versions.csv
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      193 2021-02-20 08:04:23.000000 seldon-core-1.9.0/pyproject.toml
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      107 2019-11-17 19:17:19.000000 seldon-core-1.9.0/readme.rst
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      414 2021-05-19 08:53:51.000000 seldon-core-1.9.0/requirements-dev.txt
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       74 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4202 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/api_tester.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    16954 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/batch_processor.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3052 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/flask_utils.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2954 2021-06-14 15:53:23.000000 seldon-core-1.9.0/seldon_core/gunicorn_utils.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1201 2021-02-08 15:51:37.000000 seldon-core-1.9.0/seldon_core/imports_helper.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4421 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/metadata.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    10363 2021-03-17 11:04:22.000000 seldon-core-1.9.0/seldon_core/metrics.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    15408 2021-06-14 15:53:23.000000 seldon-core-1.9.0/seldon_core/microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8270 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/microservice_tester.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2021-02-08 15:51:37.000000 seldon-core-1.9.0/seldon_core/mlmd_utils.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core/openapi/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    34888 2021-03-19 13:46:08.000000 seldon-core-1.9.0/seldon_core/openapi/seldon.json
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core/proto/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2021-03-19 13:46:10.000000 seldon-core-1.9.0/seldon_core/proto/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3798 2021-03-19 13:46:05.000000 seldon-core-1.9.0/seldon_core/proto/prediction.proto
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    63227 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/prediction_pb2.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    25729 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/prediction_pb2.pyi
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    32266 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/prediction_pb2_grpc.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      203 2019-12-04 11:53:18.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1369 2021-03-19 13:46:08.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/resource_handle.proto
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     7811 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/resource_handle_pb2.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3375 2021-03-19 13:46:08.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor.proto
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14225 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor_pb2.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1663 2021-03-19 13:46:08.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor_shape.proto
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4852 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor_shape_pb2.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2445 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/types.proto
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    12628 2021-05-23 23:16:19.000000 seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/types_pb2.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    71988 2021-05-19 08:53:51.000000 seldon-core-1.9.0/seldon_core/seldon_client.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    22252 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/seldon_methods.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3222 2019-11-17 19:17:19.000000 seldon-core-1.9.0/seldon_core/serving_test_gen.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2299 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/storage.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14871 2021-03-17 11:04:22.000000 seldon-core-1.9.0/seldon_core/user_model.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    22481 2021-02-20 08:04:23.000000 seldon-core-1.9.0/seldon_core/utils.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       22 2021-06-16 14:39:48.000000 seldon-core-1.9.0/seldon_core/version.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11321 2021-03-17 11:04:22.000000 seldon-core-1.9.0/seldon_core/wrapper.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      351 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/PKG-INFO
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2929 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/SOURCES.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/dependency_links.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      319 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/entry_points.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2021-06-16 07:54:45.000000 seldon-core-1.9.0/seldon_core.egg-info/not-zip-safe
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      453 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/requires.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       18 2021-06-16 14:42:33.000000 seldon-core-1.9.0/seldon_core.egg-info/top_level.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      697 2021-06-16 14:42:33.000000 seldon-core-1.9.0/setup.cfg
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2024 2021-06-16 14:39:48.000000 seldon-core-1.9.0/setup.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2019-12-12 13:37:59.000000 seldon-core-1.9.0/tests/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1402 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/conftest.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3361 2021-05-19 08:53:51.000000 seldon-core-1.9.0/tests/helpers.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      567 2019-11-17 19:17:19.000000 seldon-core-1.9.0/tests/resources/bad_contract.json
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      895 2019-11-17 19:17:19.000000 seldon-core-1.9.0/tests/resources/contract.json
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/custom-metrics-model/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/custom-metrics-model/.s2i/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       52 2021-05-19 08:53:51.000000 seldon-core-1.9.0/tests/resources/custom-metrics-model/.s2i/environment
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      892 2021-03-17 11:04:22.000000 seldon-core-1.9.0/tests/resources/custom-metrics-model/MyModel.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/model-template-app/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/model-template-app/.s2i/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       52 2021-05-19 08:53:51.000000 seldon-core-1.9.0/tests/resources/model-template-app/.s2i/environment
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1232 2021-02-08 15:51:37.000000 seldon-core-1.9.0/tests/resources/model-template-app/MyModel.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      192 2020-08-13 08:56:51.000000 seldon-core-1.9.0/tests/resources/model-template-app/README.md
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1024 2020-08-13 08:56:51.000000 seldon-core-1.9.0/tests/resources/model-template-app/contract.json
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/model-template-app2/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/model-template-app2/.s2i/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       70 2021-05-19 08:53:51.000000 seldon-core-1.9.0/tests/resources/model-template-app2/.s2i/environment
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/model-template-app2/mymodule/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2020-08-13 08:56:51.000000 seldon-core-1.9.0/tests/resources/model-template-app2/mymodule/__init.py__
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1232 2021-02-08 15:51:37.000000 seldon-core-1.9.0/tests/resources/model-template-app2/mymodule/my_model.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    10871 2019-11-17 19:17:19.000000 seldon-core-1.9.0/tests/resources/test.png
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       56 2019-11-17 19:17:19.000000 seldon-core-1.9.0/tests/resources/test.txt
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-06-16 14:42:33.000000 seldon-core-1.9.0/tests/resources/tracing_config/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      110 2020-08-13 08:56:51.000000 seldon-core-1.9.0/tests/resources/tracing_config/tracing.yaml
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2231 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_api_tester.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3104 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_application_exception_microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    17305 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_combiner_microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      717 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_flask_utils.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1456 2021-03-17 11:04:22.000000 seldon-core-1.9.0/tests/test_gunicorn_utils.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    18564 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_metadata.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    27264 2021-03-17 11:04:22.000000 seldon-core-1.9.0/tests/test_metrics.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9291 2021-05-19 08:53:51.000000 seldon-core-1.9.0/tests/test_microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3418 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_microservice_tester.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    37195 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_model_microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11535 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_router_microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    20884 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_runtime_metrics_tags.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    18327 2021-04-07 17:31:37.000000 seldon-core-1.9.0/tests/test_seldon_client.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1527 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_storage.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    31118 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_transformer_microservice.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1599 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_user_model.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    16437 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/test_utils.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      165 2021-02-20 08:04:23.000000 seldon-core-1.9.0/tests/utils.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       11 2020-06-24 09:10:49.000000 seldon-core-1.9.1/.gitignore
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11354 2019-11-17 19:17:19.000000 seldon-core-1.9.1/LICENSE
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       89 2019-12-04 11:53:18.000000 seldon-core-1.9.1/MANIFEST.in
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3651 2021-07-02 12:14:52.000000 seldon-core-1.9.1/Makefile
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      351 2021-07-02 12:22:10.000000 seldon-core-1.9.1/PKG-INFO
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      191 2019-11-17 19:17:19.000000 seldon-core-1.9.1/README.md
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/conda.recipe/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1090 2021-06-26 14:46:13.000000 seldon-core-1.9.1/conda.recipe/meta.yaml
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/licenses/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)   318121 2021-07-02 12:15:31.000000 seldon-core-1.9.1/licenses/license.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2750 2021-07-02 12:15:31.000000 seldon-core-1.9.1/licenses/license_info.csv
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2167 2021-07-02 12:15:31.000000 seldon-core-1.9.1/licenses/license_info.no_versions.csv
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      193 2021-06-26 14:46:13.000000 seldon-core-1.9.1/pyproject.toml
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      107 2019-11-17 19:17:19.000000 seldon-core-1.9.1/readme.rst
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      414 2021-07-02 12:15:31.000000 seldon-core-1.9.1/requirements-dev.txt
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       74 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4202 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/api_tester.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    16954 2021-07-02 12:15:31.000000 seldon-core-1.9.1/seldon_core/batch_processor.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3052 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/flask_utils.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2954 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/gunicorn_utils.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1201 2021-06-25 16:42:39.000000 seldon-core-1.9.1/seldon_core/imports_helper.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4421 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/metadata.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    10363 2021-07-02 12:15:31.000000 seldon-core-1.9.1/seldon_core/metrics.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    15408 2021-07-02 12:15:31.000000 seldon-core-1.9.1/seldon_core/microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8270 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/microservice_tester.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/mlmd_utils.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core/openapi/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    34888 2021-03-19 13:46:08.000000 seldon-core-1.9.1/seldon_core/openapi/seldon.json
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core/proto/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2021-03-19 13:46:10.000000 seldon-core-1.9.1/seldon_core/proto/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3798 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/prediction.proto
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    63227 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/prediction_pb2.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    25729 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/prediction_pb2.pyi
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    32266 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/prediction_pb2_grpc.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      203 2019-12-04 11:53:18.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1369 2021-06-25 16:42:39.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/resource_handle.proto
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     7811 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/resource_handle_pb2.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3375 2021-03-19 13:46:08.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor.proto
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14225 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor_pb2.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1663 2021-03-19 13:46:08.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor_shape.proto
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4852 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor_shape_pb2.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2445 2021-05-23 23:16:19.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/types.proto
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    12628 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/types_pb2.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    71988 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/seldon_client.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    22252 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/seldon_methods.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3222 2019-11-17 19:17:19.000000 seldon-core-1.9.1/seldon_core/serving_test_gen.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2299 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/storage.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14871 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/user_model.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    22481 2021-06-26 14:46:13.000000 seldon-core-1.9.1/seldon_core/utils.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       22 2021-07-02 12:16:37.000000 seldon-core-1.9.1/seldon_core/version.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11321 2021-07-02 12:15:31.000000 seldon-core-1.9.1/seldon_core/wrapper.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/seldon_core.egg-info/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      351 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/PKG-INFO
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2929 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      319 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/entry_points.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/not-zip-safe
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      453 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/requires.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       18 2021-07-02 12:22:09.000000 seldon-core-1.9.1/seldon_core.egg-info/top_level.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      697 2021-07-02 12:22:10.000000 seldon-core-1.9.1/setup.cfg
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2024 2021-07-02 12:16:37.000000 seldon-core-1.9.1/setup.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2019-12-12 13:37:59.000000 seldon-core-1.9.1/tests/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1402 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/conftest.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3361 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/helpers.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      567 2019-11-17 19:17:19.000000 seldon-core-1.9.1/tests/resources/bad_contract.json
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      895 2019-11-17 19:17:19.000000 seldon-core-1.9.1/tests/resources/contract.json
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/custom-metrics-model/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/custom-metrics-model/.s2i/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       52 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/resources/custom-metrics-model/.s2i/environment
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      892 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/resources/custom-metrics-model/MyModel.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/model-template-app/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/model-template-app/.s2i/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       52 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/resources/model-template-app/.s2i/environment
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1232 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/resources/model-template-app/MyModel.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      192 2021-06-25 16:42:39.000000 seldon-core-1.9.1/tests/resources/model-template-app/README.md
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1024 2021-06-25 16:42:39.000000 seldon-core-1.9.1/tests/resources/model-template-app/contract.json
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/model-template-app2/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/model-template-app2/.s2i/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       70 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/resources/model-template-app2/.s2i/environment
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/model-template-app2/mymodule/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2021-06-25 16:42:39.000000 seldon-core-1.9.1/tests/resources/model-template-app2/mymodule/__init.py__
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1232 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/resources/model-template-app2/mymodule/my_model.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    10871 2019-11-17 19:17:19.000000 seldon-core-1.9.1/tests/resources/test.png
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       56 2019-11-17 19:17:19.000000 seldon-core-1.9.1/tests/resources/test.txt
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2021-07-02 12:22:10.000000 seldon-core-1.9.1/tests/resources/tracing_config/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      110 2021-06-25 16:42:39.000000 seldon-core-1.9.1/tests/resources/tracing_config/tracing.yaml
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2231 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_api_tester.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3104 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_application_exception_microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    17305 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_combiner_microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      717 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_flask_utils.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1456 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_gunicorn_utils.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    18564 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_metadata.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    27264 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_metrics.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9291 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3418 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_microservice_tester.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    37195 2021-07-02 12:15:31.000000 seldon-core-1.9.1/tests/test_model_microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11535 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_router_microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    20884 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_runtime_metrics_tags.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    18327 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_seldon_client.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1527 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_storage.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    31118 2021-07-02 12:15:31.000000 seldon-core-1.9.1/tests/test_transformer_microservice.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1599 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/test_user_model.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    16437 2021-07-02 12:15:31.000000 seldon-core-1.9.1/tests/test_utils.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      165 2021-06-26 14:46:13.000000 seldon-core-1.9.1/tests/utils.py
```

### Comparing `seldon-core-1.9.0/LICENSE` & `seldon-core-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/Makefile` & `seldon-core-1.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/conda.recipe/meta.yaml` & `seldon-core-1.9.1/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/licenses/license.txt` & `seldon-core-1.9.1/licenses/license.txt`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/licenses/license_info.csv` & `seldon-core-1.9.1/licenses/license_info.csv`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/licenses/license_info.no_versions.csv` & `seldon-core-1.9.1/licenses/license_info.no_versions.csv`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/api_tester.py` & `seldon-core-1.9.1/seldon_core/api_tester.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/batch_processor.py` & `seldon-core-1.9.1/seldon_core/batch_processor.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/flask_utils.py` & `seldon-core-1.9.1/seldon_core/flask_utils.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/gunicorn_utils.py` & `seldon-core-1.9.1/seldon_core/gunicorn_utils.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/imports_helper.py` & `seldon-core-1.9.1/seldon_core/imports_helper.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/metadata.py` & `seldon-core-1.9.1/seldon_core/metadata.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/metrics.py` & `seldon-core-1.9.1/seldon_core/metrics.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/microservice.py` & `seldon-core-1.9.1/seldon_core/microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/microservice_tester.py` & `seldon-core-1.9.1/seldon_core/microservice_tester.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/openapi/seldon.json` & `seldon-core-1.9.1/seldon_core/openapi/seldon.json`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/prediction.proto` & `seldon-core-1.9.1/seldon_core/proto/prediction.proto`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/prediction_pb2.py` & `seldon-core-1.9.1/seldon_core/proto/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/prediction_pb2.pyi` & `seldon-core-1.9.1/seldon_core/proto/prediction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/prediction_pb2_grpc.py` & `seldon-core-1.9.1/seldon_core/proto/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/resource_handle.proto` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/resource_handle.proto`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/resource_handle_pb2.py` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/resource_handle_pb2.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor.proto` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor.proto`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor_pb2.py` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor_pb2.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor_shape.proto` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor_shape.proto`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/tensor_shape_pb2.py` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/tensor_shape_pb2.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/types.proto` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/types.proto`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/proto/tensorflow/core/framework/types_pb2.py` & `seldon-core-1.9.1/seldon_core/proto/tensorflow/core/framework/types_pb2.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/seldon_client.py` & `seldon-core-1.9.1/seldon_core/seldon_client.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/seldon_methods.py` & `seldon-core-1.9.1/seldon_core/seldon_methods.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/serving_test_gen.py` & `seldon-core-1.9.1/seldon_core/serving_test_gen.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/storage.py` & `seldon-core-1.9.1/seldon_core/storage.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/user_model.py` & `seldon-core-1.9.1/seldon_core/user_model.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/utils.py` & `seldon-core-1.9.1/seldon_core/utils.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core/wrapper.py` & `seldon-core-1.9.1/seldon_core/wrapper.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/seldon_core.egg-info/SOURCES.txt` & `seldon-core-1.9.1/seldon_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/setup.cfg` & `seldon-core-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/setup.py` & `seldon-core-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 all_extra_deps = chain.from_iterable(extras.values())
 extras["all"] = list(set(all_extra_deps))
 
 setup(
     name="seldon-core",
     author="Seldon Technologies Ltd.",
     author_email="hello@seldon.io",
-    version="1.9.0",
+    version="1.9.1",
     description="Seldon Core client and microservice wrapper",
     url="https://github.com/SeldonIO/seldon-core",
     license="Apache 2.0",
     license_files=["LICENSE"],
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6",
```

### Comparing `seldon-core-1.9.0/tests/conftest.py` & `seldon-core-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/helpers.py` & `seldon-core-1.9.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/bad_contract.json` & `seldon-core-1.9.1/tests/resources/bad_contract.json`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/contract.json` & `seldon-core-1.9.1/tests/resources/contract.json`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/custom-metrics-model/MyModel.py` & `seldon-core-1.9.1/tests/resources/custom-metrics-model/MyModel.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/model-template-app/MyModel.py` & `seldon-core-1.9.1/tests/resources/model-template-app/MyModel.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/model-template-app/contract.json` & `seldon-core-1.9.1/tests/resources/model-template-app/contract.json`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/model-template-app2/mymodule/my_model.py` & `seldon-core-1.9.1/tests/resources/model-template-app2/mymodule/my_model.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/resources/test.png` & `seldon-core-1.9.1/tests/resources/test.png`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_api_tester.py` & `seldon-core-1.9.1/tests/test_api_tester.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_application_exception_microservice.py` & `seldon-core-1.9.1/tests/test_application_exception_microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_combiner_microservice.py` & `seldon-core-1.9.1/tests/test_combiner_microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_flask_utils.py` & `seldon-core-1.9.1/tests/test_flask_utils.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_gunicorn_utils.py` & `seldon-core-1.9.1/tests/test_gunicorn_utils.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_metadata.py` & `seldon-core-1.9.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_metrics.py` & `seldon-core-1.9.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_microservice.py` & `seldon-core-1.9.1/tests/test_microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_microservice_tester.py` & `seldon-core-1.9.1/tests/test_microservice_tester.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_model_microservice.py` & `seldon-core-1.9.1/tests/test_model_microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_router_microservice.py` & `seldon-core-1.9.1/tests/test_router_microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_runtime_metrics_tags.py` & `seldon-core-1.9.1/tests/test_runtime_metrics_tags.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_seldon_client.py` & `seldon-core-1.9.1/tests/test_seldon_client.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_storage.py` & `seldon-core-1.9.1/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_transformer_microservice.py` & `seldon-core-1.9.1/tests/test_transformer_microservice.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_user_model.py` & `seldon-core-1.9.1/tests/test_user_model.py`

 * *Files identical despite different names*

### Comparing `seldon-core-1.9.0/tests/test_utils.py` & `seldon-core-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

