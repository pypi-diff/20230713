# Comparing `tmp/horde_sdk-0.1.3.tar.gz` & `tmp/horde_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horde_sdk-0.1.3.tar", last modified: Thu Jul  6 22:46:35 2023, max compression
+gzip compressed data, was "horde_sdk-0.4.0.tar", last modified: Thu Jul 13 15:19:36 2023, max compression
```

## Comparing `horde_sdk-0.1.3.tar` & `horde_sdk-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,173 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.413223 horde_sdk-0.1.3/
--rw-rw-rw-   0        0        0    35164 2023-03-31 20:26:08.000000 horde_sdk-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      139 2023-07-06 22:38:14.000000 horde_sdk-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    41647 2023-07-06 22:46:35.412220 horde_sdk-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-07-06 22:45:49.000000 horde_sdk-0.1.3/README.md
--rw-rw-rw-   0        0        0     1593 2023-07-06 22:46:26.000000 horde_sdk-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 22:46:35.413223 horde_sdk-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       55 2023-07-04 14:28:55.000000 horde_sdk-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.317085 horde_sdk-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.338206 horde_sdk-0.1.3/src/horde_sdk/
--rw-rw-rw-   0        0        0       80 2023-03-31 20:20:58.000000 horde_sdk-0.1.3/src/horde_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.358113 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/
--rw-rw-rw-   0        0        0      986 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/__init__.py
--rw-rw-rw-   0        0        0     2284 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/ai_horde_client.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.363228 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/
--rw-rw-rw-   0        0        0        0 2023-07-03 23:30:55.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/__init__.py
--rw-rw-rw-   0        0        0      429 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/_base.py
--rw-rw-rw-   0        0        0     3090 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/_shared.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.370225 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/
--rw-rw-rw-   0        0        0      634 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
--rw-rw-rw-   0        0        0     2236 2023-07-06 22:27:43.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_async.py
--rw-rw-rw-   0        0        0     2400 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_check.py
--rw-rw-rw-   0        0        0     6423 2023-07-06 22:27:43.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
--rw-rw-rw-   0        0        0     2870 2023-07-06 22:27:43.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_status.py
--rw-rw-rw-   0        0        0     1689 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
--rw-rw-rw-   0        0        0     1109 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/stats.py
--rw-rw-rw-   0        0        0      669 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/consts.py
--rw-rw-rw-   0        0        0     2490 2023-07-06 22:32:55.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/endpoints.py
--rw-rw-rw-   0        0        0     1572 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/fields.py
--rw-rw-rw-   0        0        0      385 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.371224 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/utils/
--rw-rw-rw-   0        0        0     9016 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/utils/swagger.py
--rw-rw-rw-   0        0        0     1005 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.379323 horde_sdk-0.1.3/src/horde_sdk/generic_api/
--rw-rw-rw-   0        0        0      722 2023-07-04 14:29:22.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-07-06 22:27:43.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/_error.py
--rw-rw-rw-   0        0        0      676 2023-07-04 15:25:34.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/_reflection.py
--rw-rw-rw-   0        0        0     3571 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/apimodels.py
--rw-rw-rw-   0        0        0     1237 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/endpoints.py
--rw-rw-rw-   0        0        0    10583 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/generic_client.py
--rw-rw-rw-   0        0        0      799 2023-07-05 21:42:10.000000 horde_sdk-0.1.3/src/horde_sdk/generic_api/metadata.py
--rw-rw-rw-   0        0        0      466 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/models.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.384725 horde_sdk-0.1.3/src/horde_sdk/ratings_api/
--rw-rw-rw-   0        0        0      853 2023-07-04 15:25:51.000000 horde_sdk-0.1.3/src/horde_sdk/ratings_api/__init__.py
--rw-rw-rw-   0        0        0     8599 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ratings_api/apimodels.py
--rw-rw-rw-   0        0        0      573 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/src/horde_sdk/ratings_api/endpoints.py
--rw-rw-rw-   0        0        0      886 2023-07-04 14:29:22.000000 horde_sdk-0.1.3/src/horde_sdk/ratings_api/metadata.py
--rw-rw-rw-   0        0        0      561 2023-07-04 14:29:22.000000 horde_sdk-0.1.3/src/horde_sdk/ratings_api/ratings_client.py
--rw-rw-rw-   0        0        0      433 2023-07-03 23:40:43.000000 horde_sdk-0.1.3/src/horde_sdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.351108 horde_sdk-0.1.3/src/horde_sdk.egg-info/
--rw-rw-rw-   0        0        0    41647 2023-07-06 22:46:35.000000 horde_sdk-0.1.3/src/horde_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2794 2023-07-06 22:46:35.000000 horde_sdk-0.1.3/src/horde_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 22:46:35.000000 horde_sdk-0.1.3/src/horde_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-06 22:46:35.000000 horde_sdk-0.1.3/src/horde_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 22:46:35.000000 horde_sdk-0.1.3/src/horde_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.391228 horde_sdk-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-07-06 22:20:28.000000 horde_sdk-0.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.397543 horde_sdk-0.1.3/tests/ai_horde_api/
--rw-rw-rw-   0        0        0        0 2023-07-06 22:18:04.000000 horde_sdk-0.1.3/tests/ai_horde_api/__init__.py
--rw-rw-rw-   0        0        0     3885 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/ai_horde_api/test_ai_horde_api_models.py
--rw-rw-rw-   0        0        0     1860 2023-07-06 21:50:09.000000 horde_sdk-0.1.3/tests/ai_horde_api/test_api_calls.py
--rw-rw-rw-   0        0        0     2824 2023-07-06 21:50:09.000000 horde_sdk-0.1.3/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
--rw-rw-rw-   0        0        0      819 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/ai_horde_api/test_swagger.py
--rw-rw-rw-   0        0        0      708 2023-07-06 21:50:09.000000 horde_sdk-0.1.3/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.399542 horde_sdk-0.1.3/tests/test_data/
--rw-rw-rw-   0        0        0       93 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/RequestErrorResponse.json
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.322121 horde_sdk-0.1.3/tests/test_data/ai_horde_api/
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.405050 horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/
--rw-rw-rw-   0        0        0       69 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/ImageGenerateAsyncResponse.json
--rw-rw-rw-   0        0        0      219 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/ImageGenerateCheckResponse.json
--rw-rw-rw-   0        0        0     1531 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/ImageGenerateJobResponse.json
--rw-rw-rw-   0        0        0      510 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/ImageGenerateStatusResponse.json
--rw-rw-rw-   0        0        0    18362 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/StatsModelsResponse.json
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.406050 horde_sdk-0.1.3/tests/test_data/ai_horde_api/production_responses/
--rw-rw-rw-   0        0        0    20811 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.323120 horde_sdk-0.1.3/tests/test_data/ratings_api/
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:35.410049 horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/
--rw-rw-rw-   0        0        0      666 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
--rw-rw-rw-   0        0        0      251 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
--rw-rw-rw-   0        0        0    64737 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
--rw-rw-rw-   0        0        0     5726 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
--rw-rw-rw-   0        0        0   237970 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_data/swagger.json
--rw-rw-rw-   0        0        0     3396 2023-07-06 22:28:39.000000 horde_sdk-0.1.3/tests/test_dynamically_check_apimodels.py
--rw-rw-rw-   0        0        0      302 2023-07-05 21:06:36.000000 horde_sdk-0.1.3/tests/test_generic.py
--rw-rw-rw-   0        0        0     1697 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_ratings_api_models.py
--rw-rw-rw-   0        0        0      466 2023-07-06 20:14:23.000000 horde_sdk-0.1.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.202657 horde_sdk-0.4.0/
+-rw-rw-rw-   0        0        0     1183 2023-07-13 13:14:15.000000 horde_sdk-0.4.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35164 2023-03-31 20:26:08.000000 horde_sdk-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      142 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    41971 2023-07-13 15:19:36.202657 horde_sdk-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.025282 horde_sdk-0.4.0/horde_sdk/
+-rw-rw-rw-   0        0        0      498 2023-07-13 13:45:39.000000 horde_sdk-0.4.0/horde_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.054321 horde_sdk-0.4.0/horde_sdk/ai_horde_api/
+-rw-rw-rw-   0        0        0      585 2023-07-13 13:24:07.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/__init__.py
+-rw-rw-rw-   0        0        0    14843 2023-07-13 13:58:46.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/ai_horde_clients.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.057824 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/
+-rw-rw-rw-   0        0        0     1475 2023-07-13 15:11:45.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/__init__.py
+-rw-rw-rw-   0        0        0     1298 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/_stats.py
+-rw-rw-rw-   0        0        0     3315 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/base.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.065320 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_async.py
+-rw-rw-rw-   0        0        0     2329 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_check.py
+-rw-rw-rw-   0        0        0     6483 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
+-rw-rw-rw-   0        0        0     3312 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_status.py
+-rw-rw-rw-   0        0        0     1806 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.067322 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/workers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/workers/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py
+-rw-rw-rw-   0        0        0      979 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/consts.py
+-rw-rw-rw-   0        0        0     2785 2023-07-13 13:14:15.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/endpoints.py
+-rw-rw-rw-   0        0        0     1818 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/fields.py
+-rw-rw-rw-   0        0        0      381 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_api/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.007272 horde_sdk-0.4.0/horde_sdk/ai_horde_worker/
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.068322 horde_sdk-0.4.0/horde_sdk/ai_horde_worker/locale_info/
+-rw-rw-rw-   0        0        0      190 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/ai_horde_worker/locale_info/README.md
+-rw-rw-rw-   0        0        0     2074 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.076453 horde_sdk-0.4.0/horde_sdk/generic_api/
+-rw-rw-rw-   0        0        0       60 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/generic_api/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/generic_api/_reflection.py
+-rw-rw-rw-   0        0        0    10422 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/generic_api/apimodels.py
+-rw-rw-rw-   0        0        0     1237 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/generic_api/endpoints.py
+-rw-rw-rw-   0        0        0    31143 2023-07-13 03:31:29.000000 horde_sdk-0.4.0/horde_sdk/generic_api/generic_clients.py
+-rw-rw-rw-   0        0        0      826 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/generic_api/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.078459 horde_sdk-0.4.0/horde_sdk/generic_api/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:41:36.000000 horde_sdk-0.4.0/horde_sdk/generic_api/utils/__init__.py
+-rw-rw-rw-   0        0        0    29120 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/generic_api/utils/swagger.py
+-rw-rw-rw-   0        0        0      125 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/localize.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.084460 horde_sdk-0.4.0/horde_sdk/ratings_api/
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/ratings_api/__init__.py
+-rw-rw-rw-   0        0        0     8420 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/ratings_api/apimodels.py
+-rw-rw-rw-   0        0        0      573 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/ratings_api/endpoints.py
+-rw-rw-rw-   0        0        0      895 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/ratings_api/metadata.py
+-rw-rw-rw-   0        0        0      589 2023-07-13 13:25:13.000000 horde_sdk-0.4.0/horde_sdk/ratings_api/ratings_client.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.087460 horde_sdk-0.4.0/horde_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/scripts/write_all_payload_examples.py
+-rw-rw-rw-   0        0        0      653 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/scripts/write_all_response_examples.py
+-rw-rw-rw-   0        0        0      431 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/horde_sdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.047325 horde_sdk-0.4.0/horde_sdk.egg-info/
+-rw-rw-rw-   0        0        0    41971 2023-07-13 15:19:35.000000 horde_sdk-0.4.0/horde_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8842 2023-07-13 15:19:35.000000 horde_sdk-0.4.0/horde_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:19:35.000000 horde_sdk-0.4.0/horde_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-13 15:19:35.000000 horde_sdk-0.4.0/horde_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 15:19:35.000000 horde_sdk-0.4.0/horde_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1718 2023-07-13 15:19:21.000000 horde_sdk-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 15:19:36.203659 horde_sdk-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.094458 horde_sdk-0.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.099784 horde_sdk-0.4.0/tests/ai_horde_api/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/ai_horde_api/__init__.py
+-rw-rw-rw-   0        0        0     6790 2023-07-13 13:24:07.000000 horde_sdk-0.4.0/tests/ai_horde_api/test_ai_horde_api_calls.py
+-rw-rw-rw-   0        0        0     3901 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/ai_horde_api/test_ai_horde_api_models.py
+-rw-rw-rw-   0        0        0     4830 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
+-rw-rw-rw-   0        0        0     1623 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/ai_horde_api/test_swagger.py
+-rw-rw-rw-   0        0        0     1069 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.100784 horde_sdk-0.4.0/tests/ratings_api/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/ratings_api/test_init.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.101785 horde_sdk-0.4.0/tests/test_data/
+-rw-rw-rw-   0        0        0       93 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/RequestErrorResponse.json
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.102784 horde_sdk-0.4.0/tests/test_data/ai_horde_api/
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.130523 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/
+-rw-rw-rw-   0        0        0       99 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_filters_filter_id_patch.json
+-rw-rw-rw-   0        0        0       47 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_filters_post.json
+-rw-rw-rw-   0        0        0       99 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_filters_put.json
+-rw-rw-rw-   0        0        0     1298 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json
+-rw-rw-rw-   0        0        0      488 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json
+-rw-rw-rw-   0        0        0      221 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_rate_id_post.json
+-rw-rw-rw-   0        0        0      141 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json
+-rw-rw-rw-   0        0        0      719 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json
+-rw-rw-rw-   0        0        0      337 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_pop_post.json
+-rw-rw-rw-   0        0        0      101 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_submit_post.json
+-rw-rw-rw-   0        0        0      295 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_async_post.json
+-rw-rw-rw-   0        0        0      238 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_pop_post.json
+-rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_submit_post.json
+-rw-rw-rw-   0        0        0       44 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_award_post.json
+-rw-rw-rw-   0        0        0       70 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_kai_user_id_post.json
+-rw-rw-rw-   0        0        0       44 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_transfer_post.json
+-rw-rw-rw-   0        0        0      156 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_put.json
+-rw-rw-rw-   0        0        0      156 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_sharedkey_id_patch.json
+-rw-rw-rw-   0        0        0       79 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_status_modes_put.json
+-rw-rw-rw-   0        0        0       68 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_teams_post.json
+-rw-rw-rw-   0        0        0       68 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_teams_team_id_patch.json
+-rw-rw-rw-   0        0        0      391 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_users_user_id_put.json
+-rw-rw-rw-   0        0        0      176 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.132524 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_production_responses/
+-rw-rw-rw-   0        0        0   123568 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.194655 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/
+-rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_delete_200.json
+-rw-rw-rw-   0        0        0      169 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_get_200.json
+-rw-rw-rw-   0        0        0      131 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_patch_200.json
+-rw-rw-rw-   0        0        0      169 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_get_200.json
+-rw-rw-rw-   0        0        0       46 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_post_200.json
+-rw-rw-rw-   0        0        0      131 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_put_201.json
+-rw-rw-rw-   0        0        0       69 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_regex_get_200.json
+-rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json
+-rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_202.json
+-rw-rw-rw-   0        0        0      222 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_check_id_get_200.json
+-rw-rw-rw-   0        0        0     1536 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_rate_id_post_200.json
+-rw-rw-rw-   0        0        0      515 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json
+-rw-rw-rw-   0        0        0      515 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_submit_post_200.json
+-rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_async_post_202.json
+-rw-rw-rw-   0        0        0      929 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json
+-rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json
+-rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_submit_post_200.json
+-rw-rw-rw-   0        0        0       40 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_async_post_202.json
+-rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_pop_post_200.json
+-rw-rw-rw-   0        0        0      279 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_delete_200.json
+-rw-rw-rw-   0        0        0      279 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_get_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_submit_post_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_kudos_award_post_200.json
+-rw-rw-rw-   0        0        0       30 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_kudos_transfer_post_200.json
+-rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_delete_200.json
+-rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_put_200.json
+-rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_delete_200.json
+-rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_get_200.json
+-rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_patch_200.json
+-rw-rw-rw-   0        0        0      351 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_models_get_200.json
+-rw-rw-rw-   0        0        0      348 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_totals_get_200.json
+-rw-rw-rw-   0        0        0      351 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_models_get_200.json
+-rw-rw-rw-   0        0        0      348 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_totals_get_200.json
+-rw-rw-rw-   0        0        0      181 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_status_models_get_200.json
+-rw-rw-rw-   0        0        0      139 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_status_models_model_name_get_200.json
+-rw-rw-rw-   0        0        0       94 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_get_200.json
+-rw-rw-rw-   0        0        0       94 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_put_200.json
+-rw-rw-rw-   0        0        0      114 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_status_news_get_200.json
+-rw-rw-rw-   0        0        0      397 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_status_performance_get_200.json
+-rw-rw-rw-   0        0        0      550 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json
+-rw-rw-rw-   0        0        0       54 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_post_200.json
+-rw-rw-rw-   0        0        0       53 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_delete_200.json
+-rw-rw-rw-   0        0        0      448 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_get_200.json
+-rw-rw-rw-   0        0        0       54 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_patch_200.json
+-rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json
+-rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json
+-rw-rw-rw-   0        0        0      395 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_put_200.json
+-rw-rw-rw-   0        0        0     1147 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json
+-rw-rw-rw-   0        0        0       53 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_delete_200.json
+-rw-rw-rw-   0        0        0      977 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json
+-rw-rw-rw-   0        0        0      118 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_put_200.json
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.196655 horde_sdk-0.4.0/tests/test_data/ai_horde_api/production_responses/
+-rw-rw-rw-   0        0        0    20811 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json
+-rw-rw-rw-   0        0        0        4 2023-07-13 02:41:16.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json
+-rw-rw-rw-   0        0        0   237970 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ai_horde_api/swagger.json
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.014278 horde_sdk-0.4.0/tests/test_data/ratings_api/
+drwxrwxrwx   0        0        0        0 2023-07-13 15:19:36.200659 horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/
+-rw-rw-rw-   0        0        0      666 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
+-rw-rw-rw-   0        0        0      251 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
+-rw-rw-rw-   0        0        0    64737 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
+-rw-rw-rw-   0        0        0     5726 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
+-rw-rw-rw-   0        0        0     5982 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/tests/test_dynamically_check_apimodels.py
+-rw-rw-rw-   0        0        0      320 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1650 2023-07-13 02:41:37.000000 horde_sdk-0.4.0/tests/test_ratings_api_models.py
+-rw-rw-rw-   0        0        0      474 2023-07-12 15:33:50.000000 horde_sdk-0.4.0/tests/test_utils.py
```

### Comparing `horde_sdk-0.1.3/LICENSE` & `horde_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/PKG-INFO` & `horde_sdk-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde_sdk
-Version: 0.1.3
+Version: 0.4.0
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -670,16 +670,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+[![Tests](https://github.com/Haidra-Org/horde-sdk/actions/workflows/maintests.yml/badge.svg)](https://github.com/Haidra-Org/horde-sdk/actions/workflows/maintests.yml)
+[![Documentation Status](https://readthedocs.org/projects/horde-sdk/badge/?version=latest)](https://horde-sdk.readthedocs.io/en/latest/?badge=latest)
+[![Unstable Tests](https://github.com/Haidra-Org/horde-sdk/actions/workflows/prtests.yml/badge.svg)](https://github.com/Haidra-Org/horde-sdk/actions/workflows/prtests.yml)
 # horde_sdk
 
 With the power of pydantic, you can simplify interfacing with the [AI-Horde's suite of APIs](https://github.com/db0/AI-Horde). Whether you want to request your own images, or roll your own worker software, this package may suit your needs for anything horde related.
 
-## AI-Horde
-`TODO`
-
-## Ratings API
-There is currently some support for the [Image Ratings](https://dbzer0.com/blog/the-image-ratings-are-flooding-in/) API that are rating images from the [DiffusionDB](https://poloclub.github.io/diffusiondb/) dataset. See `example.py` for an idea of how to start.
+## Documentation
+For detailed documentation, see our [read the docs page](https://horde-sdk.readthedocs.io/en/latest/index.html).
```

### Comparing `horde_sdk-0.1.3/pyproject.toml` & `horde_sdk-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "horde_sdk"
-version = "0.1.3"
+version = "0.4.0"
 description = "A python toolkit for interacting with the horde APIs, services, and ecosystem."
 authors = [
     {name = "tazlin", email = "tazlin.on.github@gmail.com"},
     {name = "db0", email = "mail@dbzer0.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "pydantic",
     "requests",
     "StrEnum",
     "loguru",
+    "babel",
+    "aiohttp",
+    "aiodns",
+    "pillow",
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Development Status :: 2 - Pre-Alpha",
 ]
 
+[tool.setuptools.package-dir]
+horde_sdk = "horde_sdk"
+
 [project.urls]
 "Homepage" = "https://github.com/Haidra-Org/horde-sdk"
 
 [tool.setuptools.package-data]
 tests = ["*.json"]
 
 [tool.ruff]
 line-length = 119
-select = ["A", "I", "E", "W", "F", "UP", "YTT", "B", "C4", "PIE", "RET", "SIM"] #, "D", "ANN"] # FIXME
+select = ["A", "I", "E", "W", "F", "UP", "YTT", "B", "C4", "PIE", "RET", "SIM", "COM"] #, "D", "ANN"] # FIXME
 ignore = [
   # Ignore D rules for non-google docstring standard
   "D203",
   "D204",
   "D213",
   "D215",
   "D400",
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/__init__.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,37 @@
-from horde_sdk.ai_horde_api.apimodels.generate._async import ImageGenerateAsyncRequest, ImageGenerateAsyncResponse
+from horde_sdk.ai_horde_api.apimodels._stats import StatsImageModelsRequest, StatsModelsResponse
+from horde_sdk.ai_horde_api.apimodels.generate._async import (
+    ImageGenerateAsyncRequest,
+    ImageGenerateAsyncResponse,
+)
 from horde_sdk.ai_horde_api.apimodels.generate._check import ImageGenerateCheckRequest, ImageGenerateCheckResponse
 from horde_sdk.ai_horde_api.apimodels.generate._pop import ImageGenerateJobPopRequest, ImageGenerateJobResponse
 from horde_sdk.ai_horde_api.apimodels.generate._status import (
-    CancelImageGenerateRequest,
+    DeleteImageGenerateRequest,
     ImageGenerateStatusRequest,
     ImageGenerateStatusResponse,
+    ImageGeneration,
+)
+from horde_sdk.ai_horde_api.apimodels.generate._submit import (
+    ImageGenerationJobSubmitRequest,
+    ImageGenerationJobSubmitResponse,
 )
-from horde_sdk.ai_horde_api.apimodels.stats import StatsImageModels, StatsModelsResponse
+from horde_sdk.ai_horde_api.apimodels.workers._workers_all import AllWorkersDetailsRequest, AllWorkersDetailsResponse
 
 __all__ = [
     "ImageGenerateAsyncRequest",
     "ImageGenerateAsyncResponse",
     "ImageGenerateCheckRequest",
     "ImageGenerateCheckResponse",
     "ImageGenerateJobPopRequest",
     "ImageGenerateJobResponse",
     "ImageGenerateStatusRequest",
     "ImageGenerateStatusResponse",
-    "CancelImageGenerateRequest",
-    "StatsImageModels",
+    "DeleteImageGenerateRequest",
+    "StatsImageModelsRequest",
     "StatsModelsResponse",
+    "ImageGenerationJobSubmitRequest",
+    "ImageGenerationJobSubmitResponse",
+    "AllWorkersDetailsRequest",
+    "AllWorkersDetailsResponse",
+    "ImageGeneration",
 ]
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/_shared.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-import pydantic
-from pydantic import Field, field_validator
+from pydantic import BaseModel, Field, field_validator
 from typing_extensions import override
 
-from horde_sdk.ai_horde_api.consts import KNOWN_SAMPLERS, KNOWN_SOURCE_PROCESSING
+from horde_sdk.ai_horde_api.consts import KNOWN_SAMPLERS
 from horde_sdk.ai_horde_api.endpoints import AI_HORDE_BASE_URL
-from horde_sdk.generic_api.apimodels import BaseRequest, BaseRequestWorkerDriven
+from horde_sdk.ai_horde_api.fields import GenerationID, WorkerID
+from horde_sdk.generic_api.apimodels import BaseRequest
 from horde_sdk.utils import seed_to_int
 
 
 class BaseAIHordeRequest(BaseRequest):
+    """Base class for all AI Horde API requests."""
+
     @override
     @classmethod
     def get_api_url(cls) -> str:
         return AI_HORDE_BASE_URL
 
 
-class LorasPayloadEntry(pydantic.BaseModel):
+class BaseImageJobRequest(BaseModel):
+    """Base class for data relating to image generation jobs."""
+
+    id_: str | GenerationID = Field(alias="id")
+    """The UUID for this job."""
+
+
+class BaseWorkerRequest(BaseModel):
+    """Base class for data relating to worker requests."""
+
+    worker_id: str | WorkerID
+    """The UUID of the worker in question for this request."""
+
+
+class LorasPayloadEntry(BaseModel):
     """Represents a single lora parameter.
 
     v2 API Model: `ModelPayloadLorasStable`
     """
 
     name: str = Field(min_length=1, max_length=255)
     """The name of the LoRa model to use."""
@@ -27,15 +43,15 @@
     """The strength of the LoRa against the stable diffusion model."""
     clip: float = Field(default=1, ge=0, le=5)
     """The strength of the LoRa against the clip model."""
     inject_trigger: str | None = Field(default=None, min_length=1, max_length=30)
     """Any trigger required to activate the LoRa model."""
 
 
-class BaseImageGenerateParam(pydantic.BaseModel):
+class BaseImageGenerateParam(BaseModel):
     """Represents some of the data included in a request to the `/v2/generate/async` endpoint.
 
     Also is the corresponding information returned on a job pop to the `/v2/generate/pop` endpoint.
     v2 API Model: `ModelPayloadStable`
     """
 
     sampler_name: KNOWN_SAMPLERS = KNOWN_SAMPLERS.k_lms
@@ -58,25 +74,17 @@
     special: dict = Field(default_factory=dict)
     steps: int = Field(default=25, ge=1)
 
     n_iter: int = Field(default=1, ge=1)
     use_nsfw_censor: bool = False
 
     @field_validator("sampler_name")
-    def sampler_name_must_be_known(cls, v):
+    def sampler_name_must_be_known(cls, v: str | KNOWN_SAMPLERS) -> str | KNOWN_SAMPLERS:
         """Ensure that the sampler name is in this list of supported samplers."""
         if v not in KNOWN_SAMPLERS.__members__:
             raise ValueError(f"Unknown sampler name {v}")
         return v
 
     @field_validator("seed")
-    def seed_to_int_if_str(cls, v):
+    def seed_to_int_if_str(cls, v: str | int) -> str | int:
         """Ensure that the seed is an integer. If it is a string, convert it to an integer."""
         return str(seed_to_int(v))
-
-
-class ImageGenerateImg2ImgData(BaseRequestWorkerDriven):
-    """Mix-in class for data relating to img2img generation."""
-
-    source_image: str | None = None
-    source_processing: KNOWN_SOURCE_PROCESSING = KNOWN_SOURCE_PROCESSING.txt2img
-    source_mask: str | None = None
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_async.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,101 @@
-from pydantic import Field, model_validator
+from pydantic import BaseModel, Field
 from typing_extensions import override
 
-from horde_sdk.ai_horde_api.apimodels._shared import (
-    BaseAIHordeRequest,
-    BaseImageGenerateParam,
-    ImageGenerateImg2ImgData,
-)
+from horde_sdk.ai_horde_api.apimodels.base import BaseAIHordeRequest, BaseImageJobRequest
+from horde_sdk.ai_horde_api.apimodels.generate._check import ImageGenerateCheckResponse
+from horde_sdk.ai_horde_api.consts import GENERATION_STATE
 from horde_sdk.ai_horde_api.endpoints import AI_HORDE_API_URL_Literals
-from horde_sdk.ai_horde_api.fields import GenerationID
+from horde_sdk.ai_horde_api.fields import ImageID, WorkerID
 from horde_sdk.consts import HTTPMethod
-from horde_sdk.generic_api.apimodels import BaseRequestWorkerDriven, BaseResponse
 
 
-class ImageGenerateAsyncResponse(BaseResponse):
-    """Represents the data returned from the `/v2/generate/async` endpoint."""
+class ImageGeneration(BaseModel):
+    """Represents the individual image generation responses in a ImageGenerateStatusResponse.
 
-    id: str | GenerationID  # noqa: A003
-    """The UUID for this image generation."""
-    kudos: float
-    message: str | None = None
+    v2 API Model: `GenerationStable`
+    """
+
+    id: str | ImageID  # noqa: A003
+    """The UUID of this image. Is always returned as a `ImageID`, but can initialized from a `str`."""
+    worker_id: str | WorkerID
+    """The UUID of the worker which generated this image."""
+    worker_name: str
+    """The name of the worker which generated this image."""
+    model: str
+    """The model which generated this image."""
+    state: GENERATION_STATE
+    """The state of this generation."""
+    img: str
+    """The generated image as a Base64-encoded .webp file."""
+    seed: str
+    """The seed which generated this image."""
+    censored: bool
+    """When true this image has been censored by the worker's safety filter."""
 
-    @override
-    @classmethod
-    def get_api_model_name(cls) -> str | None:
-        return "RequestAsync"
 
+class ImageGenerateStatusResponse(ImageGenerateCheckResponse):
+    """Represent the response from the AI-Horde API when checking the status of an image generation job.
 
-class ImageGenerationInputPayload(BaseImageGenerateParam):
-    n: int = Field(default=1, ge=1)
+    v2 API Model: `RequestStatusStable`
+    """
+
+    generations: list[ImageGeneration] = Field(default_factory=list)
+    """The individual image generation responses in this request."""
+    shared: bool | None = False
+    """If True, These images have been shared with LAION."""
 
+    @override
+    @classmethod
+    def get_api_model_name(cls) -> str | None:
+        return "RequestStatusStable"
 
-class ImageGenerateAsyncRequest(BaseAIHordeRequest, ImageGenerateImg2ImgData, BaseRequestWorkerDriven):
-    """Represents the data needed to make a request to the `/v2/generate/async` endpoint.
 
-    v2 API Model: `GenerationInputStable`
-    """
+class DeleteImageGenerateRequest(
+    BaseAIHordeRequest,
+    BaseImageJobRequest,
+):
+    """Represents a DELETE request to the `/v2/generate/status/{id}` endpoint."""
 
-    prompt: str
-    params: ImageGenerationInputPayload | None = None
+    @override
+    @classmethod
+    def get_api_model_name(cls) -> str | None:
+        return None
 
-    nsfw: bool | None = True
-    censor_nsfw: bool = False
+    @override
+    @classmethod
+    def get_http_method(cls) -> HTTPMethod:
+        return HTTPMethod.DELETE
 
-    r2: bool = True
+    @override
+    @staticmethod
+    def get_endpoint_subpath() -> str:
+        return AI_HORDE_API_URL_Literals.v2_generate_status
 
-    shared: bool = False
+    @override
+    @staticmethod
+    def get_success_response_type() -> type[ImageGenerateStatusResponse]:
+        return ImageGenerateStatusResponse
 
-    replacement_filter: bool = True
 
-    @model_validator(mode="before")
-    def validate_censor_nsfw(cls, values):
-        if values.get("censor_nsfw", None) and values.get("nsfw", None):
-            raise ValueError("censor_nsfw is only valid when nsfw is False")
-        return values
+class ImageGenerateStatusRequest(BaseAIHordeRequest, BaseImageJobRequest):
+    """Represents a GET request to the `/v2/generate/status/{id}` endpoint."""
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
-        return "GenerationInputStable"
+        return None
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
-        return HTTPMethod.POST
+        return HTTPMethod.GET
 
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
-        return AI_HORDE_API_URL_Literals.v2_generate_async
+        return AI_HORDE_API_URL_Literals.v2_generate_status
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[ImageGenerateAsyncResponse]:
-        return ImageGenerateAsyncResponse
+    def get_success_response_type() -> type[ImageGenerateStatusResponse]:
+        return ImageGenerateStatusResponse
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_check.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing_extensions import override
 
-from horde_sdk.ai_horde_api.apimodels._base import BaseImageGenerateJobRequest
-from horde_sdk.ai_horde_api.apimodels._shared import BaseAIHordeRequest
+from horde_sdk.ai_horde_api.apimodels.base import BaseAIHordeRequest, BaseImageJobRequest
 from horde_sdk.ai_horde_api.endpoints import AI_HORDE_API_URL_Literals
 from horde_sdk.consts import HTTPMethod
 from horde_sdk.generic_api.apimodels import BaseResponse
 
 
 class ImageGenerateCheckResponse(BaseResponse):
     """Represents the data returned from the `/v2/generate/check/{id}` endpoint.
@@ -36,15 +35,15 @@
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
         return "RequestStatusCheck"
 
 
-class ImageGenerateCheckRequest(BaseAIHordeRequest, BaseImageGenerateJobRequest):
+class ImageGenerateCheckRequest(BaseAIHordeRequest, BaseImageJobRequest):
     """Represents a GET request to the `/v2/generate/check/{id}` endpoint."""
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
         return None
 
@@ -56,9 +55,9 @@
     @override
     @classmethod
     def get_endpoint_subpath(cls) -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_check
 
     @override
     @classmethod
-    def get_expected_response_type(cls) -> type[ImageGenerateCheckResponse]:
+    def get_success_response_type(cls) -> type[ImageGenerateCheckResponse]:
         return ImageGenerateCheckResponse
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_pop.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_pop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pydantic
 from pydantic import Field, field_validator
 from typing_extensions import override
 
-from horde_sdk.ai_horde_api.apimodels._shared import BaseAIHordeRequest, BaseImageGenerateParam
+from horde_sdk.ai_horde_api.apimodels.base import BaseAIHordeRequest, BaseImageGenerateParam
 from horde_sdk.ai_horde_api.consts import KNOWN_SOURCE_PROCESSING
 from horde_sdk.ai_horde_api.endpoints import AI_HORDE_API_URL_Literals
 from horde_sdk.ai_horde_api.fields import GenerationID
 from horde_sdk.consts import HTTPMethod
 from horde_sdk.generic_api.apimodels import BaseRequestAuthenticated, BaseResponse
 
 
@@ -75,15 +75,15 @@
     """If img_processing is set to 'inpainting' or 'outpainting', this parameter can be optionally provided as the
     mask of the areas to inpaint. If this arg is not passed, the inpainting/outpainting mask has to be embedded as
     alpha channel."""
     r2_upload: str | None = None
     """The r2 upload link to use to upload this image."""
 
     @field_validator("source_processing")
-    def source_processing_must_be_known(cls, v):
+    def source_processing_must_be_known(cls, v: str | KNOWN_SOURCE_PROCESSING) -> str | KNOWN_SOURCE_PROCESSING:
         """Ensure that the source processing is in this list of supported source processing."""
         if v not in KNOWN_SOURCE_PROCESSING.__members__:
             raise ValueError(f"Unknown source processing {v}")
         return v
 
     @override
     @classmethod
@@ -127,15 +127,15 @@
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_pop
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[ImageGenerateJobResponse]:
+    def get_success_response_type() -> type[ImageGenerateJobResponse]:
         return ImageGenerateJobResponse
 
 
 class ImageGenerateJobPopPayload(BaseImageGenerateParam):
     prompt: str
 
     @property
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/apimodels/generate/_submit.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/apimodels/generate/_submit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from typing_extensions import override
 
-from horde_sdk.ai_horde_api.apimodels._shared import BaseAIHordeRequest
+from horde_sdk.ai_horde_api.apimodels.base import BaseAIHordeRequest
 from horde_sdk.ai_horde_api.endpoints import AI_HORDE_API_URL_Literals
 from horde_sdk.ai_horde_api.fields import GenerationID
 from horde_sdk.consts import HTTPMethod
 from horde_sdk.generic_api.apimodels import BaseRequestAuthenticated, BaseResponse
 
 
 class ImageGenerationJobSubmitResponse(BaseResponse):
     reward: float
     """The amount of kudos gained for submitting this request."""
 
+    @override
+    @classmethod
+    def get_api_model_name(cls) -> str | None:
+        return "GenerationSubmitted"
+
 
 class ImageGenerationJobSubmitRequest(BaseAIHordeRequest, BaseRequestAuthenticated):
     """Represents the data needed to make a job submit 'request' from a worker to the /v2/generate/submit endpoint.
 
     v2 API Model: `SubmitInputStable`
     """
 
@@ -42,9 +47,9 @@
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_submit
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[ImageGenerationJobSubmitResponse]:
+    def get_success_response_type() -> type[ImageGenerationJobSubmitResponse]:
         return ImageGenerationJobSubmitResponse
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/endpoints.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/endpoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import os
 
 from strenum import StrEnum
 
+from horde_sdk.generic_api.endpoints import url_with_path
+
+# TODO: Defer setting this?
 AI_HORDE_BASE_URL = "https://aihorde.net/api/"
 
-if os.environ.get("HORDE_URL", None):
-    AI_HORDE_BASE_URL = os.environ["HORDE_URL"]
+if os.environ.get("AI_HORDE_URL", None):
+    AI_HORDE_BASE_URL = os.environ["AI_HORDE_URL"]
 
-if os.environ.get("HORDE_URL_DEBUG", None):
-    AI_HORDE_BASE_URL = os.environ["HORDE_URL_DEBUG"]
+if os.environ.get("AI_HORDE_DEV_URL", None):
+    AI_HORDE_BASE_URL = os.environ["AI_HORDE_DEV_URL"]
 
 
 class AI_HORDE_API_URL_Literals(StrEnum):
     """The URL actions 'paths' to the endpoints. Includes the find/replace strings in brackets for path (non-query)
     variables."""
 
+    swagger = "/swagger.json"
+
     # Note that the leading slash is included for consistency with the swagger docs,
     # but it is dropped when the URL is actually constructed (see `url_with_path` in `horde_sdk.generic_api.endpoints`)
     v2_stats_img_models = "/v2/stats/img/models"
     v2_stats_img_totals = "/v2/stats/img/totals"
     v2_stats_text_models = "/v2/stats/text/models"
     v2_stats_text_totals = "/v2/stats/text/totals"
 
@@ -61,7 +66,14 @@
     v2_teams = "/v2/teams/{team_id}"
 
     v2_users_all = "/v2/users"
     v2_users = "/v2/users/{user_id}"
 
     v2_workers_all = "/v2/workers"
     v2_workers = "/v2/workers/{worker_id}"
+
+
+def get_ai_horde_swagger_url() -> str:
+    return url_with_path(
+        base_url=AI_HORDE_BASE_URL,
+        path=AI_HORDE_API_URL_Literals.swagger,
+    )
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ai_horde_api/fields.py` & `horde_sdk-0.4.0/horde_sdk/ai_horde_api/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,19 @@
         """Return the ID as a UUID."""
         if isinstance(self.id, uuid.UUID):
             return self.id
 
         return uuid.UUID(str(self.id), version=4)
 
     @field_validator("id")
-    def id_must_be_uuid(cls, v):
+    def id_must_be_uuid(cls, v: str | uuid.UUID) -> str | uuid.UUID:
         """Ensure that the ID is a valid UUID."""
+        if isinstance(v, uuid.UUID):
+            return v
+
         try:
             uuid.UUID(v, version=4)
         except ValueError as e:
             raise ValueError(f"Invalid UUID {v}") from e
         return v
 
     def __str__(self) -> str:
@@ -44,7 +47,11 @@
 
 class WorkerID(_UUID_Identifier):
     """Represents the ID of a worker. Instances of this class can be compared with a `str` or a UUID object."""
 
 
 class ImageID(_UUID_Identifier):
     """Represents the ID of an image. Instances of this class can be compared with a `str` or a UUID object."""
+
+
+class TeamID(_UUID_Identifier):
+    """Represents the ID of a team. Instances of this class can be compared with a `str` or a UUID object."""
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/generic_api/_reflection.py` & `horde_sdk-0.4.0/horde_sdk/generic_api/_reflection.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/src/horde_sdk/generic_api/endpoints.py` & `horde_sdk-0.4.0/horde_sdk/generic_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/src/horde_sdk/generic_api/metadata.py` & `horde_sdk-0.4.0/horde_sdk/generic_api/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class GenericHeaderFields(StrEnum):
     """`StrEnum` for data that is exclusively passed in the header of a request."""
 
     apikey = auto()
     accept = auto()
     # X_Fields = "X-Fields" # TODO?
+    client_agent = auto()
 
 
 class GenericAcceptTypes(StrEnum):
     """`StrEnum` for supported values for the header parameter 'accept'."""
 
     json = "application/json"
     # html = "application/html" # TODO?
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ratings_api/apimodels.py` & `horde_sdk-0.4.0/horde_sdk/ratings_api/apimodels.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 from enum import auto
 
 from pydantic import BaseModel, Field
 from strenum import StrEnum
 from typing_extensions import override
 
 from horde_sdk.consts import _UNDEFINED_MODEL, HTTPMethod
-from horde_sdk.generic_api import BaseRequestAuthenticated, BaseRequestUserSpecific
-from horde_sdk.generic_api.apimodels import BaseRequest, BaseResponse
+from horde_sdk.generic_api.apimodels import (
+    BaseRequest,
+    BaseRequestAuthenticated,
+    BaseRequestUserSpecific,
+    BaseResponse,
+)
 from horde_sdk.ratings_api.endpoints import RATING_API_BASE_URL, Rating_API_URL_Literals
 
 
 class BaseRatingsAPIRequest(BaseRequest):
     @override
     @classmethod
     def get_api_url(cls) -> str:
         return RATING_API_BASE_URL
 
 
 # region Responses
 class BaseImageRatingRecord(BaseModel):
     """The information about any image rating result."""
 
-    model_config = {"frozen": True}
-
     image: str
     """The URL to the image."""
     rating: int
     """The aesthetic rating the user gave."""
     artifacts: int | None
     """The quality ('artifact') rating the user gave."""
     average: float
@@ -36,26 +38,22 @@
     times_rated: int
     """The number of total ratings this image has received."""
 
 
 class ImageRatingResponseSubRecord(BaseModel):
     """A single sub-record in a response from the `/v1/image/ratings` endpoint."""
 
-    model_config = {"frozen": True}
-
     username: str
     rating: int
     artifacts: int | None
 
 
 class ImageRatingsResponse(BaseResponse):
     """The representation of the full response from `/v1/image/ratings`."""
 
-    model_config = {"frozen": True}
-
     total: int
     image: str
     image_id: uuid.UUID
     average: float
     times_rated: int
     ratings: list[ImageRatingResponseSubRecord]
 
@@ -71,16 +69,14 @@
     username: str
     """The name of the user in format `name#1234`."""
 
 
 class UserRatingsResponse(BaseResponse):
     """The representation of the full response from `/v1/user/ratings`."""
 
-    model_config = {"frozen": True}
-
     total: int
     """The total number of records in this response."""
     ratings: list[UserRatingsResponseSubRecord]
     """A `list` of all records returned."""
 
     @override
     @classmethod
@@ -91,31 +87,28 @@
 class UserValidateResponseRecord(BaseImageRatingRecord):
     """A single sub-record in a response from the `/v1/validate/{user_id}` endpoint."""
 
 
 class UserValidateResponse(BaseResponse):
     """The representation of the full response from `/v1/validate/{user_id}`."""
 
-    model_config = {"frozen": True}
-
     total: int
     """The total number of records in this response."""
     ratings: list[UserValidateResponseRecord]
     """A `list` of all records returned."""
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
         return _UNDEFINED_MODEL
 
 
 class UserCheckResponse(BaseResponse):
     """A single record from the `/v1/user/check/` endpoint."""
 
-    model_config = {"frozen": True}
     ratings_in_timeframe: int
     """The number of ratings this user submitted in the timeframe."""
     ratings_per_minute_in_timeframe: float
     """The average number of ratings per minute."""
     ratings_past_three_hours: int
     """The average number of ratings in the three hours prior to the request."""
     ratings_per_minute_for_past_three_hours: float
@@ -132,15 +125,15 @@
 
 
 # endregion
 
 # region Requests
 
 
-class BaseRequestImageSpecific(BaseRatingsAPIRequest, BaseRequestAuthenticated):
+class BaseRequestImageSpecific(BaseModel):
     """Represents the minimum for any request specifying a specific user to the API."""
 
     image_id: uuid.UUID
     """The UUID of the image."""
 
 
 class SelectableReturnFormats(StrEnum):
@@ -153,15 +146,19 @@
 class BaseSelectableReturnTypeRequest(BaseModel):
     """Mix-in class to describe an endpoint for which you can select the return data format."""
 
     format: SelectableReturnFormats  # noqa: A003
     """The format to request the response payload in, typically json."""
 
 
-class ImageRatingsRequest(BaseRatingsAPIRequest, BaseRequestAuthenticated, BaseSelectableReturnTypeRequest):
+class ImageRatingsRequest(
+    BaseRatingsAPIRequest,
+    BaseRequestAuthenticated,
+    BaseSelectableReturnTypeRequest,
+):
     """Represents the data needed to make a request to the `/v1/image/ratings/{image_id}` endpoint."""
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
         return None
 
@@ -173,15 +170,15 @@
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
         return Rating_API_URL_Literals.v1_image_ratings
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[ImageRatingsResponse]:
+    def get_success_response_type() -> type[ImageRatingsResponse]:
         return ImageRatingsResponse
 
 
 class ImageRatingsComparisonTypes(StrEnum):
     """Ways the API supports selecting a rating range."""
 
     greater_than_equal = "ge"
@@ -199,15 +196,20 @@
     artifacts: int | None = None
     """The target artifact rating, which will be compared by `artifacts_comparison`."""
     artifacts_comparison: ImageRatingsComparisonTypes | None = None
     """The way the `artifacts` will be compared. See `ImageRatingsComparisonTypes`."""
     min_ratings: int | None
 
 
-class UserValidateRequest(BaseRatingsAPIRequest, BaseRequestUserSpecific, ImageRatingsFilterableRequestBase):
+class UserValidateRequest(
+    BaseRatingsAPIRequest,
+    BaseRequestAuthenticated,
+    BaseRequestUserSpecific,
+    ImageRatingsFilterableRequestBase,
+):
     """Represents the data needed to make a request to the `/v1/user/validate/{user_id}` endpoint."""
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
         return None
 
@@ -219,19 +221,23 @@
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
         return Rating_API_URL_Literals.v1_user_validate
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[UserValidateResponse]:
+    def get_success_response_type() -> type[UserValidateResponse]:
         return UserValidateResponse
 
 
-class UserCheckRequest(BaseRatingsAPIRequest, BaseRequestUserSpecific):
+class UserCheckRequest(
+    BaseRatingsAPIRequest,
+    BaseRequestAuthenticated,
+    BaseRequestUserSpecific,
+):
     """Represents the data needed to make a request to the `/v1/user/check/` endpoint."""
 
     minutes: int = Field(ge=1)
     divergence: int = Field(ge=0)
 
     @override
     @classmethod
@@ -246,25 +252,28 @@
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
         return Rating_API_URL_Literals.v1_user_check
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[UserCheckResponse]:
+    def get_success_response_type() -> type[UserCheckResponse]:
         return UserCheckResponse
 
 
-class UserRatingsRequest(BaseRatingsAPIRequest, BaseRequestAuthenticated, ImageRatingsFilterableRequestBase):
+class UserRatingsRequest(
+    BaseRatingsAPIRequest,
+    BaseRequestAuthenticated,
+    ImageRatingsFilterableRequestBase,
+):
     """Represents the data needed to make a request to the `/v1/user/ratings/` endpoint."""
 
     limit: int
     offset: int = 0
     diverge: int | None
-    client_agent: str | None
 
     @override
     @classmethod
     def get_api_model_name(cls) -> str | None:
         return None
 
     @override
@@ -275,12 +284,12 @@
     @override
     @staticmethod
     def get_endpoint_subpath() -> str:
         return Rating_API_URL_Literals.v1_user_ratings
 
     @override
     @staticmethod
-    def get_expected_response_type() -> type[UserRatingsResponse]:
+    def get_success_response_type() -> type[UserRatingsResponse]:
         return UserRatingsResponse
 
 
 # endregion
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ratings_api/endpoints.py` & `horde_sdk-0.4.0/horde_sdk/ratings_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/src/horde_sdk/ratings_api/metadata.py` & `horde_sdk-0.4.0/horde_sdk/ratings_api/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Request metadata specific to the Ratings API."""
 from enum import auto
 
-from horde_sdk.generic_api import GenericPathFields, GenericQueryFields
+from horde_sdk.generic_api.metadata import GenericPathFields, GenericQueryFields
 
 
 class RatingsAPIPathFields(GenericPathFields):
     """Data that is exclusively passed as part of a URL path, and not after the '?' (query)."""
 
     user_id = auto()
     image_id = auto()
```

### Comparing `horde_sdk-0.1.3/src/horde_sdk.egg-info/PKG-INFO` & `horde_sdk-0.4.0/horde_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde-sdk
-Version: 0.1.3
+Version: 0.4.0
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -670,16 +670,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+[![Tests](https://github.com/Haidra-Org/horde-sdk/actions/workflows/maintests.yml/badge.svg)](https://github.com/Haidra-Org/horde-sdk/actions/workflows/maintests.yml)
+[![Documentation Status](https://readthedocs.org/projects/horde-sdk/badge/?version=latest)](https://horde-sdk.readthedocs.io/en/latest/?badge=latest)
+[![Unstable Tests](https://github.com/Haidra-Org/horde-sdk/actions/workflows/prtests.yml/badge.svg)](https://github.com/Haidra-Org/horde-sdk/actions/workflows/prtests.yml)
 # horde_sdk
 
 With the power of pydantic, you can simplify interfacing with the [AI-Horde's suite of APIs](https://github.com/db0/AI-Horde). Whether you want to request your own images, or roll your own worker software, this package may suit your needs for anything horde related.
 
-## AI-Horde
-`TODO`
-
-## Ratings API
-There is currently some support for the [Image Ratings](https://dbzer0.com/blog/the-image-ratings-are-flooding-in/) API that are rating images from the [DiffusionDB](https://poloclub.github.io/diffusiondb/) dataset. See `example.py` for an idea of how to start.
+## Documentation
+For detailed documentation, see our [read the docs page](https://horde-sdk.readthedocs.io/en/latest/index.html).
```

### Comparing `horde_sdk-0.1.3/tests/ai_horde_api/test_ai_horde_api_models.py` & `horde_sdk-0.4.0/tests/ai_horde_api/test_ai_horde_api_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from horde_sdk.ai_horde_api.apimodels.generate._async import (
     ImageGenerateAsyncRequest,
     ImageGenerationInputPayload,
 )
 from horde_sdk.ai_horde_api.consts import KNOWN_SAMPLERS, KNOWN_SOURCE_PROCESSING
 
 
-def test_api_endpoint():
+def test_api_endpoint() -> None:
     ImageGenerateAsyncRequest.get_api_url()
     ImageGenerateAsyncRequest.get_endpoint_subpath()
     ImageGenerateAsyncRequest.get_endpoint_url()
 
 
-def test_ImageGenerateAsyncRequest():
+def test_ImageGenerateAsyncRequest() -> None:
     test_async_request = ImageGenerateAsyncRequest(
         apikey="000000000",
         models=["Deliberate"],
         prompt="test prompt",
         params=ImageGenerationInputPayload(
             sampler_name=KNOWN_SAMPLERS.k_lms,
             cfg_scale=7.5,
```

### Comparing `horde_sdk-0.1.3/tests/conftest.py` & `horde_sdk-0.4.0/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,24 @@
-def pytest_collection_modifyitems(items):
+import pytest
+
+from horde_sdk.ai_horde_api.apimodels import (
+    ImageGenerateAsyncRequest,
+)
+
+
+@pytest.fixture(scope="function")
+def simple_image_gen_request() -> ImageGenerateAsyncRequest:
+    return ImageGenerateAsyncRequest(
+        apikey="0000000000",
+        prompt="a cat in a hat",
+        models=["Deliberate"],
+    )
+
+
+def pytest_collection_modifyitems(items: list) -> None:
     """Modifies test items in place to ensure test modules run in a given order."""
     MODULE_ORDER = ["tests_generic", "test_utils", "test_dynamically_check_apimodels"]
     # `test.scripts` must run first because it downloads the legacy database
     module_mapping = {item: item.module.__name__ for item in items}
 
     sorted_items = items.copy()
```

### Comparing `horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/ImageGenerateJobResponse.json` & `horde_sdk-0.4.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.09523809523809523%*

 * *Differences: {"'censor_nsfw'": 'False',*

 * * "'dry_run'": 'False',*

 * * "'models'": '[]',*

 * * "'nsfw'": 'False',*

 * * "'params'": "OrderedDict([('sampler_name', 'k_lms'), ('cfg_scale', 7.5), ('denoising_strength', "*

 * *             "0.75), ('seed', 'The little seed that could'), ('height', 512), ('width', 512), "*

 * *             "('seed_variation', 1), ('post_processing', []), ('karras', False), ('tiling', "*

 * *             "False), ('hires_fix', False), ('clip_skip', 1), ('control_type', 'canny'), "*

 * *             "('image_is_control', False),  […]*

```diff
@@ -1,64 +1,50 @@
 {
-    "id": "00000000-0000-0000-0000-000000000000",
-    "model": "string",
-    "payload": {
+    "censor_nsfw": false,
+    "dry_run": false,
+    "models": [],
+    "nsfw": false,
+    "params": {
         "cfg_scale": 7.5,
         "clip_skip": 1,
         "control_type": "canny",
-        "ddim_steps": 30,
         "denoising_strength": 0.75,
         "facefixer_strength": 0.75,
         "height": 512,
         "hires_fix": false,
         "image_is_control": false,
         "karras": false,
         "loras": [
             {
-                "clip": 1,
-                "inject_trigger": "string",
-                "model": 1,
+                "clip": 1.0,
+                "inject_trigger": "a",
+                "model": 1.0,
                 "name": "GlowingRunesAIV6"
             }
         ],
-        "n_iter": 1,
-        "post_processing": [
-            "GFPGAN"
-        ],
-        "prompt": "string",
+        "n": 1,
+        "post_processing": [],
         "return_control_map": false,
         "sampler_name": "k_lms",
         "seed": "The little seed that could",
         "seed_variation": 1,
         "special": {
-            "*": {
-                "additionalProp1": {},
-                "additionalProp2": {},
-                "additionalProp3": {}
-            }
+            "additionalProp1": {},
+            "additionalProp2": {},
+            "additionalProp3": {}
         },
+        "steps": 30,
         "tiling": false,
-        "use_nsfw_censor": true,
         "width": 512
     },
-    "r2_upload": "string",
-    "skipped": {
-        "blacklist": 0,
-        "bridge_version": 0,
-        "controlnet": 0,
-        "img2img": 0,
-        "kudos": 0,
-        "lora": 0,
-        "max_pixels": 0,
-        "models": 0,
-        "nsfw": 0,
-        "painting": 0,
-        "performance": 0,
-        "post-processing": 0,
-        "unsafe_ip": 0,
-        "untrusted": 0,
-        "worker_id": 0
-    },
-    "source_image": "string",
-    "source_mask": "string",
-    "source_processing": "img2img"
+    "prompt": "a",
+    "r2": true,
+    "replacement_filter": true,
+    "shared": false,
+    "slow_workers": true,
+    "source_image": "",
+    "source_mask": "",
+    "source_processing": "img2img",
+    "trusted_workers": false,
+    "worker_blacklist": false,
+    "workers": []
 }
```

### Comparing `horde_sdk-0.1.3/tests/test_data/ai_horde_api/example_responses/StatsModelsResponse.json` & `horde_sdk-0.4.0/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7002159083163774%*

 * *Differences: {"'day'": "{'Zelda BOTW': 5, 'Zeipher Female Model': 504, 'Zack3D': 63, 'Yiffy': 196, "*

 * *          "'Xynthii-Diffusion': 3, 'Woop-Woop Photo': 376, 'Wavyfusion': 5, 'waifu_diffusion': "*

 * *          "1064, 'Voxel Art Diffusion': 2, 'Vivid Watercolors': 35, 'VinteProtogenMix': 14, "*

 * *          "'Vintedois Diffusion': 8, 'vectorartz': 11, 'Vector Art': 22, 'Van Gogh Diffusion': 2, "*

 * *          "'Valorant Diffusion': 47, 'URPM': 3386, 'Unstable Ink Dream': 7, 'UMI Olympus': 15, "*

 * *          "'Ultraskin': 49, 'Uhmami' […]*

```diff
@@ -1,590 +1,721 @@
 {
     "day": {
-        "3DKX": 543,
-        "A to Zovya RPG": 179,
-        "ACertainThing": 1052,
-        "AIO Pixel Art": 272,
-        "Abyss OrangeMix": 5324,
-        "AbyssOrangeMix-AfterDark": 2206,
-        "Analog Diffusion": 1164,
-        "Anime Pencil Diffusion": 249,
-        "Anygen": 1159,
-        "Anything Diffusion": 35516,
-        "Anything v3": 1244,
-        "App Icon Diffusion": 168,
-        "Arcane Diffusion": 271,
-        "Archer Diffusion": 140,
-        "Asim Simpsons": 134,
-        "BPModel": 111,
-        "Balloon Art": 105,
-        "Borderlands": 166,
-        "BubblyDubbly": 189,
-        "Char": 121,
-        "CharHelper": 88,
-        "Cheese Daddys Landscape Mix": 487,
-        "ChilloutMix": 6976,
-        "ChromaV5": 313,
-        "Classic Animation Diffusion": 317,
-        "Clazy": 243,
-        "Colorful": 1412,
-        "Coloring Book": 159,
-        "Comic-Diffusion": 271,
-        "Concept Sheet": 86,
-        "Counterfeit": 12031,
-        "Cyberpunk Anime Diffusion": 368,
-        "CyriousMix": 1070,
-        "DGSpitzer Art Diffusion": 122,
-        "Dan Mumford Style": 97,
-        "Dark Victorian Diffusion": 182,
-        "Darkest Diffusion": 108,
-        "Deliberate": 100398,
-        "Disco Elysium": 107,
-        "DnD Item": 82,
-        "Double Exposure Diffusion": 144,
-        "DreamLikeSamKuvshinov": 213,
-        "Dreamlike Diffusion": 1559,
-        "Dreamlike Photoreal": 1900,
-        "Dreamshaper": 6579,
-        "DucHaiten": 370,
-        "DucHaiten Classic Anime": 126,
-        "Dungeons and Diffusion": 193,
-        "Dungeons n Waifus": 1105,
-        "Eimis Anime Diffusion": 1227,
-        "Elden Ring Diffusion": 292,
-        "Elldreth's Lucid Mix": 349,
-        "Elldreths Retro Mix": 169,
-        "Epic Diffusion": 7752,
-        "Eternos": 43,
-        "ExpMix Line": 667,
-        "Experience": 1053,
-        "FKing SciFi": 102,
-        "FaeTastic": 412,
-        "Fantasy Card Diffusion": 506,
-        "Funko Diffusion": 105,
-        "Furry Epoch": 603,
-        "Future Diffusion": 177,
-        "GTA5 Artwork Diffusion": 188,
-        "Ghibli Diffusion": 429,
-        "GorynichMix": 583,
-        "Grapefruit Hentai": 6964,
-        "Graphic-Art": 129,
-        "GuoFeng": 811,
-        "Guohua Diffusion": 273,
-        "HASDX": 1022,
-        "HRL": 397,
-        "Hassanblend": 1292,
-        "Healy's Anime Blend": 539,
-        "Hentai Diffusion": 9627,
-        "Illuminati Diffusion": 778,
-        "Inkpunk Diffusion": 419,
-        "JWST Deep Space Diffusion": 183,
-        "Jim Eidomode": 694,
-        "Kenshi": 106,
-        "Knollingcase": 86,
-        "Korestyle": 225,
-        "Laolei New Berry Protogen Mix": 193,
-        "Lawlas's yiff mix": 2924,
-        "Liberty": 3035,
-        "Marvel Diffusion": 121,
-        "Mega Merge Diffusion": 202,
-        "Microcasing": 57,
-        "Microchars": 78,
-        "Microcritters": 38,
-        "Microscopic": 85,
-        "Microworlds": 462,
-        "Midjourney Diffusion": 6696,
-        "Midjourney PaintArt": 217,
-        "Min Illust Background": 96,
-        "ModernArt Diffusion": 191,
-        "Moedel": 164,
-        "MoistMix": 257,
-        "Movie Diffusion": 187,
-        "NeverEnding Dream": 398,
-        "Nitro Diffusion": 222,
-        "Openniji": 873,
-        "OrbAI": 59,
-        "PFG": 436,
-        "PIXHELL": 79,
-        "PPP": 204,
-        "PRMJ": 114,
-        "PVC": 97,
-        "Papercut Diffusion": 151,
-        "Papercutcraft": 67,
-        "Pastel Mix": 1042,
-        "Perfect World": 1635,
-        "Poison": 509,
-        "Pokemon3D": 68,
-        "PortraitPlus": 648,
-        "Pretty 2.5D": 1911,
-        "Project Unreal Engine 5": 17297,
-        "ProtoGen": 774,
-        "Protogen Anime": 197,
-        "Protogen Infinity": 512,
-        "Pulp Vector Art": 36,
-        "RCNZ Dumb Monkey": 133,
-        "RCNZ Gorilla With A Brick": 187,
-        "RPG": 509,
-        "Rachel Walker Watercolors": 39,
-        "Rainbowpatch": 50,
-        "Ranma Diffusion": 406,
-        "RealBiter": 722,
-        "Realism Engine": 786,
-        "Realistic Vision": 9196,
-        "Redshift Diffusion": 721,
-        "Rev Animated": 8381,
-        "Robo-Diffusion": 61,
-        "Rodent Diffusion": 172,
-        "SD-Silicon": 774,
-        "Samdoesarts Ultmerge": 297,
-        "Sci-Fi Diffusion": 104,
-        "Seek.art MEGA": 163,
-        "Smoke Diffusion": 81,
-        "Something": 1657,
-        "Sonic Diffusion": 139,
-        "Spider-Verse Diffusion": 48,
-        "Squishmallow Diffusion": 48,
-        "Supermarionation": 39,
-        "Sygil-Dev Diffusion": 264,
-        "Synthwave": 82,
-        "SynthwavePunk": 39,
-        "T-Shirt Diffusion": 67,
-        "T-Shirt Print Designs": 68,
-        "TrexMix": 60,
-        "Trinart Characters": 265,
-        "Tron Legacy Diffusion": 80,
-        "UMI Olympus": 237,
-        "URPM": 8370,
-        "Uhmami": 263,
-        "Ultraskin": 145,
-        "Unstable Ink Dream": 256,
-        "Valorant Diffusion": 296,
-        "Van Gogh Diffusion": 88,
-        "Vector Art": 92,
-        "VinteProtogenMix": 86,
-        "Vintedois Diffusion": 398,
-        "Vivid Watercolors": 65,
-        "Voxel Art Diffusion": 71,
-        "Wavyfusion": 102,
-        "Woop-Woop Photo": 926,
-        "Xynthii-Diffusion": 41,
-        "Yiffy": 1918,
-        "Zack3D": 257,
-        "Zeipher Female Model": 7093,
-        "Zelda BOTW": 52,
-        "anything_v4_inpainting": 220,
-        "dreamlike_diffusion_inpainting": 115,
-        "iCoMix": 469,
-        "kurzgesagt": 81,
-        "mo-di-diffusion": 469,
-        "pix2pix": 36,
-        "stable_diffusion": 50067,
-        "stable_diffusion_2.1": 5435,
-        "stable_diffusion_2_inpainting": 52,
-        "stable_diffusion_inpainting": 266,
-        "trinart": 110,
-        "vectorartz": 33,
-        "waifu_diffusion": 3895
+        "3DKX": 76,
+        "526Mix-Animated": 42,
+        "A to Zovya RPG": 50,
+        "A-Zovya RPG Inpainting": 6,
+        "ACertainThing": 254,
+        "AIO Pixel Art": 21,
+        "Abyss OrangeMix": 2714,
+        "AbyssOrangeMix-AfterDark": 505,
+        "Analog Diffusion": 686,
+        "Analog Madness": 138,
+        "Anime Pencil Diffusion": 96,
+        "AnyLoRA": 111,
+        "Anygen": 148,
+        "Anything Diffusion": 44118,
+        "Anything Diffusion Inpainting": 28,
+        "Anything v3": 2487,
+        "Anything v5": 252,
+        "App Icon Diffusion": 5,
+        "Arcane Diffusion": 281,
+        "Archer Diffusion": 9,
+        "Art Of Mtg": 26,
+        "Asim Simpsons": 9,
+        "Aurora": 219,
+        "BB95 Furry Mix": 11640,
+        "BPModel": 28,
+        "BRA": 1289,
+        "Babes": 367,
+        "Balloon Art": 4,
+        "Borderlands": 31,
+        "BubblyDubbly": 26,
+        "BweshMix": 41,
+        "CamelliaMix 2.5D": 1177,
+        "Cetus-Mix": 106,
+        "Char": 5,
+        "CharHelper": 23,
+        "Cheese Daddys Landscape Mix": 42,
+        "ChilloutMix": 4749,
+        "ChromaV5": 9,
+        "Classic Animation Diffusion": 33,
+        "Clazy": 19,
+        "Colorful": 131,
+        "Coloring Book": 24,
+        "Comic-Diffusion": 46,
+        "Concept Sheet": 60,
+        "Counterfeit": 8274,
+        "CyberRealistic": 1522,
+        "Cyberpunk Anime Diffusion": 66,
+        "CyriousMix": 168,
+        "DGSpitzer Art Diffusion": 13,
+        "Dan Mumford Style": 6,
+        "Dark Sushi Mix": 101,
+        "Dark Victorian Diffusion": 68,
+        "Darkest Diffusion": 25,
+        "Deliberate": 104891,
+        "Deliberate Inpainting": 155,
+        "Disco Elysium": 5,
+        "Disney Pixar Cartoon Type A": 109,
+        "DnD Item": 17,
+        "DnD Map Generator": 13,
+        "Double Exposure Diffusion": 14,
+        "DreamLikeSamKuvshinov": 13,
+        "DreamShaper Inpainting": 61,
+        "Dreamlike Diffusion": 70,
+        "Dreamlike Photoreal": 444,
+        "Dreamshaper": 21434,
+        "DucHaiten": 154,
+        "DucHaiten Classic Anime": 34,
+        "Dungeons and Diffusion": 87,
+        "Dungeons n Waifus": 105,
+        "Edge Of Realism": 1904,
+        "Eimis Anime Diffusion": 777,
+        "Elden Ring Diffusion": 9,
+        "Elldreth's Lucid Mix": 14,
+        "Elldreths Retro Mix": 10,
+        "Elysium Anime": 164,
+        "Epic Diffusion": 2455,
+        "Epic Diffusion Inpainting": 23,
+        "Eternos": 5,
+        "Ether Real Mix": 21,
+        "ExpMix Line": 159,
+        "Experience": 160,
+        "FKing SciFi": 52,
+        "FaeTastic": 87,
+        "Fantasy Card Diffusion": 47,
+        "Fluffusion": 289,
+        "Funko Diffusion": 86,
+        "Furry Epoch": 235,
+        "Future Diffusion": 45,
+        "GTA5 Artwork Diffusion": 89,
+        "Galena Redux": 176,
+        "Ghibli Diffusion": 41,
+        "GhostMix": 70,
+        "GorynichMix": 312,
+        "Grapefruit Hentai": 3777,
+        "Graphic-Art": 22,
+        "GuFeng": 19,
+        "GuoFeng": 383,
+        "Guohua Diffusion": 5,
+        "HASDX": 38,
+        "HRL": 82,
+        "Hassaku": 161,
+        "Hassanblend": 559,
+        "Healy's Anime Blend": 378,
+        "Henmix Real": 607,
+        "Hentai Diffusion": 10535,
+        "ICBINP - I Can't Believe It's Not Photography": 20841,
+        "Illuminati Diffusion": 26,
+        "Inkpunk Diffusion": 50,
+        "JWST Deep Space Diffusion": 8,
+        "Jim Eidomode": 138,
+        "JoMad Diffusion": 4,
+        "Kenshi": 150,
+        "Knollingcase": 17,
+        "Korestyle": 67,
+        "Laolei New Berry Protogen Mix": 772,
+        "Lawlas's yiff mix": 1278,
+        "Liberty": 649,
+        "Lyriel": 109,
+        "Marvel Diffusion": 25,
+        "Mega Merge Diffusion": 19,
+        "MeinaMix": 190,
+        "Microcasing": 4,
+        "Microchars": 24,
+        "Microcritters": 8,
+        "Microscopic": 4,
+        "Microworlds": 13,
+        "Midjourney PaintArt": 77,
+        "Min Illust Background": 17,
+        "Mistoon Amethyst": 224,
+        "ModernArt Diffusion": 8,
+        "Moedel": 7,
+        "MoistMix": 8,
+        "MoonMix Fantasy": 117,
+        "Movie Diffusion": 111,
+        "Neurogen": 236,
+        "NeverEnding Dream": 880,
+        "Nitro Diffusion": 15,
+        "OpenJourney Diffusion": 135,
+        "Openniji": 53,
+        "OrbAI": 47,
+        "PFG": 262,
+        "PIXHELL": 19,
+        "PPP": 162,
+        "PRMJ": 11,
+        "PVC": 6,
+        "Papercut Diffusion": 10,
+        "Papercutcraft": 6,
+        "Pastel Mix": 628,
+        "Perfect World": 296,
+        "Poison": 85,
+        "Pokemon3D": 19,
+        "PortraitPlus": 82,
+        "Pretty 2.5D": 2990,
+        "Project Unreal Engine 5": 3555,
+        "ProtoGen": 11,
+        "Protogen Anime": 33,
+        "Protogen Infinity": 16,
+        "Pulp Vector Art": 23,
+        "RCNZ Dumb Monkey": 16,
+        "RCNZ Gorilla With A Brick": 158,
+        "RPG": 396,
+        "Rachel Walker Watercolors": 5,
+        "Rainbowpatch": 6,
+        "Ranma Diffusion": 90,
+        "Real Dos Mix": 36,
+        "RealBiter": 134,
+        "Realisian": 190,
+        "Realism Engine": 499,
+        "Realistic Vision": 2601,
+        "Realistic Vision Inpainting": 118,
+        "Redshift Diffusion": 64,
+        "Reliberate": 395,
+        "Rev Animated": 627,
+        "Robo-Diffusion": 9,
+        "Rodent Diffusion": 7,
+        "SD-Silicon": 30,
+        "Samaritan 3d Cartoon": 91,
+        "Samdoesarts Ultmerge": 2,
+        "Sci-Fi Diffusion": 9,
+        "Seek.art MEGA": 22,
+        "Smoke Diffusion": 12,
+        "Something": 598,
+        "Sonic Diffusion": 13,
+        "Spider-Verse Diffusion": 56,
+        "Squishmallow Diffusion": 4,
+        "Supermarionation": 18,
+        "SweetBoys 2D": 73,
+        "Sygil-Dev Diffusion": 5,
+        "Synthwave": 10,
+        "SynthwavePunk": 16,
+        "T-Shirt Diffusion": 3,
+        "T-Shirt Print Designs": 13,
+        "ToonYou": 41,
+        "TrexMix": 14,
+        "Trinart Characters": 16,
+        "Tron Legacy Diffusion": 52,
+        "UMI Olympus": 15,
+        "URPM": 3386,
+        "Uhmami": 15,
+        "Ultraskin": 49,
+        "Unstable Ink Dream": 7,
+        "Valorant Diffusion": 47,
+        "Van Gogh Diffusion": 2,
+        "Vector Art": 22,
+        "VinteProtogenMix": 14,
+        "Vintedois Diffusion": 8,
+        "Vivid Watercolors": 35,
+        "Voxel Art Diffusion": 2,
+        "Wavyfusion": 5,
+        "Western Animation Diffusion": 554,
+        "Woop-Woop Photo": 376,
+        "Xynthii-Diffusion": 3,
+        "Yiffy": 196,
+        "Zack3D": 63,
+        "Zeipher Female Model": 504,
+        "Zelda BOTW": 5,
+        "iCoMix": 7953,
+        "iCoMix Inpainting": 58,
+        "kurzgesagt": 3,
+        "majicMIX realistic": 4147,
+        "mo-di-diffusion": 26,
+        "stable_diffusion": 18700,
+        "stable_diffusion_2.1": 1402,
+        "stable_diffusion_inpainting": 817,
+        "trinart": 53,
+        "vectorartz": 11,
+        "waifu_diffusion": 1064
     },
     "month": {
-        "": 22,
-        "3DKX": 27279,
-        "A to Zovya RPG": 3727,
-        "ACertainThing": 21136,
-        "AIO Pixel Art": 9202,
-        "Abyss OrangeMix": 214407,
-        "AbyssOrangeMix-AfterDark": 42635,
-        "Analog Diffusion": 53315,
-        "Anime Pencil Diffusion": 5167,
-        "Anygen": 30998,
-        "Anything Diffusion": 1106052,
-        "Anything v3": 95710,
-        "App Icon Diffusion": 6404,
-        "Arcane Diffusion": 9302,
-        "Archer Diffusion": 6105,
-        "Asim Simpsons": 2303,
-        "BPModel": 4303,
-        "Balloon Art": 2276,
-        "Borderlands": 4604,
-        "BubblyDubbly": 3788,
-        "Char": 1516,
-        "CharHelper": 2531,
-        "Cheese Daddys Landscape Mix": 8201,
-        "ChilloutMix": 161293,
-        "ChromaV5": 7587,
-        "Classic Animation Diffusion": 7914,
-        "Clazy": 2872,
-        "Colorful": 23262,
-        "Coloring Book": 1230,
-        "Comic-Diffusion": 12000,
-        "Concept Sheet": 3497,
-        "Counterfeit": 333516,
-        "Cyberpunk Anime Diffusion": 11244,
-        "CyriousMix": 52430,
-        "DGSpitzer Art Diffusion": 2407,
-        "Dan Mumford Style": 3005,
-        "Dark Victorian Diffusion": 6057,
-        "Darkest Diffusion": 18151,
-        "Deliberate": 2589127,
-        "Disco Elysium": 2467,
-        "DnD Item": 3855,
-        "Double Exposure Diffusion": 2948,
-        "DreamLikeSamKuvshinov": 6395,
-        "Dreamlike Diffusion": 28496,
-        "Dreamlike Photoreal": 104329,
-        "Dreamshaper": 200083,
-        "DucHaiten": 8763,
-        "DucHaiten Classic Anime": 7347,
-        "Dungeons and Diffusion": 10620,
-        "Dungeons n Waifus": 19613,
-        "Eimis Anime Diffusion": 52751,
-        "Elden Ring Diffusion": 10925,
-        "Elldreth's Lucid Mix": 7128,
-        "Elldreths Retro Mix": 5015,
-        "Epic Diffusion": 183511,
-        "Eternos": 1798,
-        "ExpMix Line": 55321,
-        "Experience": 38247,
-        "FKing SciFi": 5213,
-        "FaeTastic": 45979,
-        "Fantasy Card Diffusion": 8121,
-        "Funko Diffusion": 3871,
-        "Furry Epoch": 16458,
-        "Future Diffusion": 3937,
-        "GTA5 Artwork Diffusion": 16263,
-        "GTM Ultimate Blend": 6032,
-        "Ghibli Diffusion": 4973,
-        "GorynichMix": 19641,
-        "Grapefruit Hentai": 133812,
-        "Graphic-Art": 4071,
-        "GuoFeng": 14487,
-        "Guohua Diffusion": 3227,
-        "HASDX": 21817,
-        "HRL": 10759,
-        "Hassanblend": 42319,
-        "Healy's Anime Blend": 11265,
-        "Hentai Diffusion": 422334,
-        "Illuminati Diffusion": 23517,
-        "Inkpunk Diffusion": 17695,
-        "JWST Deep Space Diffusion": 5862,
-        "Jim Eidomode": 5862,
-        "Kenshi": 35173,
-        "Knollingcase": 2966,
-        "Korestyle": 3912,
-        "Laolei New Berry Protogen Mix": 9336,
-        "Lawlas's yiff mix": 141521,
-        "Liberty": 96651,
-        "Marvel Diffusion": 2599,
-        "Mega Merge Diffusion": 5062,
-        "Microcasing": 2081,
-        "Microchars": 2197,
-        "Microcritters": 2072,
-        "Microscopic": 1655,
-        "Microworlds": 5480,
-        "Midjourney Diffusion": 142024,
-        "Midjourney PaintArt": 33792,
-        "Min Illust Background": 2588,
-        "ModernArt Diffusion": 3370,
-        "Moedel": 4248,
-        "MoistMix": 27590,
-        "Movie Diffusion": 7000,
-        "NeverEnding Dream": 51690,
-        "Nitro Diffusion": 4310,
-        "Open Journey Beta": 248,
-        "Openniji": 28838,
-        "OrbAI": 1705,
-        "PFG": 20834,
-        "PIXHELL": 960,
-        "PPP": 16159,
-        "PRMJ": 3016,
-        "PVC": 992,
-        "Papercut Diffusion": 4721,
-        "Papercutcraft": 6535,
-        "Pastel Mix": 37940,
-        "Perfect World": 17117,
-        "Poison": 25023,
-        "Pokemon3D": 2310,
-        "PortraitPlus": 18649,
-        "Pretty 2.5D": 70488,
-        "Project Unreal Engine 5": 347413,
-        "ProtoGen": 27768,
-        "Protogen Anime": 7434,
-        "Protogen Infinity": 36252,
-        "Pulp Vector Art": 2381,
-        "RCNZ Dumb Monkey": 4633,
-        "RCNZ Gorilla With A Brick": 5482,
-        "RPG": 15562,
-        "Rachel Walker Watercolors": 3035,
-        "Rainbowpatch": 2535,
-        "Ranma Diffusion": 13352,
-        "RealBiter": 23136,
-        "Realism Engine": 26505,
-        "Realistic Vision": 319098,
-        "Redshift Diffusion": 28999,
-        "Rev Animated": 154606,
-        "Robo-Diffusion": 2948,
-        "Rodent Diffusion": 4414,
-        "SD-Silicon": 11816,
-        "Samdoesarts Ultmerge": 14503,
-        "Sci-Fi Diffusion": 4786,
-        "Seek.art MEGA": 19849,
-        "Smoke Diffusion": 2152,
-        "Something": 30352,
-        "Sonic Diffusion": 3735,
-        "Spider-Verse Diffusion": 2059,
-        "Squishmallow Diffusion": 1858,
-        "Stable Diffusion 2 Depth": 42,
-        "Supermarionation": 1513,
-        "Sygil-Dev Diffusion": 2791,
-        "Synthwave": 3214,
-        "SynthwavePunk": 2067,
-        "T-Shirt Diffusion": 3258,
-        "T-Shirt Print Designs": 4878,
-        "TrexMix": 3093,
-        "Trinart Characters": 9287,
-        "Tron Legacy Diffusion": 2571,
-        "UMI Olympus": 8631,
-        "URPM": 261227,
-        "Uhmami": 7780,
-        "Ultraskin": 5351,
-        "Unstable Ink Dream": 4882,
-        "Valorant Diffusion": 5569,
-        "Van Gogh Diffusion": 2123,
-        "Vector Art": 3189,
-        "VinteProtogenMix": 7801,
-        "Vintedois Diffusion": 18223,
-        "Vivid Watercolors": 3439,
-        "Voxel Art Diffusion": 2044,
-        "Waifu Diffusion Beta": 1963,
-        "Wavyfusion": 2573,
-        "Woop-Woop Photo": 33123,
-        "Xynthii-Diffusion": 1739,
-        "Yiffy": 60025,
-        "Zack3D": 9513,
-        "Zeipher Female Model": 199364,
-        "Zelda BOTW": 2545,
-        "anything_v4_inpainting": 2771,
-        "colorbook": 1892,
-        "dreamlike_diffusion_inpainting": 999,
-        "iCoMix": 51140,
-        "kurzgesagt": 2501,
-        "mo-di-diffusion": 13538,
-        "pix2pix": 2293,
-        "stable_diffusion": 1641740,
-        "stable_diffusion_1.4": 393,
-        "stable_diffusion_2.0": 788,
-        "stable_diffusion_2.0_512": 577,
-        "stable_diffusion_2.1": 90131,
-        "stable_diffusion_2.1_512": 1099,
-        "stable_diffusion_2_inpainting": 1174,
-        "stable_diffusion_inpainting": 19478,
-        "trinart": 7035,
-        "vectorartz": 3070,
-        "waifu_diffusion": 180673
+        "": 3,
+        "3DKX": 2364,
+        "526Mix-Animated": 2238,
+        "A to Zovya RPG": 1866,
+        "A-Zovya RPG Inpainting": 565,
+        "ACertainThing": 9808,
+        "AIO Pixel Art": 1040,
+        "Abyss OrangeMix": 81603,
+        "AbyssOrangeMix-AfterDark": 24561,
+        "Analog Diffusion": 11029,
+        "Analog Madness": 3727,
+        "Anime Pencil Diffusion": 1081,
+        "AnyLoRA": 10618,
+        "Anygen": 5030,
+        "Anything Diffusion": 1143753,
+        "Anything Diffusion Inpainting": 2231,
+        "Anything v3": 99031,
+        "Anything v5": 14645,
+        "App Icon Diffusion": 1931,
+        "Arcane Diffusion": 5823,
+        "Archer Diffusion": 464,
+        "Art Of Mtg": 1604,
+        "Asim Simpsons": 520,
+        "Aurora": 9417,
+        "BB95 Furry Mix": 368237,
+        "BPModel": 651,
+        "BRA": 57208,
+        "Babes": 11178,
+        "Balloon Art": 410,
+        "Borderlands": 742,
+        "BubblyDubbly": 664,
+        "BweshMix": 7544,
+        "CamelliaMix 2.5D": 49512,
+        "Cetus-Mix": 9644,
+        "Char": 1148,
+        "CharHelper": 628,
+        "Cheese Daddys Landscape Mix": 2039,
+        "ChilloutMix": 184695,
+        "ChromaV5": 1411,
+        "Classic Animation Diffusion": 1304,
+        "Clazy": 486,
+        "Colorful": 4838,
+        "Coloring Book": 1391,
+        "Comic-Diffusion": 1457,
+        "Concept Sheet": 1078,
+        "Counterfeit": 255574,
+        "CyberRealistic": 36044,
+        "Cyberpunk Anime Diffusion": 4403,
+        "CyriousMix": 8368,
+        "DGSpitzer Art Diffusion": 443,
+        "Dan Mumford Style": 1624,
+        "Dark Sushi Mix": 7853,
+        "Dark Victorian Diffusion": 1850,
+        "Darkest Diffusion": 695,
+        "Deliberate": 3119191,
+        "Deliberate Inpainting": 8018,
+        "Disco Elysium": 612,
+        "Disney Pixar Cartoon Type A": 3368,
+        "DnD Item": 1254,
+        "DnD Map Generator": 672,
+        "Double Exposure Diffusion": 504,
+        "DreamLikeSamKuvshinov": 583,
+        "DreamShaper Inpainting": 1656,
+        "Dreamlike Diffusion": 8010,
+        "Dreamlike Photoreal": 33889,
+        "Dreamshaper": 563737,
+        "DucHaiten": 4685,
+        "DucHaiten Classic Anime": 1988,
+        "Dungeons and Diffusion": 3290,
+        "Dungeons n Waifus": 6674,
+        "Edge Of Realism": 27265,
+        "Eimis Anime Diffusion": 15073,
+        "Elden Ring Diffusion": 1446,
+        "Elldreth's Lucid Mix": 1697,
+        "Elldreths Retro Mix": 809,
+        "Elysium Anime": 4171,
+        "Epic Diffusion": 159149,
+        "Epic Diffusion Inpainting": 925,
+        "Eternos": 487,
+        "Ether Real Mix": 3721,
+        "ExpMix Line": 4597,
+        "Experience": 8186,
+        "FKing SciFi": 1554,
+        "FaeTastic": 4021,
+        "Fantasy Card Diffusion": 688,
+        "Fluffusion": 21595,
+        "Funko Diffusion": 920,
+        "Furry Epoch": 7276,
+        "Future Diffusion": 1112,
+        "GTA5 Artwork Diffusion": 8305,
+        "Galena Redux": 4557,
+        "Ghibli Diffusion": 2160,
+        "GhostMix": 3828,
+        "GorynichMix": 5598,
+        "Grapefruit Hentai": 49337,
+        "Graphic-Art": 868,
+        "GuFeng": 1127,
+        "GuoFeng": 16447,
+        "Guohua Diffusion": 462,
+        "HASDX": 1982,
+        "HRL": 2190,
+        "Hassaku": 8818,
+        "Hassanblend": 10954,
+        "Healy's Anime Blend": 3426,
+        "Henmix Real": 7012,
+        "Hentai Diffusion": 301535,
+        "ICBINP - I Can't Believe It's Not Photography": 666237,
+        "Illuminati Diffusion": 1500,
+        "Inkpunk Diffusion": 5560,
+        "JWST Deep Space Diffusion": 760,
+        "Jim Eidomode": 3414,
+        "JoMad Diffusion": 384,
+        "Kenshi": 1705,
+        "Knollingcase": 1919,
+        "Korestyle": 579,
+        "Laolei New Berry Protogen Mix": 8615,
+        "Lawlas's yiff mix": 34960,
+        "Liberty": 17348,
+        "Lyriel": 7308,
+        "Marvel Diffusion": 959,
+        "Mega Merge Diffusion": 932,
+        "MeinaMix": 6959,
+        "Microcasing": 340,
+        "Microchars": 842,
+        "Microcritters": 375,
+        "Microscopic": 349,
+        "Microworlds": 763,
+        "Midjourney PaintArt": 4710,
+        "Min Illust Background": 489,
+        "Mistoon Amethyst": 8483,
+        "ModernArt Diffusion": 1016,
+        "Moedel": 602,
+        "MoistMix": 1254,
+        "MoonMix Fantasy": 4486,
+        "Movie Diffusion": 3598,
+        "Neurogen": 5083,
+        "NeverEnding Dream": 19550,
+        "Nitro Diffusion": 671,
+        "OpenJourney Diffusion": 4683,
+        "Openniji": 1941,
+        "OrbAI": 438,
+        "PFG": 3235,
+        "PIXHELL": 717,
+        "PPP": 2964,
+        "PRMJ": 739,
+        "PVC": 540,
+        "Papercut Diffusion": 1003,
+        "Papercutcraft": 416,
+        "Pastel Mix": 21862,
+        "Perfect World": 23122,
+        "Poison": 5685,
+        "Pokemon3D": 851,
+        "PortraitPlus": 3888,
+        "Pretty 2.5D": 169098,
+        "Project Unreal Engine 5": 129699,
+        "ProtoGen": 5952,
+        "Protogen Anime": 864,
+        "Protogen Infinity": 2296,
+        "Pulp Vector Art": 522,
+        "RCNZ Dumb Monkey": 2030,
+        "RCNZ Gorilla With A Brick": 25561,
+        "RPG": 7602,
+        "Rachel Walker Watercolors": 570,
+        "Rainbowpatch": 632,
+        "Ranma Diffusion": 2050,
+        "Real Dos Mix": 1690,
+        "RealBiter": 6038,
+        "Realisian": 8207,
+        "Realism Engine": 15109,
+        "Realistic Vision": 84179,
+        "Realistic Vision Inpainting": 7177,
+        "Redshift Diffusion": 5404,
+        "Reliberate": 17937,
+        "Rev Animated": 32748,
+        "Robo-Diffusion": 1388,
+        "Rodent Diffusion": 697,
+        "SD-Silicon": 1194,
+        "Samaritan 3d Cartoon": 3058,
+        "Samdoesarts Ultmerge": 579,
+        "Sci-Fi Diffusion": 774,
+        "Seek.art MEGA": 2208,
+        "Smoke Diffusion": 480,
+        "Something": 17666,
+        "Sonic Diffusion": 1212,
+        "Spider-Verse Diffusion": 848,
+        "Squishmallow Diffusion": 479,
+        "Supermarionation": 656,
+        "SweetBoys 2D": 3128,
+        "Sygil-Dev Diffusion": 583,
+        "Synthwave": 716,
+        "SynthwavePunk": 992,
+        "T-Shirt Diffusion": 746,
+        "T-Shirt Print Designs": 1009,
+        "ToonYou": 4762,
+        "TrexMix": 3830,
+        "Trinart Characters": 939,
+        "Tron Legacy Diffusion": 943,
+        "UMI Olympus": 1215,
+        "URPM": 90233,
+        "Uhmami": 4968,
+        "Ultraskin": 2065,
+        "Unstable Ink Dream": 1674,
+        "Valorant Diffusion": 1098,
+        "Van Gogh Diffusion": 403,
+        "Vector Art": 737,
+        "VinteProtogenMix": 601,
+        "Vintedois Diffusion": 676,
+        "Vivid Watercolors": 1539,
+        "Voxel Art Diffusion": 635,
+        "Wavyfusion": 1095,
+        "Western Animation Diffusion": 5032,
+        "Woop-Woop Photo": 23994,
+        "Xynthii-Diffusion": 379,
+        "Yiffy": 14032,
+        "Zack3D": 4163,
+        "Zeipher Female Model": 18523,
+        "Zelda BOTW": 806,
+        "anything_v4_inpainting": 99,
+        "dreamlike_diffusion_inpainting": 1,
+        "horde_special::stability.ai#6901": 305,
+        "iCoMix": 138013,
+        "iCoMix Inpainting": 2139,
+        "kurzgesagt": 537,
+        "majicMIX realistic": 130809,
+        "mo-di-diffusion": 2491,
+        "pix2pix": 71,
+        "stable_diffusion": 932563,
+        "stable_diffusion_2.1": 44634,
+        "stable_diffusion_inpainting": 16707,
+        "trinart": 715,
+        "vectorartz": 770,
+        "waifu_diffusion": 35058
     },
     "total": {
-        "": 102,
-        "3DKX": 45183,
-        "A to Zovya RPG": 4608,
-        "ACertainThing": 32890,
-        "AIO Pixel Art": 15243,
-        "Abyss OrangeMix": 326624,
-        "AbyssOrangeMix-AfterDark": 69555,
-        "Analog Diffusion": 112564,
-        "Anime Pencil Diffusion": 6200,
-        "Anygen": 74125,
-        "Anything Diffusion": 2027396,
-        "Anything v3": 156787,
-        "App Icon Diffusion": 10135,
-        "Arcane Diffusion": 16690,
-        "Archer Diffusion": 8454,
-        "Asim Simpsons": 3895,
-        "BPModel": 5960,
-        "Balloon Art": 3112,
-        "Borderlands": 7289,
-        "BubblyDubbly": 7776,
-        "Char": 1516,
-        "CharHelper": 3684,
-        "Cheese Daddys Landscape Mix": 11314,
-        "ChilloutMix": 181632,
-        "ChromaV5": 16110,
-        "Classic Animation Diffusion": 12177,
-        "Clazy": 4331,
-        "Colorful": 25303,
-        "Coloring Book": 1230,
-        "Comic-Diffusion": 19438,
-        "Concept Sheet": 4853,
+        "": 160,
+        "3DKX": 68737,
+        "526Mix-Animated": 8283,
+        "A to Zovya RPG": 13875,
+        "A-Zovya RPG Inpainting": 899,
+        "ACertainThing": 65026,
+        "AIO Pixel Art": 24609,
+        "Abyss OrangeMix": 876443,
+        "AbyssOrangeMix-AfterDark": 241742,
+        "Analog Diffusion": 177864,
+        "Analog Madness": 11239,
+        "Anime Pencil Diffusion": 14456,
+        "AnyLoRA": 11084,
+        "Anygen": 108872,
+        "Anything Diffusion": 5397762,
+        "Anything Diffusion Inpainting": 2864,
+        "Anything v3": 387853,
+        "Anything v5": 21590,
+        "App Icon Diffusion": 20313,
+        "Arcane Diffusion": 60153,
+        "Archer Diffusion": 14345,
+        "Art Of Mtg": 3171,
+        "Asim Simpsons": 8090,
+        "Aurora": 20189,
+        "BB95 Furry Mix": 560260,
+        "BPModel": 11311,
+        "BRA": 78272,
+        "Babes": 16026,
+        "Balloon Art": 6941,
+        "Beautiful Realistic Asians": 85518,
+        "Borderlands": 13106,
+        "BubblyDubbly": 12599,
+        "BweshMix": 11956,
+        "CamelliaMix 2.5D": 86011,
+        "Cetus-Mix": 13452,
+        "Char": 6908,
+        "CharHelper": 7573,
+        "Cheese Daddys Landscape Mix": 33767,
+        "ChilloutMix": 987111,
+        "ChromaV5": 28944,
+        "Classic Animation Diffusion": 25889,
+        "Clazy": 9154,
+        "Colorful": 60195,
+        "Coloring Book": 6945,
+        "Comic-Diffusion": 33744,
+        "Concept Sheet": 9571,
         "ControlNet - Canny": 333,
         "ControlNet - Canny - AnyV3": 99,
         "ControlNet - Canny - Delib": 192,
         "ControlNet - Depth": 176,
         "ControlNet - HED": 2,
         "ControlNet - MLSD": 1,
         "ControlNet - Normal": 6,
         "ControlNet - Pose": 525,
         "ControlNet - Scribble": 48,
         "ControlNet - Seg": 21,
-        "Counterfeit": 451366,
-        "Cyberpunk Anime Diffusion": 19234,
-        "CyriousMix": 65087,
-        "DGSpitzer Art Diffusion": 4199,
-        "Dan Mumford Style": 4968,
-        "Dark Victorian Diffusion": 9444,
-        "Darkest Diffusion": 29349,
-        "Deliberate": 3667871,
-        "Disco Elysium": 2467,
-        "DnD Item": 6870,
-        "Double Exposure Diffusion": 5190,
-        "DreamLikeSamKuvshinov": 9916,
-        "Dreamlike Diffusion": 61130,
-        "Dreamlike Photoreal": 183066,
-        "Dreamshaper": 284399,
-        "DucHaiten": 22377,
-        "DucHaiten Classic Anime": 8738,
-        "Dungeons and Diffusion": 23395,
-        "Dungeons n Waifus": 19613,
-        "Eimis Anime Diffusion": 78564,
-        "Elden Ring Diffusion": 20127,
-        "Elldreth's Lucid Mix": 15903,
-        "Elldreths Retro Mix": 7193,
-        "Epic Diffusion": 275496,
-        "Eternos": 2962,
-        "ExpMix Line": 55321,
-        "Experience": 55050,
-        "FKing SciFi": 5213,
-        "FaeTastic": 45979,
-        "Fantasy Card Diffusion": 13770,
-        "Funko Diffusion": 5350,
-        "Furry Epoch": 27019,
-        "Future Diffusion": 6279,
-        "GTA5 Artwork Diffusion": 31221,
+        "Counterfeit": 1306099,
+        "CyberRealistic": 56212,
+        "Cyberpunk Anime Diffusion": 39522,
+        "CyriousMix": 154713,
+        "DGSpitzer Art Diffusion": 7850,
+        "Dan Mumford Style": 11199,
+        "Dark Sushi Mix": 13679,
+        "Dark Victorian Diffusion": 18668,
+        "Darkest Diffusion": 35658,
+        "Deliberate": 13190062,
+        "Deliberate Inpainting": 10949,
+        "Disco Elysium": 7509,
+        "Disney Pixar Cartoon Type A": 6995,
+        "DnD Item": 12224,
+        "DnD Map Generator": 2080,
+        "Double Exposure Diffusion": 9043,
+        "DreamLikeSamKuvshinov": 19404,
+        "DreamShaper Inpainting": 2197,
+        "Dreamlike Diffusion": 110583,
+        "Dreamlike Photoreal": 355132,
+        "Dreamshaper": 1940858,
+        "DucHaiten": 50849,
+        "DucHaiten Classic Anime": 18727,
+        "Dungeons and Diffusion": 43338,
+        "Dungeons n Waifus": 70012,
+        "Edge Of Realism": 39653,
+        "Eimis Anime Diffusion": 180826,
+        "Elden Ring Diffusion": 34324,
+        "Elldreth's Lucid Mix": 25327,
+        "Elldreths Retro Mix": 14756,
+        "Elysium Anime": 7243,
+        "Epic Diffusion": 872778,
+        "Epic Diffusion Inpainting": 1244,
+        "Eternos": 6344,
+        "Ether Real Mix": 7745,
+        "ExpMix Line": 94508,
+        "Experience": 126451,
+        "FKing SciFi": 11715,
+        "FaeTastic": 165315,
+        "Fantasy Card Diffusion": 25233,
+        "Fluffusion": 33057,
+        "Funko Diffusion": 10252,
+        "Furry Epoch": 52902,
+        "Future Diffusion": 14444,
+        "GTA5 Artwork Diffusion": 59243,
         "GTM Ultimate Blend": 20022,
-        "Ghibli Diffusion": 8260,
-        "GorynichMix": 26071,
-        "Grapefruit Hentai": 161508,
-        "Graphic-Art": 5343,
-        "GuoFeng": 16369,
-        "Guohua Diffusion": 5919,
-        "HASDX": 39056,
-        "HRL": 14403,
-        "Hassanblend": 69955,
-        "Healy's Anime Blend": 16388,
-        "Hentai Diffusion": 758158,
-        "Illuminati Diffusion": 28235,
-        "Inkpunk Diffusion": 25160,
-        "JWST Deep Space Diffusion": 7445,
-        "Jim Eidomode": 5862,
-        "Kenshi": 61021,
-        "Knollingcase": 4773,
-        "Korestyle": 3912,
-        "Laolei New Berry Protogen Mix": 19472,
-        "Lawlas's yiff mix": 229340,
-        "Liberty": 148398,
-        "Marvel Diffusion": 4110,
-        "Mega Merge Diffusion": 7296,
-        "Microcasing": 3161,
-        "Microchars": 6256,
-        "Microcritters": 3161,
-        "Microscopic": 2898,
-        "Microworlds": 8602,
-        "Midjourney Diffusion": 312230,
-        "Midjourney PaintArt": 69336,
-        "Min Illust Background": 4030,
-        "ModernArt Diffusion": 4587,
-        "Moedel": 6724,
-        "MoistMix": 40330,
-        "Movie Diffusion": 8914,
-        "NeverEnding Dream": 74372,
-        "Nitro Diffusion": 6245,
+        "Galena Redux": 10839,
+        "Ghibli Diffusion": 16078,
+        "GhostMix": 7631,
+        "GorynichMix": 56429,
+        "Grapefruit Hentai": 422749,
+        "Graphic-Art": 10428,
+        "GuFeng": 2815,
+        "GuoFeng": 109690,
+        "Guohua Diffusion": 11983,
+        "HASDX": 56737,
+        "HRL": 33816,
+        "Hassaku": 19881,
+        "Hassanblend": 189094,
+        "Healy's Anime Blend": 31833,
+        "Henmix Real": 14274,
+        "Hentai Diffusion": 1771603,
+        "ICBINP - I Can't Believe It's Not Photography": 847343,
+        "Illuminati Diffusion": 62480,
+        "Inkpunk Diffusion": 56640,
+        "JWST Deep Space Diffusion": 13062,
+        "Jim Eidomode": 26285,
+        "JoMad Diffusion": 2011,
+        "Kenshi": 75510,
+        "Knollingcase": 11100,
+        "Korestyle": 10666,
+        "Laolei New Berry Protogen Mix": 40175,
+        "Lawlas's yiff mix": 553737,
+        "Liberty": 308145,
+        "Lyriel": 45940,
+        "Marvel Diffusion": 8860,
+        "Mega Merge Diffusion": 15065,
+        "MeinaMix": 16360,
+        "Microcasing": 5768,
+        "Microchars": 12688,
+        "Microcritters": 5853,
+        "Microscopic": 5521,
+        "Microworlds": 17469,
+        "Midjourney Diffusion": 448616,
+        "Midjourney PaintArt": 93500,
+        "Min Illust Background": 7454,
+        "Mistoon Amethyst": 14131,
+        "ModernArt Diffusion": 10548,
+        "Moedel": 12249,
+        "MoistMix": 54594,
+        "MoonMix Fantasy": 19434,
+        "Movie Diffusion": 21900,
+        "Neurogen": 18198,
+        "NeverEnding Dream": 128042,
+        "Nitro Diffusion": 18483,
         "Open Journey Beta": 2797,
-        "Openniji": 53331,
-        "OrbAI": 1705,
-        "PFG": 36170,
-        "PIXHELL": 960,
-        "PPP": 29400,
-        "PRMJ": 4567,
-        "PVC": 992,
-        "Papercut Diffusion": 8782,
-        "Papercutcraft": 8171,
-        "Pastel Mix": 69063,
-        "Perfect World": 17117,
-        "Poison": 54120,
-        "Pokemon3D": 3619,
-        "PortraitPlus": 43778,
-        "Pretty 2.5D": 70488,
-        "Project Unreal Engine 5": 400939,
-        "ProtoGen": 44300,
-        "Protogen Anime": 9573,
-        "Protogen Infinity": 75488,
-        "Pulp Vector Art": 4156,
-        "RCNZ Dumb Monkey": 4633,
-        "RCNZ Gorilla With A Brick": 5482,
-        "RPG": 25281,
-        "Rachel Walker Watercolors": 5254,
-        "Rainbowpatch": 3962,
-        "Ranma Diffusion": 23770,
-        "RealBiter": 23136,
-        "Realism Engine": 26505,
-        "Realistic Vision": 547467,
-        "Redshift Diffusion": 51475,
-        "Rev Animated": 177622,
-        "Robo-Diffusion": 6145,
-        "Rodent Diffusion": 6038,
-        "SD-Silicon": 29673,
-        "Samdoesarts Ultmerge": 17269,
-        "Sci-Fi Diffusion": 8301,
-        "Seek.art MEGA": 27239,
-        "Smoke Diffusion": 3497,
-        "Something": 30352,
-        "Sonic Diffusion": 6872,
-        "Spider-Verse Diffusion": 3339,
-        "Squishmallow Diffusion": 3005,
+        "OpenJourney Diffusion": 10364,
+        "Openniji": 90732,
+        "OrbAI": 4405,
+        "PFG": 62901,
+        "PIXHELL": 5487,
+        "PPP": 51462,
+        "PRMJ": 9581,
+        "PVC": 5182,
+        "Papercut Diffusion": 18545,
+        "Papercutcraft": 12217,
+        "Pastel Mix": 146404,
+        "Perfect World": 92399,
+        "Poison": 104065,
+        "Pokemon3D": 9119,
+        "PortraitPlus": 73365,
+        "Pretty 2.5D": 432373,
+        "Project Unreal Engine 5": 1249740,
+        "ProtoGen": 98235,
+        "Protogen Anime": 18054,
+        "Protogen Infinity": 141969,
+        "Pulp Vector Art": 7228,
+        "RCNZ Dumb Monkey": 19625,
+        "RCNZ Gorilla With A Brick": 55146,
+        "RPG": 63561,
+        "Rachel Walker Watercolors": 9969,
+        "Rainbowpatch": 7860,
+        "Ranma Diffusion": 37478,
+        "Real Dos Mix": 2732,
+        "RealBiter": 103969,
+        "Realisian": 12751,
+        "Realism Engine": 94607,
+        "Realistic Vision": 1593637,
+        "Realistic Vision Inpainting": 9437,
+        "Redshift Diffusion": 85606,
+        "Reliberate": 19211,
+        "Rev Animated": 432914,
+        "Robo-Diffusion": 12451,
+        "Rodent Diffusion": 17026,
+        "SD-Silicon": 42091,
+        "Samaritan 3d Cartoon": 3264,
+        "Samdoesarts Ultmerge": 23397,
+        "Sci-Fi Diffusion": 14556,
+        "Seek.art MEGA": 43279,
+        "Smoke Diffusion": 6930,
+        "Something": 94538,
+        "Sonic Diffusion": 14817,
+        "Spider-Verse Diffusion": 7488,
+        "Squishmallow Diffusion": 5660,
         "Stable Diffusion 2 Depth": 1168,
-        "Supermarionation": 2668,
-        "Sygil-Dev Diffusion": 4143,
-        "Synthwave": 7708,
-        "SynthwavePunk": 2673,
-        "T-Shirt Diffusion": 5938,
-        "T-Shirt Print Designs": 6915,
-        "TrexMix": 3093,
-        "Trinart Characters": 13906,
-        "Tron Legacy Diffusion": 4124,
-        "UMI Olympus": 10052,
-        "URPM": 481273,
-        "Uhmami": 9246,
-        "Ultraskin": 8080,
-        "Unstable Ink Dream": 9521,
-        "Valorant Diffusion": 10121,
-        "Van Gogh Diffusion": 5079,
-        "Vector Art": 6256,
-        "VinteProtogenMix": 14474,
-        "Vintedois Diffusion": 31009,
-        "Vivid Watercolors": 6479,
-        "Voxel Art Diffusion": 3974,
+        "Supermarionation": 6075,
+        "SweetBoys 2D": 3246,
+        "Sygil-Dev Diffusion": 8014,
+        "Synthwave": 13774,
+        "SynthwavePunk": 6656,
+        "T-Shirt Diffusion": 10962,
+        "T-Shirt Print Designs": 12540,
+        "ToonYou": 7310,
+        "TrexMix": 12501,
+        "Trinart Characters": 27113,
+        "Tron Legacy Diffusion": 8103,
+        "UMI Olympus": 21460,
+        "URPM": 1298279,
+        "Uhmami": 37681,
+        "Ultraskin": 17914,
+        "Unstable Ink Dream": 18729,
+        "Valorant Diffusion": 17416,
+        "Van Gogh Diffusion": 8352,
+        "Vector Art": 11198,
+        "VinteProtogenMix": 22071,
+        "Vintedois Diffusion": 40332,
+        "Vivid Watercolors": 13537,
+        "Voxel Art Diffusion": 6952,
         "Waifu Diffusion Beta": 5639,
-        "Wavyfusion": 4490,
-        "Woop-Woop Photo": 57546,
-        "Xynthii-Diffusion": 3190,
-        "Yiffy": 102798,
-        "Zack3D": 17510,
-        "Zeipher Female Model": 329889,
-        "Zelda BOTW": 4377,
-        "anything_v4_inpainting": 2771,
+        "Wavyfusion": 8987,
+        "Western Animation Diffusion": 5032,
+        "Woop-Woop Photo": 220431,
+        "Xynthii-Diffusion": 5799,
+        "Yiffy": 196379,
+        "Zack3D": 36901,
+        "Zeipher Female Model": 627923,
+        "Zelda BOTW": 8831,
+        "anything_v4_inpainting": 23724,
         "colorbook": 7730,
-        "dreamlike_diffusion_inpainting": 999,
-        "iCoMix": 51140,
-        "kurzgesagt": 4638,
-        "mo-di-diffusion": 27105,
-        "pix2pix": 5828,
-        "stable_diffusion": 2756847,
+        "dreamlike_diffusion_inpainting": 12238,
+        "horde_special::stability.ai#6901": 935,
+        "iCoMix": 278673,
+        "iCoMix Inpainting": 2176,
+        "kurzgesagt": 8214,
+        "majicMIX realistic": 163432,
+        "mo-di-diffusion": 45725,
+        "pix2pix": 8129,
+        "stable_diffusion": 6821016,
         "stable_diffusion_1.4": 2526,
         "stable_diffusion_2.0": 3313,
         "stable_diffusion_2.0_512": 870,
-        "stable_diffusion_2.1": 122923,
+        "stable_diffusion_2.1": 405612,
         "stable_diffusion_2.1_512": 2048,
-        "stable_diffusion_2_inpainting": 1174,
-        "stable_diffusion_inpainting": 36649,
-        "trinart": 13070,
-        "vectorartz": 5130,
-        "waifu_diffusion": 334479
+        "stable_diffusion_2_inpainting": 7352,
+        "stable_diffusion_inpainting": 77383,
+        "trinart": 19891,
+        "vectorartz": 9607,
+        "waifu_diffusion": 568785
     }
 }
```

### Comparing `horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json` & `horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json` & `horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/tests/test_data/ratings_api/example_responses/UserValidateResponse.json` & `horde_sdk-0.4.0/tests/test_data/ratings_api/example_responses/UserValidateResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/tests/test_data/swagger.json` & `horde_sdk-0.4.0/tests/test_data/ai_horde_api/swagger.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.3/tests/test_ratings_api_models.py` & `horde_sdk-0.4.0/tests/test_ratings_api_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """Unit tests for Ratings API models."""
 
 
-import horde_sdk.generic_api as generic_api
-import horde_sdk.ratings_api as ratings_api
 import pydantic
 import pytest
 
+from horde_sdk.generic_api.metadata import GenericAcceptTypes
+from horde_sdk.ratings_api.apimodels import UserCheckRequest
+
 
 class Test_validators:
     """If you are unfamiliar with pydantic, this may demonstrates some of the validation functionality."""
 
     def test_user_check_request(self) -> None:
         """Shows some of the types of data expected."""
         with pytest.raises(pydantic.ValidationError, match=r".*user_id.*"):
-            ratings_api.UserCheckRequest(
+            UserCheckRequest(
                 apikey="key",
-                accept=generic_api.GenericAcceptTypes.json,
+                accept=GenericAcceptTypes.json,
                 user_id="non_numeric_userid",
                 divergence=3,
                 minutes=180,
             )
         with pytest.raises(pydantic.ValidationError, match=r".*divergence.*"):
-            ratings_api.UserCheckRequest(
+            UserCheckRequest(
                 apikey="key",
-                accept=generic_api.GenericAcceptTypes.json,
+                accept=GenericAcceptTypes.json,
                 user_id="123",
                 divergence=-1,
                 minutes=180,
             )
         with pytest.raises(pydantic.ValidationError, match=r".*user_id.*"):
-            ratings_api.UserCheckRequest(
+            UserCheckRequest(
                 apikey="key",
-                accept=generic_api.GenericAcceptTypes.json,
+                accept=GenericAcceptTypes.json,
                 user_id="non_numeric_userid",  # user_id has to be a str with only numbers
                 divergence=3,
                 minutes=180,
             )
-            ratings_api.UserCheckRequest(
+            UserCheckRequest(
                 apikey="key",
                 accept="non-enum_accept_value",  # type: ignore
                 user_id="123",
                 divergence=3,
                 minutes=180,
             )
```

