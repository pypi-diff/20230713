# Comparing `tmp/mypy-boto3-personalize-1.28.0.tar.gz` & `tmp/mypy-boto3-personalize-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-1.28.0.tar", last modified: Thu Jul  6 21:00:18 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
```

## Comparing `mypy-boto3-personalize-1.28.0.tar` & `mypy-boto3-personalize-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.566392 mypy-boto3-personalize-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:08.000000 mypy-boto3-personalize-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23642 2023-07-06 21:00:18.558392 mypy-boto3-personalize-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22141 2023-07-06 20:49:08.000000 mypy-boto3-personalize-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.546392 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-06 20:49:08.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-06 20:49:08.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50910 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:09.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62638 2023-07-06 20:49:11.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62603 2023-07-06 20:49:10.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:08.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.558392 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23642 2023-07-06 21:00:18.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 21:00:18.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:18.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 21:00:18.000000 mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:18.566392 mypy-boto3-personalize-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:49:08.000000 mypy-boto3-personalize-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.177303 mypy-boto3-personalize-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-13 19:49:15.173303 mypy-boto3-personalize-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.169303 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51525 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51435 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-13 19:48:20.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62479 2023-07-13 19:48:22.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62446 2023-07-13 19:48:21.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.173303 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:49:15.000000 mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.177303 mypy-boto3-personalize-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-13 19:48:19.000000 mypy-boto3-personalize-1.28.3/setup.py
```

### Comparing `mypy-boto3-personalize-1.28.0/LICENSE` & `mypy-boto3-personalize-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/PKG-INFO` & `mypy-boto3-personalize-1.28.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.28.0
-Summary: Type annotations for boto3.Personalize 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,15 +425,15 @@
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
     DatasetSummaryTypeDef,
-    DatasetTypeDef,
+    DatasetUpdateSummaryTypeDef,
     DefaultCategoricalHyperParameterRangeTypeDef,
     DefaultContinuousHyperParameterRangeTypeDef,
     DefaultIntegerHyperParameterRangeTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
@@ -516,14 +516,16 @@
     StartRecommenderRequestRequestTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
     StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
@@ -547,15 +549,15 @@
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeSchemaResponseTypeDef,
     ListDatasetsResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
+    DatasetTypeDef,
     DefaultHyperParameterRangesTypeDef,
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
@@ -572,14 +574,15 @@
     CreateDatasetExportJobRequestRequestTypeDef,
     DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
     MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
     CampaignTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
     AlgorithmTypeDef,
     HPOConfigTypeDef,
     CreateRecommenderRequestRequestTypeDef,
     RecommenderSummaryTypeDef,
     RecommenderUpdateSummaryTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
```

### Comparing `mypy-boto3-personalize-1.28.0/README.md` & `mypy-boto3-personalize-1.28.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,15 +393,15 @@
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
     DatasetSummaryTypeDef,
-    DatasetTypeDef,
+    DatasetUpdateSummaryTypeDef,
     DefaultCategoricalHyperParameterRangeTypeDef,
     DefaultContinuousHyperParameterRangeTypeDef,
     DefaultIntegerHyperParameterRangeTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
@@ -484,14 +484,16 @@
     StartRecommenderRequestRequestTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
     StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
@@ -515,15 +517,15 @@
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeSchemaResponseTypeDef,
     ListDatasetsResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
+    DatasetTypeDef,
     DefaultHyperParameterRangesTypeDef,
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
@@ -540,14 +542,15 @@
     CreateDatasetExportJobRequestRequestTypeDef,
     DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
     MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
     CampaignTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
     AlgorithmTypeDef,
     HPOConfigTypeDef,
     CreateRecommenderRequestRequestTypeDef,
     RecommenderSummaryTypeDef,
     RecommenderUpdateSummaryTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/__init__.py` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/__init__.pyi` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/__main__.py` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Personalize 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/client.py` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     MetricAttributionOutputTypeDef,
     RecommenderConfigTypeDef,
     SolutionConfigTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderResponseTypeDef,
     TagTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -887,14 +888,22 @@
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
 
