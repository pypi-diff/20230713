# Comparing `tmp/sensenova-1.0.2.tar.gz` & `tmp/sensenova-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensenova-1.0.2.tar", last modified: Thu Jul 13 02:54:15 2023, max compression
+gzip compressed data, was "dist/sensenova-1.0.3.tar", last modified: Thu Jul 13 11:41:59 2023, max compression
```

## Comparing `sensenova-1.0.2.tar` & `sensenova-1.0.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.465998 sensenova-1.0.2/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.2/LICENSE
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-13 02:54:15.465998 sensenova-1.0.2/PKG-INFO
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2124 2023-07-11 10:58:41.000000 sensenova-1.0.2/README.md
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.2/pyproject.toml
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.369998 sensenova-1.0.2/sensenova/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/_sensenova_scripts.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_requestor.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.401998 sensenova-1.0.2/sensenova/api_resources/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/__init__.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.425998 sensenova-1.0.2/sensenova/api_resources/abstract/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      691 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/createable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/deletable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/downloadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/engine_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/fileable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/listable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/abstract/uploadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/dataset.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/error_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/fine_tune.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      507 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/knowledge_base.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/model.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/api_resources/serving.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    16914 2023-06-29 07:30:41.000000 sensenova-1.0.2/sensenova/cli.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/error.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/object_classes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/sensenova_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/sensenova_response.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.465998 sensenova-1.0.2/sensenova/tests/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-07-12 10:50:35.000000 sensenova-1.0.2/sensenova/tests/test_chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4045 2023-07-12 11:47:55.000000 sensenova-1.0.2/sensenova/tests/test_datasets.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1158 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_fine_tunes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2066 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_knowlege_bases.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      341 2023-07-12 10:46:10.000000 sensenova-1.0.2/sensenova/tests/test_models.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_prepare_data.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      973 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/tests/test_servings.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.2/sensenova/upload_progress.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-07-11 10:58:24.000000 sensenova-1.0.2/sensenova/util.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-07-13 02:46:13.000000 sensenova-1.0.2/sensenova/validators.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-13 02:52:11.000000 sensenova-1.0.2/sensenova/version.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 02:54:15.369998 sensenova-1.0.2/sensenova.egg-info/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2392 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1725 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       65 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/entry_points.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       86 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-13 02:54:15.000000 sensenova-1.0.2/sensenova.egg-info/top_level.txt
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      631 2023-07-13 02:54:15.465998 sensenova-1.0.2/setup.cfg
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.2/setup.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.3/LICENSE
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2337 2023-07-13 11:41:59.000000 sensenova-1.0.3/PKG-INFO
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2124 2023-07-11 10:58:41.000000 sensenova-1.0.3/README.md
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.3/pyproject.toml
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/_sensenova_scripts.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_requestor.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/api_resources/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/__init__.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/api_resources/abstract/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      790 2023-07-13 11:27:47.000000 sensenova-1.0.3/sensenova/api_resources/abstract/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/createable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/deletable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/downloadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      948 2023-07-13 11:26:18.000000 sensenova-1.0.3/sensenova/api_resources/abstract/file_deletable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/fileable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/listable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/uploadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/dataset.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/error_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/fine_tune.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      559 2023-07-13 11:28:14.000000 sensenova-1.0.3/sensenova/api_resources/knowledge_base.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/model.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/serving.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    17347 2023-07-13 11:34:42.000000 sensenova-1.0.3/sensenova/cli.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/error.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/object_classes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/sensenova_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/sensenova_response.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/tests/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/tests/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-07-12 10:50:35.000000 sensenova-1.0.3/sensenova/tests/test_chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4043 2023-07-13 03:17:07.000000 sensenova-1.0.3/sensenova/tests/test_datasets.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1171 2023-07-13 04:20:15.000000 sensenova-1.0.3/sensenova/tests/test_fine_tunes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/tests/test_finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2191 2023-07-13 11:37:26.000000 sensenova-1.0.3/sensenova/tests/test_knowlege_bases.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      339 2023-07-13 04:39:51.000000 sensenova-1.0.3/sensenova/tests/test_models.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/tests/test_prepare_data.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      976 2023-07-13 04:25:50.000000 sensenova-1.0.3/sensenova/tests/test_servings.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/upload_progress.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-07-11 10:58:24.000000 sensenova-1.0.3/sensenova/util.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-07-13 02:46:13.000000 sensenova-1.0.3/sensenova/validators.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-13 11:38:41.000000 sensenova-1.0.3/sensenova/version.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova.egg-info/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2337 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1789 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       64 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/entry_points.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       86 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/top_level.txt
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      631 2023-07-13 11:41:59.000000 sensenova-1.0.3/setup.cfg
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sensenova-1.0.2/LICENSE` & `sensenova-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/PKG-INFO` & `sensenova-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python client library for the Sensenova API
-Home-page: UNKNOWN
 Author: Sensetime
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sensenova Python Library
 
 The Sensenova Python library provides convenient access to the Sensenova API from applications written in the Python
