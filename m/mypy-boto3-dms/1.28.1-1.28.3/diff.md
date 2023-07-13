# Comparing `tmp/mypy-boto3-dms-1.28.1.tar.gz` & `tmp/mypy-boto3-dms-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dms-1.28.1.tar", last modified: Fri Jul  7 19:32:38 2023, max compression
+gzip compressed data, was "mypy-boto3-dms-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-dms-1.28.1.tar` & `mypy-boto3-dms-1.28.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-dms-1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-07 19:32:38.903385 mypy-boto3-dms-1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27924 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.899385 mypy-boto3-dms-1.28.1/mypy_boto3_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73220 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    73114 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   104127 2023-07-07 19:32:02.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   104064 2023-07-07 19:32:01.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-07 19:31:59.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-07 19:32:38.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-07 19:32:38.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 19:32:38.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 19:32:38.000000 mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:32:38.903385 mypy-boto3-dms-1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-07 19:31:58.000000 mypy-boto3-dms-1.28.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-dms-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29436 2023-07-13 19:49:12.653227 mypy-boto3-dms-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-dms-1.28.3/mypy_boto3_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73220 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73114 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   103553 2023-07-13 19:47:17.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103490 2023-07-13 19:47:16.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29436 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.665227 mypy-boto3-dms-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/setup.py
```

### Comparing `mypy-boto3-dms-1.28.1/LICENSE` & `mypy-boto3-dms-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/PKG-INFO` & `mypy-boto3-dms-1.28.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.28.1
-Summary: Type annotations for boto3.DatabaseMigrationService 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,14 +401,15 @@
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
     DataFormatValueType,
+    DatabaseModeType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DescribeCertificatesPaginatorName,
     DescribeConnectionsPaginatorName,
     DescribeEndpointTypesPaginatorName,
     DescribeEndpointsPaginatorName,
     DescribeEventSubscriptionsPaginatorName,
@@ -474,15 +475,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
@@ -505,98 +505,102 @@
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
     TableStatisticsTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
+    DescribeSchemasResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     ProvisionDataTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationStatsTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
+    ResponseMetadataTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
@@ -609,50 +613,47 @@
     EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
     DatabaseResponseTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
     DescribeReplicationConfigsMessageRequestTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTableStatisticsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
+    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
     DescribeReplicationTasksMessageRequestTypeDef,
     DescribeReplicationsMessageRequestTypeDef,
-    DescribeTableStatisticsMessageRequestTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
-    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    DescribeTableStatisticsMessageRequestTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
```

### Comparing `mypy-boto3-dms-1.28.1/README.md` & `mypy-boto3-dms-1.28.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,14 +369,15 @@
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
     DataFormatValueType,
+    DatabaseModeType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DescribeCertificatesPaginatorName,
     DescribeConnectionsPaginatorName,
     DescribeEndpointTypesPaginatorName,
     DescribeEndpointsPaginatorName,
     DescribeEventSubscriptionsPaginatorName,
@@ -442,15 +443,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
@@ -473,98 +473,102 @@
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
     TableStatisticsTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
+    DescribeSchemasResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     ProvisionDataTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationStatsTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
+    ResponseMetadataTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
@@ -577,50 +581,47 @@
     EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
     DatabaseResponseTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
     DescribeReplicationConfigsMessageRequestTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTableStatisticsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
+    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
     DescribeReplicationTasksMessageRequestTypeDef,
     DescribeReplicationsMessageRequestTypeDef,
-    DescribeTableStatisticsMessageRequestTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
-    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    DescribeTableStatisticsMessageRequestTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/__init__.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/__init__.pyi` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/__main__.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DatabaseMigrationService 1.28.1\nVersion:        "
-        " 1.28.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.DatabaseMigrationService 1.28.3\nVersion:        "
+        " 1.28.3\nBuilder version: 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/client.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/client.pyi` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/literals.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
     "CompressionTypeValueType",
     "DataFormatValueType",
+    "DatabaseModeType",
     "DatePartitionDelimiterValueType",
     "DatePartitionSequenceValueType",
     "DescribeCertificatesPaginatorName",
     "DescribeConnectionsPaginatorName",
     "DescribeEndpointTypesPaginatorName",
     "DescribeEndpointsPaginatorName",
     "DescribeEventSubscriptionsPaginatorName",
@@ -79,15 +79,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AuthMechanismValueType = Literal["default", "mongodb_cr", "scram_sha_1"]
 AuthTypeValueType = Literal["no", "password"]
 CannedAclForObjectsValueType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
@@ -96,14 +95,15 @@
     "public-read",
     "public-read-write",
 ]
 CharLengthSemanticsType = Literal["byte", "char", "default"]
 CollectorStatusType = Literal["ACTIVE", "UNREGISTERED"]
 CompressionTypeValueType = Literal["gzip", "none"]
 DataFormatValueType = Literal["csv", "parquet"]