+    def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
+        """
+        Update a dataset to replace its schema with a new or existing one.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_dataset)
+        """
+
     def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/client.pyi` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     MetricAttributionOutputTypeDef,
     RecommenderConfigTypeDef,
     SolutionConfigTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderResponseTypeDef,
     TagTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -815,14 +816,21 @@
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
+    def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
+        """
+        Update a dataset to replace its schema with a new or existing one.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_dataset)
+        """
     def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/literals.py` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/literals.pyi` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/paginator.py` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/paginator.pyi` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/type_defs.py` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
-    "DatasetTypeDef",
+    "DatasetUpdateSummaryTypeDef",
     "DefaultCategoricalHyperParameterRangeTypeDef",
     "DefaultContinuousHyperParameterRangeTypeDef",
     "DefaultIntegerHyperParameterRangeTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
@@ -157,14 +157,16 @@
     "StartRecommenderRequestRequestTypeDef",
     "StartRecommenderResponseTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopRecommenderResponseTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignResponseTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
+    "UpdateDatasetResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
@@ -188,15 +190,15 @@
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
-    "DescribeDatasetResponseTypeDef",
+    "DatasetTypeDef",
     "DefaultHyperParameterRangesTypeDef",
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ListFiltersResponseTypeDef",
@@ -213,14 +215,15 @@
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
+    "DescribeDatasetResponseTypeDef",
     "AlgorithmTypeDef",
     "HPOConfigTypeDef",
     "CreateRecommenderRequestRequestTypeDef",
     "RecommenderSummaryTypeDef",
     "RecommenderUpdateSummaryTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
@@ -236,48 +239,36 @@
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
     "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
-_RequiredAlgorithmImageTypeDef = TypedDict(
-    "_RequiredAlgorithmImageTypeDef",
-    {
-        "dockerURI": str,
-    },
-)
-_OptionalAlgorithmImageTypeDef = TypedDict(
-    "_OptionalAlgorithmImageTypeDef",
+AlgorithmImageTypeDef = TypedDict(
+    "AlgorithmImageTypeDef",
     {
         "name": str,
+        "dockerURI": str,
     },
-    total=False,
 )
 
-
-class AlgorithmImageTypeDef(_RequiredAlgorithmImageTypeDef, _OptionalAlgorithmImageTypeDef):
-    pass
-
-
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
 )
 
 AutoMLResultTypeDef = TypedDict(
     "AutoMLResultTypeDef",
     {
         "bestRecipeArn": str,
     },
-    total=False,
 )
 
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
@@ -310,29 +301,27 @@
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
-    total=False,
 )
 
 BatchSegmentJobSummaryTypeDef = TypedDict(
     "BatchSegmentJobSummaryTypeDef",
     {
         "batchSegmentJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
-    total=False,
 )
 
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
@@ -345,15 +334,14 @@
         "name": str,
         "campaignArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": Sequence[str],
@@ -538,29 +526,27 @@
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetGroupTypeDef = TypedDict(
     "DatasetGroupTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
@@ -568,114 +554,102 @@
         "roleArn": str,
         "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "datasetImportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
     },
-    total=False,
 )
 
 DatasetSchemaSummaryTypeDef = TypedDict(
     "DatasetSchemaSummaryTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetSchemaTypeDef = TypedDict(
     "DatasetSchemaTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "schema": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "name": str,
         "datasetArn": str,
         "datasetType": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
+DatasetUpdateSummaryTypeDef = TypedDict(
+    "DatasetUpdateSummaryTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
         "schemaArn": str,
         "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
     "DefaultCategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": List[str],
         "isTunable": bool,
     },
-    total=False,
 )
 
 DefaultContinuousHyperParameterRangeTypeDef = TypedDict(
     "DefaultContinuousHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
         "isTunable": bool,
     },
-    total=False,
 )
 
 DefaultIntegerHyperParameterRangeTypeDef = TypedDict(
     "DefaultIntegerHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
         "isTunable": bool,
     },
