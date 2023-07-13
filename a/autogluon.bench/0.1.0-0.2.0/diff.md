# Comparing `tmp/autogluon.bench-0.1.0.tar.gz` & `tmp/autogluon.bench-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.bench-0.1.0.tar", last modified: Tue Jul 11 00:14:43 2023, max compression
+gzip compressed data, was "autogluon.bench-0.2.0.tar", last modified: Thu Jul 13 21:28:23 2023, max compression
```

## Comparing `autogluon.bench-0.1.0.tar` & `autogluon.bench-0.2.0.tar`

### file list

```diff
@@ -1,88 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14697 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.248561 autogluon.bench-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.252561 autogluon.bench-0.1.0/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/stack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/dataset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19890 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/multimodal_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/object_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/datasets/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/eval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.256561 autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/output_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/evaluate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/runbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/scripts/generate_cloud_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.260561 autogluon.bench-0.1.0/src/autogluon/bench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 00:14:33.000000 autogluon.bench-0.1.0/src/autogluon/bench/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 00:14:42.000000 autogluon.bench-0.1.0/src/autogluon/bench/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:14:43.252561 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14697 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:14:43.000000 autogluon.bench-0.1.0/src/autogluon.bench.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/sample_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/multimodal_cloud_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/multimodal_local_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/tabular_cloud_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/sample_configs/tabular_local_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/default_config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/destroy.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/docker/gpu_utilization.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/multimodal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/datasets/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/run_evaluation_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.918014 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1358 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/exec.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      464 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/runbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/scripts/generate_cloud_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/src/autogluon/bench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/src/autogluon/bench/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon/bench/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.914014 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 21:28:23.000000 autogluon.bench-0.2.0/src/autogluon.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/tests/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/tests/unittests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/benchmark/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/benchmark/test_runbenchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.910014 autogluon.bench-0.2.0/tests/unittests/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/tests/unittests/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/cloud/aws/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/cloud/aws/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/cloud/aws/test_stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:28:23.922014 autogluon.bench-0.2.0/tests/unittests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/datasets/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-13 21:28:06.000000 autogluon.bench-0.2.0/tests/unittests/datasets/test_utils.py
```

### Comparing `autogluon.bench-0.1.0/LICENSE` & `autogluon.bench-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/PKG-INFO` & `autogluon.bench-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,251 +1,225 @@
-Metadata-Version: 2.1
-Name: autogluon.bench
-Version: 0.1.0
-Summary: UNKNOWN
-Home-page: https://github.com/autogluon/autogluon-bench
-Author: AutoGluon Community
-License: Apache-2.0
-Project-URL: Bug Reports, https://github.com/autogluon/autogluon-bench/issues
-Project-URL: Source, https://github.com/autogluon/autogluon-bench/
-Description: <div align="left">
-          <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
-        </div>
-        
-        # AutoGluon-Bench
-        
-        Welcome to AutoGluon-Bench, a suite for benchmarking your AutoML frameworks.
-        
-        ## Setup
-        
-        Follow the steps below to set up autogluon-bench:
-        
-        ```bash
-        # create virtual env
-        python3 -m venv .venv_agbench
-        source .venv_agbench/bin/activate
-        ```
-        
-        Install `autogloun-bench` from PyPI:
-        
-        ```bash
-        python3 -m pip install autogluon.bench
-        ```
-        
-        Or install `autogluon-bench` from source:
-        
-        ```bash
-        git clone https://github.com/autogluon/autogluon-bench.git
-        cd autogluon-bench
-        
-        # install from source in editable mode
-        pip install -e .
-        ```
-        
-        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
-        
-        ```
-        agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
-        ```
-        
-        
-        ## Run benchmarks locally
-        
-        To run the benchmarks on your local machine, use the following command:
-        
-        ```
-        agbench run path/to/local_config_file
-        ```
-        
-        Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
-        
-        The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
-        
-        
-        ### Tabular Benchmark
-        
-        To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
-        
-        The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
-        
-        To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
-        
-        
-        ### Multimodal Benchmark
-        
-        For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
-        
-        You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
-        
-        ## Run benchmarks on AWS
-        
-        AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
-        
-        To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
-        
-        1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
-        2. Source profile or restart the terminal.
-        3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
-        ```bash
-        nvm install $VERSION  # install Node.js
-        npm install -g aws-cdk  # install aws-cdk
-        cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
-        ```
-        
-        If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
-        
-        ```bash
-        cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
-        ```
-        
-        You will need a cloud configuration file to run the benchmarks. You can edit the provided [sample cloud config files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs), or use the CLI tool to generate the cloud config files locally.
-        
-        For multimodal:
-        
-        ```
-        agbench generate-cloud-config --module multimodal --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --git-uri-branch <GIT_URI#BRANCH> --dataset-names DATASET_1,DATASET_2 --presets <PRESET_1>,<PRESET_2> --time-limit <TIME_LIMIT_1>,<TIME_LIMIT_2> --hyperparameters "key_1:value_1,key_2:value_2;key_1:value_3,key_2:value_4"
-        ```
-        
-        For tabular:
-        ```
-        agbench generate-cloud-config --module tabular --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --framework <FRAMEWORK>:<LABEL> --amlb-benchmark <BENCHMARK1>,<BENCHMARK2> --amlb-task "BENCHMARK1:DATASET1,DATASET2;BENCHMARK2:DATASET3" --amlb-constraint <CONSTRAINT>
-        ```
-        
-        For more details, you can run
-        ```
-        agbench generate-cloud-config --help
-        ```
-        
-        After having the configuration file ready, use the command below to initiate benchmark runs on cloud:
-        
-        ```
-        agbench run /path/to/cloud_config_file
-        ```
-        
-        This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
-        
-        In order for the Lambda function to submit multiple jobs simultaneously, you need to specify a list of values for each module-specific key. Each combination of configurations is saved and uploaded to your specified `METRICS_BUCKET` in S3, stored under `S3://{METRICS_BUCKET}/configs/{BENCHMARK_NAME}_{timestamp}/{BENCHMARK_NAME}_split_{UID}.yaml`. Here, `UID` is a unique ID assigned to the split.
-        
-        The AWS infrastructure configurations and submitted job IDs are saved locally at `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`. You can use this file to check the job status at any time:
-        
-        ```bash
-        agbench get-job-status --config-file /path/to/aws_configs.yaml
-        ```
-        
-        You can also check the job status using job IDs:
-        
-        ```bash
-        agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
-        
-        ```
-        
-        Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
-        
-        A cloud configuration file with time-stamped `benchmark_name` is also saved under `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml`
-        
-        By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
-        
-        ```bash
-        agbench run path/to/cloud_config_file --remove-resources
-        ```
-        
-        This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
-        
-        If you want to manually remove resources later, use:
-        
-        ```bash
-        agbench destroy-stack --config-file `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`
-        ```
-        
-        Or you can remove specific stacks by running:
-        
-        ```bash
-        agbench destroy-stack --static-resource-stack STATIC_RESOURCE_STACK_NAME --batch-stack BATCH_STACK_NAME --cdk-deploy-account CDK_DEPLOY_ACCOUNT --cdk-deploy-region CDK_DEPLOY_REGION
-        ```
-        where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
-        
-        
-        ### Configure the AWS infrastructure
-        
-        The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
-        
-        where:
-        - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
-        - `PREFIX` is used as an identifier for the stack and resources created.
-        - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
-        - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
-        - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
-        
-        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabular_cloud_configs.yaml) for reference.
-        
-        
-        ## Evaluating bechmark runs
-        
-        Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
-        In a future release, we intend to add evaluation support for multimodal benchmark results.
-        
-        
-        ### Evaluation Steps
-        
-        Begin by setting up AWS credentials for the default profile for the AWS account that has the benchmark results in S3.
-        
-        Step 1: Aggregate AMLB results on S3. After running the benchmark in [AWS mode](#run-benchmarks-on-aws), take note of the `benchmark_name` with timestamp in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml` and run the command below:
-        ```
-        agbench aggregate-amlb-results {METRICS_BUCKET} {module} {benchmark_name} --constraint {constraint}
-        ```
-        
-        This will create a new file on S3 with this signature:
-        ```
-        s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/results_automlbenchmark_{constraint}_{benchmark_name}.csv
-        ```
-        
-        Currently, aggregation is also supported for multimodal benchmark results without the `--constratint` option.
-        
-        For more details, run:
-        ```
-        agbench aggregate-amlb-results --help
-        ```
-        
-        Step 2: Further clean the aggregated results.
-        
-        If the file is still on S3 from the previous step, run:
-        ```
-        agbench clean-amlb-results {benchmark_name} --results-dir-input s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/ --benchmark-name-in-input-path --constraints constratint_1 --constraints constratint_2 --results-dir-output {results_dir_output} 
-        --out-path-prefix {out_path_prefix} --out-path-suffix {out_path_suffix}
-        ```
-        where `{results_dir_input}` can also be a local directory. This will create a local file `{results_dir_output}/{out_path_prefix}{benchmark_name}{out_path_suffix}`.
-        
-        For more details, run:
-        ```
-        agbench clean-amlb-results --help
-        ```
-        
-        Step 3: Run evaluation on multiple cleaned files from `Step 2`
-        
-        ```
-        agbench evaluate-amlb-results --frameworks_run framework_1 --frameworks_run framework_2 --results-dir-input data/results/input/prepared/openml --paths file_name_1.csv --paths file_name_2.csv --no-clean-data
-        ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Customer Service
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: >=3.8, <3.10
-Description-Content-Type: text/markdown
-Provides-Extra: tests
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
+</div>
+
+# AutoGluon-Bench
+
+Welcome to AutoGluon-Bench, a suite for benchmarking your AutoML frameworks.
+
+## Setup
+
+Follow the steps below to set up autogluon-bench:
+
+```bash
+# create virtual env and update pip
+python3 -m venv .venv_agbench
+source .venv_agbench/bin/activate
+python3 -m pip install --upgrade pip
+```
+
+Install `autogloun-bench` from PyPI:
+
+```bash
+python3 -m pip install autogluon.bench
+```
+
+Install `autogluon-bench` from source for development:
+
+```bash
+git clone https://github.com/autogluon/autogluon-bench.git
+cd autogluon-bench
+
+# install from source in editable mode
+pip install -e ".[tests]"
+```
+
+For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). We made it possible to reflect the development changes by pushing the changes to a remote GitHub branch, and providing the URI when testing on benchmark runs:
+
+```
+agbench run sample_configs/multimodal_cloud_configs.yaml --dev-branch https://github.com/suzhoum/autogluon-bench.git\#add_dev_branch
+```
+
+
+## Run benchmarks locally
+
+To run the benchmarks on your local machine, use the following command:
+
+```
+agbench run path/to/local_config_file
+```
+
+Check out our [sample local configuration files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs) for local runs.
+
+The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
+
+
+### Tabular Benchmark
+
+To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
+
+The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
+
+To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
+
+
+### Multimodal Benchmark
+
+For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
+
+You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
+
+## Run benchmarks on AWS
+
+AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
+
+To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
+
+1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
+2. Source profile or restart the terminal.
+3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
+```bash
+nvm install $VERSION  # install Node.js
+npm install -g aws-cdk  # install aws-cdk
+cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
+```
+
+If it is the first time using CDK to deploy to an AWS environment (An AWS environment is a combination of an AWS account and Region), please run the following:
+
+```bash
+cdk bootstrap aws://CDK_DEPLOY_ACCOUNT/CDK_DEPLOY_REGION
+```
+
+You will need a cloud configuration file to run the benchmarks. You can edit the provided [sample cloud config files](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs), or use the CLI tool to generate the cloud config files locally.
+
+For multimodal:
+
+```
+agbench generate-cloud-config --module multimodal --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --git-uri-branch <GIT_URI#BRANCH> --dataset-names DATASET_1,DATASET_2 --presets <PRESET_1>,<PRESET_2> --time-limit <TIME_LIMIT_1>,<TIME_LIMIT_2> --hyperparameters "key_1:value_1,key_2:value_2;key_1:value_3,key_2:value_4"
+```
+
+For tabular:
+```
+agbench generate-cloud-config --module tabular --cdk-deploy-account <AWS_ACCOUNT_ID> --cdk-deploy-region <AWS_ACCOUNT_REGION> --prefix <PREFIX> --metrics-bucket <METRICS_BUCKET> --framework <FRAMEWORK>:<LABEL> --amlb-benchmark <BENCHMARK1>,<BENCHMARK2> --amlb-task "BENCHMARK1:DATASET1,DATASET2;BENCHMARK2:DATASET3" --amlb-constraint <CONSTRAINT>
+```
+
+For more details, you can run
+```
+agbench generate-cloud-config --help
+```
+
+After having the configuration file ready, use the command below to initiate benchmark runs on cloud:
+
+```
+agbench run /path/to/cloud_config_file
+```
+
+This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
+
+In order for the Lambda function to submit multiple jobs simultaneously, you need to specify a list of values for each module-specific key. Each combination of configurations is saved and uploaded to your specified `METRICS_BUCKET` in S3, stored under `S3://{METRICS_BUCKET}/configs/{BENCHMARK_NAME}_{timestamp}/{BENCHMARK_NAME}_split_{UID}.yaml`. Here, `UID` is a unique ID assigned to the split.
+
+The AWS infrastructure configurations and submitted job IDs are saved locally at `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`. You can use this file to check the job status at any time:
+
+```bash
+agbench get-job-status --config-file /path/to/aws_configs.yaml
+```
+
+You can also check the job status using job IDs:
+
+```bash
+agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
+
+```
+
+Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
+
+A cloud configuration file with time-stamped `benchmark_name` is also saved under `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml`
+
+By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
+
+```bash
+agbench run path/to/cloud_config_file --remove-resources
+```
+
+This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
+
+If you want to manually remove resources later, use:
+
+```bash
+agbench destroy-stack --config-file `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`
+```
+
+Or you can remove specific stacks by running:
+
+```bash
+agbench destroy-stack --static-resource-stack STATIC_RESOURCE_STACK_NAME --batch-stack BATCH_STACK_NAME --cdk-deploy-account CDK_DEPLOY_ACCOUNT --cdk-deploy-region CDK_DEPLOY_REGION
+```
+where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
+
+
+### Configure the AWS infrastructure
+
+The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
+
+where:
+- `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
+- `PREFIX` is used as an identifier for the stack and resources created.
+- `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
+- `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
+- `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
+
+To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/tabular_cloud_configs.yaml) for reference.
+
+
+### Monitoring metrics for your instances on AWS
+
+A variety of metrics are available for the EC2 instances that are launched during benchmarking. These can be accessed through the AWS Console by following this navigation path: `CloudWatch` -> `All metrics` -> `AWS namespaces` -> `EC2`. For a comprehensive list of these metrics, refer to the [official AWS documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html).
+
+In addition to the standard metrics, we also provide a custom metric for `GPUUtilization`. This can be found in the `CloudWatch` section under `All metrics` -> `Custom namespaces` -> `EC2`. Please note that the `GPUUtilization` metric is also updated every five minutes.
+
+
+## Evaluating bechmark runs
+
+Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
+In a future release, we intend to add evaluation support for multimodal benchmark results.
+
+
+### Evaluation Steps
+
+Begin by setting up AWS credentials for the default profile for the AWS account that has the benchmark results in S3.
+
+Step 1: Aggregate AMLB results on S3. After running the benchmark in [AWS mode](#run-benchmarks-on-aws), take note of the `benchmark_name` with timestamp in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/{module}_cloud_configs.yaml` and run the command below:
+```
+agbench aggregate-amlb-results {METRICS_BUCKET} {module} {benchmark_name} --constraint {constraint}
+```
+
+This will create a new file on S3 with this signature:
+```
+s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/results_automlbenchmark_{constraint}_{benchmark_name}.csv
+```
+
+Currently, aggregation is also supported for multimodal benchmark results without the `--constratint` option.
+
+For more details, run:
+```
+agbench aggregate-amlb-results --help
+```
+
+Step 2: Further clean the aggregated results.
+
+If the file is still on S3 from the previous step, run:
+```
+agbench clean-amlb-results {benchmark_name} --results-dir-input s3://{METRICS_BUCKET}/aggregated/{module}/{benchmark_name}/ --benchmark-name-in-input-path --constraints constratint_1 --constraints constratint_2 --results-dir-output {results_dir_output} 
+--out-path-prefix {out_path_prefix} --out-path-suffix {out_path_suffix}
+```
+where `{results_dir_input}` can also be a local directory. This will create a local file `{results_dir_output}/{out_path_prefix}{benchmark_name}{out_path_suffix}`.
+
+For more details, run:
+```
+agbench clean-amlb-results --help
+```
+
+Step 3: Run evaluation on multiple cleaned files from `Step 2`
+
+```
+agbench evaluate-amlb-results --frameworks_run framework_1 --frameworks_run framework_2 --results-dir-input data/results/input/prepared/openml --paths file_name_1.csv --paths file_name_2.csv --no-clean-data
+```
```

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/app.py` & `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/app.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py` & `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py` & `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py` & `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py` & `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/batch_stack/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from autogluon.bench.cloud.aws.batch_stack.constructs.instance_profile import InstanceProfile
 
 """
 Sample CDK code for creating the required infrastructure for running a AWS Batch job.
 AWS Batch as the compute enviroment in which a docker image runs the benchmarking script.
 """
 
-with importlib.resources.path("autogluon.bench", "Dockerfile") as file_path:
+with importlib.resources.path("autogluon.bench.cloud.aws.docker", "Dockerfile") as file_path:
     docker_base_dir = os.path.dirname(file_path)
 
 with importlib.resources.path("autogluon.bench.cloud.aws.batch_stack.lambdas", "lambda_function.py") as file_path:
     lambda_script_dir = os.path.dirname(file_path)
 
 logger = logging.getLogger(__name__)
 
@@ -142,25 +142,33 @@
             )
         sg = ec2.SecurityGroup(
             self,
             f"{prefix}-security-group",
             vpc=vpc,
         )
 
+        # Add inbound rule for ssh access
+        # sg.add_ingress_rule(
+        #     peer=ec2.Peer.any_ipv4(),
+        #     connection=ec2.Port.tcp(22),
+        #     description="Allow SSH access from Internet"
+        # )
+
         # Currently CDK can only push to the default repo aws-cdk/assets
         # https://github.com/aws/aws-cdk/issues/12597
         # TODO: use https://github.com/cdklabs/cdk-docker-image-deployment
         docker_image_asset = ecr_assets.DockerImageAsset(
             self,
             f"{prefix}-ecr-docker-image-asset",
             directory=docker_base_dir,
             follow_symlinks=core.SymlinkFollowMode.ALWAYS,
             build_args={
                 "AG_BENCH_VERSION": os.getenv("AG_BENCH_VERSION", "latest"),
                 "AG_BENCH_DEV_URL": os.getenv("AG_BENCH_DEV_URL", ""),
+                "CDK_DEPLOY_REGION": os.environ["CDK_DEPLOY_REGION"],
             },
         )
 
         docker_container_image = ecs.ContainerImage.from_docker_image_asset(docker_image_asset)
 
         container = batch.JobDefinitionContainer(
             image=docker_container_image,
@@ -193,28 +201,43 @@
             launch_template_name=batch_launch_template_name,
             block_devices=[
                 ec2.BlockDevice(
                     device_name="/dev/xvda",
                     volume=ec2.BlockDeviceVolume.ebs(block_device_volume),
                 )
             ],
+            http_tokens=ec2.LaunchTemplateHttpTokens.OPTIONAL,
+            http_endpoint=True,
         )
 
+        cloudwatch_policy = iam.Policy(
+            self,
+            f"{prefix}-cloudwatch-policy",
+            policy_name=f"{prefix}-cloudwatch-policy",
+            statements=[
+                iam.PolicyStatement(
+                    actions=["cloudwatch:PutMetricData"],
+                    effect=iam.Effect.ALLOW,
+                    resources=["*"],
+                )
+            ],
+        )
         batch_instance_role = iam.Role(
             self,
             f"{prefix}-instance-role",
             assumed_by=iam.CompositePrincipal(
                 iam.ServicePrincipal("ec2.amazonaws.com"),
                 iam.ServicePrincipal("ecs.amazonaws.com"),
                 iam.ServicePrincipal("ecs-tasks.amazonaws.com"),
             ),
             managed_policies=[
                 iam.ManagedPolicy.from_aws_managed_policy_name("service-role/AmazonEC2ContainerServiceforEC2Role"),
             ],
         )
+        batch_instance_role.attach_inline_policy(cloudwatch_policy)
 
         metrics_bucket = static_stack.metrics_bucket
         data_bucket = static_stack.data_bucket
         if data_bucket is not None:
             data_bucket.grant_read(batch_instance_role)
         metrics_bucket.grant_read_write(batch_instance_role)
 
@@ -224,14 +247,15 @@
         compute_environment = batch.ComputeEnvironment(
             self,
             f"{prefix}-compute-environment",
             compute_resources=batch.ComputeResources(
                 allocation_strategy=batch.AllocationStrategy.BEST_FIT_PROGRESSIVE,
                 vpc=vpc,
                 vpc_subnets=ec2.SubnetSelection(subnets=vpc.private_subnets),
+                # vpc_subnets=ec2.SubnetSelection(subnets=vpc.public_subnets),  # use public subnet for ssh
                 maxv_cpus=compute_env_maxv_cpus,
                 instance_role=batch_instance_profile.profile_arn,
                 instance_types=instances,
                 security_groups=[sg],
                 type=batch.ComputeResourceType.ON_DEMAND,
                 # ec2_key_pair=f"{prefix}-perm-key", # set this if you need ssh into instance
                 launch_template=batch.LaunchTemplateSpecification(
```

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/cloud/aws/stack_handler.py` & `autogluon.bench-0.2.0/src/autogluon/bench/cloud/aws/stack_handler.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/datasets/multimodal_dataset.py` & `autogluon.bench-0.2.0/src/autogluon/bench/datasets/multimodal_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         try:
             data_path = os.path.join(self._base_folder, f"{self._split}.csv")
             self._data = pd.read_csv(data_path)
             self._data["image"] = self._data["image"].apply(
                 lambda ele: _path_expander(ele, base_folder=self._base_folder)
             )
         except FileNotFoundError as e:
-            logger.warn(e)
+            logger.warn(f"The data split {self._split} is not available.")
             self._data = None
 
     @property
     def base_folder(self):
         """Base folder that contains images"""
         return self._base_folder
 
@@ -194,15 +194,15 @@
             self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
             self._image_columns = ["Image1", "Image2"]
             for image_col in self._image_columns:
                 self._data[image_col] = self._data[image_col].apply(
                     lambda ele: _path_expander(ele, base_folder=self._base_folder)
                 )
         except FileNotFoundError as e:
-            logger.warn(e)
+            logger.warn(f"The data split {self._split} is not available.")
             self._data = None
 
     @property
     def image_columns(self):
         """List of image columns"""
         return self._image_columns
 
@@ -251,15 +251,15 @@
 
             self._data[self._image_col] = self._data[self._image_col].apply(
                 lambda ele: _path_expander(ele, base_folder=self._base_folder)
             )
             self._label_col = "relevance"
             self._data[self._label_col] = [1] * len(self._data)
         except FileNotFoundError as e:
-            logger.warn(e)
+            logger.warn(f"The data split {self._split} is not available.")
             self._data = None
 
     @property
     def image_columns(self):
         """List of image columns"""
         return [self._image_col]
```

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/datasets/object_detection_dataset.py` & `autogluon.bench-0.2.0/src/autogluon/bench/datasets/object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/datasets/registry.py` & `autogluon.bench-0.2.0/src/autogluon/bench/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/aggregate/results.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/aggregate/results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/output_context.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_context.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/benchmark_context/output_suite_context.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/constants.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/evaluate_results.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/evaluate_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py` & `autogluon.bench-0.2.0/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/benchmark.py` & `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/exec.py` & `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/exec.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py` & `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py` & `autogluon.bench-0.2.0/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/main.py` & `autogluon.bench-0.2.0/src/autogluon/bench/main.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/runbenchmark.py` & `autogluon.bench-0.2.0/src/autogluon/bench/runbenchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 from typing import List, Optional
 
 import boto3
 import botocore
 import typer
 import yaml
-from typing_extensions import Annotated
 
 from autogluon.bench import __version__ as agbench_version
 from autogluon.bench.cloud.aws.stack_handler import deploy_stack, destroy_stack
 from autogluon.bench.frameworks.multimodal.multimodal_benchmark import MultiModalBenchmark
 from autogluon.bench.frameworks.tabular.tabular_benchmark import TabularBenchmark
 from autogluon.bench.utils.general_utils import formatted_time
```

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/scripts/generate_cloud_configs.py` & `autogluon.bench-0.2.0/src/autogluon/bench/scripts/generate_cloud_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/utils/dataset_utils.py` & `autogluon.bench-0.2.0/src/autogluon/bench/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.1.0/src/autogluon/bench/utils/general_utils.py` & `autogluon.bench-0.2.0/src/autogluon/bench/utils/general_utils.py`

 * *Files identical despite different names*