+DatabaseModeType = Literal["babelfish", "default"]
 DatePartitionDelimiterValueType = Literal["DASH", "NONE", "SLASH", "UNDERSCORE"]
 DatePartitionSequenceValueType = Literal["DDMMYYYY", "MMYYYYDD", "YYYYMM", "YYYYMMDD", "YYYYMMDDHH"]
 DescribeCertificatesPaginatorName = Literal["describe_certificates"]
 DescribeConnectionsPaginatorName = Literal["describe_connections"]
 DescribeEndpointTypesPaginatorName = Literal["describe_endpoint_types"]
 DescribeEndpointsPaginatorName = Literal["describe_endpoints"]
 DescribeEventSubscriptionsPaginatorName = Literal["describe_event_subscriptions"]
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/literals.pyi` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
     "CompressionTypeValueType",
     "DataFormatValueType",
+    "DatabaseModeType",
     "DatePartitionDelimiterValueType",
     "DatePartitionSequenceValueType",
     "DescribeCertificatesPaginatorName",
     "DescribeConnectionsPaginatorName",
     "DescribeEndpointTypesPaginatorName",
     "DescribeEndpointsPaginatorName",
     "DescribeEventSubscriptionsPaginatorName",
@@ -78,14 +80,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AuthMechanismValueType = Literal["default", "mongodb_cr", "scram_sha_1"]
 AuthTypeValueType = Literal["no", "password"]
 CannedAclForObjectsValueType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
@@ -94,14 +97,15 @@
     "public-read",
     "public-read-write",
 ]
 CharLengthSemanticsType = Literal["byte", "char", "default"]
 CollectorStatusType = Literal["ACTIVE", "UNREGISTERED"]
 CompressionTypeValueType = Literal["gzip", "none"]
 DataFormatValueType = Literal["csv", "parquet"]
+DatabaseModeType = Literal["babelfish", "default"]
 DatePartitionDelimiterValueType = Literal["DASH", "NONE", "SLASH", "UNDERSCORE"]
 DatePartitionSequenceValueType = Literal["DDMMYYYY", "MMYYYYDD", "YYYYMM", "YYYYMMDD", "YYYYMMDDHH"]
 DescribeCertificatesPaginatorName = Literal["describe_certificates"]
 DescribeConnectionsPaginatorName = Literal["describe_connections"]
 DescribeEndpointTypesPaginatorName = Literal["describe_endpoint_types"]
 DescribeEndpointsPaginatorName = Literal["describe_endpoints"]
 DescribeEventSubscriptionsPaginatorName = Literal["describe_event_subscriptions"]
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/paginator.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
 
@@ -124,15 +124,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
 
@@ -142,15 +142,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
 
@@ -160,15 +160,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
 
@@ -179,15 +179,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -203,30 +203,30 @@
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
 
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 
@@ -236,15 +236,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
 
@@ -254,30 +254,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
-        self, *, ReplicationTaskArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 
@@ -288,30 +288,30 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
 
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
-        self, *, EndpointArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
 
@@ -322,13 +322,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/paginator.pyi` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
 class DescribeConnectionsPaginator(Paginator):
@@ -119,15 +119,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
 class DescribeEndpointTypesPaginator(Paginator):
@@ -136,15 +136,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
 class DescribeEndpointsPaginator(Paginator):
@@ -153,15 +153,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -171,15 +171,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -194,29 +194,29 @@
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 class DescribeReplicationInstancesPaginator(Paginator):
@@ -225,15 +225,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
 class DescribeReplicationSubnetGroupsPaginator(Paginator):
@@ -242,29 +242,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
-        self, *, ReplicationTaskArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 class DescribeReplicationTasksPaginator(Paginator):
@@ -274,29 +274,29 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
-        self, *, EndpointArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
 class DescribeTableStatisticsPaginator(Paginator):
@@ -306,13 +306,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/type_defs.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .literals import (
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
+    DatabaseModeType,
     DataFormatValueType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DmsSslModeValueType,
     EncodingTypeValueType,
     EncryptionModeValueType,
     EndpointSettingTypeValueType,
@@ -63,15 +64,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
@@ -94,98 +94,102 @@
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "TimestreamSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
     "TableStatisticsTypeDef",
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
+    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
+    "DescribeSchemasResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "ProvisionDataTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
+    "ReloadReplicationTablesResponseTypeDef",
+    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ReplicationStatsTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
+    "ResponseMetadataTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    "DescribeSchemasResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ReloadReplicationTablesResponseTypeDef",
-    "ReloadTablesResponseTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "CreateReplicationConfigMessageRequestTypeDef",
@@ -198,50 +202,47 @@
     "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "DatabaseResponseTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
     "DescribeReplicationConfigsMessageRequestTypeDef",
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     "DescribeReplicationTableStatisticsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     "DescribeReplicationTasksMessageRequestTypeDef",
     "DescribeReplicationsMessageRequestTypeDef",
-    "DescribeTableStatisticsMessageRequestTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
-    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+    "DescribeTableStatisticsMessageRequestTypeDef",
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
@@ -318,15 +319,14 @@
 AccountQuotaTypeDef = TypedDict(
     "AccountQuotaTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -340,41 +340,28 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 BatchStartRecommendationsErrorEntryTypeDef = TypedDict(
     "BatchStartRecommendationsErrorEntryTypeDef",
     {
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
-    total=False,
 )
 
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
@@ -390,44 +377,40 @@
         "CertificateArn": str,
         "CertificateOwner": str,
         "ValidFromDate": datetime,
         "ValidToDate": datetime,
         "SigningAlgorithm": str,
         "KeyLength": int,
     },
-    total=False,
 )
 
 CollectorHealthCheckTypeDef = TypedDict(
     "CollectorHealthCheckTypeDef",
     {
         "CollectorStatus": CollectorStatusType,
         "LocalCollectorS3Access": bool,
         "WebCollectorS3Access": bool,
         "WebCollectorGrantedRoleBasedAccess": bool,
     },
-    total=False,
 )
 
 InventoryDataTypeDef = TypedDict(
     "InventoryDataTypeDef",
     {
         "NumberOfDatabases": int,
         "NumberOfSchemas": int,
     },
-    total=False,
 )
 
 CollectorShortInfoResponseTypeDef = TypedDict(
     "CollectorShortInfoResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
-    total=False,
 )
 
 ComputeConfigTypeDef = TypedDict(
     "ComputeConfigTypeDef",
     {
         "AvailabilityZone": str,
         "DnsNameServers": str,
@@ -448,15 +431,14 @@
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
         "EndpointIdentifier": str,
         "ReplicationInstanceIdentifier": str,
     },
-    total=False,
 )
 
 DmsTransferSettingsTypeDef = TypedDict(
     "DmsTransferSettingsTypeDef",
     {
         "ServiceAccessRoleArn": str,
         "BucketName": str,
@@ -760,14 +742,16 @@
         "PluginName": PluginNameValueType,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
         "TrimSpaceInChar": bool,
         "MapBooleanAsBoolean": bool,
         "MapJsonbAsClob": bool,
         "MapLongVarcharAs": LongVarcharMappingTypeType,
+        "DatabaseMode": DatabaseModeType,
+        "BabelfishDatabaseName": str,
     },
     total=False,
 )
 
 _RequiredRedisSettingsTypeDef = TypedDict(
     "_RequiredRedisSettingsTypeDef",
     {
@@ -925,15 +909,14 @@
         "Status": str,
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
     },
-    total=False,
 )
 
 _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef",
     {
         "CollectorName": str,
         "ServiceAccessRoleArn": str,
@@ -952,47 +935,56 @@
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
 
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    {
+        "CollectorReferencedId": str,
+        "CollectorName": str,
+        "Description": str,
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
         "SupportLevel": str,
         "OsArchitecture": int,
         "Tooltip": str,
     },
-    total=False,
 )
 
 ServerShortInfoResponseTypeDef = TypedDict(
     "ServerShortInfoResponseTypeDef",
     {
         "ServerId": str,
         "IpAddress": str,
         "ServerName": str,
     },
-    total=False,
 )
 
 DatabaseShortInfoResponseTypeDef = TypedDict(
     "DatabaseShortInfoResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
         "DatabaseEngine": str,
     },
