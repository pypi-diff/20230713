# Comparing `tmp/sensenova-1.0.1.tar.gz` & `tmp/sensenova-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensenova-1.0.1.tar", last modified: Tue Jul 11 11:00:14 2023, max compression
+gzip compressed data, was "sensenova-1.0.2.tar", last modified: Thu Jul 13 02:54:15 2023, max compression
```

## Comparing `sensenova-1.0.1.tar` & `sensenova-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.821371 sensenova-1.0.1/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.1/LICENSE
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-11 11:00:14.821371 sensenova-1.0.1/PKG-INFO
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2124 2023-07-11 10:58:41.000000 sensenova-1.0.1/README.md
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.1/pyproject.toml
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.801371 sensenova-1.0.1/sensenova/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/_sensenova_scripts.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_requestor.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.813371 sensenova-1.0.1/sensenova/api_resources/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/__init__.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.817371 sensenova-1.0.1/sensenova/api_resources/abstract/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      691 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/createable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/deletable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/downloadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/engine_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/fileable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/listable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/abstract/uploadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/dataset.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/error_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/fine_tune.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      507 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/knowledge_base.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/model.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/api_resources/serving.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    16914 2023-06-29 07:30:41.000000 sensenova-1.0.1/sensenova/cli.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/error.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/object_classes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/sensenova_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/sensenova_response.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.821371 sensenova-1.0.1/sensenova/tests/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      867 2023-07-11 10:58:01.000000 sensenova-1.0.1/sensenova/tests/test_chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3730 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_datasets.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1158 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_fine_tunes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2066 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_knowlege_bases.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      348 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_models.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_prepare_data.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      973 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/tests/test_servings.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/upload_progress.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-07-11 10:58:24.000000 sensenova-1.0.1/sensenova/util.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-06-29 07:11:49.000000 sensenova-1.0.1/sensenova/validators.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-11 10:59:24.000000 sensenova-1.0.1/sensenova/version.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-11 11:00:14.809371 sensenova-1.0.1/sensenova.egg-info/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1725 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       65 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/entry_points.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       71 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-11 11:00:14.000000 sensenova-1.0.1/sensenova.egg-info/top_level.txt
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      613 2023-07-11 11:00:14.825371 sensenova-1.0.1/setup.cfg
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.1/setup.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.465998 sensenova-1.0.2/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.2/LICENSE
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-13 02:54:15.465998 sensenova-1.0.2/PKG-INFO
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2124 2023-07-11 10:58:41.000000 sensenova-1.0.2/README.md
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.2/pyproject.toml
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.369998 sensenova-1.0.2/sensenova/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/_sensenova_scripts.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_requestor.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.401998 sensenova-1.0.2/sensenova/api_resources/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/__init__.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.425998 sensenova-1.0.2/sensenova/api_resources/abstract/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      691 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/createable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/deletable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/downloadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/engine_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/fileable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/listable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/uploadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/dataset.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/error_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/fine_tune.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      507 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/knowledge_base.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/model.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/serving.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    16914 2023-06-29 07:30:41.000000 sensenova-1.0.2/sensenova/cli.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/error.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/object_classes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/sensenova_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/sensenova_response.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.465998 sensenova-1.0.2/sensenova/tests/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-07-12 10:50:35.000000 sensenova-1.0.2/sensenova/tests/test_chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4045 2023-07-12 11:47:55.000000 sensenova-1.0.2/sensenova/tests/test_datasets.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1158 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_fine_tunes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2066 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_knowlege_bases.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      341 2023-07-12 10:46:10.000000 sensenova-1.0.2/sensenova/tests/test_models.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_prepare_data.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      973 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_servings.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/upload_progress.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-07-11 10:58:24.000000 sensenova-1.0.2/sensenova/util.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-07-13 02:46:13.000000 sensenova-1.0.2/sensenova/validators.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-13 02:52:11.000000 sensenova-1.0.2/sensenova/version.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.369998 sensenova-1.0.2/sensenova.egg-info/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1725 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       65 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/entry_points.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       86 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/top_level.txt
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      631 2023-07-13 02:54:15.465998 sensenova-1.0.2/setup.cfg
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.2/setup.py
```

### Comparing `sensenova-1.0.1/LICENSE` & `sensenova-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/PKG-INFO` & `sensenova-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python client library for the Sensenova API
 Home-page: UNKNOWN
 Author: Sensetime
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `sensenova-1.0.1/README.md` & `sensenova-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/__init__.py` & `sensenova-1.0.2/sensenova/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/_sensenova_scripts.py` & `sensenova-1.0.2/sensenova/_sensenova_scripts.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_requestor.py` & `sensenova-1.0.2/sensenova/api_requestor.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/__init__.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/createable_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/deletable_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/downloadable_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/downloadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/engine_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/fileable_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/fileable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/listable_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/abstract/uploadable_api_resource.py` & `sensenova-1.0.2/sensenova/api_resources/abstract/uploadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/chat_completion.py` & `sensenova-1.0.2/sensenova/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/error_object.py` & `sensenova-1.0.2/sensenova/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/fine_tune.py` & `sensenova-1.0.2/sensenova/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/finetune_completion.py` & `sensenova-1.0.2/sensenova/api_resources/finetune_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/api_resources/serving.py` & `sensenova-1.0.2/sensenova/api_resources/serving.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/cli.py` & `sensenova-1.0.2/sensenova/cli.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/error.py` & `sensenova-1.0.2/sensenova/error.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/sensenova_object.py` & `sensenova-1.0.2/sensenova/sensenova_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/tests/test_chat_completion.py` & `sensenova-1.0.2/sensenova/tests/test_chat_completion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 
 import sensenova
 
 # result = sensenova.ChatCompletion.create(
 #     messages=[{"role": "user", "content": "Say this is a test!"}]
 # )
-stream = False
+stream = True
 resp = sensenova.ChatCompletion.create(
-    messages=[{"role": "user", "content": "我们如何在日常生活中减少用水"}],
-    model="llama-7b-test",
+    messages=[{"role": "user", "content": "Say this is a test!"}],
+    model="nova-ptc-xs-v1",
     stream=stream,
 )
 
 if not stream:
     resp = [resp]
 for part in resp:
     choices = part['data']["choices"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sensenova-1.0.1/sensenova/tests/test_datasets.py` & `sensenova-1.0.2/sensenova/tests/test_datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 import io
 import json
+import time
 from tempfile import NamedTemporaryFile
 
 import sensenova
 
 
 def test_dataset_add_file(id, description="1Test client??"):
     result = sensenova.Dataset.add_file(id=id, description=description)
     print(result)
     return result["url"]
 
 
 def test_dataset_list():
     result = sensenova.Dataset.list()
+    # for i in range(12):
+    #     sensenova.Dataset.delete(sid=result['datasets'][i]['id'])
+        # sleep 2s
+        # time.sleep(2)
     print(result)
 
 
 def test_dataset_retrieve(id="mrkd"):
     result = sensenova.Dataset.retrieve(id=id)
     print(result)
 
 
 def test_dataset_delete(id):
     result = sensenova.Dataset.delete(sid=id)
     print(result)
 
 
 def test_dataset_upload(url):
-    payload = [
-        {
-            "instruction": "我们如何在日常生活中减少用水？",
-            "input": "",
-            "output": "1. 使用节水装置，如节水淋浴喷头和水龙头。 \n2. 使用水箱或水桶收集家庭废水，例如洗碗和洗浴。 \n3. 在社区中提高节水意识。 \n4. 检查水管和灌溉系统的漏水情况，并及时修复它们。 \n5. 洗澡时间缩短，使用低流量淋浴头节约用水。 \n6. 收集雨水，用于园艺或其他非饮用目的。 \n7. 刷牙或擦手时关掉水龙头。 \n8. 减少浇水草坪的时间。 \n9. 尽可能多地重复使用灰水（来自洗衣机、浴室水槽和淋浴的水）。 \n10. 只购买能源效率高的洗碗机和洗衣机。"
-        },
-        {
-            "instruction": "编辑文章，使其更吸引读者。",
-            "input": "自主机器人是计算机控制的机器，被编程执行特定任务而不需要任何人类输入。自主机器人在各个行业中被越来越广泛地应用，从制造业到医疗保健再到安全。",
-            "output": "自主机器人是计算机控制的机器，被编程执行特定任务而不需要任何人类输入，从而实现了新的效率、精确度和可靠性水平。自主机器人在各个行业中被越来越广泛地应用，从制造业，它们可以使用精度和一致的质量组装复杂的组件，到医疗保健，可以协助进行医疗测试和处理，再到安全，可以监控大面积地区，保障人们和财产的安全。自主机器人还可以减少在危险或有害环境中的错误和增加安全，在工业流程的检查或维修期间等。由于其多样性，自主机器人将彻底改变我们工作方式的方式，使任务变得更加简单、快速，最终更加愉悦。"
-        }
-    ]
+    # payload = [
+    #     {
+    #         "instruction": "我们如何在日常生活中减少用水？",
+    #         "input": "",
+    #         "output": "1. 使用节水装置，如节水淋浴喷头和水龙头。 \n2. 使用水箱或水桶收集家庭废水，例如洗碗和洗浴。 \n3. 在社区中提高节水意识。 \n4. 检查水管和灌溉系统的漏水情况，并及时修复它们。 \n5. 洗澡时间缩短，使用低流量淋浴头节约用水。 \n6. 收集雨水，用于园艺或其他非饮用目的。 \n7. 刷牙或擦手时关掉水龙头。 \n8. 减少浇水草坪的时间。 \n9. 尽可能多地重复使用灰水（来自洗衣机、浴室水槽和淋浴的水）。 \n10. 只购买能源效率高的洗碗机和洗衣机。"
+    #     },
+    #     {
+    #         "instruction": "编辑文章，使其更吸引读者。",
+    #         "input": "自主机器人是计算机控制的机器，被编程执行特定任务而不需要任何人类输入。自主机器人在各个行业中被越来越广泛地应用，从制造业到医疗保健再到安全。",
+    #         "output": "自主机器人是计算机控制的机器，被编程执行特定任务而不需要任何人类输入，从而实现了新的效率、精确度和可靠性水平。自主机器人在各个行业中被越来越广泛地应用，从制造业，它们可以使用精度和一致的质量组装复杂的组件，到医疗保健，可以协助进行医疗测试和处理，再到安全，可以监控大面积地区，保障人们和财产的安全。自主机器人还可以减少在危险或有害环境中的错误和增加安全，在工业流程的检查或维修期间等。由于其多样性，自主机器人将彻底改变我们工作方式的方式，使任务变得更加简单、快速，最终更加愉悦。"
+    #     }
+    # ]
 
-
-    result = sensenova.Dataset.upload_file(aoss_url=url, file=io.StringIO(json.dumps(payload, ensure_ascii=False)))
+    with open("../../test.json") as file:
+        result = sensenova.Dataset.upload_file(aoss_url=url, file=file)
     print(result)
 
 
 def test_dataset_download(id="mrkd", file_id="1"):
     result = sensenova.Dataset.download(id=id, file_id=file_id)
     print(result.decode('utf-8'))
 
 
 def test_dataset_create(description="Test client"):
     result = sensenova.Dataset.create(description=description)
     print(result)
+    return result["dataset"]["id"]
 
 
 # test_dataset_list()
 if __name__ == "__main__":
-    id = "8ba02d7f-ece5-439c-976c-444d02d74bf8"
-    file_id = "a7cd2a40-747b-430c-8344-3dd62f02dfe8"
+    id = "e2f9075e-ed8d-4b79-87cd-072e974963fd"
+    file_id = "f22c2cd5-248d-4700-af46-a556210de46d"
     # test_dataset_list()
-    # test_dataset_delete(id=id)
+    # test_dataset_delete(id="1502c678-1341-4f5a-a073-f78b5018e0b3")
+    # test_dataset_delete(id="12d1ba23-427c-42ad-af1a-d0b927b8e3b7")
     # test_dataset_download(id=id)
-    # test_dataset_create()
+    # id = test_dataset_create()
     # url = test_dataset_add_file(id=id, description="How are YOU!")
     # print(url)
-    # url = 'https://aoss.cn-sh-01.sensecoreapi-oss.cn/nova-test-training-data/ca249841-727f-4917-a747-a58ca3000cfc?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=35C99457BF6D484C812AE6C7FCC2C459%2F20230629%2Fcn-north-1%2Fs3%2Faws4_request&X-Amz-Date=20230629T060440Z&X-Amz-Expires=600&X-Amz-SignedHeaders=host&X-Amz-Signature=ab953d05b7dfacf81ebaad59004c856a7a9d31aaabddf8e473596ae668359c0c'
     # test_dataset_upload(url)
+    # url = 'https://aoss.cn-sh-01.sensecoreapi-oss.cn/nova-test-training-data/ca249841-727f-4917-a747-a58ca3000cfc?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=35C99457BF6D484C812AE6C7FCC2C459%2F20230629%2Fcn-north-1%2Fs3%2Faws4_request&X-Amz-Date=20230629T060440Z&X-Amz-Expires=600&X-Amz-SignedHeaders=host&X-Amz-Signature=ab953d05b7dfacf81ebaad59004c856a7a9d31aaabddf8e473596ae668359c0c'
     # test_dataset_list()
     # test_dataset_retrieve(id=id)
     test_dataset_download(id=id, file_id=file_id)
```

