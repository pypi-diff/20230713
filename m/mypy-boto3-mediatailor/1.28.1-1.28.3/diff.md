# Comparing `tmp/mypy-boto3-mediatailor-1.28.1.tar.gz` & `tmp/mypy-boto3-mediatailor-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediatailor-1.28.1.tar", last modified: Fri Jul  7 19:32:38 2023, max compression
+gzip compressed data, was "mypy-boto3-mediatailor-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
```

## Comparing `mypy-boto3-mediatailor-1.28.1.tar` & `mypy-boto3-mediatailor-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-mediatailor-1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19349 2023-07-07 19:32:38.903385 mypy-boto3-mediatailor-1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33557 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33498 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-07 19:32:28.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-07 19:32:28.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52134 2023-07-07 19:32:29.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52069 2023-07-07 19:32:28.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19349 2023-07-07 19:32:38.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-07 19:32:38.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 19:32:38.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 19:32:38.000000 mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:32:38.903385 mypy-boto3-mediatailor-1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-07 19:32:27.000000 mypy-boto3-mediatailor-1.28.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.205304 mypy-boto3-mediatailor-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-13 19:49:15.201304 mypy-boto3-mediatailor-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33557 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33498 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:17.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-07-13 19:48:19.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50428 2023-07-13 19:48:18.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.201304 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:49:15.000000 mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.205304 mypy-boto3-mediatailor-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-13 19:48:16.000000 mypy-boto3-mediatailor-1.28.3/setup.py
```

### Comparing `mypy-boto3-mediatailor-1.28.1/LICENSE` & `mypy-boto3-mediatailor-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.1/PKG-INFO` & `mypy-boto3-mediatailor-1.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.28.1
-Summary: Type annotations for boto3.MediaTailor 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediatailor?color=blue)](https://pypistats.org/packages/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
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
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,14 +322,15 @@
 `mypy_boto3_mediatailor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_mediatailor.literals import (
     AccessTypeType,
     AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     GetChannelSchedulePaginatorName,
     ListAlertsPaginatorName,
     ListChannelsPaginatorName,
     ListLiveSourcesPaginatorName,
     ListPlaybackConfigurationsPaginatorName,
@@ -376,16 +377,17 @@
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     LogConfigurationForChannelTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     HttpPackageConfigurationTypeDef,
     PrefetchRetrievalTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     DashConfigurationForPutTypeDef,
     DashConfigurationTypeDef,
@@ -399,69 +401,68 @@
     DeleteSourceLocationRequestRequestTypeDef,
     DeleteVodSourceRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
     HlsConfigurationTypeDef,
     LivePreRollConfigurationTypeDef,
     LogConfigurationTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
     HlsPlaylistSettingsTypeDef,
+    ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     ListLiveSourcesRequestRequestTypeDef,
+    ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
+    ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
+    ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
-    PrefetchConsumptionTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseTypeDef,
     ListAlertsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
     CreateLiveSourceResponseTypeDef,
     CreateVodSourceRequestRequestTypeDef,
     CreateVodSourceResponseTypeDef,
     DescribeLiveSourceResponseTypeDef,
     DescribeVodSourceResponseTypeDef,
     LiveSourceTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
     UpdateLiveSourceResponseTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
     UpdateVodSourceResponseTypeDef,
     VodSourceTypeDef,
-    GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-    ListAlertsRequestListAlertsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-    ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
-    ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-    ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
-    ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     RequestOutputItemTypeDef,
     ResponseOutputItemTypeDef,
     ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediatailor-1.28.1/README.md` & `mypy-boto3-mediatailor-1.28.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediatailor?color=blue)](https://pypistats.org/packages/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
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
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,14 +290,15 @@
 `mypy_boto3_mediatailor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_mediatailor.literals import (
     AccessTypeType,
     AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     GetChannelSchedulePaginatorName,
     ListAlertsPaginatorName,
     ListChannelsPaginatorName,
     ListLiveSourcesPaginatorName,
     ListPlaybackConfigurationsPaginatorName,
@@ -344,16 +345,17 @@
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     LogConfigurationForChannelTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     HttpPackageConfigurationTypeDef,
     PrefetchRetrievalTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     DashConfigurationForPutTypeDef,
     DashConfigurationTypeDef,
@@ -367,69 +369,68 @@
     DeleteSourceLocationRequestRequestTypeDef,
     DeleteVodSourceRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
     HlsConfigurationTypeDef,
     LivePreRollConfigurationTypeDef,
     LogConfigurationTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
     HlsPlaylistSettingsTypeDef,
+    ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     ListLiveSourcesRequestRequestTypeDef,
+    ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
+    ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
+    ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
-    PrefetchConsumptionTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseTypeDef,
     ListAlertsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
     CreateLiveSourceResponseTypeDef,
     CreateVodSourceRequestRequestTypeDef,
     CreateVodSourceResponseTypeDef,
     DescribeLiveSourceResponseTypeDef,
     DescribeVodSourceResponseTypeDef,
     LiveSourceTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
     UpdateLiveSourceResponseTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
     UpdateVodSourceResponseTypeDef,
     VodSourceTypeDef,
-    GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-    ListAlertsRequestListAlertsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-    ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
-    ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-    ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
-    ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     RequestOutputItemTypeDef,
     ResponseOutputItemTypeDef,
     ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/__init__.py` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/__init__.pyi` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/__main__.py` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaTailor 1.28.1\nVersion:         1.28.1\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaTailor 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.1")
+    print("1.28.3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/client.py` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/client.pyi` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/literals.py` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccessTypeType",
     "AdMarkupTypeType",
+    "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
     "ListAlertsPaginatorName",
     "ListChannelsPaginatorName",
     "ListLiveSourcesPaginatorName",
     "ListPlaybackConfigurationsPaginatorName",
@@ -48,14 +49,15 @@
     "PaginatorName",
     "RegionName",
 )
 
 
 AccessTypeType = Literal["S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
 AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
+AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
 ListAlertsPaginatorName = Literal["list_alerts"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListLiveSourcesPaginatorName = Literal["list_live_sources"]
 ListPlaybackConfigurationsPaginatorName = Literal["list_playback_configurations"]
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/literals.pyi` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccessTypeType",
     "AdMarkupTypeType",
+    "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
     "ListAlertsPaginatorName",
     "ListChannelsPaginatorName",
     "ListLiveSourcesPaginatorName",
     "ListPlaybackConfigurationsPaginatorName",
@@ -46,14 +47,15 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AccessTypeType = Literal["S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
 AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
+AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
 ListAlertsPaginatorName = Literal["list_alerts"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListLiveSourcesPaginatorName = Literal["list_live_sources"]
 ListPlaybackConfigurationsPaginatorName = Literal["list_playback_configurations"]
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/paginator.py` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,144 +56,134 @@
     "ListLiveSourcesPaginator",
     "ListPlaybackConfigurationsPaginator",
     "ListPrefetchSchedulesPaginator",
     "ListSourceLocationsPaginator",
     "ListVodSourcesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetChannelSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetChannelScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
-
 class ListAlertsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAlertsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
         """
 
-
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
         """
 
-
 class ListLiveSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
     """
 
     def paginate(
-        self, *, SourceLocationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLiveSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
         """
 
-
 class ListPlaybackConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlaybackConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
         """
 
-
 class ListPrefetchSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
     """
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPrefetchSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
-
 class ListSourceLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
         """
 
-
 class ListVodSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
     """
 
     def paginate(
-        self, *, SourceLocationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVodSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/paginator.pyi` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,134 +56,144 @@
     "ListLiveSourcesPaginator",
     "ListPlaybackConfigurationsPaginator",
     "ListPrefetchSchedulesPaginator",
     "ListSourceLocationsPaginator",
     "ListVodSourcesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetChannelSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetChannelScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
+
 class ListAlertsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAlertsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
         """
 
+
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
         """
 
+
 class ListLiveSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
     """
 
     def paginate(
-        self, *, SourceLocationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLiveSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
         """
 
+
 class ListPlaybackConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlaybackConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
         """
 
+
 class ListPrefetchSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
     """
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPrefetchSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
+
 class ListSourceLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
         """
 
+
 class ListVodSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
     """
 
     def paginate(
-        self, *, SourceLocationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVodSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/type_defs.py` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessTypeType,
     AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     MessageTypeType,
     ModeType,
     OriginManifestTypeType,
     PlaybackModeType,
     RelativePositionType,
@@ -50,16 +51,17 @@
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionTypeDef",
     "BumperTypeDef",
     "CdnConfigurationTypeDef",
     "LogConfigurationForChannelTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "HttpPackageConfigurationTypeDef",
     "PrefetchRetrievalTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
     "DashConfigurationForPutTypeDef",
     "DashConfigurationTypeDef",
@@ -73,69 +75,68 @@
     "DeleteSourceLocationRequestRequestTypeDef",
     "DeleteVodSourceRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeLiveSourceRequestRequestTypeDef",
     "DescribeProgramRequestRequestTypeDef",
     "DescribeSourceLocationRequestRequestTypeDef",
     "DescribeVodSourceRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetChannelPolicyResponseTypeDef",
+    "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     "GetChannelScheduleRequestRequestTypeDef",
     "GetPlaybackConfigurationRequestRequestTypeDef",
     "HlsConfigurationTypeDef",
     "LivePreRollConfigurationTypeDef",
     "LogConfigurationTypeDef",
     "GetPrefetchScheduleRequestRequestTypeDef",
     "HlsPlaylistSettingsTypeDef",
+    "ListAlertsRequestListAlertsPaginateTypeDef",
     "ListAlertsRequestRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     "ListLiveSourcesRequestRequestTypeDef",
+    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     "ListPlaybackConfigurationsRequestRequestTypeDef",
+    "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
     "ListPrefetchSchedulesRequestRequestTypeDef",
+    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListSourceLocationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "ListVodSourcesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ScheduleAdBreakTypeDef",
     "TransitionTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "PrefetchConsumptionTypeDef",
-    "ConfigureLogsForChannelResponseTypeDef",
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetChannelPolicyResponseTypeDef",
     "ListAlertsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "PrefetchConsumptionTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
     "CreateLiveSourceResponseTypeDef",
     "CreateVodSourceRequestRequestTypeDef",
     "CreateVodSourceResponseTypeDef",
     "DescribeLiveSourceResponseTypeDef",
     "DescribeVodSourceResponseTypeDef",
     "LiveSourceTypeDef",
     "UpdateLiveSourceRequestRequestTypeDef",
     "UpdateLiveSourceResponseTypeDef",
     "UpdateVodSourceRequestRequestTypeDef",
     "UpdateVodSourceResponseTypeDef",
     "VodSourceTypeDef",
-    "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
-    "ListAlertsRequestListAlertsPaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
-    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
-    "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
-    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
-    "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "RequestOutputItemTypeDef",
     "ResponseOutputItemTypeDef",
     "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
@@ -212,22 +213,22 @@
 )
 
 AdMarkerPassthroughTypeDef = TypedDict(
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 AlertTypeDef = TypedDict(
     "AlertTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
+        "Category": AlertCategoryType,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
     },
 )
 
 AvailMatchingCriteriaTypeDef = TypedDict(
@@ -241,41 +242,37 @@
 AvailSuppressionTypeDef = TypedDict(
     "AvailSuppressionTypeDef",
     {
         "FillPolicy": FillPolicyType,
         "Mode": ModeType,
         "Value": str,
     },
-    total=False,
 )
 
 BumperTypeDef = TypedDict(
     "BumperTypeDef",
     {
         "EndUrl": str,
         "StartUrl": str,
     },
-    total=False,
 )
 
 CdnConfigurationTypeDef = TypedDict(
     "CdnConfigurationTypeDef",
     {
         "AdSegmentUrlPrefix": str,
         "ContentSegmentUrlPrefix": str,
     },
-    total=False,
 )
 
 LogConfigurationForChannelTypeDef = TypedDict(
     "LogConfigurationForChannelTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
-    total=False,
 )
 
 ClipRangeTypeDef = TypedDict(
     "ClipRangeTypeDef",
     {
         "EndOffsetMillis": int,
     },
@@ -285,33 +282,40 @@
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ConfigureLogsForChannelResponseTypeDef = TypedDict(
+    "ConfigureLogsForChannelResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChannelName": str,
+        "LogTypes": List[Literal["AS_RUN"]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
     },
 )
 
+ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
+    {
+        "PercentEnabled": int,
+        "PlaybackConfigurationName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HttpPackageConfigurationTypeDef = TypedDict(
     "HttpPackageConfigurationTypeDef",
     {
         "Path": str,
         "SourceGroup": str,
         "Type": TypeType,
     },
@@ -375,15 +379,14 @@
 DashConfigurationTypeDef = TypedDict(
     "DashConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
-    total=False,
 )
 
 DashPlaylistSettingsTypeDef = TypedDict(
     "DashPlaylistSettingsTypeDef",
     {
         "ManifestWindowSeconds": int,
         "MinBufferTimeSeconds": int,
@@ -487,31 +490,59 @@
     "DescribeVodSourceRequestRequestTypeDef",
     {
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
+    "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
+    {
+        "ChannelName": str,
+    },
+)
+_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
+    "_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
+    {
+        "DurationMinutes": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
+    _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
+    _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetChannelScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredGetChannelScheduleRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalGetChannelScheduleRequestRequestTypeDef = TypedDict(
@@ -540,24 +571,22 @@
 )
 
 HlsConfigurationTypeDef = TypedDict(
     "HlsConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
     },
-    total=False,
 )
 
 LivePreRollConfigurationTypeDef = TypedDict(
     "LivePreRollConfigurationTypeDef",
     {
         "AdDecisionServerUrl": str,
         "MaxDurationSeconds": int,
     },
-    total=False,
 )
 
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "PercentEnabled": int,
     },
@@ -576,14 +605,36 @@
     {
         "AdMarkupType": Sequence[AdMarkupTypeType],
         "ManifestWindowSeconds": int,
     },
     total=False,
 )
 
+_RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
+    "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
+    "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAlertsRequestListAlertsPaginateTypeDef(
+    _RequiredListAlertsRequestListAlertsPaginateTypeDef,
+    _OptionalListAlertsRequestListAlertsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAlertsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlertsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListAlertsRequestRequestTypeDef = TypedDict(
@@ -598,23 +649,53 @@
 
 class ListAlertsRequestRequestTypeDef(
     _RequiredListAlertsRequestRequestTypeDef, _OptionalListAlertsRequestRequestTypeDef
 ):
     pass
 
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
+    {
+        "SourceLocationName": str,
+    },
+)
+_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
+    _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
+    _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLiveSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListLiveSourcesRequestRequestTypeDef",
     {
         "SourceLocationName": str,
     },
 )
 _OptionalListLiveSourcesRequestRequestTypeDef = TypedDict(
@@ -629,23 +710,54 @@
 
 class ListLiveSourcesRequestRequestTypeDef(
     _RequiredListLiveSourcesRequestRequestTypeDef, _OptionalListLiveSourcesRequestRequestTypeDef
 ):
     pass
 
 
+ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
+    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlaybackConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
+    "_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
+    {
+        "PlaybackConfigurationName": str,
+    },
+)
+_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
+    "_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
+    {
+        "StreamId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
+    _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
+    _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPrefetchSchedulesRequestRequestTypeDef = TypedDict(
     "_RequiredListPrefetchSchedulesRequestRequestTypeDef",
     {
         "PlaybackConfigurationName": str,
     },
 )
 _OptionalListPrefetchSchedulesRequestRequestTypeDef = TypedDict(
@@ -662,14 +774,22 @@
 class ListPrefetchSchedulesRequestRequestTypeDef(
     _RequiredListPrefetchSchedulesRequestRequestTypeDef,
     _OptionalListPrefetchSchedulesRequestRequestTypeDef,
 ):
     pass
 
 
+ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
+    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSourceLocationsRequestRequestTypeDef = TypedDict(
     "ListSourceLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -678,14 +798,44 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef",
+    {
+        "SourceLocationName": str,
+    },
+)
+_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
+    _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
+    _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVodSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListVodSourcesRequestRequestTypeDef",
     {
         "SourceLocationName": str,
     },
 )
 _OptionalListVodSourcesRequestRequestTypeDef = TypedDict(
@@ -700,31 +850,51 @@
 
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Policy": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ScheduleAdBreakTypeDef = TypedDict(
     "ScheduleAdBreakTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
-    total=False,
 )
 
 _RequiredTransitionTypeDef = TypedDict(
     "_RequiredTransitionTypeDef",
     {
         "RelativePosition": RelativePositionType,
         "Type": str,
@@ -809,15 +979,23 @@
 )
 
 ManifestProcessingRulesTypeDef = TypedDict(
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
-    total=False,
+)
+
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "Items": List[AlertTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 _RequiredPrefetchConsumptionTypeDef = TypedDict(
     "_RequiredPrefetchConsumptionTypeDef",
     {
         "EndTime": Union[datetime, str],
     },
@@ -834,64 +1012,14 @@
 
 class PrefetchConsumptionTypeDef(
     _RequiredPrefetchConsumptionTypeDef, _OptionalPrefetchConsumptionTypeDef
 ):
     pass
 
 
-ConfigureLogsForChannelResponseTypeDef = TypedDict(
-    "ConfigureLogsForChannelResponseTypeDef",
-    {
-        "ChannelName": str,
-        "LogTypes": List[Literal["AS_RUN"]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
-    {
-        "PercentEnabled": int,
-        "PlaybackConfigurationName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "Items": List[AlertTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateLiveSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -917,15 +1045,15 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateVodSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVodSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
@@ -954,70 +1082,59 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLiveSourceResponseTypeDef = TypedDict(
     "DescribeLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVodSourceResponseTypeDef = TypedDict(
     "DescribeVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredLiveSourceTypeDef = TypedDict(
-    "_RequiredLiveSourceTypeDef",
+LiveSourceTypeDef = TypedDict(
+    "LiveSourceTypeDef",
     {
         "Arn": str,
+        "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
-    },
-)
-_OptionalLiveSourceTypeDef = TypedDict(
-    "_OptionalLiveSourceTypeDef",
-    {
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class LiveSourceTypeDef(_RequiredLiveSourceTypeDef, _OptionalLiveSourceTypeDef):
-    pass
-
-
 UpdateLiveSourceRequestRequestTypeDef = TypedDict(
     "UpdateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -1029,15 +1146,15 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVodSourceRequestRequestTypeDef = TypedDict(
     "UpdateVodSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
@@ -1052,177 +1169,30 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredVodSourceTypeDef = TypedDict(
-    "_RequiredVodSourceTypeDef",
+VodSourceTypeDef = TypedDict(
+    "VodSourceTypeDef",
     {
         "Arn": str,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
-        "SourceLocationName": str,
-        "VodSourceName": str,
-    },
-)
-_OptionalVodSourceTypeDef = TypedDict(
-    "_OptionalVodSourceTypeDef",
-    {
         "CreationTime": datetime,
+        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class VodSourceTypeDef(_RequiredVodSourceTypeDef, _OptionalVodSourceTypeDef):
-    pass
-
-
-_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
-    "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
-    {
-        "ChannelName": str,
-    },
-)
-_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
-    "_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
-    {
-        "DurationMinutes": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
-    _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-    _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
-    "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
-    "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAlertsRequestListAlertsPaginateTypeDef(
-    _RequiredListAlertsRequestListAlertsPaginateTypeDef,
-    _OptionalListAlertsRequestListAlertsPaginateTypeDef,
-):
-    pass
-
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
-    {
         "SourceLocationName": str,
+        "Tags": Dict[str, str],
+        "VodSourceName": str,
     },
 )
-_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
-    _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-    _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-):
-    pass
-
-
-ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
-    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
-    "_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
-    {
-        "PlaybackConfigurationName": str,
-    },
-)
-_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
-    "_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
-    {
-        "StreamId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
-    _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-    _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-):
-    pass
-
-
-ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
-    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef",
-    {
-        "SourceLocationName": str,
-    },
-)
-_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
-    _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
-    _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
-):
-    pass
-
 
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
@@ -1239,65 +1209,41 @@
 
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
 
-_RequiredResponseOutputItemTypeDef = TypedDict(
-    "_RequiredResponseOutputItemTypeDef",
+ResponseOutputItemTypeDef = TypedDict(
+    "ResponseOutputItemTypeDef",
     {
+        "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
+        "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
 )
-_OptionalResponseOutputItemTypeDef = TypedDict(
-    "_OptionalResponseOutputItemTypeDef",
-    {
-        "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
-        "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
-    },
-    total=False,
-)
-
 
-class ResponseOutputItemTypeDef(
-    _RequiredResponseOutputItemTypeDef, _OptionalResponseOutputItemTypeDef
-):
-    pass
-
-
-_RequiredScheduleEntryTypeDef = TypedDict(
-    "_RequiredScheduleEntryTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ProgramName": str,
-        "SourceLocationName": str,
-    },
-)
-_OptionalScheduleEntryTypeDef = TypedDict(
-    "_OptionalScheduleEntryTypeDef",
+ScheduleEntryTypeDef = TypedDict(
+    "ScheduleEntryTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
+        "Arn": str,
+        "ChannelName": str,
         "LiveSourceName": str,
+        "ProgramName": str,
         "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
+        "SourceLocationName": str,
         "VodSourceName": str,
     },
-    total=False,
 )
 
-
-class ScheduleEntryTypeDef(_RequiredScheduleEntryTypeDef, _OptionalScheduleEntryTypeDef):
-    pass
-
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "Transition": TransitionTypeDef,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -1366,15 +1312,15 @@
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceLocationResponseTypeDef = TypedDict(
     "DescribeSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
@@ -1382,44 +1328,33 @@
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSourceLocationTypeDef = TypedDict(
-    "_RequiredSourceLocationTypeDef",
-    {
-        "Arn": str,
-        "HttpConfiguration": HttpConfigurationTypeDef,
-        "SourceLocationName": str,
-    },
-)
-_OptionalSourceLocationTypeDef = TypedDict(
-    "_OptionalSourceLocationTypeDef",
+SourceLocationTypeDef = TypedDict(
+    "SourceLocationTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
+        "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
+        "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SourceLocationName": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class SourceLocationTypeDef(_RequiredSourceLocationTypeDef, _OptionalSourceLocationTypeDef):
-    pass
-
-
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1449,15 +1384,15 @@
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPlaybackConfigurationResponseTypeDef = TypedDict(
     "GetPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
@@ -1475,15 +1410,15 @@
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PlaybackConfigurationTypeDef = TypedDict(
     "PlaybackConfigurationTypeDef",
     {
         "AdDecisionServerUrl": str,
@@ -1502,15 +1437,14 @@
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
-    total=False,
 )
 
 _RequiredPutPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1561,15 +1495,15 @@
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePrefetchScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "Consumption": PrefetchConsumptionTypeDef,
@@ -1599,69 +1533,58 @@
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
         "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPrefetchScheduleResponseTypeDef = TypedDict(
     "GetPrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
         "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPrefetchScheduleTypeDef = TypedDict(
-    "_RequiredPrefetchScheduleTypeDef",
+PrefetchScheduleTypeDef = TypedDict(
+    "PrefetchScheduleTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
-    },
-)
-_OptionalPrefetchScheduleTypeDef = TypedDict(
-    "_OptionalPrefetchScheduleTypeDef",
-    {
         "StreamId": str,
     },
-    total=False,
 )
 
-
-class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
-    pass
-
-
 ListLiveSourcesResponseTypeDef = TypedDict(
     "ListLiveSourcesResponseTypeDef",
     {
         "Items": List[LiveSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVodSourcesResponseTypeDef = TypedDict(
     "ListVodSourcesResponseTypeDef",
     {
         "Items": List[VodSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
@@ -1704,56 +1627,45 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
-        "LogConfiguration": LogConfigurationForChannelTypeDef,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tier": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
-    {
         "CreationTime": datetime,
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
+        "LogConfiguration": LogConfigurationForChannelTypeDef,
+        "Outputs": List[ResponseOutputItemTypeDef],
+        "PlaybackMode": str,
         "Tags": Dict[str, str],
+        "Tier": str,
     },
-    total=False,
 )
 
-
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
@@ -1763,15 +1675,15 @@
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "LogConfiguration": LogConfigurationForChannelTypeDef,
         "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
@@ -1780,24 +1692,24 @@
         "CreationTime": datetime,
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelScheduleResponseTypeDef = TypedDict(
     "GetChannelScheduleResponseTypeDef",
     {
         "Items": List[ScheduleEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdBreakTypeDef = TypedDict(
     "AdBreakTypeDef",
     {
         "AdBreakMetadata": Sequence[KeyValuePairTypeDef],
@@ -1811,42 +1723,42 @@
 )
 
 ListSourceLocationsResponseTypeDef = TypedDict(
     "ListSourceLocationsResponseTypeDef",
     {
         "Items": List[SourceLocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlaybackConfigurationsResponseTypeDef = TypedDict(
     "ListPlaybackConfigurationsResponseTypeDef",
     {
         "Items": List[PlaybackConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPrefetchSchedulesResponseTypeDef = TypedDict(
     "ListPrefetchSchedulesResponseTypeDef",
     {
         "Items": List[PrefetchScheduleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Items": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
@@ -1882,15 +1794,15 @@
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeProgramResponseTypeDef = TypedDict(
     "DescribeProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakTypeDef],
@@ -1900,15 +1812,15 @@
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
@@ -1941,10 +1853,10 @@
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor/type_defs.pyi` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessTypeType,
     AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     MessageTypeType,
     ModeType,
     OriginManifestTypeType,
     PlaybackModeType,
     RelativePositionType,
@@ -49,16 +50,17 @@
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionTypeDef",
     "BumperTypeDef",
     "CdnConfigurationTypeDef",
     "LogConfigurationForChannelTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "HttpPackageConfigurationTypeDef",
     "PrefetchRetrievalTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
     "DashConfigurationForPutTypeDef",
     "DashConfigurationTypeDef",
@@ -72,69 +74,68 @@
     "DeleteSourceLocationRequestRequestTypeDef",
     "DeleteVodSourceRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeLiveSourceRequestRequestTypeDef",
     "DescribeProgramRequestRequestTypeDef",
     "DescribeSourceLocationRequestRequestTypeDef",
     "DescribeVodSourceRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetChannelPolicyResponseTypeDef",
+    "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     "GetChannelScheduleRequestRequestTypeDef",
     "GetPlaybackConfigurationRequestRequestTypeDef",
     "HlsConfigurationTypeDef",
     "LivePreRollConfigurationTypeDef",
     "LogConfigurationTypeDef",
     "GetPrefetchScheduleRequestRequestTypeDef",
     "HlsPlaylistSettingsTypeDef",
+    "ListAlertsRequestListAlertsPaginateTypeDef",
     "ListAlertsRequestRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     "ListLiveSourcesRequestRequestTypeDef",
+    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     "ListPlaybackConfigurationsRequestRequestTypeDef",
+    "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
     "ListPrefetchSchedulesRequestRequestTypeDef",
+    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListSourceLocationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "ListVodSourcesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ScheduleAdBreakTypeDef",
     "TransitionTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "PrefetchConsumptionTypeDef",
-    "ConfigureLogsForChannelResponseTypeDef",
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetChannelPolicyResponseTypeDef",
     "ListAlertsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "PrefetchConsumptionTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
     "CreateLiveSourceResponseTypeDef",
     "CreateVodSourceRequestRequestTypeDef",
     "CreateVodSourceResponseTypeDef",
     "DescribeLiveSourceResponseTypeDef",
     "DescribeVodSourceResponseTypeDef",
     "LiveSourceTypeDef",
     "UpdateLiveSourceRequestRequestTypeDef",
     "UpdateLiveSourceResponseTypeDef",
     "UpdateVodSourceRequestRequestTypeDef",
     "UpdateVodSourceResponseTypeDef",
     "VodSourceTypeDef",
-    "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
-    "ListAlertsRequestListAlertsPaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
-    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
-    "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
-    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
-    "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "RequestOutputItemTypeDef",
     "ResponseOutputItemTypeDef",
     "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
@@ -211,22 +212,22 @@
 )
 
 AdMarkerPassthroughTypeDef = TypedDict(
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 AlertTypeDef = TypedDict(
     "AlertTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
+        "Category": AlertCategoryType,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
     },
 )
 
 AvailMatchingCriteriaTypeDef = TypedDict(
@@ -240,41 +241,37 @@
 AvailSuppressionTypeDef = TypedDict(
     "AvailSuppressionTypeDef",
     {
         "FillPolicy": FillPolicyType,
         "Mode": ModeType,
         "Value": str,
     },
-    total=False,
 )
 
 BumperTypeDef = TypedDict(
     "BumperTypeDef",
     {
         "EndUrl": str,
         "StartUrl": str,
     },
-    total=False,
 )
 
 CdnConfigurationTypeDef = TypedDict(
     "CdnConfigurationTypeDef",
     {
         "AdSegmentUrlPrefix": str,
         "ContentSegmentUrlPrefix": str,
     },
-    total=False,
 )
 
 LogConfigurationForChannelTypeDef = TypedDict(
     "LogConfigurationForChannelTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
-    total=False,
 )
 
 ClipRangeTypeDef = TypedDict(
     "ClipRangeTypeDef",
     {
         "EndOffsetMillis": int,
     },
@@ -284,33 +281,40 @@
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ConfigureLogsForChannelResponseTypeDef = TypedDict(
+    "ConfigureLogsForChannelResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChannelName": str,
+        "LogTypes": List[Literal["AS_RUN"]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
     },
 )
 
+ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
+    {
+        "PercentEnabled": int,
+        "PlaybackConfigurationName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HttpPackageConfigurationTypeDef = TypedDict(
     "HttpPackageConfigurationTypeDef",
     {
         "Path": str,
         "SourceGroup": str,
         "Type": TypeType,
     },
@@ -372,15 +376,14 @@
 DashConfigurationTypeDef = TypedDict(
     "DashConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
-    total=False,
 )
 
 DashPlaylistSettingsTypeDef = TypedDict(
     "DashPlaylistSettingsTypeDef",
     {
         "ManifestWindowSeconds": int,
         "MinBufferTimeSeconds": int,
@@ -484,31 +487,57 @@
     "DescribeVodSourceRequestRequestTypeDef",
     {
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
+    "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
+    {
+        "ChannelName": str,
+    },
+)
+_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
+    "_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
+    {
+        "DurationMinutes": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
+    _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
+    _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
+):
+    pass
+
 _RequiredGetChannelScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredGetChannelScheduleRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalGetChannelScheduleRequestRequestTypeDef = TypedDict(
@@ -535,24 +564,22 @@
 )
 
 HlsConfigurationTypeDef = TypedDict(
     "HlsConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
     },
-    total=False,
 )
 
 LivePreRollConfigurationTypeDef = TypedDict(
     "LivePreRollConfigurationTypeDef",
     {
         "AdDecisionServerUrl": str,
         "MaxDurationSeconds": int,
     },
-    total=False,
 )
 
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "PercentEnabled": int,
     },
@@ -571,14 +598,34 @@
     {
         "AdMarkupType": Sequence[AdMarkupTypeType],
         "ManifestWindowSeconds": int,
     },
     total=False,
 )
 
+_RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
+    "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
+    "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAlertsRequestListAlertsPaginateTypeDef(
+    _RequiredListAlertsRequestListAlertsPaginateTypeDef,
+    _OptionalListAlertsRequestListAlertsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAlertsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlertsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListAlertsRequestRequestTypeDef = TypedDict(
@@ -591,23 +638,51 @@
 )
 
 class ListAlertsRequestRequestTypeDef(
     _RequiredListAlertsRequestRequestTypeDef, _OptionalListAlertsRequestRequestTypeDef
 ):
     pass
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
+    {
+        "SourceLocationName": str,
+    },
+)
+_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
+    _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
+    _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListLiveSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListLiveSourcesRequestRequestTypeDef",
     {
         "SourceLocationName": str,
     },
 )
 _OptionalListLiveSourcesRequestRequestTypeDef = TypedDict(
@@ -620,23 +695,52 @@
 )
 
 class ListLiveSourcesRequestRequestTypeDef(
     _RequiredListLiveSourcesRequestRequestTypeDef, _OptionalListLiveSourcesRequestRequestTypeDef
 ):
     pass
 
+ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
+    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlaybackConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
+    "_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
+    {
+        "PlaybackConfigurationName": str,
+    },
+)
+_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
+    "_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
+    {
+        "StreamId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
+    _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
+    _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
+):
+    pass
+
 _RequiredListPrefetchSchedulesRequestRequestTypeDef = TypedDict(
     "_RequiredListPrefetchSchedulesRequestRequestTypeDef",
     {
         "PlaybackConfigurationName": str,
     },
 )
 _OptionalListPrefetchSchedulesRequestRequestTypeDef = TypedDict(
@@ -651,14 +755,22 @@
 
 class ListPrefetchSchedulesRequestRequestTypeDef(
     _RequiredListPrefetchSchedulesRequestRequestTypeDef,
     _OptionalListPrefetchSchedulesRequestRequestTypeDef,
 ):
     pass
 
+ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
+    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSourceLocationsRequestRequestTypeDef = TypedDict(
     "ListSourceLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -667,14 +779,42 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef",
+    {
+        "SourceLocationName": str,
+    },
+)
+_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
+    _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
+    _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListVodSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListVodSourcesRequestRequestTypeDef",
     {
         "SourceLocationName": str,
     },
 )
 _OptionalListVodSourcesRequestRequestTypeDef = TypedDict(
@@ -687,31 +827,51 @@
 )
 
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Policy": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ScheduleAdBreakTypeDef = TypedDict(
     "ScheduleAdBreakTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
-    total=False,
 )
 
 _RequiredTransitionTypeDef = TypedDict(
     "_RequiredTransitionTypeDef",
     {
         "RelativePosition": RelativePositionType,
         "Type": str,
@@ -794,15 +954,23 @@
 )
 
 ManifestProcessingRulesTypeDef = TypedDict(
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
-    total=False,
+)
+
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "Items": List[AlertTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 _RequiredPrefetchConsumptionTypeDef = TypedDict(
     "_RequiredPrefetchConsumptionTypeDef",
     {
         "EndTime": Union[datetime, str],
     },
@@ -817,64 +985,14 @@
 )
 
 class PrefetchConsumptionTypeDef(
     _RequiredPrefetchConsumptionTypeDef, _OptionalPrefetchConsumptionTypeDef
 ):
     pass
 
-ConfigureLogsForChannelResponseTypeDef = TypedDict(
-    "ConfigureLogsForChannelResponseTypeDef",
-    {
-        "ChannelName": str,
-        "LogTypes": List[Literal["AS_RUN"]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
-    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
-    {
-        "PercentEnabled": int,
-        "PlaybackConfigurationName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "Items": List[AlertTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateLiveSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -898,15 +1016,15 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateVodSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVodSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
@@ -933,68 +1051,59 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLiveSourceResponseTypeDef = TypedDict(
     "DescribeLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVodSourceResponseTypeDef = TypedDict(
     "DescribeVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredLiveSourceTypeDef = TypedDict(
-    "_RequiredLiveSourceTypeDef",
+LiveSourceTypeDef = TypedDict(
+    "LiveSourceTypeDef",
     {
         "Arn": str,
+        "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
+        "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
-    },
-)
-_OptionalLiveSourceTypeDef = TypedDict(
-    "_OptionalLiveSourceTypeDef",
-    {
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class LiveSourceTypeDef(_RequiredLiveSourceTypeDef, _OptionalLiveSourceTypeDef):
-    pass
-
 UpdateLiveSourceRequestRequestTypeDef = TypedDict(
     "UpdateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -1006,15 +1115,15 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVodSourceRequestRequestTypeDef = TypedDict(
     "UpdateVodSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
@@ -1029,165 +1138,30 @@
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredVodSourceTypeDef = TypedDict(
-    "_RequiredVodSourceTypeDef",
+VodSourceTypeDef = TypedDict(
+    "VodSourceTypeDef",
     {
         "Arn": str,
-        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
-        "SourceLocationName": str,
-        "VodSourceName": str,
-    },
-)
-_OptionalVodSourceTypeDef = TypedDict(
-    "_OptionalVodSourceTypeDef",
-    {
         "CreationTime": datetime,
+        "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class VodSourceTypeDef(_RequiredVodSourceTypeDef, _OptionalVodSourceTypeDef):
-    pass
-
-_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
-    "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
-    {
-        "ChannelName": str,
-    },
-)
-_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
-    "_OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
-    {
-        "DurationMinutes": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
-    _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-    _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-):
-    pass
-
-_RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
-    "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
-    "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAlertsRequestListAlertsPaginateTypeDef(
-    _RequiredListAlertsRequestListAlertsPaginateTypeDef,
-    _OptionalListAlertsRequestListAlertsPaginateTypeDef,
-):
-    pass
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
-    {
-        "SourceLocationName": str,
-    },
-)
-_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
-    _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-    _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-):
-    pass
-
-ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
-    "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
-    "_RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
-    {
-        "PlaybackConfigurationName": str,
-    },
-)
-_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef = TypedDict(
-    "_OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
-    {
-        "StreamId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
-    _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-    _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-):
-    pass
-
-ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
-    "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef",
-    {
         "SourceLocationName": str,
+        "Tags": Dict[str, str],
+        "VodSourceName": str,
     },
 )
-_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
-    _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
-    _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
-):
-    pass
 
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
@@ -1202,61 +1176,41 @@
 )
 
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
-_RequiredResponseOutputItemTypeDef = TypedDict(
-    "_RequiredResponseOutputItemTypeDef",
+ResponseOutputItemTypeDef = TypedDict(
+    "ResponseOutputItemTypeDef",
     {
+        "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
+        "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
 )
-_OptionalResponseOutputItemTypeDef = TypedDict(
-    "_OptionalResponseOutputItemTypeDef",
-    {
-        "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
-        "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
-    },
-    total=False,
-)
-
-class ResponseOutputItemTypeDef(
-    _RequiredResponseOutputItemTypeDef, _OptionalResponseOutputItemTypeDef
-):
-    pass
 
-_RequiredScheduleEntryTypeDef = TypedDict(
-    "_RequiredScheduleEntryTypeDef",
-    {
-        "Arn": str,
-        "ChannelName": str,
-        "ProgramName": str,
-        "SourceLocationName": str,
-    },
-)
-_OptionalScheduleEntryTypeDef = TypedDict(
-    "_OptionalScheduleEntryTypeDef",
+ScheduleEntryTypeDef = TypedDict(
+    "ScheduleEntryTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
+        "Arn": str,
+        "ChannelName": str,
         "LiveSourceName": str,
+        "ProgramName": str,
         "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
+        "SourceLocationName": str,
         "VodSourceName": str,
     },
-    total=False,
 )
 
-class ScheduleEntryTypeDef(_RequiredScheduleEntryTypeDef, _OptionalScheduleEntryTypeDef):
-    pass
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "Transition": TransitionTypeDef,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -1321,15 +1275,15 @@
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceLocationResponseTypeDef = TypedDict(
     "DescribeSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
@@ -1337,42 +1291,33 @@
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSourceLocationTypeDef = TypedDict(
-    "_RequiredSourceLocationTypeDef",
-    {
-        "Arn": str,
-        "HttpConfiguration": HttpConfigurationTypeDef,
-        "SourceLocationName": str,
-    },
-)
-_OptionalSourceLocationTypeDef = TypedDict(
-    "_OptionalSourceLocationTypeDef",
+SourceLocationTypeDef = TypedDict(
+    "SourceLocationTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
+        "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
+        "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
+        "SourceLocationName": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class SourceLocationTypeDef(_RequiredSourceLocationTypeDef, _OptionalSourceLocationTypeDef):
-    pass
-
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1400,15 +1345,15 @@
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "HttpConfiguration": HttpConfigurationTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPlaybackConfigurationResponseTypeDef = TypedDict(
     "GetPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
@@ -1426,15 +1371,15 @@
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PlaybackConfigurationTypeDef = TypedDict(
     "PlaybackConfigurationTypeDef",
     {
         "AdDecisionServerUrl": str,
@@ -1453,15 +1398,14 @@
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
-    total=False,
 )
 
 _RequiredPutPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1510,15 +1454,15 @@
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePrefetchScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "Consumption": PrefetchConsumptionTypeDef,
@@ -1546,67 +1490,58 @@
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
         "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPrefetchScheduleResponseTypeDef = TypedDict(
     "GetPrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
         "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPrefetchScheduleTypeDef = TypedDict(
-    "_RequiredPrefetchScheduleTypeDef",
+PrefetchScheduleTypeDef = TypedDict(
+    "PrefetchScheduleTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
-    },
-)
-_OptionalPrefetchScheduleTypeDef = TypedDict(
-    "_OptionalPrefetchScheduleTypeDef",
-    {
         "StreamId": str,
     },
-    total=False,
 )
 
-class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
-    pass
-
 ListLiveSourcesResponseTypeDef = TypedDict(
     "ListLiveSourcesResponseTypeDef",
     {
         "Items": List[LiveSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVodSourcesResponseTypeDef = TypedDict(
     "ListVodSourcesResponseTypeDef",
     {
         "Items": List[VodSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
@@ -1645,54 +1580,45 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
-        "LogConfiguration": LogConfigurationForChannelTypeDef,
-        "Outputs": List[ResponseOutputItemTypeDef],
-        "PlaybackMode": str,
-        "Tier": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
-    {
         "CreationTime": datetime,
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
+        "LogConfiguration": LogConfigurationForChannelTypeDef,
+        "Outputs": List[ResponseOutputItemTypeDef],
+        "PlaybackMode": str,
         "Tags": Dict[str, str],
+        "Tier": str,
     },
-    total=False,
 )
 
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
@@ -1702,15 +1628,15 @@
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "LogConfiguration": LogConfigurationForChannelTypeDef,
         "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
@@ -1719,24 +1645,24 @@
         "CreationTime": datetime,
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelScheduleResponseTypeDef = TypedDict(
     "GetChannelScheduleResponseTypeDef",
     {
         "Items": List[ScheduleEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdBreakTypeDef = TypedDict(
     "AdBreakTypeDef",
     {
         "AdBreakMetadata": Sequence[KeyValuePairTypeDef],
@@ -1750,42 +1676,42 @@
 )
 
 ListSourceLocationsResponseTypeDef = TypedDict(
     "ListSourceLocationsResponseTypeDef",
     {
         "Items": List[SourceLocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlaybackConfigurationsResponseTypeDef = TypedDict(
     "ListPlaybackConfigurationsResponseTypeDef",
     {
         "Items": List[PlaybackConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPrefetchSchedulesResponseTypeDef = TypedDict(
     "ListPrefetchSchedulesResponseTypeDef",
     {
         "Items": List[PrefetchScheduleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Items": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
@@ -1819,15 +1745,15 @@
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeProgramResponseTypeDef = TypedDict(
     "DescribeProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakTypeDef],
@@ -1837,15 +1763,15 @@
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
@@ -1876,10 +1802,10 @@
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/PKG-INFO` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.28.1
-Summary: Type annotations for boto3.MediaTailor 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediatailor?color=blue)](https://pypistats.org/packages/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
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
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,14 +322,15 @@
 `mypy_boto3_mediatailor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_mediatailor.literals import (
     AccessTypeType,
     AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     GetChannelSchedulePaginatorName,
     ListAlertsPaginatorName,
     ListChannelsPaginatorName,
     ListLiveSourcesPaginatorName,
     ListPlaybackConfigurationsPaginatorName,
@@ -376,16 +377,17 @@
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     LogConfigurationForChannelTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     HttpPackageConfigurationTypeDef,
     PrefetchRetrievalTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     DashConfigurationForPutTypeDef,
     DashConfigurationTypeDef,
@@ -399,69 +401,68 @@
     DeleteSourceLocationRequestRequestTypeDef,
     DeleteVodSourceRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
     HlsConfigurationTypeDef,
     LivePreRollConfigurationTypeDef,
     LogConfigurationTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
     HlsPlaylistSettingsTypeDef,
+    ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     ListLiveSourcesRequestRequestTypeDef,
+    ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
+    ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
+    ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
-    PrefetchConsumptionTypeDef,
-    ConfigureLogsForChannelResponseTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseTypeDef,
     ListAlertsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
     CreateLiveSourceResponseTypeDef,
     CreateVodSourceRequestRequestTypeDef,
     CreateVodSourceResponseTypeDef,
     DescribeLiveSourceResponseTypeDef,
     DescribeVodSourceResponseTypeDef,
     LiveSourceTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
     UpdateLiveSourceResponseTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
     UpdateVodSourceResponseTypeDef,
     VodSourceTypeDef,
-    GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
-    ListAlertsRequestListAlertsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
-    ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
-    ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
-    ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
-    ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     RequestOutputItemTypeDef,
     ResponseOutputItemTypeDef,
     ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediatailor-1.28.1/mypy_boto3_mediatailor.egg-info/SOURCES.txt` & `mypy-boto3-mediatailor-1.28.3/mypy_boto3_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.1/setup.py` & `mypy-boto3-mediatailor-1.28.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediatailor",
-    version="1.28.1",
+    version="1.28.3",
     packages=["mypy_boto3_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaTailor 1.28.1 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder"
+        " 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