-    total=False,
 )
 
 DeleteCertificateMessageRequestTypeDef = TypedDict(
     "DeleteCertificateMessageRequestTypeDef",
     {
         "CertificateArn": str,
     },
@@ -1030,14 +1022,22 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "DatabaseIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
     "DeleteReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
     },
 )
 
@@ -1079,30 +1079,29 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
-        "Name": str,
-        "Values": Sequence[str],
+        "IndividualAssessmentNames": List[str],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Values": Sequence[str],
     },
-    total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
@@ -1142,48 +1141,44 @@
         "Sensitive": bool,
         "Units": str,
         "Applicability": str,
         "IntValueMin": int,
         "IntValueMax": int,
         "DefaultValue": str,
     },
-    total=False,
 )
 
 SupportedEndpointTypeTypeDef = TypedDict(
     "SupportedEndpointTypeTypeDef",
     {
         "EngineName": str,
         "SupportsCDC": bool,
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
-    total=False,
 )
 
 EventCategoryGroupTypeDef = TypedDict(
     "EventCategoryGroupTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
     },
-    total=False,
 )
 
 DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     {
         "MaxRecords": int,
         "NextToken": str,
@@ -1193,26 +1188,32 @@
 
 FleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
     },
-    total=False,
 )
 
 FleetAdvisorSchemaObjectResponseTypeDef = TypedDict(
     "FleetAdvisorSchemaObjectResponseTypeDef",
     {
         "SchemaId": str,
         "ObjectType": str,
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
+)
+
+DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
 DescribeOrderableReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     {
         "MaxRecords": int,
@@ -1230,28 +1231,26 @@
         "MinAllocatedStorage": int,
         "MaxAllocatedStorage": int,
         "DefaultAllocatedStorage": int,
         "IncludedAllocatedStorage": int,
         "AvailabilityZones": List[str],
         "ReleaseStatus": ReleaseStatusValuesType,
     },
-    total=False,
 )
 
 LimitationTypeDef = TypedDict(
     "LimitationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "Name": str,
         "Description": str,
         "Impact": str,
         "Type": str,
     },
-    total=False,
 )
 
 DescribeRefreshSchemasStatusMessageRequestTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
@@ -1262,15 +1261,14 @@
     {
         "EndpointArn": str,
         "ReplicationInstanceArn": str,
         "Status": RefreshSchemasStatusTypeValueType,
         "LastRefreshDate": datetime,
         "LastFailureMessage": str,
     },
-    total=False,
 )
 
 _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
@@ -1295,15 +1293,14 @@
 ReplicationInstanceTaskLogTypeDef = TypedDict(
     "ReplicationInstanceTaskLogTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
-    total=False,
 )
 
 TableStatisticsTypeDef = TypedDict(
     "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
@@ -1325,14 +1322,22 @@
         "TableState": str,
         "ValidationPendingRecords": int,
         "ValidationFailedRecords": int,
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
     },
+)
+
+DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
@@ -1349,29 +1354,49 @@
         "ReplicationTaskArn": str,
         "ReplicationTaskLastAssessmentDate": datetime,
         "AssessmentStatus": str,
         "AssessmentResultsFile": str,
         "AssessmentResults": str,
         "S3ObjectUrl": str,
     },
-    total=False,
 )
 
 ReplicationTaskIndividualAssessmentTypeDef = TypedDict(
     "ReplicationTaskIndividualAssessmentTypeDef",
     {
         "ReplicationTaskIndividualAssessmentArn": str,
         "ReplicationTaskAssessmentRunArn": str,
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
+)
+
+_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
+
+class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
+    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1386,14 +1411,30 @@
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
 
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
+    {
+        "Marker": str,
+        "Schemas": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1512,38 +1553,46 @@
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
     },
 )
 
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 ProvisionDataTypeDef = TypedDict(
     "ProvisionDataTypeDef",
     {
         "ProvisionState": str,
         "ProvisionedCapacityUnits": int,
         "DateProvisioned": datetime,
         "IsNewProvisioningAvailable": bool,
         "DateNewProvisioningDataAvailable": datetime,
         "ReasonForNewProvisioningData": str,
     },
-    total=False,
 )
 
 RdsConfigurationTypeDef = TypedDict(
     "RdsConfigurationTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
@@ -1551,29 +1600,27 @@
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
-    total=False,
 )
 
 RdsRequirementsTypeDef = TypedDict(
     "RdsRequirementsTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
-    total=False,
 )
 
 _RequiredRebootReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