### Comparing `sensenova-1.0.1/sensenova/tests/test_fine_tunes.py` & `sensenova-1.0.2/sensenova/tests/test_fine_tunes.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/tests/test_knowlege_bases.py` & `sensenova-1.0.2/sensenova/tests/test_knowlege_bases.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/tests/test_prepare_data.py` & `sensenova-1.0.2/sensenova/tests/test_prepare_data.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/tests/test_servings.py` & `sensenova-1.0.2/sensenova/tests/test_servings.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/upload_progress.py` & `sensenova-1.0.2/sensenova/upload_progress.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/util.py` & `sensenova-1.0.2/sensenova/util.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova/validators.py` & `sensenova-1.0.2/sensenova/validators.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/sensenova.egg-info/PKG-INFO` & `sensenova-1.0.2/sensenova.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python client library for the Sensenova API
 Home-page: UNKNOWN
 Author: Sensetime
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `sensenova-1.0.1/sensenova.egg-info/SOURCES.txt` & `sensenova-1.0.2/sensenova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.1/setup.cfg` & `sensenova-1.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 author = Sensetime
 license_files = LICENSE
 
 [options]
 packages = find:
 python_requires = >=3.7.1
 install_requires = 
+	requests >= 2.20
 	PyJWT == 2.6.0
 	tqdm
 	typing_extensions; python_version<"3.8"  # Needed for type hints for mypy
 	aiohttp
 
 [options.entry_points]
 console_scripts =
```