@@ -112,8 +109,7 @@
 ```sh
 sensenova tools fine_tunes.prepare_data -f data.json
 ```
 
 ## Requirements
 
 - Python 3.7.1+
-
```

### Comparing `sensenova-1.0.2/README.md` & `sensenova-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/__init__.py` & `sensenova-1.0.3/sensenova/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/_sensenova_scripts.py` & `sensenova-1.0.3/sensenova/_sensenova_scripts.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_requestor.py` & `sensenova-1.0.3/sensenova/api_requestor.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/__init__.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from sensenova.api_resources.abstract.api_resource import APIResource
 from sensenova.api_resources.abstract.listable_api_resource import ListableAPIResource
 from sensenova.api_resources.abstract.createable_api_resource import CreatableAPIResource
 from sensenova.api_resources.abstract.deletable_api_resource import DeletableAPIResource
 from sensenova.api_resources.abstract.engine_api_resource import EngineAPIResource
 from sensenova.api_resources.abstract.fileable_api_resource import FileableAPIResource
 from sensenova.api_resources.abstract.downloadable_api_resource import DownloadableAPIResource
-from sensenova.api_resources.abstract.uploadable_api_resource import UploadableAPIResource
+from sensenova.api_resources.abstract.uploadable_api_resource import UploadableAPIResource
+from sensenova.api_resources.abstract.file_deletable_api_resource import FileDeletableAPIResource
```

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/createable_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/deletable_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/downloadable_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/downloadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/engine_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/fileable_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/fileable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/listable_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/abstract/uploadable_api_resource.py` & `sensenova-1.0.3/sensenova/api_resources/abstract/uploadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/chat_completion.py` & `sensenova-1.0.3/sensenova/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/error_object.py` & `sensenova-1.0.3/sensenova/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/fine_tune.py` & `sensenova-1.0.3/sensenova/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/finetune_completion.py` & `sensenova-1.0.3/sensenova/api_resources/finetune_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/api_resources/serving.py` & `sensenova-1.0.3/sensenova/api_resources/serving.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/cli.py` & `sensenova-1.0.3/sensenova/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,19 @@
         print(resp)
 
     @classmethod
     def download(cls, args):
         resp = sensenova.KnowledgeBase.download(id=args.id, file_id=args.file_id)
         print(resp.decode("utf-8"))
 
+    @classmethod
+    def delete_file(cls, args):
+        resp = sensenova.KnowledgeBase.delete_file(args.id, args.file_id)
+        print(resp)
+
 
 class Dataset:
     @classmethod
     def create(cls, args):
         resp = sensenova.Dataset.create(
             description=args.description
         )
@@ -346,14 +351,19 @@
     sub = subparsers.add_parser("knowledge-bases.list")
     sub.set_defaults(func=KnowledgeBase.list)
 
     sub = subparsers.add_parser("knowledge-bases.download")
     sub.add_argument("-i", "--id", required=True, help="The knowledge bases ID")
     sub.add_argument("-f", "--file_id", required=True, help="The knowledge bases file ID")
     sub.set_defaults(func=KnowledgeBase.download)
+
+    sub = subparsers.add_parser("knowledge-bases.delete_file")
+    sub.add_argument("-i", "--id", required=True, help="The knowledge bases ID")
+    sub.add_argument("-f", "--file_id", required=True, help="The knowledge bases file ID")
+    sub.set_defaults(func=KnowledgeBase.delete_file)
     # datasets
     sub = subparsers.add_parser("datasets.create")
 
     sub.add_argument(
         "-d",
         "--description",
         required=False,
```