@@ -1615,14 +1662,30 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
+ReloadReplicationTablesResponseTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1632,24 +1695,22 @@
     {
         "ReplicationInstanceClass": str,
         "AllocatedStorage": int,
         "MultiAZ": bool,
         "EngineVersion": str,
         "NetworkType": str,
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 ReplicationStatsTypeDef = TypedDict(
     "ReplicationStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
@@ -1659,24 +1720,22 @@
         "TablesErrored": int,
         "FreshStartDate": datetime,
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
-    total=False,
 )
 
 ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunProgressTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
-    total=False,
 )
 
 ReplicationTaskStatsTypeDef = TypedDict(
     "ReplicationTaskStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
@@ -1686,27 +1745,45 @@
         "TablesErrored": int,
         "FreshStartDate": datetime,
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
-    total=False,
+)
+
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
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    {
+        "LsaAnalysisId": str,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 SchemaShortInfoResponseTypeDef = TypedDict(
     "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
     },
-    total=False,
 )
 
 _RequiredStartReplicationMessageRequestTypeDef = TypedDict(
     "_RequiredStartReplicationMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
         "StartReplicationType": str,
@@ -1816,14 +1893,31 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "AccountQuotas": List[AccountQuotaTypeDef],
+        "UniqueAccountIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1967,149 +2061,61 @@
 
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
 
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    {
-        "CollectorReferencedId": str,
-        "CollectorName": str,
-        "Description": str,
-        "ServiceAccessRoleArn": str,
-        "S3BucketName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "DatabaseIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "AccountQuotas": List[AccountQuotaTypeDef],
-        "UniqueAccountIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    {
-        "IndividualAssessmentNames": List[str],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
-    {
-        "Marker": str,
-        "Schemas": List[str],
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReloadReplicationTablesResponseTypeDef = TypedDict(
-    "ReloadReplicationTablesResponseTypeDef",
-    {
-        "ReplicationConfigArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    {
-        "LsaAnalysisId": str,
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 BatchStartRecommendationsResponseTypeDef = TypedDict(
     "BatchStartRecommendationsResponseTypeDef",
     {
         "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCertificateResponseTypeDef = TypedDict(
     "DeleteCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCertificatesResponseTypeDef = TypedDict(
     "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportCertificateResponseTypeDef = TypedDict(
     "ImportCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CollectorResponseTypeDef = TypedDict(
     "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
@@ -2122,15 +2128,14 @@
         "CollectorHealthCheck": CollectorHealthCheckTypeDef,
         "LastDataReceived": str,
         "RegisteredDate": str,
         "CreatedDate": str,
         "ModifiedDate": str,
         "InventoryData": InventoryDataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateReplicationConfigMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "SourceEndpointArn": str,
@@ -2199,39 +2204,38 @@
         "ComputeConfig": ComputeConfigTypeDef,
         "ReplicationSettings": str,
         "SupplementalSettings": str,
         "TableMappings": str,
         "ReplicationConfigCreateTime": datetime,
         "ReplicationConfigUpdateTime": datetime,
     },
-    total=False,
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionsResponseTypeDef = TypedDict(
     "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestConnectionResponseTypeDef = TypedDict(
     "TestConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
         "EndpointIdentifier": str,
@@ -2321,15 +2325,14 @@
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
         "TimestreamSettings": TimestreamSettingsTypeDef,
     },
-    total=False,
 )
 
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
@@ -2381,87 +2384,122 @@
     pass
 
 
 CreateEventSubscriptionResponseTypeDef = TypedDict(
     "CreateEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventSubscriptionResponseTypeDef = TypedDict(
     "DeleteEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventSubscriptionsResponseTypeDef = TypedDict(
     "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEventSubscriptionResponseTypeDef = TypedDict(
     "ModifyEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatabaseResponseTypeDef = TypedDict(
     "DatabaseResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "IpAddress": str,
         "NumberOfSchemas": int,
         "Server": ServerShortInfoResponseTypeDef,
         "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
         "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
+)
+
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeConnectionsMessageRequestTypeDef = TypedDict(
     "DescribeConnectionsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointTypesMessageRequestTypeDef = TypedDict(
     "DescribeEndpointTypesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeEndpointsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2473,25 +2511,50 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": Literal["replication-instance"],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2581,24 +2644,42 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2645,206 +2726,88 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageRequestTypeDef",
+DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
         "WithoutSettings": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationsMessageRequestTypeDef",
+DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
+        "WithoutSettings": bool,
     },
     total=False,
 )
 
-_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-    },
-)
-_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
+DescribeReplicationsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationsMessageRequestTypeDef",
     {
+        "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
-class DescribeTableStatisticsMessageRequestTypeDef(
-    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
-    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
-):
-    pass
-
-
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
-    total=False,
 )
-
-DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "WithoutSettings": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "EndpointArn": str,
-    },
-)
-_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
-    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
+    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
-_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
     {
+        "MaxRecords": int,
+        "Marker": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
-    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+class DescribeTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
 
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
@@ -2938,161 +2901,159 @@
 )
 
 DescribeEndpointSettingsResponseTypeDef = TypedDict(
     "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
         "EndpointSettings": List[EndpointSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointTypesResponseTypeDef = TypedDict(
     "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
         "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
         "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
     "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
         "Limitations": List[LimitationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RefreshSchemasResponseTypeDef = TypedDict(
     "RefreshSchemasResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
     "DescribeReplicationTableStatisticsResponseTypeDef",
     {
         "ReplicationConfigArn": str,
         "Marker": str,
         "ReplicationTableStatistics": List[TableStatisticsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableStatisticsResponseTypeDef = TypedDict(
     "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
 )
 
 RdsRecommendationTypeDef = TypedDict(
     "RdsRecommendationTypeDef",
     {
         "RequirementsToTarget": RdsRequirementsTypeDef,
         "TargetConfiguration": RdsConfigurationTypeDef,
     },
-    total=False,
 )
 
 StartRecommendationsRequestEntryTypeDef = TypedDict(
     "StartRecommendationsRequestEntryTypeDef",
     {
         "DatabaseId": str,
         "Settings": RecommendationSettingsTypeDef,
@@ -3170,15 +3131,14 @@
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationCreateTime": datetime,
         "ReplicationUpdateTime": datetime,
         "ReplicationLastStopTime": datetime,
     },
-    total=False,
 )
 
 ReplicationTaskAssessmentRunTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
@@ -3189,15 +3149,14 @@
         "ServiceAccessRoleArn": str,
         "ResultLocationBucket": str,
         "ResultLocationFolder": str,
         "ResultEncryptionMode": str,
         "ResultKmsKeyArn": str,
         "AssessmentRunName": str,
     },
-    total=False,
 )
 
 ReplicationTaskTypeDef = TypedDict(
     "ReplicationTaskTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
@@ -3215,15 +3174,14 @@
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationTaskArn": str,
         "ReplicationTaskStats": ReplicationTaskStatsTypeDef,
         "TaskData": str,
         "TargetReplicationInstanceArn": str,
     },
-    total=False,
 )
 
 SchemaResponseTypeDef = TypedDict(
     "SchemaResponseTypeDef",
     {
         "CodeLineCount": int,
         "CodeSize": int,
@@ -3231,137 +3189,134 @@
         "Server": ServerShortInfoResponseTypeDef,
         "DatabaseInstance": DatabaseShortInfoResponseTypeDef,
         "SchemaId": str,
         "SchemaName": str,
         "OriginalSchema": SchemaShortInfoResponseTypeDef,
         "Similarity": float,
     },
-    total=False,
 )
 
 ReplicationSubnetGroupTypeDef = TypedDict(
     "ReplicationSubnetGroupTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "SupportedNetworkTypes": List[str],
     },
-    total=False,
 )
 
 DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationConfigResponseTypeDef = TypedDict(
     "CreateReplicationConfigResponseTypeDef",
     {
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationConfigResponseTypeDef = TypedDict(
     "DeleteReplicationConfigResponseTypeDef",
     {
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationConfigsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationConfigs": List[ReplicationConfigTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationConfigResponseTypeDef = TypedDict(
     "ModifyReplicationConfigResponseTypeDef",
     {
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEndpointResponseTypeDef = TypedDict(
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsResponseTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationDataTypeDef = TypedDict(
     "RecommendationDataTypeDef",
     {
         "RdsEngine": RdsRecommendationTypeDef,
     },
-    total=False,
 )
 
 BatchStartRecommendationsRequestRequestTypeDef = TypedDict(
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
@@ -3369,163 +3324,163 @@
 )
 
 DescribeReplicationsResponseTypeDef = TypedDict(
     "DescribeReplicationsResponseTypeDef",
     {
         "Marker": str,
         "Replications": List[ReplicationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "Replication": ReplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "Replication": ReplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationTaskResponseTypeDef = TypedDict(
     "CreateReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskResponseTypeDef = TypedDict(
     "DeleteReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTasksResponseTypeDef = TypedDict(
     "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTasks": List[ReplicationTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationTaskResponseTypeDef = TypedDict(
     "ModifyReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MoveReplicationTaskResponseTypeDef = TypedDict(
     "MoveReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskResponseTypeDef = TypedDict(
     "StartReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationTaskResponseTypeDef = TypedDict(
     "StopReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
         "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
     "CreateReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
     "ModifyReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationInstanceTypeDef = TypedDict(
     "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
@@ -3550,73 +3505,71 @@
         "ReplicationInstanceIpv6Addresses": List[str],
         "PubliclyAccessible": bool,
         "SecondaryAvailabilityZone": str,
         "FreeUntil": datetime,
         "DnsNameServers": str,
         "NetworkType": str,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "CreatedDate": str,
         "Status": str,
         "Preferred": bool,
         "Settings": RecommendationSettingsTypeDef,
         "Data": RecommendationDataTypeDef,
     },
-    total=False,
 )
 
 CreateReplicationInstanceResponseTypeDef = TypedDict(
     "CreateReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationInstanceResponseTypeDef = TypedDict(
     "DeleteReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
         "ReplicationInstances": List[ReplicationInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationInstanceResponseTypeDef = TypedDict(
     "ModifyReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootReplicationInstanceResponseTypeDef = TypedDict(
     "RebootReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationsResponseTypeDef = TypedDict(
     "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/type_defs.pyi` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .literals import (
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
+    DatabaseModeType,
     DataFormatValueType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DmsSslModeValueType,
     EncodingTypeValueType,
     EncryptionModeValueType,
     EndpointSettingTypeValueType,
@@ -62,15 +63,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
@@ -93,98 +93,102 @@
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "TimestreamSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
     "TableStatisticsTypeDef",
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
+    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
+    "DescribeSchemasResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "ProvisionDataTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
+    "ReloadReplicationTablesResponseTypeDef",
+    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ReplicationStatsTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
+    "ResponseMetadataTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    "DescribeSchemasResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ReloadReplicationTablesResponseTypeDef",
-    "ReloadTablesResponseTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "CreateReplicationConfigMessageRequestTypeDef",
@@ -197,50 +201,47 @@
     "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "DatabaseResponseTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
     "DescribeReplicationConfigsMessageRequestTypeDef",
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     "DescribeReplicationTableStatisticsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     "DescribeReplicationTasksMessageRequestTypeDef",
     "DescribeReplicationsMessageRequestTypeDef",
-    "DescribeTableStatisticsMessageRequestTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
-    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+    "DescribeTableStatisticsMessageRequestTypeDef",
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
@@ -317,15 +318,14 @@
 AccountQuotaTypeDef = TypedDict(
     "AccountQuotaTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -339,41 +339,28 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 BatchStartRecommendationsErrorEntryTypeDef = TypedDict(
     "BatchStartRecommendationsErrorEntryTypeDef",
     {
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
-    total=False,
 )
 
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
@@ -389,44 +376,40 @@
         "CertificateArn": str,
         "CertificateOwner": str,
         "ValidFromDate": datetime,
         "ValidToDate": datetime,
         "SigningAlgorithm": str,
         "KeyLength": int,
     },
-    total=False,
 )
 
 CollectorHealthCheckTypeDef = TypedDict(
     "CollectorHealthCheckTypeDef",
     {
         "CollectorStatus": CollectorStatusType,
         "LocalCollectorS3Access": bool,
         "WebCollectorS3Access": bool,
         "WebCollectorGrantedRoleBasedAccess": bool,
     },
-    total=False,
 )
 
 InventoryDataTypeDef = TypedDict(
     "InventoryDataTypeDef",
     {
         "NumberOfDatabases": int,
         "NumberOfSchemas": int,
     },
-    total=False,
 )
 
 CollectorShortInfoResponseTypeDef = TypedDict(
     "CollectorShortInfoResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
-    total=False,
 )
 
 ComputeConfigTypeDef = TypedDict(
     "ComputeConfigTypeDef",
     {
         "AvailabilityZone": str,
         "DnsNameServers": str,
@@ -447,15 +430,14 @@
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
         "EndpointIdentifier": str,
         "ReplicationInstanceIdentifier": str,
     },
-    total=False,
 )
 
 DmsTransferSettingsTypeDef = TypedDict(
     "DmsTransferSettingsTypeDef",
     {
         "ServiceAccessRoleArn": str,
         "BucketName": str,
@@ -755,14 +737,16 @@
         "PluginName": PluginNameValueType,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
         "TrimSpaceInChar": bool,
         "MapBooleanAsBoolean": bool,
         "MapJsonbAsClob": bool,
         "MapLongVarcharAs": LongVarcharMappingTypeType,
+        "DatabaseMode": DatabaseModeType,
+        "BabelfishDatabaseName": str,
     },
     total=False,
 )
 
 _RequiredRedisSettingsTypeDef = TypedDict(
     "_RequiredRedisSettingsTypeDef",
     {
@@ -916,15 +900,14 @@
         "Status": str,
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
     },
-    total=False,
 )
 
 _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef",
     {
         "CollectorName": str,
         "ServiceAccessRoleArn": str,
@@ -941,47 +924,56 @@
 
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    {
+        "CollectorReferencedId": str,
+        "CollectorName": str,
+        "Description": str,
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
         "SupportLevel": str,
         "OsArchitecture": int,
         "Tooltip": str,
     },
-    total=False,
 )
 
 ServerShortInfoResponseTypeDef = TypedDict(
     "ServerShortInfoResponseTypeDef",
     {
         "ServerId": str,
         "IpAddress": str,
         "ServerName": str,
     },
-    total=False,
 )
 
 DatabaseShortInfoResponseTypeDef = TypedDict(
     "DatabaseShortInfoResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
         "DatabaseEngine": str,
     },
-    total=False,
 )
 
 DeleteCertificateMessageRequestTypeDef = TypedDict(
     "DeleteCertificateMessageRequestTypeDef",
     {
         "CertificateArn": str,
     },
@@ -1019,14 +1011,22 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "DatabaseIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
     "DeleteReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
     },
 )
 
@@ -1068,30 +1068,29 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
-        "Name": str,
-        "Values": Sequence[str],
+        "IndividualAssessmentNames": List[str],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Values": Sequence[str],
     },
-    total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
@@ -1129,48 +1128,44 @@
         "Sensitive": bool,
         "Units": str,
         "Applicability": str,
         "IntValueMin": int,
         "IntValueMax": int,
         "DefaultValue": str,
     },
-    total=False,
 )
 
 SupportedEndpointTypeTypeDef = TypedDict(
     "SupportedEndpointTypeTypeDef",
     {
         "EngineName": str,
         "SupportsCDC": bool,
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
-    total=False,
 )
 
 EventCategoryGroupTypeDef = TypedDict(
     "EventCategoryGroupTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
     },
-    total=False,
 )
 
 DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     {
         "MaxRecords": int,
         "NextToken": str,
@@ -1180,26 +1175,32 @@
 
 FleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
     },
-    total=False,
 )
 
 FleetAdvisorSchemaObjectResponseTypeDef = TypedDict(
     "FleetAdvisorSchemaObjectResponseTypeDef",
     {
         "SchemaId": str,
         "ObjectType": str,
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
+)
+
+DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
 DescribeOrderableReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     {
         "MaxRecords": int,
@@ -1217,28 +1218,26 @@
         "MinAllocatedStorage": int,
         "MaxAllocatedStorage": int,
         "DefaultAllocatedStorage": int,
         "IncludedAllocatedStorage": int,
         "AvailabilityZones": List[str],
         "ReleaseStatus": ReleaseStatusValuesType,
     },
-    total=False,
 )
 
 LimitationTypeDef = TypedDict(
     "LimitationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "Name": str,
         "Description": str,
         "Impact": str,
         "Type": str,
     },
-    total=False,
 )
 
 DescribeRefreshSchemasStatusMessageRequestTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
@@ -1249,15 +1248,14 @@
     {
         "EndpointArn": str,
         "ReplicationInstanceArn": str,
         "Status": RefreshSchemasStatusTypeValueType,
         "LastRefreshDate": datetime,
         "LastFailureMessage": str,
     },
-    total=False,
 )
 
 _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
@@ -1280,15 +1278,14 @@
 ReplicationInstanceTaskLogTypeDef = TypedDict(
     "ReplicationInstanceTaskLogTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
-    total=False,
 )
 
 TableStatisticsTypeDef = TypedDict(
     "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
@@ -1310,14 +1307,22 @@
         "TableState": str,
         "ValidationPendingRecords": int,
         "ValidationFailedRecords": int,
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
     },
+)
+
+DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
@@ -1334,29 +1339,47 @@
         "ReplicationTaskArn": str,
         "ReplicationTaskLastAssessmentDate": datetime,
         "AssessmentStatus": str,
         "AssessmentResultsFile": str,
         "AssessmentResults": str,
         "S3ObjectUrl": str,
     },
-    total=False,
 )
 
 ReplicationTaskIndividualAssessmentTypeDef = TypedDict(
     "ReplicationTaskIndividualAssessmentTypeDef",
     {
         "ReplicationTaskIndividualAssessmentArn": str,
         "ReplicationTaskAssessmentRunArn": str,
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
+)
+
+_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
+class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
+    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1369,14 +1392,30 @@
 )
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
+    {
+        "Marker": str,
+        "Schemas": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1487,38 +1526,46 @@
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
     },
 )
 
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 ProvisionDataTypeDef = TypedDict(
     "ProvisionDataTypeDef",
     {
         "ProvisionState": str,
         "ProvisionedCapacityUnits": int,
         "DateProvisioned": datetime,
         "IsNewProvisioningAvailable": bool,
         "DateNewProvisioningDataAvailable": datetime,
         "ReasonForNewProvisioningData": str,
     },
-    total=False,
 )
 
 RdsConfigurationTypeDef = TypedDict(
     "RdsConfigurationTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
@@ -1526,29 +1573,27 @@
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
-    total=False,
 )
 
 RdsRequirementsTypeDef = TypedDict(
     "RdsRequirementsTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
-    total=False,
 )
 
 _RequiredRebootReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
@@ -1588,14 +1633,30 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
+ReloadReplicationTablesResponseTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1605,24 +1666,22 @@
     {
         "ReplicationInstanceClass": str,
         "AllocatedStorage": int,
         "MultiAZ": bool,
         "EngineVersion": str,
         "NetworkType": str,
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 ReplicationStatsTypeDef = TypedDict(
     "ReplicationStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
@@ -1632,24 +1691,22 @@
         "TablesErrored": int,
         "FreshStartDate": datetime,
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
-    total=False,
 )
 
 ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunProgressTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
-    total=False,
 )
 
 ReplicationTaskStatsTypeDef = TypedDict(
     "ReplicationTaskStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
@@ -1659,27 +1716,45 @@
         "TablesErrored": int,
         "FreshStartDate": datetime,
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
-    total=False,
+)
+
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
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    {
+        "LsaAnalysisId": str,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 SchemaShortInfoResponseTypeDef = TypedDict(
     "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
     },
-    total=False,
 )
 
 _RequiredStartReplicationMessageRequestTypeDef = TypedDict(
     "_RequiredStartReplicationMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
         "StartReplicationType": str,
@@ -1783,14 +1858,31 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "AccountQuotas": List[AccountQuotaTypeDef],
+        "UniqueAccountIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1924,149 +2016,61 @@
 )
 
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    {
-        "CollectorReferencedId": str,
-        "CollectorName": str,
-        "Description": str,
-        "ServiceAccessRoleArn": str,
-        "S3BucketName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "DatabaseIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "AccountQuotas": List[AccountQuotaTypeDef],
-        "UniqueAccountIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    {
-        "IndividualAssessmentNames": List[str],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
-    {
-        "Marker": str,
-        "Schemas": List[str],
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReloadReplicationTablesResponseTypeDef = TypedDict(
-    "ReloadReplicationTablesResponseTypeDef",
-    {
-        "ReplicationConfigArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    {
-        "LsaAnalysisId": str,
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 BatchStartRecommendationsResponseTypeDef = TypedDict(
     "BatchStartRecommendationsResponseTypeDef",
     {
         "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCertificateResponseTypeDef = TypedDict(
     "DeleteCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCertificatesResponseTypeDef = TypedDict(
     "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportCertificateResponseTypeDef = TypedDict(
     "ImportCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CollectorResponseTypeDef = TypedDict(
     "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
@@ -2079,15 +2083,14 @@
         "CollectorHealthCheck": CollectorHealthCheckTypeDef,
         "LastDataReceived": str,
         "RegisteredDate": str,
         "CreatedDate": str,
         "ModifiedDate": str,
         "InventoryData": InventoryDataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateReplicationConfigMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "SourceEndpointArn": str,
@@ -2152,39 +2155,38 @@
         "ComputeConfig": ComputeConfigTypeDef,
         "ReplicationSettings": str,
         "SupplementalSettings": str,
         "TableMappings": str,
         "ReplicationConfigCreateTime": datetime,
         "ReplicationConfigUpdateTime": datetime,
     },
-    total=False,
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionsResponseTypeDef = TypedDict(
     "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestConnectionResponseTypeDef = TypedDict(
     "TestConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
         "EndpointIdentifier": str,
@@ -2272,15 +2274,14 @@
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
         "TimestreamSettings": TimestreamSettingsTypeDef,
     },
-    total=False,
 )
 
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
@@ -2330,87 +2331,122 @@
 ):
     pass
 
 CreateEventSubscriptionResponseTypeDef = TypedDict(
     "CreateEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventSubscriptionResponseTypeDef = TypedDict(
     "DeleteEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventSubscriptionsResponseTypeDef = TypedDict(
     "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEventSubscriptionResponseTypeDef = TypedDict(
     "ModifyEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatabaseResponseTypeDef = TypedDict(
     "DatabaseResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "IpAddress": str,
         "NumberOfSchemas": int,
         "Server": ServerShortInfoResponseTypeDef,
         "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
         "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
+)
+
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
     total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeConnectionsMessageRequestTypeDef = TypedDict(
     "DescribeConnectionsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointTypesMessageRequestTypeDef = TypedDict(
     "DescribeEndpointTypesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeEndpointsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2422,25 +2458,50 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": Literal["replication-instance"],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2530,24 +2591,42 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2592,201 +2671,85 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageRequestTypeDef",
+DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
         "WithoutSettings": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationsMessageRequestTypeDef",
+DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
+        "WithoutSettings": bool,
     },
     total=False,
 )
 
-_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-    },
-)
-_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
+DescribeReplicationsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationsMessageRequestTypeDef",
     {
+        "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class DescribeTableStatisticsMessageRequestTypeDef(
-    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
-    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
-):
-    pass
-
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
-    total=False,
 )
-
-DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "WithoutSettings": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "EndpointArn": str,
-    },
-)
-_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
-    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
+    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
-_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
     {
+        "MaxRecords": int,
+        "Marker": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
-    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+class DescribeTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -2879,161 +2842,159 @@
 )
 
 DescribeEndpointSettingsResponseTypeDef = TypedDict(
     "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
         "EndpointSettings": List[EndpointSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointTypesResponseTypeDef = TypedDict(
     "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
         "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
         "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
     "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
         "Limitations": List[LimitationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RefreshSchemasResponseTypeDef = TypedDict(
     "RefreshSchemasResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
     "DescribeReplicationTableStatisticsResponseTypeDef",
     {
         "ReplicationConfigArn": str,
         "Marker": str,
         "ReplicationTableStatistics": List[TableStatisticsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableStatisticsResponseTypeDef = TypedDict(
     "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
 )
 
 RdsRecommendationTypeDef = TypedDict(
     "RdsRecommendationTypeDef",
     {
         "RequirementsToTarget": RdsRequirementsTypeDef,
         "TargetConfiguration": RdsConfigurationTypeDef,
     },
-    total=False,
 )
 
 StartRecommendationsRequestEntryTypeDef = TypedDict(
     "StartRecommendationsRequestEntryTypeDef",
     {
         "DatabaseId": str,
         "Settings": RecommendationSettingsTypeDef,
@@ -3107,15 +3068,14 @@
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationCreateTime": datetime,
         "ReplicationUpdateTime": datetime,
         "ReplicationLastStopTime": datetime,
     },
-    total=False,
 )
 
 ReplicationTaskAssessmentRunTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
@@ -3126,15 +3086,14 @@
         "ServiceAccessRoleArn": str,
         "ResultLocationBucket": str,
         "ResultLocationFolder": str,
         "ResultEncryptionMode": str,
         "ResultKmsKeyArn": str,
         "AssessmentRunName": str,
     },
-    total=False,
 )
 
 ReplicationTaskTypeDef = TypedDict(
     "ReplicationTaskTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
@@ -3152,15 +3111,14 @@
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationTaskArn": str,
         "ReplicationTaskStats": ReplicationTaskStatsTypeDef,
         "TaskData": str,
         "TargetReplicationInstanceArn": str,
     },
-    total=False,
 )
 
 SchemaResponseTypeDef = TypedDict(
     "SchemaResponseTypeDef",
     {
         "CodeLineCount": int,
         "CodeSize": int,
@@ -3168,137 +3126,134 @@
         "Server": ServerShortInfoResponseTypeDef,
         "DatabaseInstance": DatabaseShortInfoResponseTypeDef,
         "SchemaId": str,
         "SchemaName": str,
         "OriginalSchema": SchemaShortInfoResponseTypeDef,
         "Similarity": float,
     },
-    total=False,
 )
 
 ReplicationSubnetGroupTypeDef = TypedDict(
     "ReplicationSubnetGroupTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "SupportedNetworkTypes": List[str],
     },
-    total=False,
 )
 
 DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationConfigResponseTypeDef = TypedDict(
     "CreateReplicationConfigResponseTypeDef",
     {
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationConfigResponseTypeDef = TypedDict(
     "DeleteReplicationConfigResponseTypeDef",
     {
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationConfigsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationConfigs": List[ReplicationConfigTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationConfigResponseTypeDef = TypedDict(
     "ModifyReplicationConfigResponseTypeDef",
     {
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEndpointResponseTypeDef = TypedDict(
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsResponseTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationDataTypeDef = TypedDict(
     "RecommendationDataTypeDef",
     {
         "RdsEngine": RdsRecommendationTypeDef,
     },
-    total=False,
 )
 
 BatchStartRecommendationsRequestRequestTypeDef = TypedDict(
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
@@ -3306,163 +3261,163 @@
 )
 
 DescribeReplicationsResponseTypeDef = TypedDict(
     "DescribeReplicationsResponseTypeDef",
     {
         "Marker": str,
         "Replications": List[ReplicationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "Replication": ReplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "Replication": ReplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationTaskResponseTypeDef = TypedDict(
     "CreateReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskResponseTypeDef = TypedDict(
     "DeleteReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTasksResponseTypeDef = TypedDict(
     "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTasks": List[ReplicationTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationTaskResponseTypeDef = TypedDict(
     "ModifyReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MoveReplicationTaskResponseTypeDef = TypedDict(
     "MoveReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskResponseTypeDef = TypedDict(
     "StartReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationTaskResponseTypeDef = TypedDict(
     "StopReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
         "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
     "CreateReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
     "ModifyReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationInstanceTypeDef = TypedDict(
     "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
@@ -3487,73 +3442,71 @@
         "ReplicationInstanceIpv6Addresses": List[str],
         "PubliclyAccessible": bool,
         "SecondaryAvailabilityZone": str,
         "FreeUntil": datetime,
         "DnsNameServers": str,
         "NetworkType": str,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "CreatedDate": str,
         "Status": str,
         "Preferred": bool,
         "Settings": RecommendationSettingsTypeDef,
         "Data": RecommendationDataTypeDef,
     },
-    total=False,
 )
 
 CreateReplicationInstanceResponseTypeDef = TypedDict(
     "CreateReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationInstanceResponseTypeDef = TypedDict(
     "DeleteReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
         "ReplicationInstances": List[ReplicationInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationInstanceResponseTypeDef = TypedDict(
     "ModifyReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootReplicationInstanceResponseTypeDef = TypedDict(
     "RebootReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationsResponseTypeDef = TypedDict(
     "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/waiter.py` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms/waiter.pyi` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/PKG-INFO` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.28.1
-Summary: Type annotations for boto3.DatabaseMigrationService 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,14 +401,15 @@
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
     DataFormatValueType,
+    DatabaseModeType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DescribeCertificatesPaginatorName,
     DescribeConnectionsPaginatorName,
     DescribeEndpointTypesPaginatorName,
     DescribeEndpointsPaginatorName,
     DescribeEventSubscriptionsPaginatorName,
@@ -474,15 +475,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
@@ -505,98 +505,102 @@
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
     TableStatisticsTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
+    DescribeSchemasResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     ProvisionDataTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationStatsTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
+    ResponseMetadataTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
@@ -609,50 +613,47 @@
     EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
     DatabaseResponseTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
     DescribeReplicationConfigsMessageRequestTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTableStatisticsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
+    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
     DescribeReplicationTasksMessageRequestTypeDef,
     DescribeReplicationsMessageRequestTypeDef,
-    DescribeTableStatisticsMessageRequestTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
-    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    DescribeTableStatisticsMessageRequestTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
```

### Comparing `mypy-boto3-dms-1.28.1/mypy_boto3_dms.egg-info/SOURCES.txt` & `mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.1/setup.py` & `mypy-boto3-dms-1.28.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dms",
-    version="1.28.1",
+    version="1.28.3",
     packages=["mypy_boto3_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DatabaseMigrationService 1.28.1 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with"
+        " mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