-    total=False,
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
@@ -808,15 +782,14 @@
         "accountId": str,
         "trackingId": str,
         "datasetGroupArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DescribeFeatureTransformationRequestRequestTypeDef = TypedDict(
     "DescribeFeatureTransformationRequestRequestTypeDef",
     {
         "featureTransformationArn": str,
     },
@@ -828,15 +801,14 @@
         "name": str,
         "featureTransformationArn": str,
         "defaultParameters": Dict[str, str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
     },
-    total=False,
 )
 
 DescribeFilterRequestRequestTypeDef = TypedDict(
     "DescribeFilterRequestRequestTypeDef",
     {
         "filterArn": str,
     },
@@ -850,15 +822,14 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
         "filterExpression": str,
         "status": str,
     },
-    total=False,
 )
 
 DescribeMetricAttributionRequestRequestTypeDef = TypedDict(
     "DescribeMetricAttributionRequestRequestTypeDef",
     {
         "metricAttributionArn": str,
     },
@@ -880,15 +851,14 @@
         "featureTransformationArn": str,
         "status": str,
         "description": str,
         "creationDateTime": datetime,
         "recipeType": str,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DescribeRecommenderRequestRequestTypeDef = TypedDict(
     "DescribeRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
@@ -927,29 +897,27 @@
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 FilterSummaryTypeDef = TypedDict(
     "FilterSummaryTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
         "status": str,
     },
-    total=False,
 )
 
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
@@ -1206,15 +1174,14 @@
         "name": str,
         "metricAttributionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "recipeProvider": Literal["SERVICE"],
         "domain": DomainType,
@@ -1240,15 +1207,14 @@
         "name": str,
         "recipeArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
-    total=False,
 )
 
 ListRecommendersRequestListRecommendersPaginateTypeDef = TypedDict(
     "ListRecommendersRequestListRecommendersPaginateTypeDef",
     {
         "datasetGroupArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1307,15 +1273,14 @@
     {
         "solutionVersionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 ListSolutionsRequestListSolutionsPaginateTypeDef = TypedDict(
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     {
         "datasetGroupArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1339,15 +1304,14 @@
         "name": str,
         "solutionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recipeArn": str,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -1392,15 +1356,14 @@
 )
 
 TunedHPOParamsTypeDef = TypedDict(
     "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
-    total=False,
 )
 
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
@@ -1448,14 +1411,30 @@
     "UpdateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UpdateDatasetRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetRequestRequestTypeDef",
+    {
+        "datasetArn": str,
+        "schemaArn": str,
+    },
+)
+
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "datasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateMetricAttributionResponseTypeDef = TypedDict(
     "UpdateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1549,15 +1528,14 @@
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredUpdateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
@@ -1785,15 +1763,14 @@
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
-    total=False,
 )
 
 ListMetricAttributionMetricsResponseTypeDef = TypedDict(
     "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
@@ -1858,30 +1835,36 @@
     {
         "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
     {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
     },
 )
 
 DefaultHyperParameterRangesTypeDef = TypedDict(
     "DefaultHyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeTypeDef],
     },
-    total=False,
 )
 
 DescribeEventTrackerResponseTypeDef = TypedDict(
     "DescribeEventTrackerResponseTypeDef",
     {
         "eventTracker": EventTrackerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1999,15 +1982,14 @@
         "jobOutput": BatchInferenceJobOutputTypeDef,
         "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateBatchInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchInferenceJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
@@ -2047,15 +2029,14 @@
         "jobInput": BatchSegmentJobInputTypeDef,
         "jobOutput": BatchSegmentJobOutputTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateBatchSegmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchSegmentJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
@@ -2118,15 +2099,14 @@
         "roleArn": str,
         "status": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 CreateMetricAttributionRequestRequestTypeDef = TypedDict(
     "CreateMetricAttributionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
@@ -2143,15 +2123,14 @@
         "datasetGroupArn": str,
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 UpdateMetricAttributionRequestRequestTypeDef = TypedDict(
     "UpdateMetricAttributionRequestRequestTypeDef",
     {
         "addMetrics": Sequence[MetricAttributeTypeDef],
         "removeMetrics": Sequence[str],
@@ -2171,40 +2150,46 @@
         "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
     },
-    total=False,
 )
 
 DescribeDatasetImportJobResponseTypeDef = TypedDict(
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
         "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
         "defaultHyperParameterRanges": DefaultHyperParameterRangesTypeDef,
         "defaultResourceConfig": Dict[str, str],
         "trainingInputMode": str,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 HPOConfigTypeDef = TypedDict(
     "HPOConfigTypeDef",
     {
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
@@ -2245,27 +2230,25 @@
         "datasetGroupArn": str,
         "recipeArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 RecommenderUpdateSummaryTypeDef = TypedDict(
     "RecommenderUpdateSummaryTypeDef",
     {
         "recommenderConfig": RecommenderConfigTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
-    total=False,
 )
 
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
@@ -2354,15 +2337,14 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
         "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
         "modelMetrics": Dict[str, float],
     },
-    total=False,
 )
 
 _RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSolutionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
@@ -2401,15 +2383,14 @@
         "solutionConfig": SolutionConfigTypeDef,
         "autoMLResult": AutoMLResultTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestSolutionVersion": SolutionVersionSummaryTypeDef,
     },
-    total=False,
 )
 
 SolutionVersionTypeDef = TypedDict(
     "SolutionVersionTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
@@ -2424,15 +2405,14 @@
         "trainingMode": TrainingModeType,
         "tunedHPOParams": TunedHPOParamsTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize/type_defs.pyi` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
-    "DatasetTypeDef",
+    "DatasetUpdateSummaryTypeDef",
     "DefaultCategoricalHyperParameterRangeTypeDef",
     "DefaultContinuousHyperParameterRangeTypeDef",
     "DefaultIntegerHyperParameterRangeTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
@@ -156,14 +156,16 @@
     "StartRecommenderRequestRequestTypeDef",
     "StartRecommenderResponseTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopRecommenderResponseTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignResponseTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
+    "UpdateDatasetResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
@@ -187,15 +189,15 @@
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
-    "DescribeDatasetResponseTypeDef",
+    "DatasetTypeDef",
     "DefaultHyperParameterRangesTypeDef",
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ListFiltersResponseTypeDef",
@@ -212,14 +214,15 @@
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
+    "DescribeDatasetResponseTypeDef",
     "AlgorithmTypeDef",
     "HPOConfigTypeDef",
     "CreateRecommenderRequestRequestTypeDef",
     "RecommenderSummaryTypeDef",
     "RecommenderUpdateSummaryTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
@@ -235,46 +238,36 @@
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
     "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
-_RequiredAlgorithmImageTypeDef = TypedDict(
-    "_RequiredAlgorithmImageTypeDef",
-    {
-        "dockerURI": str,
-    },
-)
-_OptionalAlgorithmImageTypeDef = TypedDict(
-    "_OptionalAlgorithmImageTypeDef",
+AlgorithmImageTypeDef = TypedDict(
+    "AlgorithmImageTypeDef",
     {
         "name": str,
+        "dockerURI": str,
     },
-    total=False,
 )
 
-class AlgorithmImageTypeDef(_RequiredAlgorithmImageTypeDef, _OptionalAlgorithmImageTypeDef):
-    pass
-
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
 )
 
 AutoMLResultTypeDef = TypedDict(
     "AutoMLResultTypeDef",
     {
         "bestRecipeArn": str,
     },
-    total=False,
 )
 
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
@@ -305,29 +298,27 @@
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
-    total=False,
 )
 
 BatchSegmentJobSummaryTypeDef = TypedDict(
     "BatchSegmentJobSummaryTypeDef",
     {
         "batchSegmentJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
-    total=False,
 )
 
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
@@ -340,15 +331,14 @@
         "name": str,
         "campaignArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": Sequence[str],
@@ -531,29 +521,27 @@
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetGroupTypeDef = TypedDict(
     "DatasetGroupTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
@@ -561,114 +549,102 @@
         "roleArn": str,
         "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "datasetImportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
     },
-    total=False,
 )
 
 DatasetSchemaSummaryTypeDef = TypedDict(
     "DatasetSchemaSummaryTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetSchemaTypeDef = TypedDict(
     "DatasetSchemaTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "schema": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
-    total=False,
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "name": str,
         "datasetArn": str,
         "datasetType": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
+DatasetUpdateSummaryTypeDef = TypedDict(
+    "DatasetUpdateSummaryTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
         "schemaArn": str,
         "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
     "DefaultCategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": List[str],
         "isTunable": bool,
     },
-    total=False,
 )
 
 DefaultContinuousHyperParameterRangeTypeDef = TypedDict(
     "DefaultContinuousHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
         "isTunable": bool,
     },
-    total=False,
 )
 
 DefaultIntegerHyperParameterRangeTypeDef = TypedDict(
     "DefaultIntegerHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
         "isTunable": bool,
     },
-    total=False,
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
@@ -801,15 +777,14 @@
         "accountId": str,
         "trackingId": str,
         "datasetGroupArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DescribeFeatureTransformationRequestRequestTypeDef = TypedDict(
     "DescribeFeatureTransformationRequestRequestTypeDef",
     {
         "featureTransformationArn": str,
     },
@@ -821,15 +796,14 @@
         "name": str,
         "featureTransformationArn": str,
         "defaultParameters": Dict[str, str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
     },
-    total=False,
 )
 
 DescribeFilterRequestRequestTypeDef = TypedDict(
     "DescribeFilterRequestRequestTypeDef",
     {
         "filterArn": str,
     },
@@ -843,15 +817,14 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
         "filterExpression": str,
         "status": str,
     },
-    total=False,
 )
 
 DescribeMetricAttributionRequestRequestTypeDef = TypedDict(
     "DescribeMetricAttributionRequestRequestTypeDef",
     {
         "metricAttributionArn": str,
     },
@@ -873,15 +846,14 @@
         "featureTransformationArn": str,
         "status": str,
         "description": str,
         "creationDateTime": datetime,
         "recipeType": str,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DescribeRecommenderRequestRequestTypeDef = TypedDict(
     "DescribeRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
@@ -920,29 +892,27 @@
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 FilterSummaryTypeDef = TypedDict(
     "FilterSummaryTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
         "status": str,
     },
-    total=False,
 )
 
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
@@ -1199,15 +1169,14 @@
         "name": str,
         "metricAttributionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "recipeProvider": Literal["SERVICE"],
         "domain": DomainType,
@@ -1233,15 +1202,14 @@
         "name": str,
         "recipeArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
-    total=False,
 )
 
 ListRecommendersRequestListRecommendersPaginateTypeDef = TypedDict(
     "ListRecommendersRequestListRecommendersPaginateTypeDef",
     {
         "datasetGroupArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1300,15 +1268,14 @@
     {
         "solutionVersionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 ListSolutionsRequestListSolutionsPaginateTypeDef = TypedDict(
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     {
         "datasetGroupArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1332,15 +1299,14 @@
         "name": str,
         "solutionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recipeArn": str,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -1385,15 +1351,14 @@
 )
 
 TunedHPOParamsTypeDef = TypedDict(
     "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
-    total=False,
 )
 
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
@@ -1441,14 +1406,30 @@
     "UpdateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UpdateDatasetRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetRequestRequestTypeDef",
+    {
+        "datasetArn": str,
+        "schemaArn": str,
+    },
+)
+
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "datasetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateMetricAttributionResponseTypeDef = TypedDict(
     "UpdateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1540,15 +1521,14 @@
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredUpdateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
@@ -1760,15 +1740,14 @@
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
-    total=False,
 )
 
 ListMetricAttributionMetricsResponseTypeDef = TypedDict(
     "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
@@ -1833,30 +1812,36 @@
     {
         "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
     {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
     },
 )
 
 DefaultHyperParameterRangesTypeDef = TypedDict(
     "DefaultHyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeTypeDef],
     },
-    total=False,
 )
 
 DescribeEventTrackerResponseTypeDef = TypedDict(
     "DescribeEventTrackerResponseTypeDef",
     {
         "eventTracker": EventTrackerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1974,15 +1959,14 @@
         "jobOutput": BatchInferenceJobOutputTypeDef,
         "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateBatchInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchInferenceJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
@@ -2020,15 +2004,14 @@
         "jobInput": BatchSegmentJobInputTypeDef,
         "jobOutput": BatchSegmentJobOutputTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateBatchSegmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchSegmentJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
@@ -2087,15 +2070,14 @@
         "roleArn": str,
         "status": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 CreateMetricAttributionRequestRequestTypeDef = TypedDict(
     "CreateMetricAttributionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
@@ -2112,15 +2094,14 @@
         "datasetGroupArn": str,
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
-    total=False,
 )
 
 UpdateMetricAttributionRequestRequestTypeDef = TypedDict(
     "UpdateMetricAttributionRequestRequestTypeDef",
     {
         "addMetrics": Sequence[MetricAttributeTypeDef],
         "removeMetrics": Sequence[str],
@@ -2140,40 +2121,46 @@
         "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
     },
-    total=False,
 )
 
 DescribeDatasetImportJobResponseTypeDef = TypedDict(
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
         "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
         "defaultHyperParameterRanges": DefaultHyperParameterRangesTypeDef,
         "defaultResourceConfig": Dict[str, str],
         "trainingInputMode": str,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 HPOConfigTypeDef = TypedDict(
     "HPOConfigTypeDef",
     {
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
@@ -2212,27 +2199,25 @@
         "datasetGroupArn": str,
         "recipeArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 RecommenderUpdateSummaryTypeDef = TypedDict(
     "RecommenderUpdateSummaryTypeDef",
     {
         "recommenderConfig": RecommenderConfigTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
-    total=False,
 )
 
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
@@ -2321,15 +2306,14 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
         "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
         "modelMetrics": Dict[str, float],
     },
-    total=False,
 )
 
 _RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSolutionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
@@ -2366,15 +2350,14 @@
         "solutionConfig": SolutionConfigTypeDef,
         "autoMLResult": AutoMLResultTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestSolutionVersion": SolutionVersionSummaryTypeDef,
     },
-    total=False,
 )
 
 SolutionVersionTypeDef = TypedDict(
     "SolutionVersionTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
@@ -2389,15 +2372,14 @@
         "trainingMode": TrainingModeType,
         "tunedHPOParams": TunedHPOParamsTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.28.0
-Summary: Type annotations for boto3.Personalize 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,15 +425,15 @@
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
     DatasetSummaryTypeDef,
-    DatasetTypeDef,
+    DatasetUpdateSummaryTypeDef,
     DefaultCategoricalHyperParameterRangeTypeDef,
     DefaultContinuousHyperParameterRangeTypeDef,
     DefaultIntegerHyperParameterRangeTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
@@ -516,14 +516,16 @@
     StartRecommenderRequestRequestTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
     StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
@@ -547,15 +549,15 @@
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeSchemaResponseTypeDef,
     ListDatasetsResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
+    DatasetTypeDef,
     DefaultHyperParameterRangesTypeDef,
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
@@ -572,14 +574,15 @@
     CreateDatasetExportJobRequestRequestTypeDef,
     DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
     MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
     CampaignTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
     AlgorithmTypeDef,
     HPOConfigTypeDef,
     CreateRecommenderRequestRequestTypeDef,
     RecommenderSummaryTypeDef,
     RecommenderUpdateSummaryTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
```

### Comparing `mypy-boto3-personalize-1.28.0/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy-boto3-personalize-1.28.3/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.0/setup.py` & `mypy-boto3-personalize-1.28.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Personalize 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder"
+        " 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