### Comparing `sensenova-1.0.2/sensenova/error.py` & `sensenova-1.0.3/sensenova/error.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/sensenova_object.py` & `sensenova-1.0.3/sensenova/sensenova_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/tests/test_chat_completion.py` & `sensenova-1.0.3/sensenova/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/tests/test_datasets.py` & `sensenova-1.0.3/sensenova/tests/test_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     return result["dataset"]["id"]
 
 
 # test_dataset_list()
 if __name__ == "__main__":
     id = "e2f9075e-ed8d-4b79-87cd-072e974963fd"
     file_id = "f22c2cd5-248d-4700-af46-a556210de46d"
-    # test_dataset_list()
+    test_dataset_list()
     # test_dataset_delete(id="1502c678-1341-4f5a-a073-f78b5018e0b3")
     # test_dataset_delete(id="12d1ba23-427c-42ad-af1a-d0b927b8e3b7")
     # test_dataset_download(id=id)
     # id = test_dataset_create()
     # url = test_dataset_add_file(id=id, description="How are YOU!")
     # print(url)
     # test_dataset_upload(url)
     # url = 'https://aoss.cn-sh-01.sensecoreapi-oss.cn/nova-test-training-data/ca249841-727f-4917-a747-a58ca3000cfc?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=35C99457BF6D484C812AE6C7FCC2C459%2F20230629%2Fcn-north-1%2Fs3%2Faws4_request&X-Amz-Date=20230629T060440Z&X-Amz-Expires=600&X-Amz-SignedHeaders=host&X-Amz-Signature=ab953d05b7dfacf81ebaad59004c856a7a9d31aaabddf8e473596ae668359c0c'
     # test_dataset_list()
-    # test_dataset_retrieve(id=id)
-    test_dataset_download(id=id, file_id=file_id)
+    test_dataset_retrieve(id=id)
+    # test_dataset_download(id=id, file_id=file_id)
```

### Comparing `sensenova-1.0.2/sensenova/tests/test_fine_tunes.py` & `sensenova-1.0.3/sensenova/tests/test_fine_tunes.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 
 import sensenova
 
 
 def test_finetune_create():
     result = sensenova.FineTune.create(
         hyperparams= {
-            "learning_rate": 0.0001,
-            "lora_alpha": 32,
-            "lora_dropout": 0.05,
-            "lora_rank": 8,
-            "lr_scheduler_type": "cosine",
             "max_steps": 10,
-            "modules_to_save": "embed_tokens,lm_head",
-            "save_steps": 10,
+            "method": "lora",
+            "lr_scheduler_type": "cosine",
+            "learning_rate": 0.0001,
             "warmup_ratio": 0.03,
-            "weight_decay": 0
+            "weight_decay": 0,
+            "save_steps": 10,
+            "modules_to_save": "word_embeddings",
+            "lora_rank": 8,
+            "lora_dropout": 0.05,
+            "lora_alpha": 32
         },
         model="nova-ptc-xs-v1",
-        suffix="wz",
-        training_file="12d1ba23-427c-42ad-af1a-d0b927b8e3b7"
+        suffix="wand",
+        training_file="e2f9075e-ed8d-4b79-87cd-072e974963fd"
     )
     print(result)
 
 
 def test_finetune_list():
     resp = sensenova.FineTune.list()
     print(resp)
 
 def test_finetune_cancel(id):
     resp = sensenova.FineTune.cancel(id)
     print(resp)
 
 
 if __name__ == "__main__":
-    id = 'ft-a3afd31f335447ac8157d8471789a11c'
+    id = 'ft-62e72ad8e1624bdc812cbfc71940505d'
     # test_finetune_list()
     # test_finetune_create()
-    test_finetune_list()
-    # res = sensenova.FineTune.retrieve(id=id)
-    # print(res)
+    # test_finetune_list()
+    print(sensenova.FineTune.retrieve(id=id))
     # test_finetune_cancel(id=id)
-    print(sensenova.FineTune.delete(sid=id))
+    # print(sensenova.FineTune.delete(sid=id))
     # test_finetune_list()
```

### Comparing `sensenova-1.0.2/sensenova/tests/test_knowlege_bases.py` & `sensenova-1.0.3/sensenova/tests/test_knowlege_bases.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,19 +57,21 @@
 def test_knowledge_base_create(description="Test client"):
     result = sensenova.KnowledgeBase.create(description=description)
     print(result)
 
 
 # test_knowledge_base_list()
 if __name__ == "__main__":
-    id = "sf88e224517394ba0aceb9917efefd123"
-    file_id = "9cb27fb844d04ef9b16806843f63ca15"
-    test_knowledge_base_list()
+    id = "s53df1f33ff8f4cad957dcf6d24365937"
+    file_id = "4d97311f90ad4c68a49924979b0a34d8"
+    # test_knowledge_base_list()
     # test_knowledge_base_delete(id=id)
     # test_knowledge_base_download(id=id)
     # test_knowledge_base_create()
     # url = test_knowledge_base_add_file(id=id, description="How are YOU!")
     # test_knowledge_base_upload(url)
     # test_knowledge_base_retrieve(id=id)
     # test_knowledge_base_delete(id=id)
     # test_knowledge_base_list()
-    test_knowledge_base_download(id=id, file_id=file_id)
+    # test_knowledge_base_download(id=id, file_id=file_id)
+    # print(sensenova.KnowledgeBase.delete(id))
+    # print(sensenova.KnowledgeBase.delete_file(sid=id, file_id=file_id))
```

### Comparing `sensenova-1.0.2/sensenova/tests/test_prepare_data.py` & `sensenova-1.0.3/sensenova/tests/test_prepare_data.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/tests/test_servings.py` & `sensenova-1.0.3/sensenova/tests/test_servings.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 
 def test_serving_relaunch(id):
     resp = sensenova.Serving.relaunch(id)
     print(resp)
 
 
 if __name__ == "__main__":
-    id = "a0f0caee-1cfb-4a5c-b2ef-d041d80476cb"
-    model_id = "llama-7b-test:wzh"
+    id = "26f8d926-0579-40e8-a934-5ec99a84ab7e"
+    model_id = "llama-7b-test:wzh2"
     # test_finetune_list()
     # test_serving_list()
     # test_serving_list()
 
     # test_serving_create(model_id)
-    test_serving_cancel(id)
+    # test_serving_cancel(id)
     # print(sensenova.Serving.delete(sid=id))
-    test_serving_relaunch(id)
-    # test_serving_retrieve(id)
+    # test_serving_relaunch(id)
+    test_serving_retrieve(id)
     # test_serving_cancel()
     # test_serving_list()
```

### Comparing `sensenova-1.0.2/sensenova/upload_progress.py` & `sensenova-1.0.3/sensenova/upload_progress.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/util.py` & `sensenova-1.0.3/sensenova/util.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova/validators.py` & `sensenova-1.0.3/sensenova/validators.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.2/sensenova.egg-info/PKG-INFO` & `sensenova-1.0.3/sensenova.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python client library for the Sensenova API
-Home-page: UNKNOWN
 Author: Sensetime
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sensenova Python Library
 
 The Sensenova Python library provides convenient access to the Sensenova API from applications written in the Python
@@ -112,8 +109,7 @@
 ```sh
 sensenova tools fine_tunes.prepare_data -f data.json
 ```
 
 ## Requirements
 
 - Python 3.7.1+
-
```

### Comparing `sensenova-1.0.2/sensenova.egg-info/SOURCES.txt` & `sensenova-1.0.3/sensenova.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 sensenova/api_resources/serving.py
 sensenova/api_resources/abstract/__init__.py
 sensenova/api_resources/abstract/api_resource.py
 sensenova/api_resources/abstract/createable_api_resource.py
 sensenova/api_resources/abstract/deletable_api_resource.py
 sensenova/api_resources/abstract/downloadable_api_resource.py
 sensenova/api_resources/abstract/engine_api_resource.py
+sensenova/api_resources/abstract/file_deletable_api_resource.py
 sensenova/api_resources/abstract/fileable_api_resource.py
 sensenova/api_resources/abstract/listable_api_resource.py
 sensenova/api_resources/abstract/uploadable_api_resource.py
 sensenova/tests/__init__.py
 sensenova/tests/test_chat_completion.py
 sensenova/tests/test_datasets.py
 sensenova/tests/test_fine_tunes.py
```

### Comparing `sensenova-1.0.2/setup.cfg` & `sensenova-1.0.3/setup.cfg`

 * *Files identical despite different names*

